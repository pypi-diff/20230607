# Comparing `tmp/git_ws-0.9.2.tar.gz` & `tmp/git_ws-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_ws-0.9.2.tar", max compression
+gzip compressed data, was "git_ws-1.0.0.tar", max compression
```

## Comparing `git_ws-0.9.2.tar` & `git_ws-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    10236 2022-11-21 22:11:53.360966 git_ws-0.9.2/README.md
--rw-r--r--   0        0        0     2020 2022-11-21 22:11:53.364966 git_ws-0.9.2/gitws/__init__.py
--rw-r--r--   0        0        0      829 2022-11-21 22:11:53.364966 git_ws-0.9.2/gitws/__main__.py
--rw-r--r--   0        0        0     2316 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/_basemodel.py
--rw-r--r--   0        0        0    16680 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/_cli/__init__.py
--rw-r--r--   0        0        0     4369 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/_cli/common.py
--rw-r--r--   0        0        0     8803 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/_cli/config.py
--rw-r--r--   0        0        0     4628 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/_cli/dep.py
--rw-r--r--   0        0        0     3036 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/_cli/info.py
--rw-r--r--   0        0        0     4208 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/_cli/manifest.py
--rw-r--r--   0        0        0     3804 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/_cli/options.py
--rw-r--r--   0        0        0     2583 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/_cli/remote.py
--rw-r--r--   0        0        0     3452 2022-11-22 06:39:29.843025 git_ws-0.9.2/gitws/_url.py
--rw-r--r--   0        0        0     4110 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/_util.py
--rw-r--r--   0        0        0    15710 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/appconfig.py
--rw-r--r--   0        0        0     5133 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/clone.py
--rw-r--r--   0        0        0     2162 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/const.py
--rw-r--r--   0        0        0    29962 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/datamodel.py
--rw-r--r--   0        0        0     3601 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/deptree.py
--rw-r--r--   0        0        0     4764 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/exceptions.py
--rw-r--r--   0        0        0    19068 2022-11-22 07:04:07.505637 git_ws-0.9.2/gitws/git.py
--rw-r--r--   0        0        0    27104 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/gitws.py
--rw-r--r--   0        0        0    11461 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/iters.py
--rw-r--r--   0        0        0     1281 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/manifestfinder.py
--rw-r--r--   0        0        0     9273 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/workspace.py
--rw-r--r--   0        0        0     1420 2022-11-21 22:11:53.368966 git_ws-0.9.2/gitws/workspacefinder.py
--rw-r--r--   0        0        0     2631 2022-11-22 07:16:55.657327 git_ws-0.9.2/pyproject.toml
--rw-r--r--   0        0        0    11302 1970-01-01 00:00:00.000000 git_ws-0.9.2/setup.py
--rw-r--r--   0        0        0    11211 1970-01-01 00:00:00.000000 git_ws-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    15893 2023-03-24 09:50:58.637207 git_ws-1.0.0/README.md
+-rw-r--r--   0        0        0     4339 2023-03-22 22:59:30.360352 git_ws-1.0.0/gitws/__init__.py
+-rw-r--r--   0        0        0      834 2023-03-22 22:59:30.360352 git_ws-1.0.0/gitws/__main__.py
+-rw-r--r--   0        0        0     2325 2023-03-22 22:59:30.360352 git_ws-1.0.0/gitws/_basemodel.py
+-rw-r--r--   0        0        0    19415 2023-06-07 20:20:04.547206 git_ws-1.0.0/gitws/_cli/__init__.py
+-rw-r--r--   0        0        0     4378 2023-03-22 22:59:30.360352 git_ws-1.0.0/gitws/_cli/common.py
+-rw-r--r--   0        0        0     8808 2023-03-22 22:59:30.360352 git_ws-1.0.0/gitws/_cli/config.py
+-rw-r--r--   0        0        0     4801 2023-03-22 22:59:30.360352 git_ws-1.0.0/gitws/_cli/dep.py
+-rw-r--r--   0        0        0     3705 2023-03-27 21:51:51.061952 git_ws-1.0.0/gitws/_cli/info.py
+-rw-r--r--   0        0        0     4213 2023-03-22 22:59:30.360352 git_ws-1.0.0/gitws/_cli/manifest.py
+-rw-r--r--   0        0        0     4757 2023-06-07 20:20:04.547206 git_ws-1.0.0/gitws/_cli/options.py
+-rw-r--r--   0        0        0     2612 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/_cli/remote.py
+-rw-r--r--   0        0        0     5497 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/_filerefupdater.py
+-rw-r--r--   0        0        0     3693 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/_url.py
+-rw-r--r--   0        0        0     4438 2023-06-07 20:20:04.547206 git_ws-1.0.0/gitws/_util.py
+-rw-r--r--   0        0        0    15719 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/appconfig.py
+-rw-r--r--   0        0        0     6184 2023-04-16 19:53:26.936660 git_ws-1.0.0/gitws/clone.py
+-rw-r--r--   0        0        0     2142 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/const.py
+-rw-r--r--   0        0        0    38080 2023-06-07 20:20:04.547206 git_ws-1.0.0/gitws/datamodel.py
+-rw-r--r--   0        0        0     4033 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/deptree.py
+-rw-r--r--   0        0        0     5509 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/exceptions.py
+-rw-r--r--   0        0        0    22171 2023-06-07 20:20:04.551206 git_ws-1.0.0/gitws/git.py
+-rw-r--r--   0        0        0    33393 2023-06-07 20:20:04.551206 git_ws-1.0.0/gitws/gitws.py
+-rw-r--r--   0        0        0    13343 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/iters.py
+-rw-r--r--   0        0        0     1537 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/manifestfinder.py
+-rw-r--r--   0        0        0    11828 2023-06-07 20:20:04.551206 git_ws-1.0.0/gitws/workspace.py
+-rw-r--r--   0        0        0     1429 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/workspacefinder.py
+-rw-r--r--   0        0        0     2684 2023-06-07 20:40:24.211022 git_ws-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    16774 1970-01-01 00:00:00.000000 git_ws-1.0.0/PKG-INFO
```

### Comparing `git_ws-0.9.2/README.md` & `git_ws-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,116 +5,280 @@
 [![Coverage Status](https://coveralls.io/repos/github/c0fec0de/git-ws/badge.svg?branch=main)](https://coveralls.io/github/c0fec0de/git-ws?branch=main)
 [![python-versions](https://img.shields.io/pypi/pyversions/git-ws.svg)](https://pypi.python.org/pypi/git-ws)
 [![pylint](https://img.shields.io/badge/linter-pylint-%231674b1?style=flat)](https://www.pylint.org/)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # Git Workspace - Multi Repository Management Tool
 
-* [Installation](#installation)
-* [Usage](#usage)
-* [Cheat-Sheet](#cheat-sheet)
-* [Python API](#api)
-* [Alternatives](#alternatives)
+* [Installation](https://github.com/c0fec0de/git-ws#-installation)
+* [Usage](https://github.com/c0fec0de/git-ws#-usage)
+* [Getting Started](https://github.com/c0fec0de/git-ws#-getting-started)
+* [Cheat-Sheet](https://github.com/c0fec0de/git-ws#%EF%B8%8F-cheat-sheet)
+* [Python API](https://github.com/c0fec0de/git-ws#-python-api)
+* [Alternatives](https://github.com/c0fec0de/git-ws#-alternatives)
 
 Git Workspace is a lightweight tool for creating and managing *workspaces* consisting of several interdependent `git` repositories. Starting from a *main repository*, Git Workspace discovers dependencies specified in a *manifest file*, fetching any specified required repositories and assembling them into a single workspace.
 
 ![Workspace](https://github.com/c0fec0de/git-ws/raw/main/docs/images/workspace.png)
 
 👉 You can read more about the used [nomenclature](https://git-ws.readthedocs.io/en/latest/manual/nomenclature.html) in the [documentation](https://git-ws.readthedocs.io/en/latest/index.html).
 
 
-# 📦 Installation
+
+## 📦 Installation
 
 Git Workspace is written in Python and - as usual - installing it is pretty easy:
 
 ```bash
 pip install git-ws
 ```
 
-And that's it! Ideally, if your project also uses Python, we recommend adding Git Workspace as a dependency to it as well, so that you can track the exact version of it together with your other dependencies. For example, if you use `poetry`, add it by running
+And that's it! Ideally, if your project also uses Python, we recommend adding Git Workspace as a dependency to it as well so that you can track the exact version of it together with your other dependencies. For example, if you use `poetry`, add it by running
 
 ```bash
-# Add Git Workspace as development dependency:
+# Add Git Workspace as a development dependency:
 poetry add --group dev git-ws
 ```
 
+For testing you can try:
+
+```bash
+git ws --version
+```
+
 
-# 📔 Usage
+## 📔 Usage
 
 Git Workspace is integrated into git `git ws` - this is what you will be using most of the time.
 
-Let's assume we have a project called `myapp`, which requires a library `mylib` that is maintained in another `git` repository. In order to use this project with Git Workspace, `myapp` needs to provide a so called *manifest*. An Git Workspace manifest is a simple [TOML](https://toml.io/) file - by default called `git-ws.toml` in the project's root folder - which defines the dependencies a project has as well as some other meta information. A minimal manifest for our project could look like this:
+#### The Manifest
+
+Let's assume we have a project called `myapp`, which requires a library `mylib` that is maintained in another `git` repository. In order to use this project with Git Workspace, `myapp` needs to provide a so called *manifest*. A Git Workspace manifest is a simple [TOML](https://toml.io/) file - by default called `git-ws.toml` in the project's root folder - which defines the dependencies a project has as well as some other meta information. A minimal manifest for our project could look like this:
 
 ```toml
 [[dependencies]]
 name = "mylib"
 url = "git@github.com:example/mylib.git"
 revision = "v2.3.4"
 ```
 
-If `myapp` and `mylib` are stored on the same server (side-by-side), than the manifest can even be simpler:
+If `myapp` and `mylib` are stored on the same server (side-by-side), then the manifest can even be simpler:
 
 ```toml
 [[dependencies]]
 name = "mylib"
 revision = "v2.3.4"
 ```
 
-The project will be searched via a relative path (which is either `../mylib` or `../mylib.git` depending on the main repository's URL). Relative paths are in general useful as they allow to use the same protocol for the main repository as well as any of its dependencies.
+The project will be searched via a relative path (which is either `../mylib` or `../mylib.git` depending on the main repository's URL). Relative paths are in general useful as they allow using the same protocol for the main repository as well as any of its dependencies.
+
+See the [Manifest Documentation](https://git-ws.readthedocs.io/en/latest/manual/manifest.html) for any further details on available options.
+
+#### The Initial Clone
 
 To build a workspace from a project prepared like that, simply clone it via `git ws`:
 
 ```bash
 cd $HOME/Projects
-mkdir my_app_workspace
-cd my_app_workspace
 git ws clone --update git@github.com:example/myapp.git
 ```
 
 👉 Without the `--update` option, only the main repository will be fetched.
 
 The above will clone the app repository and also the library side-by-side:
 
 ```bash
-ls -a
+ls -a myapp/
 # Should print something like
 .
 ..
 .git-ws
 myapp
 mylib
 ```
 
 As you can see, besides the two repositories we wanted, there is also a hidden `.git-ws` folder where the tool stores the needed configuration data.
 
-Sometimes there are use cases where using `git ws clone` cannot be used. For example, when a CI/CD system creates the initial clone of the main repository, you may need a way to fetch the remaining projects. This can be done by simply running the following within the main project:
+The [`git ws clone` documentation](https://git-ws.readthedocs.io/en/latest/manual/command-line-interface/workspace-management.html#git-ws-clone) describes all options.
+
+#### Initialization
+
+Sometimes there are use cases where using `git ws clone` cannot be used. For example, when you set up your manifest for the first time or when a CI/CD system creates the initial clone of the main repository, you may need a way to fetch the remaining projects. This can be done by simply running the following **within** the main project:
 
 ```bash
 git ws init --update
 ```
 
 👉 As with `git ws clone`, without the `--update`, no dependencies will be fetched.
 
-Another important use case is keeping a workspace up-to-date. Lets say you pull in an update in the main repository, which in turn might cause changes in the manifest to be pulled in as well. Updating the existing workspace is as simple as
+This command initializes the workspace and just needs to run once.
+Changes to the manifest require an update operation (see next section) but no re-initialization.
+
+#### Updating
+
+Another important use case is keeping a workspace up-to-date. Let's say you pull in an update in the main repository, which in turn might cause changes in the manifest to be pulled in as well. Updating the existing workspace is as simple as
 
 ```bash
 # Update the workspace (main and all dependent repositories):
 git ws update
 
 # Alternatively, run `git rebase` instead of `git pull` in dependencies:
 git ws update --rebase
 ```
-## Cheat-Sheet
+
+#### Non-Git Main Projects
+
+`git ws` can leave the manifest version control to any other version control system (Subversion, VCS, DesignSync, etc.).
+Just manage the manifest file `git-ws.toml` within the version control system of your choice.
+Run `git ws init --update` or `git ws init --update -M path/to/git-ws.toml` in the intended workspace directory.
+
+👉 As before, without the `--update`, no dependencies will be fetched.
+
+**Inside** a git clone, `git ws init` uses the actual git project as the *main project* of the workspace.
+**Outside** a git clone, `git ws init` initializes a workspace *without* a *main project*.
+
+👉 There are just two drawbacks of a workspace without a main project:
+
+1. `git ws tag` has no main project to tag and will fail. Please use [`git ws manifest freeze`](https://git-ws.readthedocs.io/en/latest/manual/command-line-interface/manifest.html#git-ws-manifest-freeze).
+2. Relative URLs are not supported, as there is no URL to be relative to. Please use `remotes`:
+
+```toml
+[[remotes]]
+name = "main"
+url-base = "git@github.example.com:your-group"
+
+[[dependencies]]
+name = "dep1"
+remote = "main"
+```
+
+## 👍 Getting Started
+
+Please ensure a proper [installation](https://github.com/c0fec0de/git-ws#-installation).
+
+Lets take a clone of an example project, which does not use ``git ws`` yet.
+
+```bash
+mkdir -p $HOME/Projects/Example-Workspace
+cd $HOME/Projects/Example-Workspace
+git clone https://github.com/c0fec0de/git-ws-example-one.git
+# Cloning into 'git-ws-example-one'...
+# remote: Enumerating objects: 3, done.
+# remote: Counting objects: 100% (3/3), done.
+# remote: Compressing objects: 100% (2/2), done.
+# remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
+# Receiving objects: 100% (3/3), done.
+```
+
+Now you should have one git clone in your workspace directory. Let's use it as *main project*.
+At first, we need a manifest file ``git-ws.toml``.
+
+```bash
+cd git-ws-example-one
+git ws manifest create
+# Manifest 'git-ws.toml' created.
+git add git-ws.toml
+```
+
+Now, we need to initialize the workspace
+
+```bash
+git ws init
+# ===== . (MAIN 'git-ws-example-one') =====
+# Workspace initialized at '..'.
+# Please continue with:
+#
+#     git ws update
+#
+```
+
+The parent directory became the ``git ws`` *workspace directory* .
+The actual git clone is the *main project* now.
+``git ws`` suggests to run ``git ws update``.
+You can try, but nothing will happen yet, as the manifest is quite empty.
+
+Let's add our first dependency ``git-ws-example-lib``, which is located on the same git server.
+You can manually edit the manifest file ``git-ws.toml``, or you just run
+
+```bash
+git ws dep add git-ws-example-lib
+```
+
+Feel free to inspect the ``git-ws.toml`` file.
+``git ws update`` will now apply the manifest changes and pull the new dependency:
+
+
+```bash
+git ws update
+# ===== . (MAIN 'git-ws-example-one', revision='main') =====
+# Pulling branch 'main'.
+# Already up to date.
+# ===== ../git-ws-example-lib ('git-ws-example-lib') =====
+# git-ws WARNING Clone git-ws-example-lib has no revision!
+# Cloning 'https://github.com/c0fec0de/git-ws-example-lib.git'.
+# Cloning into '../git-ws-example-lib'...
+# remote: Enumerating objects: 3, done.
+# remote: Counting objects: 100% (3/3), done.
+# remote: Compressing objects: 100% (2/2), done.
+# remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
+# Receiving objects: 100% (3/3), done.
+```
+
+Please note the warning:
+
+```bash
+# git-ws WARNING Clone git-ws-example-lib has no revision!
+```
+
+It is strongly recommended to specify a default revision for all dependencies. The command
+
+```bash
+git ws default revision main
+```
+
+solves that for you. Any successive ``git ws update`` is now free of this warning:
+
+```
+===== . (MAIN 'git-ws-example-one', revision='main') =====
+Pulling branch 'main'.
+Already up to date.
+===== ../git-ws-example-lib ('git-ws-example-lib', revision='main') =====
+Pulling branch 'main'.
+Already up to date.
+```
+
+Now you can add, commit and push your changes to the ``git-ws.toml`` file.
+Other colleagues should use now:
+
+```bash
+cd $HOME/Projects
+git ws clone --update YOUR-REPO-URL
+
+# OR
+
+cd $HOME/Projects/Workspace
+git clone YOUR-REPO-URL
+cd <directory>
+git ws init --update
+```
+
+``git ws status`` shows all changes within all git clones in the workspace.
+``git ws add`` runs likewise the ``git add`` operation in the associated git clones.
+Please see the next section for an overview of all commands.
+
+
+## 🕹️ Cheat-Sheet
 
 #### Initialization
 
 | Command | Description |
 | --- | --- |
 | `git ws clone URL` | Clone git repository from `URL` as main repository and initialize Git Workspace |
-| `git ws init` | Initialize Git Workspace. Use current git clone as main repository |
+| `git ws init` (**inside** a git clone) | Initialize Git Workspace at parent directory. Use current git clone as main repository |
+| `git ws init` (**outside** a git clone) | Initialize Git Workspace at current directory. No main repository. |
 | `git ws manifest create` | Create well documented, empty manifest |
 
 #### Basic
 
 | Command | Description |
 | --- | --- |
 | `git ws update` | Pull latest changes on main repository and all dependent repositories (clone them if needed) |
@@ -152,41 +316,44 @@
 | `git ws info main-path`      | Print Path to Main Git Clone. |
 | `git ws info project-paths`  | Print Paths to all git clones. |
 | `git ws info workspace-path` | Print Path to Workspace. |
 | `git ws info dep-tree` | Print Dependency Tree. |
 | `git ws info dep-tree --dot \| dot -Tpng > dep-tree.png` | Draw Dependency Diagramm (needs [graphviz](https://graphviz.org)) |
 
 
+See the [command-line interface documentation](https://git-ws.readthedocs.io/en/latest/manual/command-line-interface/index.html) for any further details.
+
+
 ## 🐍 Python API
 
 Git Workspace is written in Python. Besides the `git ws` command line tool, there is also an API which you can use to further automate workspace creation and maintenance. If you are interested, have a look into the [API documentation](https://git-ws.readthedocs.io/en/latest/api/gitws.html).
 
 
 ## 🤝 Alternatives
 
-Before writing Git Workspace, we investigates several other existing tools in the hope they would fulfil out needs. In particular, we looked into the following tools and methodologies which are widely used to organize large projects:
+Before writing Git Workspace, we investigated several other existing tools in the hope they would fulfil our needs. In particular, we looked into the following tools and methodologies which are widely used to organize large projects:
 
 - [`git submodules`](https://git-scm.com/book/en/v2/Git-Tools-Submodules).
 - Google's [repo](https://gerrit.googlesource.com/git-repo/) tool.
 - The [`west`](https://docs.zephyrproject.org/latest/develop/west/index.html) tool developed in the scope of [Zephyr](https://www.zephyrproject.org/).
 - Leaving the pure `git` domain, one can also use a package manager like [`conan`](https://conan.io/).
-- And lastly, there are also approaches to still pack everything into a large so called *monorepo*.
+- And lastly, there are also approaches to still pack everything into a large, so called *monorepo*.
 
-Unfortunately, none of the tools we tested really satisfied us. But hey, as we are developers - *why not starting our own tool for the purpose?*
+Unfortunately, none of the tools we tested really satisfied us. But hey, as we are developers - *why not start our own tool for the purpose?*
 
-And that's what we did - Git Workspace is a our tool for managing a large workspace consisting of several smaller `git` projects. Here is how it compares to the other tools we evaluated:
+And that's what we did - Git Workspace is our tool for managing a large workspace consisting of several smaller `git` projects. Here is how it compares to the other tools we evaluated:
 
 
 |                           | `git submodules` | `repo` | `west` | *Monorepos* | `git ws` |
 | ------------------------- | ---------------- | ------ | ------ | ----------- | --------- |
 | Reusable Components       | ✅               | ✅     | ✅     | ➖          | ✅        |
 | Ease of Use               | ➖               | ✅     | ✅     | ✅          | ✅        |
 | Editable Components       | ➖               | ✅     | ➖     | ✅          | ✅        |
 | Freezing Configurations   | ✅               | ✅     | ✅     | ✅          | ✅        |
 | Transitive Dependencies   | ➖               | ➖     | ✅     | ➖          | ✅        |
 | Relative Dependency Paths | ✅               | ✅     | ➖     | ➖          | ✅        |
 | Branches as dependencies  | ➖               | ✅     | ✅     | ➖          | ✅        |
 
-👉 Please note that our view on the various features might be biased. As we did, always look at all the options available to you before deciding for one tool or the other. While the other tools in comparison did not model what we needed for our workflow, they might just be what you are looking for.
+👉 Please note that our view on the various features might be biased. As we did, always look at all the options available to you before deciding on one tool or the other. While the other tools in comparison did not model what we needed for our workflow, they might just be what you are looking for.
 
-If you want to learn more, have a look into the [documentation](https://git-ws.readthedocs.io/en/latest/manual/why.html).
+If you want to learn more, have a look into [Why We Started Git Workspace](https://git-ws.readthedocs.io/en/latest/manual/why.html).
```

### Comparing `git_ws-0.9.2/gitws/__main__.py` & `git_ws-1.0.0/gitws/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `git_ws-0.9.2/gitws/_basemodel.py` & `git_ws-1.0.0/gitws/_basemodel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -19,16 +19,16 @@
 
 
 class BaseModel(pydantic.BaseModel, allow_mutation=False):
     """
     Refined :any:`pydantic.BaseModel`.
 
     * Data Models are immutable.
-    * The `repr` implementation skips fields, which are identical to their default value.
-    * A `new` implementation eases the creation of new instances with the same values.
+    * The ``repr`` implementation skips fields, which are identical to their default value.
+    * A ``new`` implementation eases the creation of new instances with the same values.
     """
 
     def __repr_args__(self: pydantic.BaseModel):
         return [
             (key, value) for key, value in self.__dict__.items() if value != self.__fields__[key].field_info.default
         ]
```

### Comparing `git_ws-0.9.2/gitws/_cli/__init__.py` & `git_ws-1.0.0/gitws/_cli/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -17,48 +17,58 @@
 """Command Line Interface."""
 import logging
 from pathlib import Path
 
 import click
 import coloredlogs  # type: ignore
 
-from gitws import AppConfig, Defaults, GitWS, ManifestSpec
+from gitws import AppConfig, AppConfigLocation, Defaults, GitWS, ManifestSpec
 from gitws._util import resolve_relative
 from gitws.const import MANIFEST_PATH_DEFAULT
 from gitws.git import FileStatus, State
 
 from .common import COLOR_INFO, Context, Error, exceptionhandling, get_loglevel, pass_context
 from .config import config
 from .dep import dep
 from .info import info
 from .manifest import manifest
 from .options import (
     command_option,
     command_options_option,
+    depth_option,
     force_option,
     group_filters_option,
+    main_path_option,
     manifest_option,
-    path_option,
     paths_argument,
     process_command,
     process_command_options,
-    process_path,
+    process_main_path,
     process_paths,
     projects_option,
     reverse_option,
+    unshallow_option,
     update_option,
+    ws_path_option,
 )
 from .remote import remote
 
 _LOGGING_FORMAT = "%(name)s %(levelname)s %(message)s"
 
 
-@click.group(context_settings=dict(help_option_names=["-h", "--help"]))
+def _version_option():  # pragma: no cover
+    # Add support for click 7.x.x and click 8.x.x
+    if click.version_option.__kwdefaults__ and "package_name" in click.version_option.__kwdefaults__:
+        return click.version_option(package_name="git-ws")
+    return click.version_option()
+
+
+@click.group(context_settings={"help_option_names": ["-h", "--help"]})
 @click.option("-v", "--verbose", count=True)
-@click.version_option(package_name="git-ws")
+@_version_option()
 @click.pass_context
 def main(ctx=None, verbose=0):
     """
     Git Workspace - Multi Repository Management Tool.
     """
     app_config = AppConfig()
     level = get_loglevel(verbose)
@@ -67,81 +77,115 @@
         coloredlogs.install(level=level, fmt=_LOGGING_FORMAT)
     else:
         logging.basicConfig(level=level, format=_LOGGING_FORMAT)
     ctx.obj = Context(verbose=verbose, color=color)
 
 
 @main.command()
-@path_option()
+@main_path_option()
+@ws_path_option()
 @manifest_option(initial=True)
 @group_filters_option(initial=True)
+@depth_option()
 @update_option()
 @force_option()
 @pass_context
-def init(context, path=None, manifest_path=None, group_filters=None, update: bool = False, force: bool = False):
+def init(
+    context,
+    ws_path=None,
+    main_path=None,
+    manifest_path=None,
+    group_filters=None,
+    depth=None,
+    update: bool = False,
+    force: bool = False,
+):
     """
-    Initialize Git Workspace.
+    Initialize Git Workspace *with* or *without* main project.
 
-    The actual directory MUST be a valid git clone, which has been
-    either created by 'git init' or 'git clone'.
+    *with* main project: run `git ws init` in the directory of an actual git clone OR
+    run `git ws init PATH_TO_MAIN_GIT_CLONE`. The git clone becomes the main project
+    in both cases.
+
+    *without* main project: run `git ws init` in the intended workspace directory.
+    No main git project is needed.
+
+    In any of these cases a manifest file (i.e. `git-ws.toml`) is required.
+    It can be created via `git ws manifest create`.
     """
     with exceptionhandling(context):
-        path = process_path(path)
+        main_path = process_main_path(main_path)
         gws = GitWS.init(
-            main_path=path, manifest_path=manifest_path, group_filters=group_filters, force=force, secho=context.secho
+            path=ws_path,
+            main_path=main_path,
+            manifest_path=manifest_path,
+            group_filters=group_filters,
+            depth=depth,
+            force=force,
+            secho=context.secho,
         )
         click.secho(f"Workspace initialized at {str(resolve_relative(gws.path))!r}.")
         if update:
             gws.update(skip_main=True)
         else:
             click.secho("Please continue with:\n\n    git ws update\n", fg=COLOR_INFO)
 
 
 @main.command()
+@click.option("--prune", is_flag=True, default=False, help="Remove obsolete git clones")
+@force_option()
 @pass_context
-def deinit(context):
+def deinit(context, prune: bool = False, force: bool = False):
     """
     Deinitialize Git Workspace.
     """
     with exceptionhandling(context):
         gws = GitWS.from_path(secho=context.secho)
-        gws.deinit()
+        gws.deinit(prune=prune, force=force)
         click.secho(f"Workspace deinitialized at {str(resolve_relative(gws.path))!r}.")
 
 
 @main.command()
 @click.argument("url")
-@path_option()
+@main_path_option()
+@ws_path_option(nomain=True)
 @manifest_option(initial=True)
 @group_filters_option(initial=True)
 @click.option("--revision", help="Revision to be checked out. Tag, Branch or SHA")
+@depth_option()
 @update_option()
 @force_option()
 @pass_context
 def clone(
     context,
     url,
-    path=None,
+    ws_path=None,
+    main_path=None,
     manifest_path=None,
     group_filters=None,
+    depth=None,
     revision=None,
     update: bool = False,
     force: bool = False,
 ):
     """
-    Create a git clone and initialize Git Workspace.
+    Create a git clone from URL and initialize Git Workspace.
+
+    MAIN_PATH is optional. If not specified `REPONAME/REPONAME/` by default.
     """
     with exceptionhandling(context):
-        path = process_path(path)
+        main_path = process_main_path(main_path)
         gws = GitWS.clone(
             url,
-            main_path=path,
+            path=ws_path,
+            main_path=main_path,
             manifest_path=manifest_path,
             group_filters=group_filters,
             revision=revision,
+            depth=depth,
             force=force,
             secho=context.secho,
         )
         if update:
             gws.update(skip_main=True)
         else:
             click.secho(
@@ -187,53 +231,57 @@
 @manifest_option()
 @group_filters_option()
 @reverse_option()
 @command_option
 @pass_context
 def git(context, command, projects=None, manifest_path=None, group_filters=None, reverse=False):
     """
-    Run git command on projects.
+    Run git COMMAND on projects.
 
-    This command behaves identical to `git ws foreach -- git`.
+    This command is identical to `git ws foreach -- git COMMAND`.
     """
     with exceptionhandling(context):
         command = process_command(command)
         gws = GitWS.from_path(manifest_path=manifest_path, group_filters=group_filters, secho=context.secho)
         gws.run_foreach(("git",) + command, project_paths=projects, reverse=reverse)
 
 
 @main.command()
 @projects_option()
 @manifest_option()
 @group_filters_option()
 @command_options_option
+@unshallow_option()
 @pass_context
-def fetch(context, command_options=None, projects=None, manifest_path=None, group_filters=None):
+def fetch(context, command_options=None, projects=None, manifest_path=None, group_filters=None, unshallow=False):
     """
     Run 'git fetch' on projects.
 
-    This command behaves identical to `git ws foreach -- git fetch`.
+    This command is identical to `git ws foreach -- git fetch COMMAND_OPTIONS`.
     """
     with exceptionhandling(context):
         command_options = process_command_options(command_options)
         gws = GitWS.from_path(manifest_path=manifest_path, group_filters=group_filters, secho=context.secho)
-        gws.run_foreach(("git", "fetch") + command_options, project_paths=projects)
+        base_cmd = ("git", "fetch")
+        if unshallow:
+            base_cmd = base_cmd + ("--unshallow",)
+        gws.run_foreach(base_cmd + command_options, project_paths=projects)
 
 
 @main.command()
 @projects_option()
 @manifest_option()
 @group_filters_option()
 @command_options_option
 @pass_context
 def pull(context, command_options=None, projects=None, manifest_path=None, group_filters=None):
     """
     Run 'git pull' on projects.
 
-    This command behaves identical to `git ws foreach -- git pull`.
+    This command is identical to `git ws foreach -- git pull COMMAND_OPTIONS`.
     """
     with exceptionhandling(context):
         command_options = process_command_options(command_options)
         gws = GitWS.from_path(manifest_path=manifest_path, group_filters=group_filters, secho=context.secho)
         gws.run_foreach(("git", "pull") + command_options, project_paths=projects)
 
 
@@ -243,15 +291,15 @@
 @group_filters_option()
 @command_options_option
 @pass_context
 def push(context, command_options=None, projects=None, manifest_path=None, group_filters=None):
     """
     Run 'git push' on projects (in reverse order).
 
-    This command behaves identical to `git ws foreach --reverse -- git push`.
+    This command is identical to `git ws foreach --reverse -- git push COMMAND_OPTIONS`.
     """
     with exceptionhandling(context):
         command_options = process_command_options(command_options)
         gws = GitWS.from_path(manifest_path=manifest_path, group_filters=group_filters, secho=context.secho)
         gws.run_foreach(("git", "push") + command_options, project_paths=projects, reverse=True)
 
 
@@ -261,35 +309,36 @@
 @group_filters_option()
 @command_options_option
 @pass_context
 def rebase(context, command_options=None, projects=None, manifest_path=None, group_filters=None):
     """
     Run 'git rebase' on projects.
 
-    This command behaves identical to `git ws foreach -- git rebase`.
+    This command is identical to `git ws foreach -- git rebase COMMAND_OPTIONS`.
     """
     with exceptionhandling(context):
         command_options = process_command_options(command_options)
         gws = GitWS.from_path(manifest_path=manifest_path, group_filters=group_filters, secho=context.secho)
         gws.run_foreach(("git", "rebase") + command_options, project_paths=projects)
 
 
 @main.command()
 @paths_argument()
 @click.option("--branch", "-b", is_flag=True, help="show branch information")
+@click.option("--banner", "-B", is_flag=True, help="show banner of each project")
 @manifest_option()
 @group_filters_option()
 @pass_context
-def status(context, manifest_path=None, group_filters=None, paths=None, branch: bool = False):
+def status(context, manifest_path=None, group_filters=None, paths=None, branch: bool = False, banner: bool = False):
     """
-    Run 'git status' (displayed paths include the actual clone path).
+    Run 'git status' on PATHS or all files (displayed paths include the actual clone path).
     """
     with exceptionhandling(context):
         gws = GitWS.from_path(manifest_path=manifest_path, group_filters=group_filters, secho=context.secho)
-        for status in gws.status(paths=process_paths(paths), branch=branch):
+        for status in gws.status(paths=process_paths(paths), branch=branch, banner=banner):
             text = str(status)
             if isinstance(status, FileStatus):
                 fgidx = "red" if status.work in (State.IGNORED, State.UNTRACKED) else "green"
                 parts = (
                     context.style(text[0], fg=fgidx),
                     context.style(text[1], fg="red"),
                     text[2:],
@@ -303,15 +352,15 @@
 @paths_argument()
 @click.option("--stat", "stat", is_flag=True, help="show diffstat instead of patch.")
 @manifest_option()
 @group_filters_option()
 @pass_context
 def diff(context, manifest_path=None, group_filters=None, paths=None, stat=False):
     """
-    Run 'git diff' on paths (displayed paths include the actual clone path).
+    Run 'git diff' on PATHS or all files (displayed paths include the actual clone path).
     """
     with exceptionhandling(context):
         gws = GitWS.from_path(manifest_path=manifest_path, group_filters=group_filters, secho=context.secho)
         if stat:
             for diffstat in gws.diffstat(paths=process_paths(paths)):
                 click.echo(str(diffstat))
         else:
@@ -322,15 +371,15 @@
 @paths_argument()
 @force_option()
 @manifest_option()
 @group_filters_option()
 @pass_context
 def checkout(context, manifest_path=None, group_filters=None, paths=None, force: bool = False):
     """
-    Run 'git checkout' on paths and choose the right git clone and manifest revision automatically.
+    Run 'git checkout' on PATHS and choose the right git clone and manifest revision automatically.
 
     Checkout all clones to their manifest revision, if no paths are given.
     """
     with exceptionhandling(context):
         gws = GitWS.from_path(manifest_path=manifest_path, group_filters=group_filters, secho=context.secho)
         gws.checkout(process_paths(paths), force=force)
 
@@ -340,15 +389,15 @@
 @click.option("--force", "-f", "force", is_flag=True, help="allow adding otherwise ignored files")
 @click.option("--all", "-A", "all_", is_flag=True, help="add changes from all tracked and untracked files")
 @manifest_option()
 @group_filters_option()
 @pass_context
 def add(context, manifest_path=None, group_filters=None, paths=None, force=False, all_=False):
     """
-    Run 'git add' on paths and choose the right git clone automatically.
+    Run 'git add' on PATHS and choose the right git clone automatically.
     """
     with exceptionhandling(context):
         gws = GitWS.from_path(manifest_path=manifest_path, group_filters=group_filters, secho=context.secho)
         gws.add(process_paths(paths), force=force, all_=all_)
 
 
 # pylint: disable=invalid-name
@@ -358,29 +407,29 @@
 @click.option("--cached", "cached", is_flag=True, help="only remove from index")
 @click.option("-r", "recursive", is_flag=True, help="allow recursive removal")
 @manifest_option()
 @group_filters_option()
 @pass_context
 def rm(context, manifest_path=None, group_filters=None, paths=None, force=False, cached=False, recursive=False):
     """
-    Run 'git rm' on paths and choose the right git clone automatically.
+    Run 'git rm' on PATHS and choose the right git clone automatically.
     """
     with exceptionhandling(context):
         gws = GitWS.from_path(manifest_path=manifest_path, group_filters=group_filters, secho=context.secho)
         gws.rm(process_paths(paths), force=force, cached=cached, recursive=recursive)
 
 
 @main.command()
 @paths_argument()
 @manifest_option()
 @group_filters_option()
 @pass_context
 def reset(context, manifest_path=None, group_filters=None, paths=None):
     """
-    Run 'git reset' on paths and choose the right git clone automatically.
+    Run 'git reset' on PATHS and choose the right git clone automatically.
     """
     with exceptionhandling(context):
         gws = GitWS.from_path(manifest_path=manifest_path, group_filters=group_filters, secho=context.secho)
         gws.reset(process_paths(paths))
 
 
 @main.command()
@@ -388,15 +437,15 @@
 @click.option("--all", "-a", "all_", is_flag=True, help="commit all changed files")
 @paths_argument()
 @manifest_option()
 @group_filters_option()
 @pass_context
 def commit(context, manifest_path=None, group_filters=None, paths=None, message=None, all_=False):
     """
-    Run 'git commit' on paths and choose the right git clone automatically.
+    Run 'git commit' on PATHS and choose the right git clone automatically.
     """
     with exceptionhandling(context):
         if not message:
             raise ValueError("Please provide a commit message.")
         gws = GitWS.from_path(manifest_path=manifest_path, group_filters=group_filters, secho=context.secho)
         gws.commit(message, process_paths(paths), all_=all_)
 
@@ -406,15 +455,15 @@
 @click.option("--message", "-m", help="tag message")
 @click.option("--force", "-f", is_flag=True, help="replace the tag if exists")
 @manifest_option()
 @group_filters_option()
 @pass_context
 def tag(context, name, manifest_path=None, group_filters=None, message=None, force=None):
     """
-    Create git tag on main repository.
+    Create git tag NAME on main repository.
 
     This includes freezing all dependencies.
     """
     with exceptionhandling(context):
         gws = GitWS.from_path(manifest_path=manifest_path, group_filters=group_filters, secho=context.secho)
         gws.tag(name, msg=message, force=force)
 
@@ -424,17 +473,17 @@
 @manifest_option()
 @group_filters_option()
 @reverse_option()
 @command_option
 @pass_context
 def foreach(context, command, projects=None, manifest_path=None, group_filters=None, reverse=False):
     """
-    Run 'command' on projects.
+    Run COMMAND on projects.
 
-    Please use '--' to separate 'git ws' command line options from options forwarded to the `command`
+    Please use '--' to separate 'git ws' command line options from options forwarded to the COMMAND
     (i.e. `git ws foreach -- ls -l`)
     """
     with exceptionhandling(context):
         command = process_command(command)
         gws = GitWS.from_path(manifest_path=manifest_path, group_filters=group_filters, secho=context.secho)
         gws.run_foreach(command, project_paths=projects, reverse=reverse)
 
@@ -444,54 +493,79 @@
 @manifest_option()
 @group_filters_option()
 @reverse_option()
 @command_option
 @pass_context
 def submodule(context, command, projects=None, manifest_path=None, group_filters=None, reverse=False):
     """
-    Run git submodule command on projects.
+    Run git submodule COMMAND on projects.
 
-    This command behaves identical to `git ws foreach -- git submodule`.
+    This command is identical to `git ws foreach -- git submodule COMMAND`.
     """
     with exceptionhandling(context):
         command = process_command(command)
         gws = GitWS.from_path(manifest_path=manifest_path, group_filters=group_filters, secho=context.secho)
         gws.run_foreach(("git", "submodule") + command, project_paths=projects, reverse=reverse)
 
 
 @main.command()
 @manifest_option(initial=True)
-@click.argument("name", type=click.Choice(tuple(Defaults.__fields__)))
+@click.argument("name", type=click.Choice(tuple(Defaults().dict(by_alias=True))))
 @click.argument("value")
 @pass_context
 def default(context, manifest_path, name, value):
     """
-    Set Default in Manifest.
+    Set DEFAULT in Manifest to VALUE.
     """
     with exceptionhandling(context):
         manifest_path = Path(manifest_path)
         manifest_spec = ManifestSpec.load(manifest_path)
         defaults = manifest_spec.defaults.update_fromstr({name: value if value else None})
         manifest_spec = manifest_spec.update(defaults=defaults)
         manifest_spec.save(manifest_path)
 
 
-@main.command()
+@main.command(name="group-filters")
 @manifest_option(initial=True)
 @click.argument("value")
 @pass_context
 def group_filters(context, manifest_path, value):
     """
-    Set Group Filter.
+    Set Group Filter to VALUE.
+
+    The group filter selects/deselects dependencies based on their path and/or groups.
     """
     with exceptionhandling(context):
         manifest_path = Path(manifest_path)
         manifest_spec = ManifestSpec.load(manifest_path)
         manifest_spec = manifest_spec.update_fromstr({"group-filters": value if value else None})
         manifest_spec.save(manifest_path)
 
 
+@main.command()
+@projects_option()
+@manifest_option()
+@group_filters_option()
+@pass_context
+def unshallow(context, projects=None, manifest_path=None, group_filters=None):
+    """
+    Convert Shallow Clones To Complete Ones.
+
+    Given projects are fetched and converted to complete clones with entire history if not already.
+    Without any given project, all existing clones will be converted and any future clone will be complete too.
+    """
+    with exceptionhandling(context):
+        gws = GitWS.from_path(manifest_path=manifest_path, group_filters=group_filters, secho=context.secho)
+        if not projects:
+            with gws.workspace.app_config.edit(AppConfigLocation.WORKSPACE) as config:
+                config.depth = 0
+        for clone in gws.foreach(project_paths=projects):
+            git = clone.git
+            if git.get_shallow():
+                git.fetch(unshallow=True)
+
+
 main.add_command(config)
 main.add_command(info)
 main.add_command(manifest)
 main.add_command(remote)
 main.add_command(dep)
```

### Comparing `git_ws-0.9.2/gitws/_cli/common.py` & `git_ws-1.0.0/gitws/_cli/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -42,15 +42,15 @@
     0: logging.WARNING,
     1: logging.INFO,
     2: logging.DEBUG,
 }
 
 
 def get_loglevel(verbose: int):
-    """Return `logging.level` according to verbosity."""
+    """Return ``logging.level`` according to verbosity."""
     return _LOGLEVELMAP.get(verbose, logging.DEBUG)
 
 
 class Context(BaseModel):
 
     """Command Line Context."""
 
@@ -60,15 +60,15 @@
     def secho(self, message, **kwargs):
         """Print with color support similar to :any:`click.secho()."""
         if self.color:
             return click.secho(message, **kwargs)
         return click.echo(message)
 
     def style(self, text, **kwargs):
-        """Format `text`."""
+        """Format ``text``."""
         if self.color:
             return click.style(text, **kwargs)
         return text
 
 
 pass_context = click.make_pass_decorator(Context)
```

### Comparing `git_ws-0.9.2/gitws/_cli/config.py` & `git_ws-1.0.0/gitws/_cli/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -88,15 +88,15 @@
 @system_option
 @user_option
 @workspace_option
 @format_option
 @pass_context
 def get(context, option, target, format_):
     """
-    Get the value of a configuration option.
+    Get the value of a configuration OPTION.
 
     This prints the value of the specified option. If selected,
     the value of a specific configuration file will be read. Otherwise, the
     computed value of the configuration option is shown.
 
     The computed configuration value is created by
     merging the system, user and workspace configuration files in that order.
@@ -131,15 +131,15 @@
     "ignore_unknown",
     is_flag=True,
     help="Set the option, even if it is not known to the application. Note that this bypasses any type checking.",
 )
 @pass_context
 def set_(context, option, value, target, ignore_unknown):
     """
-    Set the configuration option to the given value.
+    Set the configuration OPTION to the given VALUE.
 
     This sets an option to the given value. If no specific configuration file
     is selected, then this will update the workspace configuration if run
     from within a workspace. Otherwise, the user configuration will be updated.
     """
     with exceptionhandling(context):
         config = AppConfig()
@@ -163,15 +163,15 @@
 @click.argument("option")
 @system_option
 @user_option
 @workspace_option
 @pass_context
 def delete(context, option, target):
     """
-    Remove the option from the configuration.
+    Remove the OPTION from the configuration.
 
     This removes the specified option from the selected configuration file. If
     no configuration file is explicitly selected, this will operate on the
     workspace configuration if ran from within a workspace. Otherwise, this
     will operate on the user configuration.
     """
     with exceptionhandling(context):
```

### Comparing `git_ws-0.9.2/gitws/_cli/dep.py` & `git_ws-1.0.0/gitws/_cli/dep.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -58,15 +58,15 @@
     path=None,
     dep_manifest_path=None,
     groups=None,
     with_groups=None,
     submodules=None,
 ):
     """
-    Add Dependency.
+    Add Dependency NAME.
     """
     with exceptionhandling(context):
         manifest_path = Path(manifest_path)
         manifest_spec = ManifestSpec.load(manifest_path)
         dependencies = list(manifest_spec.dependencies)
         dependencies.append(
             ProjectSpec(name=name).update_fromstr(
@@ -83,34 +83,39 @@
                 }
             )
         )
         manifest_spec = manifest_spec.update(dependencies=dependencies)
         manifest_spec.save(manifest_path)
 
 
+_DEP_ATTRIBUTES = tuple(
+    (item for item in ProjectSpec(name="dummy").dict(by_alias=True) if item not in ("linkfiles", "copyfiles"))
+)
+
+
 @dep.command(name="set")
 @manifest_option(initial=True)
 @click.argument("dep")
-@click.argument("name", type=click.Choice(tuple(ProjectSpec.__fields__)))
+@click.argument("attribute", type=click.Choice(_DEP_ATTRIBUTES))
 @click.argument("value")
 @pass_context
-def set_(context, manifest_path, dep, name, value):
+def set_(context, manifest_path, dep, attribute, value):
     """
-    Set Value For Dependency.
+    Set ATTRIBUTE For Dependency DEP to VALUE.
     """
     with exceptionhandling(context):
         manifest_path = Path(manifest_path)
         manifest_spec = ManifestSpec.load(manifest_path)
         dependencies = list(manifest_spec.dependencies)
         for idx, dependency in enumerate(dependencies):
             if dependency.name == dep:
                 break
         else:
             raise ValueError(f"Unknown dependency {dep!r}")
-        dependencies[idx] = dependencies[idx].update_fromstr({name: value if value else None})
+        dependencies[idx] = dependencies[idx].update_fromstr({attribute: value if value else None})
         manifest_spec = manifest_spec.update(dependencies=dependencies)
         manifest_spec.save(manifest_path)
 
 
 @dep.command(name="list")
 @manifest_option(initial=True)
 @pass_context
@@ -128,15 +133,15 @@
 
 @dep.command()
 @click.argument("name")
 @manifest_option(initial=True)
 @pass_context
 def delete(context, name, manifest_path):
     """
-    Delete Dependency.
+    Delete Dependency NAME.
     """
     with exceptionhandling(context):
         manifest_path = Path(manifest_path)
         manifest_spec = ManifestSpec.load(manifest_path)
         dependencies = list(manifest_spec.dependencies)
         for idx, dep in enumerate(manifest_spec.dependencies):
             if dep.name == name:
```

### Comparing `git_ws-0.9.2/gitws/_cli/info.py` & `git_ws-1.0.0/gitws/_cli/info.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -18,63 +18,82 @@
 
 import click
 from anytree import ContStyle, RenderTree
 
 from gitws import GitWS
 
 from ..deptree import DepDotExporter
+from ..exceptions import NoMainError
 from .common import exceptionhandling, pass_context
 from .options import group_filters_option, manifest_option
 
 
 @click.group()
 def info():
     """
     Git Workspace Information.
     """
 
 
-@info.command()
+@info.command(name="workspace-path")
 @pass_context
 def workspace_path(context):
     """
     Print Path to Workspace.
     """
     with exceptionhandling(context):
         gws = GitWS.from_path()
         click.echo(str(gws.path))
 
 
-@info.command()
+@info.command(name="main-path")
 @pass_context
 def main_path(context):
     """
-    Print Path to Main Git Clone.
+    Print Path to Main Project. This command fails on workspaces without main project.
     """
     with exceptionhandling(context):
         gws = GitWS.from_path()
-        click.echo(str(gws.workspace.main_path))
+        main_path = gws.workspace.main_path
+        if not main_path:
+            raise NoMainError()
+        click.echo(str(main_path))
 
 
-@info.command()
+@info.command(name="base-path")
+@pass_context
+def base_path(context):
+    """
+    Print Path to Main Project Or Workspace.
+
+    Print path to main project on workspaces *with* main project.
+    Print path to workspace on workspaces *without* main project.
+    """
+    with exceptionhandling(context):
+        gws = GitWS.from_path()
+        base_path = gws.workspace.base_path
+        click.echo(str(base_path))
+
+
+@info.command(name="project-paths")
 @manifest_option()
 @group_filters_option()
 @pass_context
 def project_paths(context, manifest_path=None, group_filters=None):
     """
     Print Paths to all git clones.
     """
     with exceptionhandling(context):
         gws = GitWS.from_path(manifest_path=manifest_path, group_filters=group_filters)
         for project in gws.projects():
             project_path = gws.workspace.get_project_path(project)
             click.echo(project_path)
 
 
-@info.command()
+@info.command(name="dep-tree")
 @manifest_option()
 @group_filters_option()
 @click.option("--dot", "-d", "dot", is_flag=True, help="Export DOT Format to be forwarded to graphviz.")
 @click.option("--primary", "-p", is_flag=True, help="Display primary dependencies only.")
 @pass_context
 def dep_tree(context, manifest_path=None, group_filters=None, dot: bool = False, primary: bool = False):
     """
```

### Comparing `git_ws-0.9.2/gitws/_cli/manifest.py` & `git_ws-1.0.0/gitws/_cli/manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `git_ws-0.9.2/gitws/_cli/options.py` & `git_ws-1.0.0/gitws/_cli/options.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -56,29 +56,32 @@
 def force_option():
     """Force Option."""
     return click.option("--force", "-f", is_flag=True, help="Enfore operation.")
 
 
 def group_filters_option(initial=False):
     """Group Filter Option."""
-    if initial:
-        help_ = """\
+    help_ = """\
 Group Filtering.
-TODO: more details.
-The setting becomes default for all successive runs.
+All groups from the main manifest are enabled by default,
+unless deactivated by the `[group-filters]` section or this option.
+This option has the highest precedence and can be specified multiple times.
 """
+    if initial:
+        help_ = f"{help_}The setting becomes default for all successive runs."
     else:
-        help_ = """\
-Group Filtering.
-TODO: more details.
-Initial clone/init filter settings by default.
-"""
+        help_ = f"{help_}Initial clone/init filter settings are used by default."
     return click.option("--group-filter", "-G", "group_filters", metavar="FILTER", multiple=True, help=help_)
 
 
+def unshallow_option():
+    """Convert To A Complete Repository."""
+    return click.option("--unshallow", is_flag=True, help="convert to a complete repository")
+
+
 def reverse_option():
     """Reverse Option."""
     help_ = "Operate in Reverse Order. Start with last dependency instead of main repository."
     return click.option("--reverse", "-R", "reverse", is_flag=True, help=help_)
 
 
 def output_option():
@@ -88,30 +91,50 @@
         "-O",
         "output",
         type=click.Path(dir_okay=False),
         help="Write Manifest to file instead of STDOUT.",
     )
 
 
-def path_option():
-    """Path."""
-    return click.argument("path", nargs=-1, type=click.UNPROCESSED)
+def ws_path_option(nomain: bool = False):
+    """Workspace Path Option."""
+    if nomain:
+        descr = "Workspace Path. Parent directory of main project by default."
+    else:
+        descr = "Workspace Path. Parent directory of main project or current working directory by default."
+    return click.option(
+        "--ws-path",
+        "-w",
+        "ws_path",
+        type=click.Path(file_okay=False),
+        help=descr,
+    )
+
+
+def main_path_option():
+    """Main Repository Path."""
+    return click.argument("main_path", nargs=-1, type=click.UNPROCESSED)
+
+
+def depth_option():
+    """Depth Option."""
+    return click.option("--depth", type=int, help="Create clones shallow of that depth.")
 
 
-def process_path(value) -> Optional[Path]:
-    """Process `path_option`."""
+def process_main_path(value) -> Optional[Path]:
+    """Process ``path_option``."""
     if value:
         if len(value) > 1:
             raise click.UsageError("more than one PATH specified")
         return Path(value[0])
     return None
 
 
 def process_paths(paths) -> Tuple[Path, ...]:
-    """Process `paths_argument`."""
+    """Process ``paths_argument``."""
     return tuple(Path(path) for path in paths)
 
 
 def paths_argument():
     """Paths."""
     return click.argument("paths", nargs=-1, type=click.UNPROCESSED)
```

### Comparing `git_ws-0.9.2/gitws/_cli/remote.py` & `git_ws-1.0.0/gitws/_cli/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -36,15 +36,15 @@
 @remote.command()
 @click.argument("name")
 @click.argument("url_base")
 @manifest_option(initial=True)
 @pass_context
 def add(context, name, url_base, manifest_path):
     """
-    Add Remote.
+    Add Remote NAME with URL_BASE.
     """
     with exceptionhandling(context):
         manifest_path = Path(manifest_path)
         manifest_spec = ManifestSpec.load(manifest_path)
         remotes = list(manifest_spec.remotes)
         remotes.append(Remote(name=name, url_base=url_base))
         manifest_spec = manifest_spec.update(remotes=remotes)
@@ -67,15 +67,15 @@
 
 @remote.command()
 @click.argument("name")
 @manifest_option(initial=True)
 @pass_context
 def delete(context, name, manifest_path):
     """
-    Delete Remote.
+    Delete Remote NAME.
     """
     with exceptionhandling(context):
         manifest_path = Path(manifest_path)
         manifest_spec = ManifestSpec.load(manifest_path)
         remotes = list(manifest_spec.remotes)
         for idx, remote in enumerate(manifest_spec.remotes):
             if remote.name == name:
```

### Comparing `git_ws-0.9.2/gitws/_url.py` & `git_ws-1.0.0/gitws/_url.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -11,22 +11,23 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with Git Workspace. If not, see <https://www.gnu.org/licenses/>.
 
 """Set of URL Helper Functions."""
+from typing import Optional
 from urllib import parse
 
 
-def urljoin(base, url):
+def urljoin(base: Optional[str], url: str) -> str:
     """
-    Resolve a `url` relative to `base`.
+    Resolve a ``url`` relative to ``base``.
 
-    Other than `urllib.parse.urljoin` this function supports relative URLs on SSH.
+    Other than ``urllib.parse.urljoin`` this function supports relative URLs on SSH.
 
     >>> urljoin('https://domain.com/base/repo1.git', 'https://domain.com/base/repo2.git')
     'https://domain.com/base/repo2.git'
     >>> urljoin('https://domain.com/base/repo1.git/', 'repo2.git')
     'https://domain.com/base/repo1.git/repo2.git'
     >>> urljoin('https://domain.com/base/repo1.git', '../repo2.git')
     'https://domain.com/base/repo2.git'
@@ -55,17 +56,17 @@
     baseparsed = parse.urlparse(base)
     httpbase = parse.urlunparse(("http",) + baseparsed[1:])
     joined = parse.urljoin(httpbase, url)
     joinedparsed = parse.urlparse(joined)
     return parse.urlunparse((baseparsed.scheme,) + joinedparsed[1:])
 
 
-def urlsub(base, name):
+def urlsub(base: Optional[str], name: str) -> str:
     """
-    Create sub-url for `name` with suffix of `base`.
+    Create sub-url for ``name`` with suffix of ``base``.
 
     >>> urlsub('https://domain.com/base/repo1', 'repo2')
     'repo2'
     >>> urlsub('https://domain.com/base/repo1.git', 'repo2')
     'repo2.git'
     >>> urlsub('https://domain.com/base/repo1.suffix', 'repo2')
     'repo2.suffix'
@@ -83,15 +84,21 @@
     try:
         _, bsuffix = bname.rsplit(".", 1)
     except ValueError:
         return name
     return f"{name}.{bsuffix}"
 
 
-def strip_user_password(url):
+def is_urlabs(url: str) -> bool:
+    """Is URL absolute."""
+    urlparsed = parse.urlparse(url)
+    return bool(urlparsed.scheme)
+
+
+def strip_user_password(url: str) -> str:
     """
     Strip User and/or Password.
 
     >>> strip_user_password('https://domain.com/base/repo1')
     'https://domain.com/base/repo1'
     >>> strip_user_password('https://user@domain.com/base/repo1')
     'https://domain.com/base/repo1'
```

### Comparing `git_ws-0.9.2/gitws/_util.py` & `git_ws-1.0.0/gitws/_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -26,46 +26,63 @@
 
 _LOGGER = logging.getLogger("git-ws")
 # Dependencies to any gitws module are forbidden here!
 
 
 def run(cmd, cwd=None, capture_output=False, check=True, secho=None):
     """Simplified wrapper around :any:`subprocess.run`."""
-    cwdrel = resolve_relative(cwd) if cwd else None
+    cwdrelstr = str(resolve_relative(cwd)) if cwd else None
     # format errors in red
     stderr = None if capture_output or not secho else subprocess.PIPE
     try:
         result = subprocess.run(cmd, capture_output=capture_output, stderr=stderr, check=check, cwd=cwd)
-        _LOGGER.debug("run(%r, cwd='%s') OK stdout=%r stderr=%r", cmd, cwdrel, result.stdout, result.stderr)
+        _LOGGER.debug("run(%r, cwd=%r) OK stdout=%r stderr=%r", cmd, cwdrelstr, result.stdout, result.stderr)
         if stderr and result.stderr:
             secho(result.stderr.decode("utf-8").rstrip())
         return result
     except subprocess.CalledProcessError as error:
-        _LOGGER.debug("run(%r, cwd='%s') FAILED stdout=%r stderr=%r", cmd, cwdrel, error.stdout, error.stderr)
+        _LOGGER.debug("run(%r, cwd=%r) FAILED stdout=%r stderr=%r", cmd, cwdrelstr, error.stdout, error.stderr)
         if stderr and error.stderr:
             secho(error.stderr.decode("utf-8").rstrip(), fg="red", err=True)
         raise error
 
 
 # pylint: disable=unused-argument
 def no_echo(text: str, err=False, **kwargs):
-    """Just suppress `text`."""
+    """Just suppress ``text``."""
     if err:
-        print(err, file=sys.stderr)
+        print(text, file=sys.stderr)
 
 
 def resolve_relative(path: Path, base: Optional[Path] = None) -> Path:
     """
-    Return resolved `path` relative to `base`.
+    Return resolved ``path`` relative to ``base``.
 
-    :param path (Path): Path
-    :param base (Path): Base Path. Current Working Directory by default.
+    Args:
+        path: Path
+
+    Keyword Args:
+        base: Base Path. Current Working Directory by default.
     """
     base = (base or Path.cwd()).resolve()
     path = (base / path).resolve()
+    return relative(path, base)
+
+
+def relative(path: Path, base: Optional[Path] = None) -> Path:
+    """
+    Return ``path`` relative to ``base``.
+
+    Args:
+        path: Path
+
+    Keyword Args:
+        base: Base Path. Current Working Directory by default.
+    """
+    base = base or Path.cwd()
     try:
         return path.relative_to(base)
     except ValueError:
         # Try to determine a relative path, which is save
         relpath = Path(os.path.relpath(path, start=base))
         abspath = (base / relpath).resolve()
         if path == abspath:
```

### Comparing `git_ws-0.9.2/gitws/appconfig.py` & `git_ws-1.0.0/gitws/appconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -123,16 +123,16 @@
     In case the current directory is not within a workspace (and no path to a
     workspace has been explicitly set in the constructor), the workspace configuration file
     is skipped. In any case, the configurations are merged in that order, i.e. options from the
     system configuration file have the lowest priority, while the ones from the workspace have
     highest priority.
 
     On top, the class will also evaluate environment variables named `GIT_WS_*` and allow overriding
-    configuration values that way. For example, the `manifest_path` option can be explicitly overridden by
-    setting the `GIT_WS_MANIFEST_PATH` environment variable.
+    configuration values that way. For example, the ``manifest_path`` option can be explicitly overridden by
+    setting the ``GIT_WS_MANIFEST_PATH`` environment variable.
 
     Keyword Args:
 
         system_config_dir: The path to where the system configuration file is stored. If not set, a platform specific
                            system configuration path will be used.
         user_config_dir: The path to where the user configuration file is stored. If not set, a platform specific
                            user configuration path will be used.
```

### Comparing `git_ws-0.9.2/gitws/clone.py` & `git_ws-1.0.0/gitws/clone.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -11,20 +11,21 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with Git Workspace. If not, see <https://www.gnu.org/licenses/>.
 
 """
-Clone.
+A Clone.
 
 A :any:`Clone` is just the assembly of a :any:`Project` and its corresponding git interface (:any:`Git`).
 """
 
 import logging
+from contextlib import suppress
 from pathlib import Path
 from typing import Generator, List, Optional, Tuple
 
 from ._util import get_repr
 from .appconfig import AppConfig
 from .datamodel import Project
 from .git import Git
@@ -32,65 +33,87 @@
 
 _LOGGER = logging.getLogger("git-ws")
 
 
 class Clone:
 
     """
-    Clone - A Pair Of Project And Git Interface.
+    Clone - A Pair Of Project Definition And Git Interface.
 
     Args:
-        project: Project
-        git: Git.
+        project: Project Definition.
+        git: Git Interface.
     """
 
     def __init__(self, project: Project, git: Git):
         self.project = project
         self.git = git
 
     @staticmethod
     def from_project(workspace: Workspace, project: Project, secho=None) -> "Clone":
-        """Create :any:`Clone` for `project` in `workspace`."""
+        """Create :any:`Clone` for ``project`` in ``workspace``."""
         project_path = workspace.get_project_path(project, relative=True)
         clone_cache = AppConfig().options.clone_cache
         git = Git(project_path, clone_cache=clone_cache, secho=secho)
         return Clone(project, git)
 
-    def check(self, exists=True, diff=True, no_revision=True):
+    def check(self, exists=True, diff=True):
         """
-        Check Clone.
+        Check Clone And Emit Warnings On Logger.
+
+        The following checks are processed:
+
+        * Check that the git clone exists (if ``exists=True``).
+        * Check that the actual git clone revision matches the ``project.revision`` (if ``diff=True``).
+        * The revision check is skipped on the main project.
 
         Keyword Args:
             exists: Check if cloned.
             diff: Check if revisions differ
-            no_revision: No revision specification.
         """
+        # exists
         if exists:
             self.git.check()
         project = self.project
-        projectrev = project.revision
-        if projectrev:
+        info = project.info
+        # revision
+        if project.revision:
             if diff:
-                try:
+                clonerev = None
+                with suppress(FileNotFoundError):
                     clonerev = self.git.get_revision()
-                except FileNotFoundError:
-                    clonerev = None
-                if clonerev and projectrev != clonerev:
-                    _LOGGER.warning("Clone %s is on different revision: %r", project.info, clonerev)
+                if clonerev and project.revision != clonerev:
+                    _LOGGER.warning("Clone %s is on different revision: %r", info, clonerev)
         elif not project.is_main:
-            if no_revision:
-                _LOGGER.warning("Clone %s has no revision!", project.info)
+            _LOGGER.warning("Clone %s has no revision!", info)
+        # URL
+        if diff and project.url:
+            cloneurl = None
+            with suppress(FileNotFoundError):
+                cloneurl = self.git.get_url()
+            if project.url != cloneurl:
+                if cloneurl:
+                    _LOGGER.warning("Clone %s remote origin is %r but intends to be: %r", info, cloneurl, project.url)
+                else:
+                    _LOGGER.warning("Clone %s has no remote origin but intends to be: %r", info, project.url)
 
     def __repr__(self):
         return get_repr(self, (self.project, self.git))
 
     @property
     def info(self):
         """
         `repr`-like info string but more condensed.
+
+        >>> import gitws
+        >>> project = gitws.Project(name='pname', path='ppath', revision='prevision')
+        >>> git = gitws.Git('gpath')
+        >>> clone = gitws.Clone(project, git)
+        >>> clone.info
+        "gpath ('pname', revision='prevision')"
         """
         project = self.project
         path = str(self.git.path)
         options = get_repr(
             args=(project.name,),
             kwargs=(
                 ("revision", project.revision, None),
@@ -104,20 +127,20 @@
 
 
 ClonePaths = Tuple[Clone, Tuple[Path, ...]]
 
 
 def map_paths(clones: Tuple[Clone, ...], paths: Optional[Tuple[Path, ...]]) -> Generator[ClonePaths, None, None]:
     """
-    Map `paths` to `clones`.
+    Map ``paths`` to ``clones``.
 
-    Associate the given `paths` to the corresponding `clones`.
+    Associate the given ``paths`` to the corresponding ``clones``.
 
-    If `paths` is not empty, the corresponding clone and paths pairs are yielded.
-    If `paths` is empty, just all clones with an empty paths tuple are yielded.
+    * If ``paths`` is not empty, the corresponding clone and paths pairs are yielded.
+    * If ``paths`` is empty, just all clones with an empty paths tuple are yielded.
     """
     if paths:
         clonepaths: Tuple[Tuple[Clone, List[Path]], ...] = tuple((clone, []) for clone in clones)
         # We operate on the absolute paths, but keep track of the specified ones.
         origpaths: List[Path] = list(paths)
         abspaths: List[Path] = [path.resolve() for path in paths]
         # Start path matching at the clones with the deepest folder
```

### Comparing `git_ws-0.9.2/gitws/const.py` & `git_ws-1.0.0/gitws/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -18,15 +18,15 @@
 
 from pathlib import Path
 
 GIT_WS_PATH = Path(".git-ws")
 """
 The sub-folder in which the tool stores workspace related data.
 
-This path is relative to the workspace folder or the main project root.
+This path is relative to the workspace folder.
 """
 
 MANIFESTS_PATH = GIT_WS_PATH / "manifests"
 
 CONFIG_FILE_NAME = "config.toml"
 """Name of the config file in the :any:`GIT_WS_PATH`."""
```

### Comparing `git_ws-0.9.2/gitws/datamodel.py` & `git_ws-1.0.0/gitws/datamodel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -13,42 +13,43 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with Git Workspace. If not, see <https://www.gnu.org/licenses/>.
 
 """
 Central :any:`GitWS` Datamodel.
 
-* :any:`Group`: Dependency Group. A string.
-* :any:`Groups`: Tuple of Group instances.
-* :any:`GroupFilter`: Group Filter Specification. A string.
-* :any:`GroupFilters`: Tuple of GroupFilter instances.
+* :any:`Group`: Dependency Group. A string (i.e. 'test').
+* :any:`Groups`: Tuple of :any:`Group` instances.
+* :any:`GroupFilter`: Group Filter Specification. A string (i.e. '+test@path').
+* :any:`GroupFilters`: Tuple of :any:`GroupFilter` instances.
 * :any:`GroupSelect`: Group Selection. A converted :any:`GroupFilter` as needed by :any:`GitWS`.
-* :any:`GroupSelects`: Tuple of GroupSelect instances.
-* :any:`Remote`: Remote Alias.
-* :any:`Defaults`: Default Values.
-* :any:`ProjectSpec`: Dependency Specification from Manifest File.
-* :any:`Project`: A Single Dependency as needed by :any:`GitWS`.
-* :any:`ManifestSpec`: Specification of the actual project.
-* :any:`Manifest`: Manifest as needed by :any:`GitWS`.
+* :any:`GroupSelects`: Tuple of :any:`GroupSelect` instances.
+* :any:`ManifestSpec`: Manifest specification for the actual project.
+* :any:`Manifest`: Manifest as needed by :any:`GitWS` derived from :any:`ManifestSpec`.
+* :any:`ProjectSpec`: Dependency Specification in :any:`ManifestSpec`.
+* :any:`Project`: A Single Dependency as needed by :any:`GitWS` derived from :any:`ProjectSpec`.
+* :any:`Remote`: Remote Alias in :any:`ManifestSpec`.
+* :any:`Defaults`: Default Values in :any:`ManifestSpec`.
 * :any:`AppConfigData`: :any:`GitWS` Configuration.
 """
 
+# pylint: disable=too-many-lines
 
 import re
 from pathlib import Path
-from typing import Any, Dict, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
 import tomlkit
 from pydantic import BaseSettings, Extra, Field, root_validator, validator
 
 from ._basemodel import BaseModel
-from ._url import urljoin, urlsub
+from ._url import is_urlabs, urljoin, urlsub
 from ._util import add_comment, add_info, as_dict, get_repr, resolve_relative
 from .const import MANIFEST_PATH_DEFAULT
-from .exceptions import ManifestError, ManifestNotFoundError
+from .exceptions import ManifestError, ManifestNotFoundError, NoAbsUrlError
 
 _RE_GROUP = re.compile(r"\A[a-zA-Z0-9_][a-zA-Z0-9_\-]*\Z")
 
 ProjectPaths = Tuple[
     str,
 ]
 
@@ -63,15 +64,15 @@
 """
 
 
 def validate_group(group):
     """
     Validate Group.
 
-    Group is just a `str` for performance reasons. This function does the validation.
+    Group is just a ``str`` for performance reasons. This function does the validation.
     """
     mat = _RE_GROUP.match(group)
     if not mat:
         raise ValueError(f"Invalid group {group!r}")
 
 
 class Groups(tuple):
@@ -79,18 +80,19 @@
     """Groups."""
 
     @staticmethod
     def validate(groups):
         """
         Validate Groups.
 
-        Groups are just a `tuple` of `str` for performance reasons. This function does the validation.
+        Groups are just a ``tuple`` of ``str`` for performance reasons. This function does the validation.
         """
         for group in groups:
             validate_group(group)
+        return groups
 
 
 _RE_GROUP_FILTER = re.compile(r"\A(?P<select>[\-\+])(?P<group>[a-zA-Z0-9_][a-zA-Z0-9_\-]*)?(@(?P<path>.+))?\Z")
 
 GroupFilter = str
 """
 Group Filter.
@@ -102,15 +104,15 @@
 """
 
 
 def validate_group_filter(group_filter):
     """
     Groups Filter.
 
-    Group Filters are just a `tuple` of `str` for performance reasons. This function does the validation.
+    Group Filters are just a ``tuple`` of ``str`` for performance reasons. This function does the validation.
     """
     mat = _RE_GROUP_FILTER.match(group_filter)
     if not mat:
         raise ValueError(f"Invalid group filter {group_filter!r}")
 
 
 class GroupFilters(tuple):
@@ -121,18 +123,19 @@
     """
 
     @staticmethod
     def validate(group_filters):
         """
         Check Groups Filter.
 
-        Group Filters are just a `tuple` of `str` for performance reasons. This function does the validation.
+        Group Filters are just a ``tuple`` of ``str`` for performance reasons. This function does the validation.
         """
         for group_filter in group_filters:
             validate_group_filter(group_filter)
+        return group_filters
 
 
 class GroupSelect(BaseModel):
 
     """
     Group Selection.
 
@@ -143,29 +146,31 @@
         group: Group Name.
         path: Path.
     """
 
     group: Optional[Group] = None
     """Group."""
     select: bool
-    """Selected or not."""
+    """Selected ('+') or not ('-')."""
     path: Optional[str] = None
     """Path."""
 
     @staticmethod
     def from_group_filter(group_filter) -> "GroupSelect":
         """
-        Create Group Selection from `group_filter`.
+        Create Group Selection from ``group_filter``.
 
         >>> GroupSelect.from_group_filter("+test")
         GroupSelect(group='test', select=True)
         >>> GroupSelect.from_group_filter("-test")
         GroupSelect(group='test', select=False)
         >>> GroupSelect.from_group_filter("-test@path")
         GroupSelect(group='test', select=False, path='path')
+        >>> GroupSelect.from_group_filter("-@path")
+        GroupSelect(select=False, path='path')
         >>> GroupSelect.from_group_filter("te-st")
         Traceback (most recent call last):
             ...
         ValueError: Invalid group selection 'te-st'
         """
         mat = _RE_GROUP_FILTER.match(group_filter)
         if not mat:
@@ -178,20 +183,20 @@
         select = "+" if self.select else "-"
         path = f"@{self.path}" if self.path else ""
         return f"{select}{self.group}{path}"
 
 
 class GroupSelects(tuple):
 
-    """Collection from :any:`GroupSelect`."""
+    """Collection of :any:`GroupSelect`."""
 
     @staticmethod
     def from_group_filters(group_filters: Optional[GroupFilters] = None) -> "GroupSelects":
         """
-        Creage :any:`GroupSelects` from `group_filters`.
+        Create :any:`GroupSelects` from ``group_filters``.
 
         >>> GroupSelects.from_group_filters()
         ()
         >>> GroupSelects.from_group_filters(('', ))
         ()
         >>> GroupSelects.from_group_filters(('+test', ))
         (GroupSelect(group='test', select=True),)
@@ -201,15 +206,15 @@
         group_filters = group_filters or GroupFilters()
         items = [item.strip() for item in group_filters]
         return GroupSelects(GroupSelect.from_group_filter(item) for item in items if item)
 
     @staticmethod
     def from_groups(groups: Optional[Groups] = None) -> "GroupSelects":
         """
-        Creage :any:`GroupSelects` from `group_filters`.
+        Create :any:`GroupSelects` from ``group_filters``.
 
         >>> GroupSelects.from_groups()
         ()
         >>> GroupSelects.from_groups(('', ))
         ()
         >>> GroupSelects.from_groups(('test', ))
         (GroupSelect(group='test', select=True),)
@@ -219,15 +224,15 @@
         groups = groups or Groups()
         items = [item.strip() for item in groups]
         return GroupSelects(GroupSelect(group=item, select=True) for item in items if item)
 
 
 class Remote(BaseModel, allow_population_by_field_name=True):
     """
-    Remote Alias.
+    Remote Alias - Remote URL Helper.
 
     Args:
         name: Remote Name
 
     Keyword Args:
         url_base: Base URL. Optional.
     """
@@ -235,19 +240,19 @@
     name: str
     """The Name of the Remote. Must be unique within Manifest."""
 
     url_base: str = Field(None, alias="url-base")
     """URL to a directory of repositories."""
 
 
-class Defaults(BaseModel):
+class Defaults(BaseModel, allow_population_by_field_name=True):
     """
     Default Values.
 
-    These default values are used, if the project does not specify them.
+    These default values are used, if a :any:`ProjectSpec` does not specify them.
 
     Keyword Args:
         remote: Remote Name.
         revision: Revision. Tag or Branch. SHA does not make sense here.
         groups: Dependency Groups.
         with_groups: Group Selection for refered projects.
     """
@@ -255,88 +260,134 @@
     remote: Optional[str] = None
     """Remote name if not specified by the dependency. The remote must have been defined previously."""
 
     revision: Optional[str] = None
     """The revision if not specified by the dependency. Tag or Branch. SHA does not make sense here."""
 
     groups: Optional[Groups] = Groups()
-    """The `groups` if not specified by the dependency."""
+    """The ``groups`` attribute if not specified by the dependency."""
 
-    with_groups: Optional[Groups] = Groups()
-    """The `with_groups` if not specified by the dependency."""
+    with_groups: Optional[Groups] = Field(Groups(), alias="with-groups")
+    """The ``with_groups`` attribute if not specified by the dependency."""
 
     submodules: bool = True
-    """Initialize and Update `git submodules`."""
+    """Initialize and Update `git submodules`. `True` by default."""
+
+    @validator("groups", allow_reuse=True)
+    def _groups(cls, values):
+        # pylint: disable=no-self-argument
+        return Groups.validate(values)
+
+    @validator("with_groups", allow_reuse=True)
+    def _with_groups(cls, values):
+        # pylint: disable=no-self-argument
+        return Groups.validate(values)
+
+
+class FileRef(BaseModel):
+    """
+    File Reference (Symbolic Link or File to Copy).
+
+    File Reference to Workspace from Project.
+
+    Keyword Args:
+        src: Source - relative path to the project directory.
+        dest: Destination - relative path to the workspace directory.
+    """
+
+    src: str
+    """Source - relative path to the project directory."""
+
+    dest: str
+    """Destination - relative path to the workspace directory."""
+
+
+FileRefs = Tuple[FileRef, ...]
+ProjectFileRefs = Dict[str, FileRefs]
+FileRefsMutable = List[FileRef]
+ProjectFileRefsMutable = Dict[str, FileRefsMutable]
 
 
 class Project(BaseModel, allow_population_by_field_name=True):
 
     """
     Project.
 
     A project describes a dependency.
 
     Args:
         name: Name.
         path: Project Filesystem Path. Relative to Workspace Root Directory.
 
     Keyword Args:
-        url: URL. Assembled from `remote`s `url_base`, `sub_url` and/or `name`.
+        url: URL. Assembled from ``remote`` s ``url_base``, ``sub_url`` and/or ``name``.
         revision: Revision to be checked out. Tag, branch or SHA.
-        manifest_path: Path to manifest. Relative to ProjectSpec Filesystem Path. `git-ws.toml` by default.
+        manifest_path: Path to the manifest file. Relative to ``path`` of project. ``git-ws.toml`` by default.
         groups: Dependency Groups.
         with_groups: Group Selection for refered project.
+        submodules: initialize and update `git submodules`
+        linkfiles: symbolic links to be created in the workspace
+        copyfiles: files to be created in the workspace
         is_main: Project is Main Project.
 
     The :any:`ProjectSpec` represents the User Interface. The options which can be specified in the manifest file.
     The :any:`Project` is the resolved version of :any:`ProjectSpec` with all calculated information needed by
     :any:`GitWS` to operate.
 
     :any:`Project.from_spec()` resolves a :any:`ProjectSpec` into a :any:`Project`.
     :any:`ProjectSpec.from_project()` does the reverse.
+
+    .. note::
+        :any:`Project.from_spec()` resolves some attributes irreversible.
+        So ``Project.from_spec(ProjectSpec.from_project())`` will not
+        return the original project.
     """
 
     name: str
     """Dependency Name."""
 
     path: str
-    """Dependency Path. `name` will be used as default."""
+    """Dependency Path. ``name`` will be used as default."""
 
     url: Optional[str] = None
-    """URL. Assembled from `remote`s `url_base`, `sub_url` and/or `name`."""
+    """URL. Assembled from ``remote`` s ``url_base``, ``sub_url`` and/or ``name``."""
 
     revision: Optional[str] = None
     """Revision to be checked out. Tag, branch or SHA."""
 
     manifest_path: str = str(MANIFEST_PATH_DEFAULT)
-    """Path to the manifest file. Relative to `path`."""
+    """Path to the manifest file. Relative to ``path`` of project. ``git-ws.toml`` by default."""
 
     groups: Groups = Groups()
     """Dependency Groups."""
 
     with_groups: Groups = Field(Groups(), alias="with-groups")
-    """Group Selection for refered project."""
+    """Group Selection for referred project."""
 
     submodules: bool = True
     """Initialize and Update `git submodules`."""
 
+    linkfiles: Tuple[FileRef, ...] = tuple()
+    """Symbolic Links To Be Created In The workspace."""
+
+    copyfiles: Tuple[FileRef, ...] = tuple()
+    """Files To Be Created In The Workspace."""
+
     is_main: bool = False
     """Project is the main project."""
 
     @validator("groups", allow_reuse=True)
     def _groups(cls, values):
-        # pylint: disable=no-self-argument,no-self-use
-        Groups.validate(values)
-        return values
+        # pylint: disable=no-self-argument
+        return Groups.validate(values)
 
     @validator("with_groups", allow_reuse=True)
     def _with_groups(cls, values):
-        # pylint: disable=no-self-argument,no-self-use
-        Groups.validate(values)
-        return values
+        # pylint: disable=no-self-argument
+        return Groups.validate(values)
 
     @property
     def info(self):
         """
         `repr`-like info string but more condensed.
 
         >>> Project(name='name', path='name').info
@@ -363,34 +414,37 @@
         return self.name
 
     @staticmethod
     def from_spec(
         manifest_spec: "ManifestSpec", spec: "ProjectSpec", refurl: Optional[str] = None, resolve_url: bool = False
     ) -> "Project":
         """
-        Create :any:`Project` from `manifest_spec` and `spec`.
+        Create :any:`Project` from ``manifest_spec`` and ``spec``.
 
         Args:
             manifest_spec: Manifest Specification.
             spec: Base project to be resolved.
 
         Keyword Args:
-            refurl: Remote URL of the `manifest_spec`. If specified, relative URLs are resolved.
+            refurl: Remote URL of the ``manifest_spec``.
             resolve_url: Resolve URLs to absolute ones.
 
+        Raises:
+            NoAbsUrlError: On ``resolve_url=True`` if ``refurl`` is ``None`` and project uses a relative URL.
+
         :any:`Project.from_spec()` resolves a :any:`ProjectSpec` into a :any:`Project`.
         :any:`ProjectSpec.from_project()` does the reverse.
         """
-        assert not resolve_url or refurl, "resolve_url requires refurl"
         defaults = manifest_spec.defaults
         remotes = manifest_spec.remotes
         project_groups = spec.groups or defaults.groups
         project_with_groups = spec.with_groups or defaults.with_groups
-        url = spec.url
         submodules = spec.submodules if spec.submodules is not None else defaults.submodules
+        # URL
+        url = spec.url
         if not url:
             # URL assembly
             project_remote = spec.remote or defaults.remote
             project_sub_url = spec.sub_url or urlsub(refurl, spec.name)
             if project_remote:
                 for remote in remotes:
                     if remote.name == project_remote:
@@ -398,200 +452,221 @@
                         break
                 else:
                     raise ValueError(f"Unknown remote {spec.remote} for project {spec.name}")
             else:
                 url = f"../{project_sub_url}"
 
         # Resolve relative URLs.
-        if resolve_url:
+        if resolve_url and not is_urlabs(url):
+            if not refurl:
+                raise NoAbsUrlError(spec.name)
             url = urljoin(refurl, url)
+
+        # Create
         return Project(
             name=spec.name,
             path=spec.path or spec.name,
             url=url,
             revision=spec.revision or defaults.revision,
             manifest_path=spec.manifest_path,
             groups=project_groups,
             with_groups=project_with_groups,
             submodules=submodules,
+            linkfiles=spec.linkfiles,
+            copyfiles=spec.copyfiles,
         )
 
 
 class ProjectSpec(BaseModel, allow_population_by_field_name=True):
     """
     Project Dependency Specification
 
     A project specifies the reference to a repository.
 
     Args:
         name: Name.
 
     Keyword Args:
-        remote: Remote Alias
+        remote: Remote Alias - Remote URL Helper
         sub_url: URL relative to :any:`Remote.url_base`.
         url: URL
         revision: Revision
         path: Project Filesystem Path. Relative to Workspace Root Directory.
-        manifest_path: Path to manifest. Relative to ProjectSpec Filesystem Path. `git-ws.toml` by default.
+        manifest_path: Path to the manifest file. Relative to ``path`` of project. ``git-ws.toml`` by default.
         groups: Dependency Groups.
         with_groups: Group Selection for refered project.
+        submodules: initialize and update `git submodules`
+        linkfiles: symbolic links to be created in the workspace
+        copyfiles: files to be created in the workspace
 
     Some parameters are restricted:
 
-    * `remote` and `url` are mutually exclusive.
-    * `url` and `sub-url` are likewise mutually exclusive
-    * `sub-url` requires a `remote`.
+    * ``remote`` and ``url`` are mutually exclusive.
+    * ``url`` and ``sub-url`` are likewise mutually exclusive
+    * ``sub-url`` requires a ``remote``.
 
     The :any:`ProjectSpec` represents the User Interface. The options which can be specified in the manifest file.
     The :any:`Project` is the resolved version of :any:`ProjectSpec` with all calculated information needed by
     :any:`GitWS` to operate.
-
-    :any:`Project.from_spec()` resolves a :any:`ProjectSpec` into a :any:`Project`.
-    :any:`ProjectSpec.from_project()` does the reverse.
     """
 
     name: str
     """Dependency Name."""
 
     remote: Optional[str] = None
-    """Remote Alias Name. The `remote` must have been defined previously."""
+    """Remote Alias Name. The ``remote`` must have been defined previously."""
 
     sub_url: Optional[str] = Field(None, alias="sub-url")
-    """Relative URL to `remote`s `url_base` OR the URL of the manifest file."""
+    """Relative URL to ``remote`` s ``url_base`` OR the URL of the manifest file."""
 
     url: Optional[str] = None
     """Absolute URL."""
 
     revision: Optional[str] = None
     """Revision to be checked out."""
 
     path: Optional[str] = None
-    """Path within workspace. `name` will be used as default."""
+    """Path within workspace. ``name`` will be used as default."""
 
     manifest_path: Optional[str] = Field(str(MANIFEST_PATH_DEFAULT), alias="manifest-path")
-    """Path to the manifest file. Relative to `path`."""
+    """Path to the manifest file. Relative to ``path`` of project. ``git-ws.toml`` by default."""
 
     groups: Groups = Groups()
     """Dependency Groups."""
 
     with_groups: Groups = Field(Groups(), alias="with-groups")
     """Group Selection for refered project."""
 
     submodules: Optional[bool] = None
     """Initialize and Update `git submodules`."""
 
+    linkfiles: Tuple[FileRef, ...] = tuple()
+    """Symbolic Links To Be Created In The Workspace."""
+
+    copyfiles: Tuple[FileRef, ...] = tuple()
+    """Files To Be Created In The Workspace."""
+
     @root_validator(allow_reuse=True)
     def _remote_or_url(cls, values):
-        # pylint: disable=no-self-argument,no-self-use
+        # pylint: disable=no-self-argument
         remote = values.get("remote", None)
         sub_url = values.get("sub_url", None)
         url = values.get("url", None)
         if remote and url:
             raise ValueError("'remote' and 'url' are mutually exclusive")
         if url and sub_url:
             raise ValueError("'url' and 'sub-url' are mutually exclusive")
         if sub_url and not remote:
             raise ValueError("'sub-url' requires 'remote'")
         return values
 
     @validator("groups", allow_reuse=True)
     def _groups(cls, values):
-        # pylint: disable=no-self-argument,no-self-use
-        Groups.validate(values)
-        return values
+        # pylint: disable=no-self-argument
+        return Groups.validate(values)
 
     @validator("with_groups", allow_reuse=True)
     def _with_groups(cls, values):
-        # pylint: disable=no-self-argument,no-self-use
-        Groups.validate(values)
-        return values
+        # pylint: disable=no-self-argument
+        return Groups.validate(values)
 
     @staticmethod
     def from_project(project: Project) -> "ProjectSpec":
         """
-        Create :any:`ProjectSpec` from `project`.
+        Create :any:`ProjectSpec` from ``project``.
 
         Args:
             project: The source :any:`Project`.
 
-        ..note::
+        .. note::
             :any:`Project.from_spec()` resolves some attributes irreversible.
             So ``Project.from_spec(ProjectSpec.from_project())`` will not
             return the original project.
         """
         return ProjectSpec(
             name=project.name,
             path=project.path,
             url=project.url,
             revision=project.revision,
             manifest_path=project.manifest_path,
             groups=project.groups,
             with_groups=project.with_groups,
             submodules=project.submodules,
+            linkfiles=project.linkfiles,
+            copyfiles=project.copyfiles,
         )
 
 
 class Manifest(BaseModel, extra=Extra.allow, allow_population_by_field_name=True):
 
     """
-    Manifest.
+    The Manifest.
 
     A manifest describes the actual project and its dependencies.
 
     Keyword Args:
-        group_filters. Group Filtering.
+        group_filters: Group Filtering.
+        linkfiles: symbolic links to be created in the workspace
+        copyfiles: files to be created in the workspace
         dependencies: Dependency Projects.
         path: Filesystem Path. Relative to Workspace Root Directory.
 
     The :any:`ManifestSpec` represents the User Interface. The options which can be specified in the manifest file.
     The :any:`Manifest` is the resolved version of :any:`ManifestSpec` with all calculated information needed by
     :any:`GitWS` to operate.
 
     :any:`Manifest.from_spec()` resolves a :any:`ManifestSpec` into a :any:`Manifest`.
     """
 
     group_filters: GroupFilters = Field(GroupFilters(), alias="group-filters")
-    """Group Filtering."""
+    """Default Group Selection and Deselection."""
+
+    linkfiles: Tuple[FileRef, ...] = tuple()
+    """Symbolic Links To Be Created In The Workspace."""
+
+    copyfiles: Tuple[FileRef, ...] = tuple()
+    """Files To Be Created In The Workspace."""
 
     dependencies: Tuple[Project, ...] = tuple()
-    """Dependencies."""
+    """Dependencies - Other Projects To Be Cloned In The Workspace."""
 
     path: Optional[str] = None
     """Path to the manifest file, relative to project path."""
 
     @validator("group_filters", allow_reuse=True)
     def _group_filters(cls, values):
-        # pylint: disable=no-self-argument,no-self-use
-        GroupFilters.validate(values)
-        return values
+        # pylint: disable=no-self-argument
+        return GroupFilters.validate(values)
 
     @staticmethod
     def from_spec(
         spec: "ManifestSpec", path: Optional[str] = None, refurl: Optional[str] = None, resolve_url: bool = False
     ) -> "Manifest":
         """
         Create :any:`Manifest` from :any:`ManifestSpec`.
 
         Args:
             spec: The source :any:`ManifestSpec`.
 
         Keyword Args:
-            path: File path of the `spec`.
-            refurl: URL of the repository containing `spec`.
-            resolve_url: Convert relative to absolute URLs. Requires `refurl`.
+            path: File path of the ``spec``.
+            refurl: URL of the repository containing ``spec``.
+            resolve_url: Convert relative to absolute URLs. Requires ``refurl``.
 
-        If `refurl` is specified, any relative URL in the :any:`ManifestSpec` and referred :any:`ProjectSpec` s
-        are resolved to a absolute URLs.
+        Raises:
+            NoAbsUrlError: On ``resolve_url=True`` if ``refurl`` is ``None`` and project uses a relative URL.
         """
         dependencies = [
             Project.from_spec(spec, project_spec, refurl=refurl, resolve_url=resolve_url)
             for project_spec in spec.dependencies
         ]
         return Manifest(
             group_filters=spec.group_filters,
+            linkfiles=spec.linkfiles,
+            copyfiles=spec.copyfiles,
             dependencies=dependencies,
             path=path,
         )
 
 
 class ManifestSpec(BaseModel, allow_population_by_field_name=True):
 
@@ -603,74 +678,81 @@
     The :any:`ManifestSpec` represents the User Interface. The options which can be specified in the manifest file.
     The :any:`Manifest` is the resolved version of :any:`ManifestSpec` with all calculated information needed by
     :any:`GitWS` to operate.
 
     Keyword Args:
         version: Version String. Actually 1.0.
         remotes: Remote Aliases.
-        group_filters. Group Filtering.
+        group_filters: Group Filtering.
+        linkfiles: symbolic links to be created in the workspace
+        copyfiles: files to be created in the workspace
         defaults: Default settings.
         dependencies: Dependency Projects.
     """
 
     version: str = Field(default="1.0")
     """
     Manifest Version Identifier.
 
-    Actual Version: `1.0`.
+    Actual Version: ``1.0``.
     """
 
-    remotes: Tuple[Remote, ...] = tuple()
-    """Remotes."""
-
     group_filters: GroupFilters = Field(GroupFilters(), alias="group-filters")
-    """Group Filtering."""
+    """Default Group Selection and Deselection."""
+
+    linkfiles: Tuple[FileRef, ...] = tuple()
+    """Symbolic Links To Be Created In The Workspace."""
+
+    copyfiles: Tuple[FileRef, ...] = tuple()
+    """Files To Be Created In The Workspace."""
+
+    remotes: Tuple[Remote, ...] = tuple()
+    """Remotes - Helpers to Simplify URL Handling."""
 
     defaults: Defaults = Defaults()
     """Default Values."""
 
     dependencies: Tuple[ProjectSpec, ...] = tuple()
-    """Dependencies."""
+    """Dependencies - Other Projects To Be Cloned In The Workspace."""
 
     @root_validator(allow_reuse=True)
     def _remotes_unique(cls, values):
-        # pylint: disable=no-self-argument,no-self-use
+        # pylint: disable=no-self-argument
         names = set()
         for remote in values.get("remotes", None) or []:
             name = remote.name
             if name not in names:
                 names.add(name)
             else:
                 raise ValueError(f"Remote name {name!r} is used more than once")
         return values
 
     @root_validator(allow_reuse=True)
     def _deps_unique(cls, values):
-        # pylint: disable=no-self-argument,no-self-use
+        # pylint: disable=no-self-argument
         names = set()
         for dep in values.get("dependencies", None) or []:
             name = dep.name
             if name not in names:
                 names.add(name)
             else:
                 raise ValueError(f"Dependency name {name!r} is used more than once")
         return values
 
     @validator("group_filters", allow_reuse=True)
     def _group_filters(cls, values):
-        # pylint: disable=no-self-argument,no-self-use
-        GroupFilters.validate(values)
-        return values
+        # pylint: disable=no-self-argument
+        return GroupFilters.validate(values)
 
     @classmethod
     def load(cls, path: Path) -> "ManifestSpec":
         """
-        Load :any:`ManifestSpec` from `path`.
+        Load :any:`ManifestSpec` from ``path``.
 
-        The file referenced by `path` must be a TOML file according to the manifest scheme.
+        The file referenced by ``path`` must be a TOML file according to the manifest scheme.
 
         Raises:
             ManifestNotFoundError: if file is not found
             ManifestError: On syntax or data scheme errors.
         """
         try:
             content = path.read_text()
@@ -686,20 +768,113 @@
     def dump(
         self, doc: Optional[tomlkit.TOMLDocument] = None, path: Optional[Path] = None, minimal: bool = False
     ) -> str:
         """
         Return :any:`ManifestSpec` as string.
 
         The output will include an inline documentation of all available options.
-        If `doc` or `path` are specified, any additional attributes and comments are **kept**.
+        If ``doc`` or ``path`` are specified, any additional attributes and comments are **kept**.
 
         Keyword Args:
             doc: Existing document to be updated.
             path: Path to possibly existing document.
             minimal: Skip unset
+
+        >>> print(ManifestSpec(defaults=Defaults(revision='main'), dependencies=(ProjectSpec(name='mylib'),)).dump())
+        version = "1.0"
+        ##
+        ## Git Workspace's Manifest. Please see the documentation at:
+        ##
+        ## https://git-ws.readthedocs.io/en/latest/manual/manifest.html
+        ##
+        <BLANKLINE>
+        <BLANKLINE>
+        # group-filters = ["-doc", "-feature@path"]
+        group-filters = []
+        <BLANKLINE>
+        <BLANKLINE>
+        # [[remotes]]
+        # name = "myremote"
+        # url-base = "https://github.com/myuser"
+        <BLANKLINE>
+        <BLANKLINE>
+        [defaults]
+        revision = "main"
+        <BLANKLINE>
+        # remote = "myserver"
+        # revision = "main"
+        # groups = ["test"]
+        # with-groups = ["doc"]
+        <BLANKLINE>
+        <BLANKLINE>
+        ## A full flavored dependency using a 'remote':
+        # [[dependencies]]
+        # name = "myname"
+        # remote = "remote"
+        # sub-url = "my.git"
+        # revision = "main"
+        # path = "mydir"
+        # groups = ["group"]
+        #
+        # [[dependencies.linkfiles]]
+        # src = "file0-in-mydir.txt"
+        # dest = "link0-in-workspace.txt"
+        #
+        # [[dependencies.linkfiles]]
+        # src = "file1-in-mydir.txt"
+        # dest = "link1-in-workspace.txt"
+        #
+        # [[dependencies.copyfiles]]
+        # src = "file0-in-mydir.txt"
+        # dest = "file0-in-workspace.txt"
+        #
+        # [[dependencies.copyfiles]]
+        # src = "file1-in-mydir.txt"
+        # dest = "file1-in-workspace.txt"
+        <BLANKLINE>
+        ## A full flavored dependency using a 'url':
+        # [[dependencies]]
+        # name = "myname"
+        # url = "https://github.com/myuser/my.git"
+        # revision = "main"
+        # path = "mydir"
+        # groups = ["group"]
+        #
+        # [[dependencies.linkfiles]]
+        # src = "file0-in-mydir.txt"
+        # dest = "link0-in-workspace.txt"
+        #
+        # [[dependencies.linkfiles]]
+        # src = "file1-in-mydir.txt"
+        # dest = "link1-in-workspace.txt"
+        #
+        # [[dependencies.copyfiles]]
+        # src = "file0-in-mydir.txt"
+        # dest = "file0-in-workspace.txt"
+        #
+        # [[dependencies.copyfiles]]
+        # src = "file1-in-mydir.txt"
+        # dest = "file1-in-workspace.txt"
+        <BLANKLINE>
+        ## A minimal dependency:
+        # [[dependencies]]
+        # name = "my"
+        [[dependencies]]
+        name = "mylib"
+        <BLANKLINE>
+        <BLANKLINE>
+        # [[linkfiles]]
+        # src = "file-in-main-clone.txt"
+        # dest = "link-in-workspace.txt"
+        <BLANKLINE>
+        <BLANKLINE>
+        # [[copyfiles]]
+        # src = "file-in-main-clone.txt"
+        # dest = "file-in-workspace.txt"
+        <BLANKLINE>
         """
         assert not doc or not path, "'doc' and 'path' are mutually exclusive."
         if doc is None:
             if path and path.exists():
                 doc = tomlkit.parse(path.read_text())
             else:
                 doc = self._create()
@@ -708,23 +883,25 @@
         else:
             data = {
                 "version": ManifestSpec().version,
                 "remotes": tomlkit.aot(),
                 "group-filters": tuple(),
                 "defaults": {},
                 "dependencies": tomlkit.aot(),
+                "linkfiles": tomlkit.aot(),
+                "copyfiles": tomlkit.aot(),
             }
             data.update(as_dict(self))
         for key, value in data.items():
             doc[key] = value
         return tomlkit.dumps(doc)
 
     def save(self, path: Path, update=True):
         """
-        Save :any:`ManifestSpec` at `path`.
+        Save :any:`ManifestSpec` at ``path``.
 
         The file will include an inline documentation of all available options.
 
         Keyword Args:
             update: Additional attributes and comments added by the user are **kept**.
                     Otherwise the file is just overwritten.
         """
@@ -732,15 +909,15 @@
         if update:
             path.write_text(self.dump(path=path))
         else:
             path.write_text(self.dump())
 
     @classmethod
     def upgrade(cls, path: Path):
-        """Upgrade :any:`ManifestSpec` at `path` to latest version including documentation."""
+        """Upgrade :any:`ManifestSpec` at ``path`` to latest version including documentation."""
         # read
         content = path.read_text()
         try:
             olddoc = tomlkit.parse(content)
             olddata = dict(olddoc)
             olddata.pop("groups", None)
             obj = cls(**olddata)
@@ -773,15 +950,15 @@
 https://git-ws.readthedocs.io/en/latest/manual/manifest.html
 """,
         )
         doc.add(tomlkit.nl())
         doc.add(tomlkit.nl())
 
         # Group Filtering
-        example = ManifestSpec(group_filters=GroupFilters(("+test", "-doc", "+feature@path")))
+        example = ManifestSpec(group_filters=GroupFilters(("-doc", "-feature@path")))
         add_comment(doc, example.dump(doc=tomlkit.document(), minimal=True)[:-1])
         doc.add("group-filters", tomlkit.array())
         doc.add(tomlkit.nl())
         doc.add(tomlkit.nl())
 
         # Remotes
         example = ManifestSpec(remotes=[Remote(name="myremote", url_base="https://github.com/myuser")])
@@ -790,15 +967,15 @@
         doc.add(tomlkit.nl())
         doc.add(tomlkit.nl())
 
         # Defaults
         doc.add("defaults", as_dict(Defaults()))
         example = ManifestSpec(
             defaults=Defaults(
-                remote="myserver", revision="main", groups=("+test",), with_groups=("doc",), submodules=True
+                remote="myserver", revision="main", groups=("test",), with_groups=("doc",), submodules=True
             )
         )
         add_comment(doc, "\n".join(example.dump(doc=tomlkit.document(), minimal=True).split("\n")[1:-1]))
         doc.add(tomlkit.nl())
         doc.add(tomlkit.nl())
 
         # Dependencies
@@ -809,14 +986,22 @@
                     name="myname",
                     remote="remote",
                     sub_url="my.git",
                     revision="main",
                     path="mydir",
                     manifest_path="git-ws.toml",
                     groups=("group",),
+                    linkfiles=[
+                        FileRef(src="file0-in-mydir.txt", dest="link0-in-workspace.txt"),
+                        FileRef(src="file1-in-mydir.txt", dest="link1-in-workspace.txt"),
+                    ],
+                    copyfiles=[
+                        FileRef(src="file0-in-mydir.txt", dest="file0-in-workspace.txt"),
+                        FileRef(src="file1-in-mydir.txt", dest="file1-in-workspace.txt"),
+                    ],
                 )
             ]
         )
         add_comment(doc, example.dump(doc=tomlkit.document(), minimal=True)[:-1])
         doc.add(tomlkit.nl())
 
         add_info(doc, "A full flavored dependency using a 'url':")
@@ -825,25 +1010,47 @@
                 ProjectSpec(
                     name="myname",
                     url="https://github.com/myuser/my.git",
                     revision="main",
                     path="mydir",
                     manifest_path="git-ws.toml",
                     groups=("group",),
+                    linkfiles=[
+                        FileRef(src="file0-in-mydir.txt", dest="link0-in-workspace.txt"),
+                        FileRef(src="file1-in-mydir.txt", dest="link1-in-workspace.txt"),
+                    ],
+                    copyfiles=[
+                        FileRef(src="file0-in-mydir.txt", dest="file0-in-workspace.txt"),
+                        FileRef(src="file1-in-mydir.txt", dest="file1-in-workspace.txt"),
+                    ],
                 )
             ]
         )
         add_comment(doc, example.dump(doc=tomlkit.document(), minimal=True)[:-1])
         doc.add(tomlkit.nl())
 
         add_info(doc, "A minimal dependency:")
         example = ManifestSpec(dependencies=[ProjectSpec(name="my", submodules=None)])
         add_comment(doc, example.dump(doc=tomlkit.document(), minimal=True)[:-1])
 
         doc.add("dependencies", tomlkit.aot())
+        doc.add(tomlkit.nl())
+        doc.add(tomlkit.nl())
+
+        # linkfíles
+        example = ManifestSpec(linkfiles=[FileRef(src="file-in-main-clone.txt", dest="link-in-workspace.txt")])
+        add_comment(doc, example.dump(doc=tomlkit.document(), minimal=True)[:-1])
+        doc.add("linkfiles", tomlkit.aot())
+        doc.add(tomlkit.nl())
+        doc.add(tomlkit.nl())
+
+        # copyfíles
+        example = ManifestSpec(copyfiles=[FileRef(src="file-in-main-clone.txt", dest="file-in-workspace.txt")])
+        add_comment(doc, example.dump(doc=tomlkit.document(), minimal=True)[:-1])
+        doc.add("copyfiles", tomlkit.aot())
 
         # Done
         return doc
 
 
 class AppConfigData(BaseSettings, extra=Extra.allow):
     """
@@ -855,45 +1062,53 @@
 
     manifest_path: Optional[str] = Field(
         description="The path (relative to the project's root folder) to the manifest file."
     )
     """
     The path of the manifest file within a repository.
 
-    If this is not defined, the default is :any:`MANIFEST_PATH_DEFAULT`.
+    If this is not defined, the default is ``git-ws.toml``.
 
-    This option can be overridden by specifying the `GIT_WS_MANIFEST_PATH` environment variable.
+    This option can be overridden by specifying the ``GIT_WS_MANIFEST_PATH`` environment variable.
     """
 
     color_ui: Optional[bool] = Field(description="If set to true, the output the tool generates will be colored.")
     """
     Defines if outputs by the tool shall be colored.
 
     If this is not defined, output will be colored by default.
 
-    This option can be overridden by specifying the `GIT_WS_COLOR_UI` environment variable.
+    This option can be overridden by specifying the ``GIT_WS_COLOR_UI`` environment variable.
     """
 
     group_filters: Optional[GroupFilters] = Field(description="The groups to operate on.")
     """
     The groups to operate on.
 
     This is a filter for groups to operate on during workspace actions.
 
-    This option can be overridden by specifying the `GIT_WS_GROUP_FILTERS` environment variable.
+    This option can be overridden by specifying the ``GIT_WS_GROUP_FILTERS`` environment variable.
     """
 
     clone_cache: Optional[Path] = Field(description="Local Cache for Git Clones.")
     """
     Clone Cache.
 
-    Initial cloning a dependency takes a while. If you do this often (i.e. in CI/CD), this consumes time.
-    The local filesystem cache directory will be used, to re-use already cloned data.
+    Initial cloning all dependencies takes a while. This sums up if done often (i.e. in CI/CD).
+    This local filesystem cache directory will be used, to re-use already cloned data.
+
+    This option can be overridden by specifying the ``GIT_WS_CLONE_CACHE`` environment variable.
+    """
+
+    depth: Optional[int] = Field(description="Default Clone Depth for New Clones")
+    """
+    Default Clone Depth.
 
-    This option can be overridden by specifying the `GIT_WS_CLONE_CACHE` environment variable.
+    New clones are created with the given depth.
+    0 deactivates shallow cloning.
     """
 
     @staticmethod
     def defaults() -> Dict[str, Any]:
         """
         As all configuration options must be optional, this option provides the default values.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `git_ws-0.9.2/gitws/deptree.py` & `git_ws-1.0.0/gitws/deptree.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -10,15 +10,23 @@
 # Git Workspace is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with Git Workspace. If not, see <https://www.gnu.org/licenses/>.
 
-"""Dependency Tree."""
+"""
+Dependency Tree.
+
+Translate the dependencies into a human readable tree:
+
+* :any:`get_deptree()` creates a :any:`anytree.Node` tree.
+* :any:`anytree.RenderTree(deptree))` can translate print it.
+* :any:`DepDotExporter(deptree)` dumps a graphviz `dot` notation of the tree.
+"""
 
 import logging
 from typing import List, Tuple
 
 from anytree import NodeMixin
 from anytree.exporter import DotExporter
 
@@ -37,16 +45,25 @@
     def __init__(self, project, is_primary=False, parent=None):
         self.project = project
         self.is_primary = is_primary
         self.parent = parent
 
 
 def get_deptree(workspace: Workspace, manifest: Manifest, primary: bool = False) -> DepNode:
-    """Calculate Dependency Tree."""
-    main = str(workspace.info.main_path)
+    """
+    Calculate Dependency Tree.
+
+    Args:
+        workspace: The Workspace
+        manifest: The Manifest
+
+    Keyword Args:
+        primary: Reduce tree to primary dependencies only.
+    """
+    main = str(workspace.info.main_path or "")
     main_node = DepNode(Project(name=main, path=main), is_primary=True)
     primaries: List[str] = []
     edges: List[Tuple[str, str]] = []
     _build(primaries, edges, workspace, main_node, manifest, primary=primary)
     return main_node
```

### Comparing `git_ws-0.9.2/gitws/exceptions.py` & `git_ws-1.0.0/gitws/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -13,30 +13,34 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with Git Workspace. If not, see <https://www.gnu.org/licenses/>.
 
 """Collection Of All Exceptions Which Might Occur."""
 
 from pathlib import Path
+from typing import Optional
 
 
 class UninitializedError(RuntimeError):
     """Git Workspace Has Not Been Initialized."""
 
     def __init__(self):
         super().__init__("git workspace has not been initialized yet.")
 
 
 class InitializedError(RuntimeError):
     """Git Workspace Has Already Been Initialized."""
 
-    def __init__(self, path, main_path):
-        super().__init__(
-            f"git workspace has already been initialized at {str(path)!r} with main repo at {str(main_path)!r}."
-        )
+    def __init__(self, path: Path, main_path: Optional[Path]):
+        msg = f"git workspace has already been initialized at {str(path)!r}"
+        if main_path:
+            msg = f"{msg} with main repo at {str(main_path)!r}."
+        else:
+            msg = f"{msg}."
+        super().__init__(msg)
         self.path = path
         self.main_path = main_path
 
 
 class NoGitError(RuntimeError):
     """Git Clone Has Not Been Initialized."""
 
@@ -56,27 +60,28 @@
     """Manifest Already Exists."""
 
     def __init__(self, path):
         super().__init__(f"Manifest exists at {str(path)!r}.")
 
 
 class OutsideWorkspaceError(RuntimeError):
-    """Project Is Located Outside Of Workspace."""
+    """Reference To Outside Of Workspace."""
 
-    def __init__(self, path, project_path):
-        super().__init__(f"Project {str(project_path)!r} is located outside {str(path)!r}.")
+    def __init__(self, workspace_path, path, what):
+        super().__init__(f"{what} {str(path)!r} is refers outside of workspace ({str(workspace_path)!r}).")
+        self.workspace_path = workspace_path
         self.path = path
-        self.project_path = project_path
 
 
 class WorkspaceNotEmptyError(RuntimeError):
     """Workspace Is Not Empty."""
 
-    def __init__(self, path):
-        super().__init__(f"Workspace {str(path)!r} is not an empty directory.")
+    def __init__(self, path, items):
+        items = ", ".join(str(item) for item in items)
+        super().__init__(f"Workspace {str(path)!r} is not an empty directory. It contains: {items}.")
         self.path = path
 
 
 class ManifestError(RuntimeError):
     """The Manifest Is Invalid."""
 
     def __init__(self, path, details):
@@ -99,24 +104,24 @@
 
     def __init__(self, location: str):
         super().__init__(f"The configuration location {location} is not known")
         self.location = location
 
 
 class InvalidConfigurationValueError(RuntimeError):
-    """An invalid configuration value has been passed to the application."""
+    """An Invalid Configuration Value Has Been Passed To The Application."""
 
     def __init__(self, key: str, value):
         super().__init__(f"Invalid value {value} has been passed to option {key}")
         self.key = key
         self.value = value
 
 
 class InvalidConfigurationOptionError(RuntimeError):
-    """An invalid configuration option has been passed to the applicaiton."""
+    """An Invalid Configuration Option Has Been Passed To The Applicaiton."""
 
     def __init__(self, key):
         super().__init__(f"Unknown configuration option {key}")
         self.key = key
 
 
 class GitCloneMissingError(RuntimeError):
@@ -132,22 +137,39 @@
 
     def __init__(self, project_path):
         super().__init__(f"Git Clone {str(project_path)!r} contains changes.")
         self.project_path = project_path
 
 
 class GitCloneMissingOriginError(RuntimeError):
-    """Git Clone has no remote 'origin'."""
+    """Git Clone Has No Remote ``Origin``."""
 
     def __init__(self, project_path, remote="origin"):
         super().__init__(f"Git Clone {str(project_path)!r} has not remote '{remote}'.")
         self.project_path = project_path
         self.remote = remote
 
 
 class GitTagExistsError(RuntimeError):
 
-    """Git Tag already exists."""
+    """Git Tag Already Exists."""
 
     def __init__(self, tag):
         super().__init__(f"tag {tag} already exists")
         self.tag = tag
+
+
+class NoMainError(RuntimeError):
+    """Workspace Has No Main Project."""
+
+    def __init__(self):
+        super().__init__("Workspace has been initialized from manifest only, without a main project.")
+
+
+class NoAbsUrlError(RuntimeError):
+    """No Relative Url Possible."""
+
+    def __init__(self, project_name: str):
+        super().__init__(
+            "Absolute URL required. Please specify an absolute 'url' or a 'sub_url'"
+            f" with a 'remote' for {project_name!r}."
+        )
```

### Comparing `git_ws-0.9.2/gitws/git.py` & `git_ws-1.0.0/gitws/git.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -10,20 +10,29 @@
 # Git Workspace is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with Git Workspace. If not, see <https://www.gnu.org/licenses/>.
 
-"""Git Utilities."""
+"""
+Our Git Helper.
+
+We know, that there are libraries for that.
+But we just want to have a lean programmatic interface to git.
+Just with the functionality **we** need. Not more.
+
+We currently do NOT check the git version and try to use the common subset.
+"""
 import hashlib
 import logging
 import os
 import re
 import shutil
+import subprocess
 from enum import Enum
 from pathlib import Path
 from typing import Generator, List, Optional, Tuple, Union
 
 from ._basemodel import BaseModel
 from ._url import strip_user_password
 from ._util import get_repr, no_echo, run
@@ -63,28 +72,26 @@
     UPDATED_UNMERGED = "U"
 
     def __str__(self):
         return self.value
 
 
 class Status(BaseModel):
-    """Status (One `git status` line."""
+    """Status (One ``git status`` line)."""
 
     def with_path(self, path: Path) -> "Status":
-        """Return :any:`Status` with `path`."""
+        """Return :any:`Status` with ``path`` as prefix."""
         raise NotImplementedError()
 
     def has_work_changes(self) -> Optional[bool]:
         """Has Work Changes."""
-        # pylint: disable=no-self-use
         return None  # pragma: no cover
 
     def has_index_changes(self) -> Optional[bool]:
         """Has Index Changes."""
-        # pylint: disable=no-self-use
         return None  # pragma: no cover
 
     def has_changes(self) -> Optional[bool]:
         """Has Changes."""
         return self.has_index_changes() or self.has_work_changes()
 
 
@@ -125,21 +132,21 @@
     def __str__(self):
         if self.orig_path:
             return f"{self.index}{self.work} {self.orig_path!s} -> {self.path!s}"
         return f"{self.index}{self.work} {self.path!s}"
 
     @staticmethod
     def from_str(line) -> "FileStatus":
-        """Create v1 porcelain output."""
+        """Create from ``git status --porcelain`` Output."""
         mat = _RE_STATUS.match(line)
         assert mat, f"Invalid pattern {line}"
         return FileStatus(**mat.groupdict())
 
     def with_path(self, path: Path) -> "FileStatus":
-        """Return :any:`FileStatus` with `path`."""
+        """Return :any:`FileStatus` with ``path`` as prefix."""
         if self.orig_path:
             return self.update(path=path / self.path, orig_path=path / self.orig_path)
         return self.update(path=path / self.path)
 
     def has_work_changes(self) -> bool:
         """Has Work Changes."""
         return self.work not in (State.UNMODIFIED, State.IGNORED, State.UNTRACKED)
@@ -147,72 +154,87 @@
     def has_index_changes(self) -> bool:
         """Has Index Changes."""
         return self.index not in (State.UNMODIFIED, State.IGNORED, State.UNTRACKED)
 
 
 class BranchStatus(Status):
 
-    """Branch Status."""
+    """
+    Branch Status Line From ``git status`` command.
+
+    >>> branchstatus = BranchStatus.from_str('main...origin/main')
+    >>> branchstatus
+    BranchStatus(info='main...origin/main')
+    >>> str(branchstatus)
+    'main...origin/main'
+    """
 
     info: str
-    """Info."""
+    """Branch Status String."""
 
     def __str__(self):
         return self.info
 
     @staticmethod
     def from_str(line) -> "BranchStatus":
-        """Create from v1 porcelain output."""
+        """Create from ``git status --porcelain`` Output."""
         return BranchStatus(info=line)
 
     def with_path(self, path: Path) -> "BranchStatus":
-        """Return :any:`BranchStatus` with `path`."""
+        """Return :any:`BranchStatus` with ``path`` as prefix."""
         # pylint: disable=unused-argument
         return self
 
 
 class DiffStat(BaseModel):
 
     """
-    Diff Status.
+    Diff Status Line From ``git diff --stat`` command.
+
+    >>> diffstat = DiffStat.from_str(' path/file.txt | 16 ++++++++--------')
+    >>> diffstat
+    DiffStat(path=PosixPath('path/file.txt'), stat='16 ++++++++--------')
+    >>> str(diffstat)
+    ' path/file.txt | 16 ++++++++--------'
+    >>> str(diffstat.with_path(Path('base')))
+    ' base/path/file.txt | 16 ++++++++--------'
     """
 
     path: Path
-    """Path."""
+    """File Path."""
 
     stat: str
-    """Diff Status."""
+    """Diff Status Line."""
 
     def __str__(self):
         return f" {self.path} | {self.stat}"
 
     @staticmethod
     def from_str(line) -> "DiffStat":
-        """Create from `diff --stat` output."""
+        """Create from ``git diff --stat`` Output."""
         mat = _RE_DIFFSTAT.match(line)
         assert mat, f"Invalid pattern {line}"
         return DiffStat(**mat.groupdict())
 
     def with_path(self, path: Path) -> "DiffStat":
-        """Return :any:`DiffStat` with `path`."""
+        """Return :any:`DiffStat` with ``path`` as prefix."""
         return self.update(path=path / self.path)
 
 
 class Git:
 
     """
     Our Git REPO Helper.
 
-    We know, that there are libraries for that.
-    But we just want to have a lean programmatic interface to git.
-    Just with the functionality **we** need. Not more.
+    To initialize a git repository in the current working directory:
 
-    We currently do NOT check the git version, but try to use a quite common subset.
+    >>> Git.init()
+    Git(...)
 
-    The easiest way to start:
+    The easiest way to start with an existing clone:
 
     >>> git = Git.from_path()
     """
 
     # pylint: disable=too-many-public-methods
 
     def __init__(self, path: Path, clone_cache: Optional[Path] = None, secho=None):
@@ -220,78 +242,114 @@
         self.clone_cache = clone_cache
         self.secho = secho or no_echo
 
     def __repr__(self):
         return get_repr(self, (self.path,))
 
     @staticmethod
+    def init(path: Optional[Path] = None) -> "Git":
+        """Initialize new git repository at ``path``."""
+        path = path or Path.cwd()
+        path.mkdir(parents=True, exist_ok=True)
+        run(("git", "init"), cwd=path)
+        return Git(path)
+
+    @staticmethod
     def find_path(path: Optional[Path] = None) -> Path:
         """Determine Top Directory of Git Clone."""
         path = path or Path.cwd()
         result = run(("git", "rev-parse", "--show-cdup"), capture_output=True, check=False, cwd=path)
         if result.stderr:
             raise NoGitError()
         cdup = result.stdout.decode("utf-8").strip()
         return (path / cdup).resolve()
 
     @staticmethod
     def from_path(path: Optional[Path] = None, secho=None) -> "Git":
-        """Create GIT Repo Helper from `path`."""
+        """Create GIT Repo Helper from ``path``."""
         path = Git.find_path(path=path)
         clone_cache = AppConfig().options.clone_cache
         return Git(path=path, clone_cache=clone_cache, secho=secho)
 
     def is_cloned(self) -> bool:
-        """Return if clone already exists."""
+        """Determine if clone already exists."""
         if not self.path.exists() or not self.path.is_dir():
             return False
         result = self._run(("rev-parse", "--show-cdup"), capture_output=True, check=False)
         cloned = not result.stderr and not result.stdout.strip()
         _LOGGER.info("Git(%r).is_cloned() = %r", str(self.path), cloned)
         return cloned
 
     def check(self):
-        """Check clone."""
+        """Check Clone for Existance."""
         if not self.is_cloned():
             raise GitCloneMissingError(self.path)
 
     def set_config(self, name, value):
-        """Set Git Configuration `name` to `value`."""
+        """Set Git Configuration Variable ``name`` to ``value``."""
         self._run(("config", name, value))
 
-    def clone(self, url, revision: Optional[str] = None):
-        """Clone `url` and checkout `revision`."""
-        _LOGGER.info("Git(%r).clone(%r, revision=%r)", str(self.path), url, revision)
+    def clone(self, url, revision: Optional[str] = None, depth: Optional[int] = None):
+        """
+        Clone ``url`` and checkout ``revision``.
+
+        The checkout is done to ``self.path``.
+        If ``self.clone_cache`` directory path is set, the clone uses the given path as local filesystem cache.
+        """
+        _LOGGER.info("Git(%r).clone(%r, revision=%r, depth=%r)", str(self.path), url, revision, depth)
         assert not self.path.exists() or not any(self.path.iterdir())
+        # This is bad code, because:
+        # * `git clone` does have an option for SHA/tag/revision
+        # * we re-use a filesystem cache for clones.
         if self.clone_cache:
             self._clone_cache(url)
+            if depth:
+                # strip down clone copy to given depth
+                self._run(("fetch", "--depth", str(depth), "origin", revision or "HEAD"))
+        elif depth and revision:
+            self.path.mkdir(parents=True)
+            self._run(("init",), capture_output=True)
+            self._run(("remote", "add", "origin", str(url)))
+            self._run(("fetch", "--depth", str(depth), "origin", revision), capture_output=True)
+        elif depth:
+            run(("git", "clone", "--depth", str(depth), "--", str(url), str(self.path)))
         else:
             run(("git", "clone", "--", str(url), str(self.path)))
         if revision:
             self._run(("checkout", revision), capture_output=True)
 
     def _clone_cache(self, url):
         baseurl = strip_user_password(url)
         # cache index
         key = hashlib.sha256(baseurl.encode("utf-8")).hexdigest()
         cache = self.clone_cache / key
-        # cache update
+        # Restore user/password credentials, repair corrupted cache
+        if cache.exists():
+            self.secho("Using clone-cache")
+            try:
+                self._run(("remote", "add", "origin", str(url)), capture_output=True, cwd=cache)
+                self._run(("reset", "--hard"), capture_output=True, cwd=cache)
+                self._run(("clean", "-xdf"), capture_output=True, cwd=cache)
+            except subprocess.CalledProcessError:  # pragma: no cover
+                shutil.rmtree(cache)  # broken
+        # Cache Update
+        if cache.exists():
+            self._run(("fetch", "origin"), capture_output=True, cwd=cache)
+            try:
+                branch = self._run2str(("branch",), regex=_RE_BRANCH, cwd=cache)
+                self._run(("branch", f"--set-upstream-to=origin/{branch}", "main"), capture_output=True, cwd=cache)
+                self._run(("merge", f"origin/{branch}"), capture_output=True, cwd=cache)
+            except subprocess.CalledProcessError:  # pragma: no cover
+                shutil.rmtree(cache)  # broken
+        # (Re-)Init Cache
         if not cache.exists():
             self.secho("Initializing clone-cache")
             cache.mkdir(parents=True)
             run(("git", "clone", "--", str(url), str(cache)))
-        else:
-            self.secho("Using clone-cache")
-            # Restore user/password credentials
-            self._run(("remote", "add", "origin", str(url)), cwd=cache)
-            self._run(("fetch", "origin"), cwd=cache)
-            branch = self._run2str(("branch",), regex=_RE_BRANCH, cwd=cache)
-            self._run(("branch", f"--set-upstream-to=origin/{branch}", "main"), cwd=cache)
-            self._run(("merge", f"origin/{branch}"), capture_output=True, cwd=cache)
-        # use cache
+        _LOGGER.debug("Copy %s to  %s)", cache, self.path)
         shutil.copytree(cache, self.path)
         # Remove user/password credentials from cache
         self._run(("remote", "remove", "origin"), cwd=cache)
 
     def get_tag(self) -> Optional[str]:
         """Get Actual Tag."""
         tag = self._run2str(("describe", "--exact-match", "--tags"), check=False) or None
@@ -300,35 +358,35 @@
 
     def get_branch(self) -> Optional[str]:
         """Get Actual Branch."""
         branch = self._run2str(("branch",), regex=_RE_BRANCH)
         _LOGGER.info("Git(%r).get_branch() = %r", str(self.path), branch)
         return branch
 
-    def get_sha(self) -> Optional[str]:
-        """Get SHA."""
-        sha = self._run2str(("rev-parse", "HEAD"), check=False) or None
-        _LOGGER.info("Git(%r).get_sha() = %r", str(self.path), sha)
+    def get_sha(self, revision: Optional[str] = None) -> Optional[str]:
+        """Get Actual SHA."""
+        sha = self._run2str(("rev-parse", revision or "HEAD"), check=False) or None
+        _LOGGER.info("Git(%r).get_sha(%r) = %r", str(self.path), revision, sha)
         return sha
 
     def get_revision(self) -> Optional[str]:
         """
         Get Revision.
 
         We try several things, the winner takes it all:
 
         1. Get Actual Tag
         2. Get Actual Branch
         3. Get SHA.
-        4. `None` if empty repo.
+        4. ``None`` if empty repo.
         """
         return self.get_branch() or self.get_tag() or self.get_sha()
 
     def get_url(self) -> Optional[str]:
-        """Get Actual URL of 'origin'."""
+        """Get Actual URL of ``origin``."""
         url = self._run2str(("remote", "-v"), regex=_RE_URL, check=False)
         _LOGGER.info("Git(%r).get_url() = %r", str(self.path), url)
         return url
 
     def checkout(self, revision: Optional[str] = None, paths: Optional[Paths] = None, force: bool = False):
         """
         Checkout Revision.
@@ -342,52 +400,53 @@
         if revision:
             args.append(revision)
         if force:
             args.append("--force")
         self._run(args, paths=paths)
         _LOGGER.info("Git(%r).checkout(revision=%r, paths=%r, force=%r)", str(self.path), revision, paths, force)
 
-    def fetch(self):
+    def fetch(self, shallow: Optional[str] = None, unshallow: bool = False):
         """Fetch."""
-        _LOGGER.info("Git(%r).fetch()", str(self.path))
-        self._run(("fetch",))
+        _LOGGER.info("Git(%r).fetch(shallow=%r)", str(self.path), shallow)
+        assert not shallow or not unshallow, "shallow and unshallow are mutally exclusive"
+        if shallow:
+            self._run(("fetch", "origin", shallow))
+        elif unshallow:
+            self._run(("fetch", "--unshallow"))
+        else:
+            self._run(("fetch",))
 
     def merge(self, commit):
         """Merge."""
         _LOGGER.info("Git(%r).merge(%r)", str(self.path), commit)
         self._run(("merge", commit))
 
-    def pull(self):
-        """Pull."""
-        _LOGGER.info("Git(%r).pull()", str(self.path))
-        self._run(("pull",))
-
     def rebase(self):
         """Rebase."""
         _LOGGER.info("Git(%r).rebase()", str(self.path))
         self._run(("rebase",))
 
     def add(self, paths: Optional[Paths] = None, force: bool = False, all_: bool = False):
         """
-        Add.
+        Add Files.
 
         Args:
             paths: File Paths to add.
 
         Keyword Args:
             force: allow adding otherwise ignored files.
             all_: add changes from all tracked and untracked files.
         """
         _LOGGER.info("Git(%r).add(%r, force=%r, all_=%r)", str(self.path), paths, force, all_)
         self._run(["add"], booloptions=(("--force", force), ("--all", all_)), paths=paths)
 
     # pylint: disable=invalid-name
     def rm(self, paths: Paths, cached: bool = False, force: bool = False, recursive: bool = False):
         """
-        Remove.
+        Remove Files.
 
         Keyword Args:
             cached: only remove from the index
             force: override the up-to-date check
             recursive: allow recursive removal
         """
         _LOGGER.info(
@@ -400,15 +459,15 @@
             args.append("--force")
         if recursive:
             args.append("-r")
         self._run(args, paths=paths)
 
     def reset(self, paths: Paths):
         """
-        Reset.
+        Reset Files.
 
         Args:
             paths: File paths.
         """
         _LOGGER.info("Git(%r).reset(%r)", str(self.path), paths)
         self._run(("reset",), paths=paths)
 
@@ -445,26 +504,26 @@
         if force:
             args.append("--force")
         if msg:
             args += ["-m", msg]
         self._run(args)
 
     def get_tags(self, pattern: Optional[str] = None) -> Tuple[str, ...]:
-        """Get Tags matching `pattern` or all."""
+        """Get Tags matching ``pattern`` or all."""
         cmd = ["tag", "-l"]
         if pattern:
             cmd.append(pattern)
         return tuple(self._run2lines(cmd, skip_empty=True))
 
     def status(self, paths: Optional[Paths] = None, branch: bool = False) -> Generator[Status, None, None]:
         """
         Git Status.
 
         Keyword Args:
-            branch: Show branch.
+            branch: Show branch too.
         """
         _LOGGER.info("Git(%r).status(paths=%r, branch=%r)", str(self.path), paths, branch)
         if branch:
             lines = self._run2lines(("status", "--porcelain", "--branch"), paths=paths)
             yield BranchStatus.from_str(lines[0])
             lines = lines[1:]
         else:
@@ -494,19 +553,17 @@
         """
         Git Diff Statistics.
 
         Keyword Args:
             paths: Paths.
         """
         _LOGGER.info("Git(%r).diffstat(paths=%r)", str(self.path), paths)
-        lines = self._run2lines(("diff", "--stat"), paths=paths)
-        if lines:
-            # skip last line for now
-            for line in lines[:-1]:
-                yield DiffStat.from_str(line)
+        lines = self._run2lines(("diff", "--stat"), paths=paths)[:-1]
+        for line in lines:
+            yield DiffStat.from_str(line)
 
     def submodule_update(self, init: bool = False, recursive: bool = False):
         """
         Submodule Update.
 
         Keyword Args:
             init: Initialize.
@@ -528,32 +585,40 @@
         return any(status.has_changes() for status in self.status())
 
     def is_empty(self):
         """
         Clone does not contain any changes.
 
         A clone is empty if there are:
+
         * no files changed
         * no commits which are not pushed yet
         * nothing stashed
         """
         _LOGGER.info("Git(%r).is_empty()", str(self.path))
         lines = self._run2lines(("status", "--porcelain", "--branch"))
         if len(lines) > 1:
             return False
         if self._run2str(("stash", "list")):
             return False
-        if lines[0].startswith("## No commits yet on "):
+        if lines[0].startswith("## No commits yet on "):  # pragma: no cover
             return True
         if "[ahead " in lines[0]:
             return False
         if not self.get_url():
             return False
         return True
 
+    def get_shallow(self) -> Optional[str]:
+        """Get Shallow."""
+        try:
+            return (self.path / ".git" / "shallow").read_text()
+        except FileNotFoundError:
+            return None
+
     def _run(
         self,
         args: Args,
         paths: Optional[Paths] = None,
         booloptions: Optional[BoolOptions] = None,
         cwd: Optional[Path] = None,
         **kwargs,
```

### Comparing `git_ws-0.9.2/gitws/gitws.py` & `git_ws-1.0.0/gitws/gitws.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -21,21 +21,29 @@
 """
 import logging
 import shutil
 import urllib
 from pathlib import Path
 from typing import Generator, List, Optional, Tuple
 
-from ._util import no_echo, removesuffix, resolve_relative, run
+from ._filerefupdater import CopyFileUpdater, LinkFileUpdater
+from ._util import get_repr, no_echo, removesuffix, resolve_relative, run
 from .appconfig import AppConfig
 from .clone import Clone, map_paths
 from .const import MANIFEST_PATH_DEFAULT, MANIFESTS_PATH
 from .datamodel import GroupFilters, Manifest, ManifestSpec, Project, ProjectPaths, ProjectSpec
 from .deptree import DepNode, get_deptree
-from .exceptions import GitCloneNotCleanError, GitTagExistsError, InitializedError, ManifestExistError
+from .exceptions import (
+    GitCloneNotCleanError,
+    GitTagExistsError,
+    InitializedError,
+    ManifestExistError,
+    NoGitError,
+    NoMainError,
+)
 from .git import DiffStat, Git, Status
 from .iters import ManifestIter, ProjectIter
 from .manifestfinder import find_manifest
 from .workspace import Workspace
 
 _LOGGER = logging.getLogger("git-ws")
 _COLOR_BANNER = "green"
@@ -44,27 +52,27 @@
 
 
 class GitWS:
     """
     Multi Repository Management.
 
     Args:
-        workspace: workspace.
+        workspace: The Workspace Representation.
         manifest_path: Manifest File Path. **Resolved** Path.
         group_filters: Group Filters.
 
     Keyword Args:
-        secho: `click.secho` like print method for verbose output.
+        secho: :any:`click.secho` like print method for verbose output.
 
     There are static methods to create a :any:`GitWS` instances in the different szenarios:
 
-    * :any:`GitWS.from_path()`: Create :any:`GitWS` for EXISTING workspace at `path`.
-    * :any:`GitWS.create()`: Create NEW workspace at `path` and return corresponding :any:`GitWS`.
-    * :any:`GitWS.init()`: Initialize NEW Workspace for git clone at `main_path` and return corresponding :any:`GitWS`.
-    * :any:`GitWS.clone()`: Clone git `url`, initialize NEW Workspace and return corresponding :any:`GitWS`.
+    * :any:`GitWS.from_path()`: Create :any:`GitWS` for EXISTING workspace at ``path``.
+    * :any:`GitWS.create()`: Create NEW workspace at ``path`` and return corresponding :any:`GitWS`.
+    * :any:`GitWS.init()`: Initialize NEW Workspace and return corresponding :any:`GitWS`.
+    * :any:`GitWS.clone()`: Clone git ``url``, initialize NEW Workspace and return corresponding :any:`GitWS`.
     """
 
     # pylint: disable=too-many-public-methods
 
     def __init__(
         self,
         workspace: Workspace,
@@ -82,190 +90,286 @@
             return (self.workspace, self.manifest_path, self.group_filters) == (
                 other.workspace,
                 other.manifest_path,
                 other.group_filters,
             )
         return NotImplemented
 
+    def __repr__(self):
+        return get_repr(self, (self.workspace, self.manifest_path, self.group_filters))
+
     @property
     def path(self) -> Path:
         """
         GitWS Workspace Root Directory.
         """
         return self.workspace.path
 
     @property
-    def main_path(self) -> Path:
+    def main_path(self) -> Optional[Path]:
         """
         GitWS Workspace Main Directory.
         """
         return self.workspace.main_path
 
+    @property
+    def base_path(self) -> Path:
+        """
+        GitWS Workspace Main Directory (if the workspace has a main project) or GitWS Workspace Directory.
+        """
+        return self.workspace.base_path
+
     @staticmethod
     def from_path(
         path: Optional[Path] = None,
         manifest_path: Optional[Path] = None,
         group_filters: Optional[GroupFilters] = None,
         secho=None,
     ) -> "GitWS":
         """
-        Create :any:`GitWS` for EXISTING workspace at `path`.
+        Create :any:`GitWS` for EXISTING workspace at ``path``.
 
         Keyword Args:
             path: Path within the workspace (Default is the current working directory).
-            mainfest_path: Manifest File Path. Relative to `main_path`. Default is taken from Configuration.
+            manifest_path: Manifest File Path. Relative to ``base_path``. Default is taken from Configuration.
             group_filters: Group Filters. Default is taken from Configuration.
-            secho: `click.secho` like print method for verbose output.
+            secho: :any:`click.secho` like print method for verbose output.
         """
         workspace = Workspace.from_path(path=path)
-        if not manifest_path:
-            manifest_path = find_manifest(workspace.main_path)
+        main_path = workspace.main_path
+        if main_path and not manifest_path:
+            manifest_path = find_manifest(main_path)
         manifest_path = workspace.get_manifest_path(manifest_path=manifest_path)
-        ManifestSpec.load(manifest_path)  # check manifest
+        GitWS.check_manifest(manifest_path)
         if group_filters:
             GroupFilters.validate(group_filters)
         group_filters = workspace.get_group_filters(group_filters=group_filters or None)
         return GitWS(workspace, manifest_path, group_filters, secho=secho)
 
     @staticmethod
     def create(
         path: Path,
-        main_path: Path,
+        main_path: Optional[Path] = None,
         manifest_path: Optional[Path] = None,
         group_filters: Optional[GroupFilters] = None,
+        depth: Optional[int] = None,
         force: bool = False,
         secho=None,
     ) -> "GitWS":
         """
-        Create NEW workspace at `path` and return corresponding :any:`GitWS`.
+        Create NEW workspace at ``path`` and return corresponding :any:`GitWS`.
 
         Args:
             path: Workspace Path.
-            main_path: Main Project Path.
 
         Keyword Args:
-            mainfest_path: Manifest File Path. Relative to `main_path`. Default is 'git-ws.toml'.
+            main_path: Main Project Path.
+            manifest_path: Manifest File Path. Relative to ``main_path`` if given, otherwise relative to ``path``.
+                           Default is ``git-ws.toml``.
                            This value is written to the configuration.
             group_filters: Default Group Filters.
                            This value is written to the configuration.
+            depth: Shallow Clone Depth.
             force: Ignore that the workspace exists.
-            secho: `click.secho` like print method for verbose output.
+            secho: :any:`click.secho` like print method for verbose output.
         """
         _LOGGER.debug(
-            "GitWS.create(%r, %r, manifest_path=%r, group-filters=%r)",
+            "GitWS.create(%r, main_path=%r, manifest_path=%r, group-filters=%r)",
             str(path),
             str(main_path),
             str(manifest_path),
             group_filters,
         )
+        # Relative to main_path if given, or workspace path as fallback
         # We need to resolve in inverted order, otherwise the manifest_path is broken
-        # `manifest_path` can be absolute or relative to `main_path`. we need it relative to `main_path`.
-        manifest_path_rel = resolve_relative(manifest_path or MANIFEST_PATH_DEFAULT, base=main_path)
-        # `main_path` can be absolute or relative to `path`. we need it relative to `path`.
-        main_path = resolve_relative(main_path, base=path)
+        # ``manifest_path`` can be absolute or relative to ``base_path``. we need it relative to ``base_path``.
+        manifest_path_rel = resolve_relative(manifest_path or MANIFEST_PATH_DEFAULT, base=(main_path or path))
+        if main_path:
+            # ``main_path`` can be absolute or relative to ``path``. we need it relative to ``path``.
+            main_path = resolve_relative(main_path, base=path)
+            base_path = path / main_path
+        else:
+            base_path = path
         # check manifest
-        ManifestSpec.load(path / main_path / manifest_path_rel)
+        GitWS.check_manifest(base_path / manifest_path_rel)
         # check group_filters
         if group_filters:
             GroupFilters.validate(group_filters)
         # Create Workspace
-        workspace = Workspace.init(path, main_path, manifest_path_rel, group_filters=group_filters or None, force=force)
+        workspace = Workspace.init(
+            path,
+            main_path=main_path,
+            manifest_path=manifest_path_rel,
+            group_filters=group_filters or None,
+            depth=depth,
+            force=force,
+        )
         group_filters = workspace.get_group_filters(group_filters=group_filters)
         # Check for tagged manifest
-        if not manifest_path:
-            manifest_path_rel = find_manifest(path / main_path) or manifest_path_rel
-        return GitWS(workspace, path / main_path / manifest_path_rel, group_filters, secho=secho)
+        if main_path and not manifest_path:
+            manifest_path_rel = find_manifest(base_path) or manifest_path_rel
+        return GitWS(workspace, base_path / manifest_path_rel, group_filters, secho=secho)
 
     @staticmethod
     def init(
+        path: Optional[Path] = None,
         main_path: Optional[Path] = None,
         manifest_path: Optional[Path] = None,
         group_filters: Optional[GroupFilters] = None,
+        depth: Optional[int] = None,
         force: bool = False,
         secho=None,
     ) -> "GitWS":
         """
-        Initialize NEW Workspace for git clone at `main_path` and return corresponding :any:`GitWS`.
-
-        The parent directory of `main_path` becomes the workspace directory.
+        Initialize NEW Workspace and return corresponding :any:`GitWS`.
 
         Keyword Args:
+            path: Workspace Path. Parent directory of the main git clone directory or current working
+                  directory by default.
             main_path: Main Project Path.
-            mainfest_path: Manifest File Path. Relative to `main_path`. Default is 'git-ws.toml'.
+            manifest_path: Manifest File Path. Relative to ``main_path``. Default is ``git-ws.toml``.
                            This value is written to the configuration.
             group_filters: Default Group Filters.
                            This value is written to the configuration.
+            depth: Shallow Clone Depth.
             force: Ignore that the workspace exists.
-            secho: `click.secho` like print method for verbose output.
+            secho: :any:`click.secho` like print method for verbose output.
+
+        This method has different modes depending on ``main_path`` and the current working directory:
+
+        * if ``main_path`` refers to a git clone, it is taken as main project.
+        * if ``main_path`` is ``None`` but the current working directory contains a git clone,
+          it is taken as main project
+        * if ``main_path`` is ``None`` and the current working directory does **not** contain a git clone,
+          the workspace is initialized **without** main project.
         """
         secho = secho or no_echo
-        main_path = Git.find_path(path=main_path)
-        path = main_path.parent
+        if main_path:
+            # Initialize with explicit main project
+            main_path = Git.find_path(path=main_path)
+            path = path or main_path.parent
+        else:
+            # Are we in a git clone?
+            try:
+                # YES --> use it as main project
+                main_path = Git.find_path()
+                path = path or main_path.parent
+            except NoGitError:
+                # NO --> no main project
+                path = path or Path.cwd()
         if not force:
             info = Workspace.is_init(path)
             if info:
                 raise InitializedError(path, info.main_path)
-            Workspace.check_empty(path, main_path)
-        name = main_path.name
-        secho(f"===== {resolve_relative(main_path)} (MAIN {name!r}) =====", fg=_COLOR_BANNER)
+            # There might be anything in the workspace if we have no clean main repo!
+            if main_path:
+                Workspace.check_empty(path, main_path)
+        if main_path:
+            name = main_path.name
+            secho(f"===== {resolve_relative(main_path)} (MAIN {name!r}) =====", fg=_COLOR_BANNER)
         return GitWS.create(
-            path, main_path, manifest_path=manifest_path, group_filters=group_filters, force=force, secho=secho
+            path,
+            main_path=main_path,
+            manifest_path=manifest_path,
+            group_filters=group_filters,
+            depth=depth,
+            force=force,
+            secho=secho,
         )
 
-    def deinit(self):
+    def deinit(
+        self,
+        prune: bool = False,
+        force: bool = False,
+    ):
         """
         De-Initialize :any:`GitWS`.
 
         The workspace is not working anymore after that. The corresponding :any:`GitWS` instance should be deleted.
+
+        Keyword Args:
+            prune: Remove dependencies, including non-project data!
+            force: Enforce to prune repositories with changes.
         """
+        if prune:
+            self._prune(self.workspace, force=force)
         return self.workspace.deinit()
 
     @staticmethod
+    def check_manifest(manifest_path: Path):
+        """
+        Check Manifest at ``manifest_path``.
+
+        Read in and evaluate.
+
+        Raises:
+            ManifestNotFoundError: If manifest does not exists.
+            ManifestError: If manifest is broken.
+        """
+        manifest_spec = ManifestSpec.load(manifest_path)
+        Manifest.from_spec(manifest_spec, path=str(manifest_path))
+
+    @staticmethod
     def clone(
         url: str,
+        path: Optional[Path] = None,
         main_path: Optional[Path] = None,
         manifest_path: Optional[Path] = None,
         group_filters: Optional[GroupFilters] = None,
+        depth: Optional[int] = None,
         revision: Optional[str] = None,
         force: bool = False,
         secho=None,
     ) -> "GitWS":
         """
-        Clone git `url`, initialize NEW Workspace and return corresponding :any:`GitWS`.
+        Clone git ``url``, initialize NEW Workspace and return corresponding :any:`GitWS`.
 
         Args:
             url: Main Project URL.
 
         Keyword Args:
-            main_path: Main Project Path.
-            mainfest_path: Manifest File Path. Relative to `main_path`. Default is 'git-ws.toml'.
+            path: Workspace Path. Parent directory of Git Clone Root Directory by default.
+            main_path: Main Project Path. Twice the URL stem in the current working directory by default.
+            manifest_path: Manifest File Path. Relative to ``main_path``. Default is ``git-ws.toml``.
                            This value is written to the configuration.
             group_filters: Default Group Filters.
                            This value is written to the configuration.
+            depth: Shallow Clone Depth.
             revision: Revision instead of default one.
             force: Ignore that the workspace is not empty.
-            secho: `click.secho` like print method for verbose output.
+            secho: :any:`click.secho` like print method for verbose output.
         """
         secho = secho or no_echo
         parsedurl = urllib.parse.urlparse(url)
         name = removesuffix(Path(parsedurl.path).name, ".git")
         if main_path is None:
             main_path = Path.cwd() / name / name
         else:
             main_path = main_path.resolve()
         main_path.parent.mkdir(parents=True, exist_ok=True)
-        path = main_path.parent
+        main_path_rel = resolve_relative(main_path)
+        path = path or main_path.parent
         if not force:
             Workspace.check_empty(path, main_path)
-        secho(f"===== {resolve_relative(main_path)} (MAIN {name!r}) =====", fg=_COLOR_BANNER)
+        secho(f"===== {main_path_rel} (MAIN {name!r}) =====", fg=_COLOR_BANNER)
         secho(f"Cloning {url!r}.", fg=_COLOR_ACTION)
-        clone_cache = AppConfig().options.clone_cache
-        git = Git(resolve_relative(main_path), clone_cache=clone_cache, secho=secho)
-        git.clone(url, revision=revision)
-        return GitWS.create(path, main_path, manifest_path=manifest_path, group_filters=group_filters, secho=secho)
+        options = AppConfig().options
+        clone_cache = options.clone_cache
+        if depth is None:
+            depth = options.depth
+        git = Git(main_path_rel, clone_cache=clone_cache, secho=secho)
+        git.clone(url, revision=revision, depth=depth)
+        return GitWS.create(
+            path,
+            main_path=main_path,
+            manifest_path=manifest_path,
+            group_filters=group_filters,
+            depth=depth,
+            secho=secho,
+        )
 
     def update(
         self,
         project_paths: Optional[ProjectPaths] = None,
         skip_main: bool = False,
         prune: bool = False,
         rebase: bool = False,
@@ -282,212 +386,249 @@
         Keyword Args:
             project_paths: Limit operation to these projects.
             skip_main: Exclude main project.
             prune: Remove obsolete files from workspace, including non-project data!
             rebase: Rebase instead of merge.
             force: Enforce to prune repositories with changes.
         """
+        # pylint: disable=too-many-locals
         workspace = self.workspace
-        used: List[Path] = [workspace.info.main_path]
+        main_path = workspace.info.main_path
+        depth = workspace.app_config.options.depth
+        used: List[Path] = []
+        linkfileupdater = LinkFileUpdater(workspace.path, secho=self.secho)
+        copyfileupdater = CopyFileUpdater(workspace.path, secho=self.secho)
         for clone in self._foreach(project_paths=project_paths, skip_main=skip_main, resolve_url=True):
-            used.append(Path(clone.project.path))
+            project = clone.project
+            used.append(Path(project.path))
             clone.check(diff=False, exists=False)
-            self._update(clone, rebase)
+            self._update(clone, rebase, depth)
+            linkfileupdater.set(project.path, project.linkfiles)
+            copyfileupdater.set(project.path, project.copyfiles)
+        if main_path and not skip_main:
+            used.append(main_path)
+            manifest_spec = self.get_manifest_spec()
+            main_path_str = str(workspace.info.main_path)
+            linkfileupdater.set(main_path_str, manifest_spec.linkfiles)
+            copyfileupdater.set(main_path_str, manifest_spec.copyfiles)
         if prune:
             self._prune(workspace, used, force=force)
+        if workspace.info.project_linkfiles or workspace.info.project_copyfiles or linkfileupdater or copyfileupdater:
+            # Update Links/Copies
+            self.secho("===== Update Files =====", fg=_COLOR_BANNER)
+            with workspace.edit_info() as info:
+                # Remove all obsolete files first, to all re-map without issues
+                linkfileupdater.remove(info.project_linkfiles)
+                copyfileupdater.remove(info.project_copyfiles)
+                linkfileupdater.update(info.project_linkfiles)
+                copyfileupdater.update(info.project_copyfiles)
 
-    def _update(self, clone: Clone, rebase: bool):
+    def _update(self, clone: Clone, rebase: bool, depth: Optional[int]):
         # Clone
         project = clone.project
         git = clone.git
         if git.is_cloned():
             # Determine actual version
             tag = git.get_tag()
             branch = git.get_branch()
             sha = git.get_sha()
+            revision = branch or tag or sha
 
             if project.revision in (sha, tag) and not branch:
                 self.secho("Nothing to do.", fg=_COLOR_ACTION)
+            elif git.get_shallow():
+                self.secho("Fetching.", fg=_COLOR_ACTION)
+                git.fetch(shallow=project.revision or revision)
+                shallow_sha = git.get_sha(revision="FETCH_HEAD")
+                git.checkout(shallow_sha)
             else:
-                revision = branch or tag or sha
+                # Fetch
+                self.secho("Fetching.", fg=_COLOR_ACTION)
+                git.fetch()
 
                 # Checkout
-                fetched = False
                 if project.revision and revision != project.revision:
-                    self.secho("Fetching.", fg=_COLOR_ACTION)
-                    git.fetch()
-                    fetched = True
                     git.checkout(project.revision)
                     branch = git.get_branch()
                     revision = branch or tag or sha
 
-                # Pull or Rebase in case we are on a branch (or have switched to it.)
+                # Rebase / Merge
                 if branch:
                     if rebase:
-                        if not fetched:
-                            self.secho("Fetching.", fg=_COLOR_ACTION)
-                            git.fetch()
                         self.secho(f"Rebasing branch {branch!r}.", fg=_COLOR_ACTION)
                         git.rebase()
                     else:
-                        if not fetched:
-                            self.secho(f"Pulling branch {branch!r}.", fg=_COLOR_ACTION)
-                            git.pull()
-                        else:
-                            self.secho(f"Merging branch {branch!r}.", fg=_COLOR_ACTION)
-                            git.merge(f"origin/{branch}")
+                        self.secho(f"Merging branch {branch!r}.", fg=_COLOR_ACTION)
+                        git.merge(f"origin/{branch}")
 
         else:
             self.secho(f"Cloning {project.url!r}.", fg=_COLOR_ACTION)
-            git.clone(project.url, revision=project.revision)
+            git.clone(project.url, revision=project.revision, depth=depth)
 
         if project.submodules:
             git.submodule_update(init=True, recursive=True)
 
-    def _prune(self, workspace: Workspace, used: List[Path], force: bool = False):
+    def _prune(self, workspace: Workspace, used: Optional[List[Path]] = None, force: bool = False):
+        used = used or []
         for obsolete_path in workspace.iter_obsoletes(used):
             rel_path = resolve_relative(obsolete_path)
             self.secho(f"===== {rel_path} (OBSOLETE) =====", fg=_COLOR_BANNER)
             self.secho(f"Removing {str(rel_path)!r}.", fg=_COLOR_ACTION)
             git = Git(obsolete_path, secho=self.secho)
             if force or not git.is_cloned() or git.is_empty():
                 shutil.rmtree(obsolete_path, ignore_errors=True)
             else:
                 raise GitCloneNotCleanError(resolve_relative(rel_path))
 
     def status(
         self,
         paths: Optional[Tuple[Path, ...]] = None,
+        banner: bool = False,
         branch: bool = False,
     ) -> Generator[Status, None, None]:
         """
-        Enriched Git Status.
+        Enriched Git Status - aka ``git status``.
+
+        The given ``paths`` are automatically mapped to the corresponding git clones.
 
         Keyword Args:
-            paths: Limit Git Status to `paths` only.
+            paths: Limit Git Status to ``paths`` only.
             branch: Dump branch information.
 
         Yields:
-            Status
+            :any:`Status`
         """
         for clone, cpaths in map_paths(tuple(self.clones()), paths):
-            self.secho(f"===== {clone.info} =====", fg=_COLOR_BANNER)
+            if banner:
+                self.secho(f"===== {clone.info} =====", fg=_COLOR_BANNER)
             clone.check()
             path = clone.git.path
             for status in clone.git.status(paths=cpaths, branch=branch):
                 yield status.with_path(path)
 
     def diff(self, paths: Optional[Tuple[Path, ...]] = None):
         """
-        Enriched Git Diff.
+        Enriched Git Diff - aka ``git diff``.
 
         Keyword Args:
-            paths: Limit Git Diff to `paths` only.
+            paths: Limit Git Diff to ``paths`` only.
         """
         for clone, cpaths in map_paths(tuple(self.clones()), paths):
             self.secho(f"===== {clone.info} =====", fg=_COLOR_BANNER)
             clone.check()
             clone.git.diff(paths=cpaths, prefix=Path(clone.project.path))
 
     def diffstat(self, paths: Optional[Tuple[Path, ...]] = None) -> Generator[DiffStat, None, None]:
         """
-        Enriched Git Diff Status.
+        Enriched Git Diff Status - aka ``git diff --stat``.
 
         Keyword Args:
-            paths: Limit Git Diff to `paths` only.
+            paths: Limit Git Diff to ``paths`` only.
 
         Yields:
-            DiffStat
+            :any:`DiffStat`
         """
         for clone, cpaths in map_paths(tuple(self.clones()), paths):
             self.secho(f"===== {clone.info} =====", fg=_COLOR_BANNER)
             clone.check()
             path = clone.git.path
             for diffstat in clone.git.diffstat(paths=cpaths):
                 yield diffstat.with_path(path)
 
     def checkout(self, paths: Optional[Tuple[Path, ...]] = None, force: bool = False):
         """
-        Enriched Git Checkout.
+        Enriched Git Checkout - aka ``git checkout``.
+
+        The given ``paths`` are automatically mapped to the corresponding git clones.
 
         Keyword Args:
-            paths: Limit Checkout to `paths` only. Otherwise run checkout on all git clones.
+            paths: Limit Checkout to ``paths`` only. Otherwise run checkout on all git clones.
             force: force checkout (throw away local modifications)
-
         """
         if paths:
             # Checkout specific files only
             for clone, cpaths in map_paths(tuple(self.clones()), paths):
                 self.secho(f"===== {clone.info} =====", fg=_COLOR_BANNER)
                 clone.check()
                 clone.git.checkout(revision=clone.project.revision, paths=cpaths, force=force)
         else:
             # Checkout all clones
+            depth = self.workspace.app_config.options.depth
             for clone in self.clones(resolve_url=True):
                 self.secho(f"===== {clone.info} =====", fg=_COLOR_BANNER)
                 git = clone.git
                 project = clone.project
                 if not git.is_cloned():
                     self.secho(f"Cloning {project.url!r}.", fg=_COLOR_ACTION)
-                    git.clone(project.url, revision=project.revision)
+                    git.clone(project.url, revision=project.revision, depth=depth)
                 if project.revision and not project.is_main:
                     git.checkout(revision=project.revision, force=force)
                 clone.check(exists=False)
 
     def add(self, paths: Tuple[Path, ...], force: bool = False, all_: bool = False):
         """
-        Add paths to index.
+        Add paths to index - aka ``git add``.
+
+        The given ``paths`` are automatically mapped to the corresponding git clones.
 
         Args:
-            paths: Paths to be added
+            paths: Paths to be added.
 
         Keyword Args:
             force: allow adding otherwise ignored files.
             all_: add changes from all tracked and untracked files.
         """
         if paths:
             for clone, cpaths in map_paths(tuple(self.clones()), paths):
-                clone.git.check()
+                clone.check()
                 clone.git.add(cpaths, force=force)
         else:
             if all_:
                 for clone in self.clones():
-                    clone.git.check()
+                    clone.check()
                     clone.git.add(all_=True, force=force)
             else:
                 raise ValueError("Nothing specified, nothing added.")
 
     # pylint: disable=invalid-name
     def rm(self, paths: Tuple[Path, ...], cached: bool = False, force: bool = False, recursive: bool = False):
         """
-        Remove.
+        Remove ``paths`` - aka ``git rm``
+
+        The given ``paths`` are automatically mapped to the corresponding git clones.
 
         Args:
             paths: Paths.
 
         Keyword Args:
             cached: only remove from the index
             force: override the up-to-date check
             recursive: allow recursive removal
         """
         if not paths:
             raise ValueError("Nothing specified, nothing removed.")
         for clone, cpaths in map_paths(tuple(self.clones()), paths):
-            clone.git.check()
+            clone.check()
             clone.git.rm(cpaths, cached=cached, force=force, recursive=recursive)
 
     def reset(self, paths: Tuple[Path, ...]):
-        """Reset `paths`."""
+        """
+        Reset ``paths`` - aka ``git reset``.
+
+        The given ``paths`` are automatically mapped to the corresponding git clones.
+        """
         for clone, cpaths in map_paths(tuple(self.clones()), paths):
-            clone.git.check()
+            clone.check()
             clone.git.reset(cpaths)
 
     def commit(self, msg: str, paths: Tuple[Path, ...], all_: bool = False):
         """
-        Commit.
+        Commit - aka ``git commit``.
+
+        The given ``paths`` are automatically mapped to the corresponding git clones.
 
         Args:
             msg: Commit Message
 
         Keyword Args:
             paths: Paths.
             all_: commit all changed files
@@ -507,76 +648,79 @@
             for clone in clones:
                 self.secho(f"===== {clone.info} =====", fg=_COLOR_BANNER)
                 clone.check()
                 clone.git.commit(msg, all_=all_)
 
     def tag(self, name: str, msg: Optional[str] = None, force: bool = False):
         """
-        Create Git Tag.
+        Create Git Tag `name` with `msg`.
 
         The following steps are done to create a valid tag:
 
-        1. store a frozen manifest to `main_path/.git-ws/manifests/<name>.toml`
-        2. commit frozen manifest from `main_path/.git-ws/manifests/<name>.toml`
+        1. store a frozen manifest to ``main_path/.git-ws/manifests/<name>.toml``
+        2. commit frozen manifest from ``main_path/.git-ws/manifests/<name>.toml``
         3. create git tag.
         """
+        main_path = self.main_path
+        if not main_path:
+            raise NoMainError()
         clone = Clone.from_project(self.workspace, next(self.projects()), secho=self.secho)
         self.secho(f"===== {clone.info} =====", fg=_COLOR_BANNER)
         git = clone.git
         # check
         if not force and git.get_tags(name):
             raise GitTagExistsError(name)
         # freeze
         manifest_path = MANIFESTS_PATH / f"{name}.toml"
         manifest_spec = self.get_manifest_spec(freeze=True, resolve=True)
-        (self.main_path / MANIFESTS_PATH).mkdir(exist_ok=True, parents=True)
-        (self.main_path / manifest_path).touch()
-        manifest_spec.save(self.main_path / manifest_path)
+        (main_path / MANIFESTS_PATH).mkdir(exist_ok=True, parents=True)
+        (main_path / manifest_path).touch()
+        manifest_spec.save(main_path / manifest_path)
         # commit
         paths = (manifest_path,)
         git.add(paths, force=True)
-        if any(git.status(paths=paths)):
-            git.commit(msg or name, paths=paths)
+        git.commit(msg or name, paths=paths)
         # tag
         git.tag(name, msg=msg, force=force)
 
     def run_foreach(
         self,
         command,
         project_paths: Optional[ProjectPaths] = None,
         reverse: bool = False,
     ):
         """
-        Run `command` on each clone.
+        Run ``command`` on each clone.
 
         Args:
             command: Command to run
 
         Keyword Args:
             project_paths: Limit to projects only.
             reverse: Operate in reverse order.
         """
         for clone in self.foreach(project_paths=project_paths, reverse=reverse):
             run(command, cwd=clone.git.path)
 
     def foreach(
-        self, project_paths: Optional[ProjectPaths] = None, resolve_url: bool = False, reverse: bool = False
+        self, project_paths: Optional[ProjectPaths] = None, reverse: bool = False
     ) -> Generator[Clone, None, None]:
         """
         User Level Clone Iteration.
 
+        We are printing the a banner for each clone.
+
         Keyword Args:
             project_paths: Limit to projects only.
-            resolve_url: Resolve URLs to absolute ones.
             reverse: Operate in reverse order.
 
         Yields:
-            Clone
+            :any:`Clone`
         """
-        for clone in self._foreach(project_paths=project_paths, resolve_url=resolve_url, reverse=reverse):
+        for clone in self._foreach(project_paths=project_paths, resolve_url=True, reverse=reverse):
             clone.check()
             yield clone
 
     def _foreach(
         self,
         project_paths: Optional[ProjectPaths] = None,
         skip_main: bool = False,
@@ -590,71 +734,81 @@
             if project_paths_filter(project):
                 self.secho(f"===== {clone.info} =====", fg=_COLOR_BANNER)
                 yield clone
             else:
                 self.secho(f"===== SKIPPING {clone.info} =====", fg=_COLOR_SKIP)
 
     def clones(
-        self, skip_main: bool = False, resolve_url: bool = False, reverse: bool = False
+        self, skip_main: bool = False, resolve_url: bool = True, reverse: bool = False
     ) -> Generator[Clone, None, None]:
         """
         Iterate over Clones.
 
         Keyword Args:
             skip_main: Skip Main Repository.
             resolve_url: Resolve URLs to absolute ones.
             reverse: Operate in reverse order.
 
         Yields:
-            Clone
+            :any:`Clone`
         """
         workspace = self.workspace
         projects = self.projects(skip_main=skip_main, resolve_url=resolve_url)
         if reverse:
             projects = reversed(tuple(projects))  # type: ignore
         for project in projects:
             clone = Clone.from_project(workspace, project, secho=self.secho)
             yield clone
 
     def projects(self, skip_main: bool = False, resolve_url: bool = False) -> Generator[Project, None, None]:
         """
-        Iterate over Projects.
+        Iterate over Projects in actual workspace.
 
         Keyword Args:
             skip_main: Skip Main Repository.
             resolve_url: Resolve URLs to absolute ones.
 
         Yields:
-            Project
+            :any:`Project`
         """
         workspace = self.workspace
         manifest_path = self.manifest_path
         group_filters = self.group_filters
         yield from ProjectIter(workspace, manifest_path, group_filters, skip_main=skip_main, resolve_url=resolve_url)
 
     def manifests(
         self,
     ) -> Generator[Manifest, None, None]:
-        """Iterate over Manifests."""
+        """
+        Iterate Over Manifests In Actual Workspace.
+        """
         workspace = self.workspace
         manifest_path = self.manifest_path
         group_filters = self.group_filters
         yield from ManifestIter(workspace, manifest_path, group_filters)
 
     @staticmethod
     def create_manifest(manifest_path: Path = MANIFEST_PATH_DEFAULT) -> Path:
-        """Create Manifest File at `manifest_path`within `project`."""
+        """Create Manifest File at ``manifest_path``."""
         if manifest_path.exists():
             raise ManifestExistError(manifest_path)
         manifest_spec = ManifestSpec()
         manifest_spec.save(manifest_path)
         return manifest_path
 
     def get_manifest_spec(self, freeze: bool = False, resolve: bool = False) -> ManifestSpec:
-        """Get Manifest."""
+        """
+        Get Manifest Specification.
+
+        Read the manifest file with the manifest specification.
+
+        Keyword Args:
+            freeze: Determine actual SHA of each project and use it as revision.
+            resolve: Add project specification of all transient dependencies.
+        """
         workspace = self.workspace
         manifest_path = self.manifest_path
         manifest_spec = ManifestSpec.load(manifest_path)
         if resolve:
             rdeps: List[ProjectSpec] = []
             for project in self.projects(skip_main=True):
                 project_spec = ProjectSpec.from_project(project)
@@ -665,21 +819,29 @@
         if freeze:
             manifest = Manifest.from_spec(manifest_spec)
             fdeps: List[ProjectSpec] = []
             for project_spec, project in zip(manifest_spec.dependencies, manifest.dependencies):
                 project_path = workspace.get_project_path(project)
                 git = Git(resolve_relative(project_path), secho=self.secho)
                 git.check()
-                revision = git.get_tag() or git.get_sha()
+                revision = git.get_sha()
                 fdeps.append(project_spec.update(revision=revision))
             manifest_spec = manifest_spec.update(dependencies=fdeps)
         return manifest_spec
 
     def get_manifest(self, freeze: bool = False, resolve: bool = False) -> Manifest:
-        """Get Manifest."""
+        """
+        Get Manifest.
+
+        Read the manifest file with the manifest specification and translate to manifest.
+
+        Keyword Args:
+            freeze: Determine actual SHA of each project and use it as revision.
+            resolve: Add project specification of all transient dependencies.
+        """
         manifest_path = self.workspace.get_manifest_path()
         manifest_spec = self.get_manifest_spec(freeze=freeze, resolve=resolve)
         return Manifest.from_spec(manifest_spec, path=str(manifest_path))
 
     def get_deptree(self, primary=False) -> DepNode:
         """Get Dependency Tree."""
         manifest = self.get_manifest()
```

### Comparing `git_ws-0.9.2/gitws/iters.py` & `git_ws-1.0.0/gitws/iters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -10,15 +10,20 @@
 # Git Workspace is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with Git Workspace. If not, see <https://www.gnu.org/licenses/>.
 
-""":any:`Manifest` and :any:`Project` Iterators."""
+"""
+Helpers to iterate over all :any:`Manifest` or :any:`Project` instances.
+
+Please note, these iterators require a :any:`Workspace` with existing manifest files within.
+The creation/cloning of missing project dependencies during the iteration is supported.
+"""
 import logging
 from fnmatch import fnmatchcase
 from pathlib import Path
 from typing import Callable, Generator, List, Optional, Tuple
 
 from ._util import resolve_relative
 from .datamodel import GroupFilters, Groups, GroupSelects, Manifest, ManifestSpec, Project
@@ -31,28 +36,28 @@
 FilterFunc = Callable[[str, Groups], bool]
 
 
 class ManifestIter:
     """
     Iterate over all :any:`Manifest` s.
 
-    The iterator takes a `workspace` and the path to a manifest file (`manifest_path`) of the main project.
+    The iterator takes a :any:`Workspace` and the path to a manifest file (`manifest_path`) of the main project.
     The manifest is read (:any:`ManifestSpec`) and translated to a :any:`Manifest`, which is yielded.
     The manifest files of the dependencies are also read, translated to a :any:`Manifest` and yielded likewise,
     until all manifest files and their dependencies are read.
     Dependencies which have been already yielded are not evaluated again.
     Means the first dependency (i.e. from the MAIN project) wins. Including the specified attributes (i.e. revision).
 
     Args:
         workspace: The actual workspace
-        manifest_path: Path to the manifest file **in the main project**.
+        manifest_path: Path to the manifest file.
         group_filters: Group Filters.
 
     Yields:
-        Manifest
+        :any:`Manifest`
     """
 
     # pylint: disable=too-few-public-methods
     def __init__(self, workspace: Workspace, manifest_path: Path, group_filters: GroupFilters):
         self.workspace: Workspace = workspace
         self.manifest_path: Path = manifest_path
         self.group_filters: GroupFilters = group_filters
@@ -108,15 +113,15 @@
             yield from self.__iter(dep_manifest_path, dep_manifest_spec, dep_filter)
 
 
 class ProjectIter:
     """
     Iterate over all :any:`Project` s.
 
-    The iterator takes a `workspace` and the path to a manifest file (`manifest_path`) of the main project.
+    The iterator takes a :any:`Workspace` and the path to a manifest file (`manifest_path`) of the main project.
     The manifest is read (:any:`ManifestSpec`) and all dependencies are translated to :any:`Project` s, which are
     yielded.
     The manifest files of the dependencies are also read, translated to a :any:`Project` s and yielded likewise,
     until all manifest files and their dependencies are read.
     Dependencies which have been already yielded are not evaluated again.
     Means the first dependency (i.e. from the MAIN project) wins. Including the specified attributes (i.e. revision).
 
@@ -126,15 +131,15 @@
         group_filters: Group Filters.
 
     Keyword Args:
         skip_main: Do not yield main project.
         resolve_url: Resolve relative URLs to absolute ones.
 
     Yields:
-        Project
+        :any:`Project`
     """
 
     # pylint: disable=too-few-public-methods
 
     def __init__(
         self,
         workspace: Workspace,
@@ -149,42 +154,51 @@
         self.skip_main: bool = skip_main
         self.resolve_url: bool = resolve_url
         self.__done: List[str] = []
 
     def __iter__(self) -> Generator[Project, None, None]:
         workspace = self.workspace
         info = workspace.info
-        self.__done = [str(info.main_path)]
-        if not self.skip_main:
-            main_path = info.main_path
-            main_git = Git(resolve_relative(workspace.main_path))
-            revision = main_git.get_revision()
-            yield Project(name=main_path.name, path=str(main_path), revision=revision, is_main=True)
+        main_path_rel = str(info.main_path or "")
+        self.__done = [main_path_rel]
         try:
             manifest_spec = ManifestSpec.load(self.manifest_path)
         except ManifestNotFoundError:
-            pass
-        else:
+            manifest_spec = ManifestSpec()
+        main_path = workspace.main_path
+        if main_path and not self.skip_main:
+            main_git = Git(resolve_relative(main_path))
+            revision = main_git.get_revision()
+            yield Project(
+                name=main_path.name,
+                path=main_path_rel,
+                revision=revision,
+                linkfiles=manifest_spec.linkfiles,
+                copyfiles=manifest_spec.copyfiles,
+                is_main=True,
+            )
+        if manifest_spec.dependencies:
             group_filters: GroupFilters = manifest_spec.group_filters + self.group_filters  # type: ignore
             group_selects = GroupSelects.from_group_filters(group_filters)
             filter_ = create_filter(group_selects, default=True)
-            yield from self.__iter(self.workspace.main_path, manifest_spec, filter_)
+            yield from self.__iter(main_path, manifest_spec, filter_)
 
     def __iter(
-        self, project_path: Path, manifest_spec: ManifestSpec, filter_: FilterFunc
+        self, project_path: Optional[Path], manifest_spec: ManifestSpec, filter_: FilterFunc
     ) -> Generator[Project, None, None]:
         # pylint: disable=too-many-locals
         deps: List[Tuple[Path, ManifestSpec, GroupSelects]] = []
         refurl: Optional[str] = None
         done: List[str] = self.__done
-        if manifest_spec.dependencies:
-            git = Git(resolve_relative(project_path))
+        if project_path and manifest_spec.dependencies:
+            project_path_rel = resolve_relative(project_path)
+            git = Git(project_path_rel)
             refurl = git.get_url()
             if not refurl:
-                raise GitCloneMissingOriginError(resolve_relative(project_path))
+                raise GitCloneMissingOriginError(project_path_rel)
 
         _LOGGER.debug("%r", manifest_spec)
 
         for spec in manifest_spec.dependencies:
             dep_project = Project.from_spec(manifest_spec, spec, refurl=refurl, resolve_url=self.resolve_url)
 
             # Update every path just once
@@ -217,72 +231,91 @@
             yield from self.__iter(dep_project_path, dep_manifest, dep_filter)
 
 
 def create_filter(group_selects: GroupSelects, default: bool = False) -> FilterFunc:
     """
     Create Group Filter Function.
 
-    Filter projects based on their `path` and `groups`.
-    The filter has `group_selects`. A specification which groups should be included or excluded.
-    The default selection of these groups is controlled by `default`.
+    Filter projects based on their ``path`` and ``groups``.
+    The filter has ``group_selects``, a specification which groups should be included or excluded.
+    The default selection of these groups is controlled by ``default``.
 
     Keyword Args:
-        group_selects: Iterable with :any`GroupSelect`.
-        default: Default selection of all `groups`.
+        group_selects: Iterable with :any:`GroupSelect`.
+        default: Default selection of all ``groups``.
 
-    >>> group_filters=('+test', '+doc', '+feature@dep', '-doc')
+    >>> group_filters = ('-@special', '+test', '+doc', '+feature@dep', '-doc')
     >>> group_selects = GroupSelects.from_group_filters(group_filters)
     >>> groupfilter = create_filter(group_selects)
-    >>> groupfilter('sub', tuple())
+    >>> groupfilter('sub', tuple())  # selected as there is no group
     True
-    >>> groupfilter('sub', ('foo', 'bar'))
+    >>> groupfilter('sub', ('foo', 'bar'))  # no group selected by group_filters
     False
-    >>> groupfilter('sub', ('test',))
+    >>> groupfilter('sub', ('test',))  # 'test' is selected by group_filters
     True
-    >>> groupfilter('sub', ('doc',))
+    >>> groupfilter('sub', ('doc',))  # 'doc' is deselected by group_filters
     False
-    >>> groupfilter('sub', ('test', 'doc'))
+    >>> groupfilter('sub', ('test', 'doc'))  # 'test' is selected by group_filters
     True
-    >>> groupfilter('sub', ('feature',))
+    >>> groupfilter('sub', ('feature',))  # 'feature' is only selected for 'dep', but not 'sub'
     False
-    >>> groupfilter('dep', ('feature',))
+    >>> groupfilter('dep', ('feature',))  # 'feature' is only selected for 'dep'
     True
+    >>> groupfilter('special', tuple())  # deselected, even without group
+    False
+    >>> groupfilter('special', ('foo', 'bar'))  # deselected
+    False
+    >>> groupfilter('special', ('test', 'bar'))  # deselected, but overwritten by '+test'
+    True
+
+    The same, but with ``default=True``:
 
     >>> groupfilter = create_filter(group_selects, default=True)
-    >>> groupfilter('sub', tuple())
+    >>> groupfilter('sub', tuple())  # selected as there is no group
     True
-    >>> groupfilter('sub', ('foo', 'bar'))
+    >>> groupfilter('sub', ('foo', 'bar'))  # no group selected by group_filters, but `default=True`
     True
-    >>> groupfilter('sub', ('test',))
+    >>> groupfilter('sub', ('test',))  # 'test' is selected by group_filters
     True
-    >>> groupfilter('sub', ('doc',))
+    >>> groupfilter('sub', ('doc',))  # 'doc' is deselected by group_filters
     False
-    >>> groupfilter('sub', ('test', 'doc'))
+    >>> groupfilter('sub', ('test', 'doc'))  # 'test' is selected by group_filters
     True
-    >>> groupfilter('sub', ('feature',))
+    >>> groupfilter('sub', ('feature',))  # 'feature' is only selected for 'dep', but not 'sub', but `default=True`
     True
-    >>> groupfilter('dep', ('feature',))
+    >>> groupfilter('dep', ('feature',))  # 'feature' is only selected for 'dep'
+    True
+    >>> groupfilter('special', tuple())  # deselected, even without group
+    False
+    >>> groupfilter('special', ('foo', 'bar'))  # deselected
+    False
+    >>> groupfilter('special', ('test', 'bar'))  # deselected, but overwritten by '+test'
     True
     """
 
     if group_selects:
 
         def filter_(path: str, groups: Groups):
             if groups:
                 selects = {group: default for group in groups}
-                for group_select in group_selects:
-                    if group_select.group not in selects:
-                        # not relevant group name
-                        continue
-                    if group_select.path and not fnmatchcase(path, group_select.path):
-                        # not relevant path
-                        continue
-                    selects[group_select.group] = group_select.select
-                return any(selects.values())
-            return True
+            else:
+                selects = {None: True}
+            for group_select in group_selects:
+                group = group_select.group
+                if group and group not in selects:
+                    # not relevant group name
+                    continue
+                if group_select.path and not fnmatchcase(path, group_select.path):
+                    # not relevant path
+                    continue
+                if group:
+                    selects[group] = group_select.select
+                else:
+                    selects = {group: group_select.select for group in selects}
+            return any(selects.values())
 
     else:
 
         def filter_(path: str, groups: Groups):
             # pylint: disable=unused-argument
             if groups:
                 return default
```

### Comparing `git_ws-0.9.2/gitws/manifestfinder.py` & `git_ws-1.0.0/gitws/manifestfinder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -10,25 +10,31 @@
 # Git Workspace is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with Git Workspace. If not, see <https://www.gnu.org/licenses/>.
 
-"""Find proper manifest."""
+"""GIT Tag Related Manifest Finder."""
 
 from pathlib import Path
 from typing import Optional
 
 from .const import MANIFESTS_PATH
 from .git import Git
 
 
 def find_manifest(path: Path) -> Optional[Path]:
-    """Return Path to manifest if clone has been tagged before."""
+    """
+    Return Path to manifest if clone has been tagged before.
+
+    The git clone at ``path`` can be checked out to a tag, branch or SHA.
+    If the clone has been tagged by by :any:`GitWS` and this tag is currently checked out,
+    this function will return the path to the related manifest.
+    """
     if path.exists():
         git = Git(path=path)
         if not git.get_branch():
             tag = git.get_tag()
             if tag:
                 manifest_path = MANIFESTS_PATH / f"{tag}.toml"
                 if (path / manifest_path).exists():
```

### Comparing `git_ws-0.9.2/gitws/workspace.py` & `git_ws-1.0.0/gitws/workspace.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -13,29 +13,30 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with Git Workspace. If not, see <https://www.gnu.org/licenses/>.
 
 """
 Workspace Handling.
 
-The :any:`Workspace` class represents the file system location containing all git clones.
+The :any:`Workspace` class represents the location containing all git clones.
 :any:`Info` is a helper.
 """
 import logging
 import shutil
+from contextlib import contextmanager
 from pathlib import Path
 from typing import Any, Dict, Generator, List, Optional
 
 import tomlkit
 
 from ._basemodel import BaseModel
 from ._util import resolve_relative
 from .appconfig import AppConfig, AppConfigData, AppConfigLocation
 from .const import GIT_WS_PATH, INFO_PATH, MANIFEST_PATH_DEFAULT
-from .datamodel import GroupFilters, Project
+from .datamodel import GroupFilters, Project, ProjectFileRefsMutable
 from .exceptions import InitializedError, OutsideWorkspaceError, UninitializedError, WorkspaceNotEmptyError
 from .workspacefinder import find_workspace
 
 _LOGGER = logging.getLogger("git-ws")
 
 
 class Info(BaseModel):
@@ -45,64 +46,89 @@
     The workspace information container assembles all information which has to be kept persistant between tool
     invocations.
 
     Keyword Args:
         main_path: Path to main project. Relative to workspace root directory.
     """
 
-    main_path: Path
+    main_path: Optional[Path] = None
     """
     Path to main project. Relative to workspace root directory.
     """
 
+    project_linkfiles: ProjectFileRefsMutable = {}
+    """
+    Project Symlinks.
+
+    These symlinks have been created by GitWS and will be removed if not needed anymore.
+    """
+
+    project_copyfiles: ProjectFileRefsMutable = {}
+    """
+    Project File Copies.
+
+    These files have been copied by GitWS and will be removed if not needed anymore.
+    """
+
     @staticmethod
     def load(path: Path) -> "Info":
         """
-        Load Workspace Information from GitWS root directory at `path`.
+        Load Workspace Information from GitWS root directory at ``path``.
 
-        The workspace information is stored at `{path}/.gitws/info.toml`.
+        The workspace information is stored at ``{path}/.gitws/info.toml``.
 
         Args:
             path: Path to GitWS root directory.
         """
         infopath = path / INFO_PATH
         doc = tomlkit.parse(infopath.read_text())
         return Info(
-            main_path=doc["main_path"],
+            main_path=doc.get("main_path", None),
+            project_linkfiles=doc.get("project_linkfiles", {}),
+            project_copyfiles=doc.get("project_copyfiles", {}),
         )
 
     def save(self, path: Path):
         """
-        Save Workspace Information at GitWS root directory at `path`.
+        Save Workspace Information at GitWS root directory at ``path``.
 
-        The workspace information is stored at `{path}/.gitws/info.toml`.
+        The workspace information is stored at ``{path}/.gitws/info.toml``.
 
         Args:
             path: Path to GitWS root directory.
         """
         infopath = path / INFO_PATH
         infopath.parent.mkdir(parents=True, exist_ok=True)
+        # structure
         try:
             doc = tomlkit.parse(infopath.read_text())
         except FileNotFoundError:
             doc = tomlkit.document()
             doc.add(tomlkit.comment("Git Workspace System File. DO NOT EDIT."))
             doc.add(tomlkit.nl())
-            doc.add("main_path", "")  # type: ignore
-        doc["main_path"] = str(self.main_path)
+        # update
+        selfdict = self.dict(exclude_none=True)
+        selfdict["main_path"] = str(self.main_path) if self.main_path else None
+        for name, value in selfdict.items():
+            if value:
+                doc[name] = value
+            else:
+                doc.pop(name, None)
+        # write
         infopath.write_text(tomlkit.dumps(doc))
 
 
 class Workspace:
 
     """
     Workspace.
 
     The workspace contains all git clones, but is *NOT* a git clone itself.
-    A workspace refers to a main git clone, which defines the workspace content (i.e. dependencies).
+    A workspace refers to a main git clone or a standalone manifest, which defines the workspace content
+    (i.e. dependencies).
 
     Args:
         path: Workspace Root Directory.
         info: Workspace Information.
     """
 
     def __init__(self, path: Path, info: Info):
@@ -122,35 +148,35 @@
 
         Keyword Args:
             path (Path): directory or file within the workspace. Current working directory by default.
 
         Raises:
             UninitializedError: If directory of file is not within a workspace.
 
-        The workspace root directory contains a sub directory `.gitws`.
-        This one is searched upwards the given `path`.
+        The workspace root directory contains a sub directory ``.gitws``.
+        This one is searched upwards the given ``path``.
         """
         path = find_workspace(path=path)
         if path:
             return path
         raise UninitializedError()
 
     @staticmethod
     def from_path(path=None) -> "Workspace":
         """
-        Create :any:`Workspace` for existing workspace at `path`.
+        Create :any:`Workspace` for existing workspace at ``path``.
 
         Keyword Args:
             path (Path): directory or file within the workspace. Current working directory by default.
 
         Raises:
             UninitializedError: If directory of file is not within a workspace.
 
-        The workspace root directory contains a sub directory `.gitws`.
-        This one is searched upwards the given `path`.
+        The workspace root directory contains a sub directory ``.gitws``.
+        This one is searched upwards the given ``path``.
         """
         path = Workspace.find_path(path=path)
         info = Info.load(path)
         workspace = Workspace(path, info)
         _LOGGER.info("Workspace path=%s main=%s", path, info.main_path)
         _LOGGER.info("%r", workspace.config)
         return workspace
@@ -160,76 +186,94 @@
         """Return :any:`Info` if workspace is already initialized."""
         infopath = path / INFO_PATH
         if infopath.exists():
             return Info.load(path)
         return None
 
     @staticmethod
-    def check_empty(path: Path, main_path: Path):
-        """Check if Workspace at `path` with `main_path` is empty."""
-        if any(item != main_path for item in path.iterdir()):
-            raise WorkspaceNotEmptyError(resolve_relative(path))
+    def check_empty(path: Path, main_path: Optional[Path]):
+        """Check if Workspace at ``path`` with ``main_path`` is empty."""
+        items = [item for item in path.iterdir() if item != main_path]
+        if any(items):
+            raise WorkspaceNotEmptyError(resolve_relative(path), items)
 
     @staticmethod
     def init(
         path: Path,
-        main_path: Path,
+        main_path: Optional[Path] = None,
         manifest_path: Optional[Path] = None,
         group_filters: Optional[GroupFilters] = None,
+        depth: Optional[int] = None,
         force: bool = False,
     ) -> "Workspace":
         """
-        Initialize new :any:`Workspace` at `path`.
+        Initialize new :any:`Workspace` at ``path``.
 
         Args:
             path:  Path to the workspace
-            main_path:  Path to the main project. Relative to `path`.
 
         Keyword Args:
-            manifest_path:  Path to the manifest file. Relative to `main_path`. Default is `git-ws.toml`.
+            main_path:  Path to the main project. Relative to ``path``.
+            manifest_path:  Path to the manifest file. Relative to ``main_path`` or ``path``.
+                            Default is ``git-ws.toml``.
             group_filters: Group Filters.
+            depth: Shallow Clone Depth.
             force: Ignore that the workspace exists.
 
         Raises:
-            OutsideWorkspaceError: `main_path` is not within `path`.
+            InitializedError: ``path`` already contains workspace.
+            OutsideWorkspaceError: ``main_path`` is not within ``path``.
         """
         if not force:
             info = Workspace.is_init(path)
             if info:
                 raise InitializedError(path, info.main_path)
 
         # Normalize
-        try:
-            main_path = (path / main_path).resolve().relative_to(path.resolve())
-        except ValueError:
-            raise OutsideWorkspaceError(path, main_path) from None
+        if main_path:
+            try:
+                main_path = (path / main_path).resolve().relative_to(path.resolve())
+            except ValueError:
+                raise OutsideWorkspaceError(path, main_path, "Project") from None
 
         # Initialize Info
         info = Info(main_path=main_path)
         info.save(path)
         workspace = Workspace(path.resolve(), info)
         with workspace.app_config.edit(AppConfigLocation.WORKSPACE) as config:
             config.manifest_path = str(manifest_path or MANIFEST_PATH_DEFAULT)
             config.group_filters = group_filters
+            config.depth = depth
         _LOGGER.info("Workspace path=%s main=%s", path, info.main_path)
         _LOGGER.info("%r", workspace.config)
         return workspace
 
     def deinit(self):
         """
         Deinitialize.
 
-        Remove `GIT_WS_PATH` directory.
+        Remove ``GIT_WS_PATH`` directory.
         """
         shutil.rmtree(self.path / GIT_WS_PATH)
 
     @property
-    def main_path(self) -> Path:
-        """Resolved Path to main project."""
-        return self.path / self.info.main_path
+    def main_path(self) -> Optional[Path]:
+        """Resolved Path To Main Project."""
+        info_main_path = self.info.main_path
+        if info_main_path:
+            return self.path / info_main_path
+        return None
+
+    @property
+    def base_path(self) -> Path:
+        """Resolved Path To Main Project Or Workspace."""
+        info_main_path = self.info.main_path
+        if info_main_path:
+            return self.path / info_main_path
+        return self.path
 
     @property
     def config(self) -> AppConfigData:
         """Application Configuration Values."""
         return self.app_config.options
 
     def get_project_path(self, project: Project, relative: bool = False) -> Path:
@@ -244,33 +288,63 @@
         """
         project_path = self.path / project.path
         if relative:
             project_path = resolve_relative(project_path)
         return project_path
 
     def get_manifest_path(self, manifest_path: Optional[Path] = None) -> Path:
-        """Get Resolved Manifest Path."""
-        return self.main_path / (manifest_path or self.app_config.options.manifest_path or MANIFEST_PATH_DEFAULT)
+        """
+        Get Resolved Manifest Path.
+
+        Keyword Args:
+            manifest_path: Absolute Or Relative (To ``self.base_path``) Manifest Path.
+
+        The manifest path is choosen according to the following list, the first matching wins:
+
+        * Explicit manifest path specified by ``manifest_path``.
+        * Path from configuration (set during ``init``, ``clone`` or later on).
+        * ``git-ws.toml`` (default)
+        """
+        return self.base_path / (manifest_path or self.app_config.options.manifest_path or MANIFEST_PATH_DEFAULT)
 
     def get_group_filters(self, group_filters: Optional[GroupFilters] = None) -> GroupFilters:
-        """Get Group Selects."""
+        """
+        Get Group Filters.
+
+        Keyword Args:
+            group_filters: Group Filters.
+
+        The group filter is choosen according to the following list, the first matching wins:
+
+        * Explicit group filter specified by ``group_filters``.
+        * Path from configuration (set during ``init``, ``clone`` or later on).
+        * empty group filters.
+        """
         if group_filters is None:
             return self.app_config.options.group_filters or GroupFilters()
         return group_filters
 
     def iter_obsoletes(self, used: List[Path]) -> Generator[Path, None, None]:
-        """Yield obsolete paths except `used` ones."""
+        """Yield paths except *used* ones."""
         usemap: Dict[str, Any] = {GIT_WS_PATH.name: {}}
         for path in used:
             pathmap = usemap
             for part in path.parts:
                 pathmap[part] = {}
                 pathmap = pathmap[part]
         yield from _iter_obsoletes(self.path, usemap)
 
+    @contextmanager
+    def edit_info(self) -> Generator[Info, None, None]:
+        """Yield Contextmanager to edit :any:`Info` and write back changes."""
+        try:
+            yield self.info
+        finally:
+            self.info.save(self.path)
+
 
 def _iter_obsoletes(path, usemap):
     for sub in sorted(path.iterdir()):
         if sub.name in usemap:
             subusemap = usemap[sub.name]
             if subusemap:
                 yield from _iter_obsoletes(sub, subusemap)
```

### Comparing `git_ws-0.9.2/gitws/workspacefinder.py` & `git_ws-1.0.0/gitws/workspacefinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 c0fec0de
+# Copyright 2022-2023 c0fec0de
 #
 # This file is part of Git Workspace.
 #
 # Git Workspace is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -24,16 +24,16 @@
 def find_workspace(path: Optional[Path] = None) -> Optional[Path]:
     """
     Find Workspace Root Directory.
 
     Keyword Args:
         path (Path): directory or file within the workspace. Current working directory by default.
 
-    The workspace root directory contains a sub directory `.gitws`.
-    This one is searched upwards the given `path`.
+    The workspace root directory contains a sub directory ``.gitws``.
+    This one is searched upwards the given ``path``.
     """
     spath = path or Path.cwd()
     while True:
         gitwspath = spath / INFO_PATH
         if gitwspath.exists():
             return spath
         if spath == spath.parent:
```

### Comparing `git_ws-0.9.2/pyproject.toml` & `git_ws-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git-ws"
-version = "0.9.2"
+version = "1.0.0"
 description = "Git Workspace - Multi Repository Management Tool"
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 authors = [
     "c0fec0de <c0fec0de@gmail.com>",
     "Martin Höher <martin@rpdev.net>",
 ]
@@ -22,28 +22,28 @@
 "Documentation" = "https://git-ws.readthedocs.io/en/latest/"
 "Bug Tracker" = "https://github.com/c0fec0de/git-ws/issues"
 
 [tool.poetry.scripts]
 git-ws = 'gitws._cli:main'
 
 [tool.poetry.dependencies]
-python = '^3.7'
+python = '^3.7.2'
 anytree = "*"
 appdirs = "^1.4.4"
-click = '^8.0.0'
+click = '>=6.7.0,<9.0.0'
 coloredlogs = '^15.0.1'
 pydantic = '^1.10.0'
 tomlkit = '>=0.11.5,<1.0.0'
 
 [tool.poetry.group.test.dependencies]
 black = '^22.3.0'
 coverage = '^6.4.4'
 isort = '^5.9'
-mypy = ">=0.971"
-pylint = '^2.13.5'
+mypy = "~1.0.0"
+pylint = '^2.15'
 pytest = '^6.2'
 tabulate = '>=0.8.10,<1.0.0'
 types-appdirs = "^1.4.3"
 
 [tool.poetry.group.doc.dependencies]
 sphinx = '^5.1.1'
 sphinx-rtd-theme = "^1.0.0"
@@ -101,27 +101,30 @@
 isolated_build = True
 
 [tox:.package]
 basepython = python3
 
 [testenv:py]
 allowlist_externals = *
+setenv =
+    LANGUAGE=en_US
+
 commands =
-    poetry install --with=dev --with=doc
+    poetry install --with=test --with=doc
     poetry run black .
     poetry run isort .
-    poetry run coverage run --branch -m pytest --doctest-glob=docs/*.rst --doctest-modules --ignore-glob=tests/testdata* --ignore=docs/conf.py --log-level=DEBUG -vv --junitxml=report.xml
+    poetry run coverage run --source=gitws --branch -m pytest --doctest-glob=docs/*.rst --doctest-modules --ignore-glob=tests/testdata* --ignore=docs/conf.py --log-level=DEBUG -vv --junitxml=report.xml
     poetry run coverage report
     poetry run coverage html
     poetry run coverage xml
     poetry run pylint gitws tests
     poetry run mypy gitws
     poetry run make html -C docs
 
 [testenv:py-min]
 allowlist_externals = *
 commands =
-    poetry install --without=dev --without=doc
+    poetry install --without=test --without=doc
     poetry run python -c 'import gitws'
     poetry run git-ws --version
     poetry run python -m gitws --version
 """
```

### Comparing `git_ws-0.9.2/setup.py` & `git_ws-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,383 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: git-ws
+Version: 1.0.0
+Summary: Git Workspace - Multi Repository Management Tool
+License: LGPL-3.0-or-later
+Author: c0fec0de
+Author-email: c0fec0de@gmail.com
+Requires-Python: >=3.7.2,<4.0.0
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: anytree
+Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Requires-Dist: click (>=6.7.0,<9.0.0)
+Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
+Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: tomlkit (>=0.11.5,<1.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['gitws', 'gitws._cli']
+[![PyPI Version](https://badge.fury.io/py/git-ws.svg)](https://badge.fury.io/py/git-ws)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/git-ws.svg?label=pypi%20downloads)](https://pypi.python.org/pypi/git-ws)
+[![Python Build](https://github.com/c0fec0de/git-ws/actions/workflows/main.yml/badge.svg)](https://github.com/c0fec0de/git-ws/actions/workflows/main.yml)
+[![Documentation](https://readthedocs.org/projects/git-ws/badge/?version=latest)](https://git-ws.readthedocs.io/en/latest/?badge=latest)
+[![Coverage Status](https://coveralls.io/repos/github/c0fec0de/git-ws/badge.svg?branch=main)](https://coveralls.io/github/c0fec0de/git-ws?branch=main)
+[![python-versions](https://img.shields.io/pypi/pyversions/git-ws.svg)](https://pypi.python.org/pypi/git-ws)
+[![pylint](https://img.shields.io/badge/linter-pylint-%231674b1?style=flat)](https://www.pylint.org/)
+[![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-package_data = \
-{'': ['*']}
+# Git Workspace - Multi Repository Management Tool
 
-install_requires = \
-['anytree',
- 'appdirs>=1.4.4,<2.0.0',
- 'click>=8.0.0,<9.0.0',
- 'coloredlogs>=15.0.1,<16.0.0',
- 'pydantic>=1.10.0,<2.0.0',
- 'tomlkit>=0.11.5,<1.0.0']
-
-entry_points = \
-{'console_scripts': ['git-ws = gitws._cli:main']}
-
-setup_kwargs = {
-    'name': 'git-ws',
-    'version': '0.9.2',
-    'description': 'Git Workspace - Multi Repository Management Tool',
-    'long_description': '[![PyPI Version](https://badge.fury.io/py/git-ws.svg)](https://badge.fury.io/py/git-ws)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/git-ws.svg?label=pypi%20downloads)](https://pypi.python.org/pypi/git-ws)\n[![Python Build](https://github.com/c0fec0de/git-ws/actions/workflows/main.yml/badge.svg)](https://github.com/c0fec0de/git-ws/actions/workflows/main.yml)\n[![Documentation](https://readthedocs.org/projects/git-ws/badge/?version=latest)](https://git-ws.readthedocs.io/en/latest/?badge=latest)\n[![Coverage Status](https://coveralls.io/repos/github/c0fec0de/git-ws/badge.svg?branch=main)](https://coveralls.io/github/c0fec0de/git-ws?branch=main)\n[![python-versions](https://img.shields.io/pypi/pyversions/git-ws.svg)](https://pypi.python.org/pypi/git-ws)\n[![pylint](https://img.shields.io/badge/linter-pylint-%231674b1?style=flat)](https://www.pylint.org/)\n[![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n# Git Workspace - Multi Repository Management Tool\n\n* [Installation](#installation)\n* [Usage](#usage)\n* [Cheat-Sheet](#cheat-sheet)\n* [Python API](#api)\n* [Alternatives](#alternatives)\n\nGit Workspace is a lightweight tool for creating and managing *workspaces* consisting of several interdependent `git` repositories. Starting from a *main repository*, Git Workspace discovers dependencies specified in a *manifest file*, fetching any specified required repositories and assembling them into a single workspace.\n\n![Workspace](https://github.com/c0fec0de/git-ws/raw/main/docs/images/workspace.png)\n\n👉 You can read more about the used [nomenclature](https://git-ws.readthedocs.io/en/latest/manual/nomenclature.html) in the [documentation](https://git-ws.readthedocs.io/en/latest/index.html).\n\n\n# 📦 Installation\n\nGit Workspace is written in Python and - as usual - installing it is pretty easy:\n\n```bash\npip install git-ws\n```\n\nAnd that\'s it! Ideally, if your project also uses Python, we recommend adding Git Workspace as a dependency to it as well, so that you can track the exact version of it together with your other dependencies. For example, if you use `poetry`, add it by running\n\n```bash\n# Add Git Workspace as development dependency:\npoetry add --group dev git-ws\n```\n\n\n# 📔 Usage\n\nGit Workspace is integrated into git `git ws` - this is what you will be using most of the time.\n\nLet\'s assume we have a project called `myapp`, which requires a library `mylib` that is maintained in another `git` repository. In order to use this project with Git Workspace, `myapp` needs to provide a so called *manifest*. An Git Workspace manifest is a simple [TOML](https://toml.io/) file - by default called `git-ws.toml` in the project\'s root folder - which defines the dependencies a project has as well as some other meta information. A minimal manifest for our project could look like this:\n\n```toml\n[[dependencies]]\nname = "mylib"\nurl = "git@github.com:example/mylib.git"\nrevision = "v2.3.4"\n```\n\nIf `myapp` and `mylib` are stored on the same server (side-by-side), than the manifest can even be simpler:\n\n```toml\n[[dependencies]]\nname = "mylib"\nrevision = "v2.3.4"\n```\n\nThe project will be searched via a relative path (which is either `../mylib` or `../mylib.git` depending on the main repository\'s URL). Relative paths are in general useful as they allow to use the same protocol for the main repository as well as any of its dependencies.\n\nTo build a workspace from a project prepared like that, simply clone it via `git ws`:\n\n```bash\ncd $HOME/Projects\nmkdir my_app_workspace\ncd my_app_workspace\ngit ws clone --update git@github.com:example/myapp.git\n```\n\n👉 Without the `--update` option, only the main repository will be fetched.\n\nThe above will clone the app repository and also the library side-by-side:\n\n```bash\nls -a\n# Should print something like\n.\n..\n.git-ws\nmyapp\nmylib\n```\n\nAs you can see, besides the two repositories we wanted, there is also a hidden `.git-ws` folder where the tool stores the needed configuration data.\n\nSometimes there are use cases where using `git ws clone` cannot be used. For example, when a CI/CD system creates the initial clone of the main repository, you may need a way to fetch the remaining projects. This can be done by simply running the following within the main project:\n\n```bash\ngit ws init --update\n```\n\n👉 As with `git ws clone`, without the `--update`, no dependencies will be fetched.\n\nAnother important use case is keeping a workspace up-to-date. Lets say you pull in an update in the main repository, which in turn might cause changes in the manifest to be pulled in as well. Updating the existing workspace is as simple as\n\n```bash\n# Update the workspace (main and all dependent repositories):\ngit ws update\n\n# Alternatively, run `git rebase` instead of `git pull` in dependencies:\ngit ws update --rebase\n```\n## Cheat-Sheet\n\n#### Initialization\n\n| Command | Description |\n| --- | --- |\n| `git ws clone URL` | Clone git repository from `URL` as main repository and initialize Git Workspace |\n| `git ws init` | Initialize Git Workspace. Use current git clone as main repository |\n| `git ws manifest create` | Create well documented, empty manifest |\n\n#### Basic\n\n| Command | Description |\n| --- | --- |\n| `git ws update` | Pull latest changes on main repository and all dependent repositories (clone them if needed) |\n| `git ws update --rebase` | Same as above, but fetch and rebase instead of pull |\n| `git ws status` | Run `git status` on all repositories (displayed paths include the actual clone path) |\n| `git ws add FILES` | Run `git add FILE` on `FILES` in the corresponding repositories |\n| `git ws reset FILES` | Run `git reset FILE` on `FILES` in the corresponding repositories. Undo `git add` |\n| `git ws commit FILES -m MESSAGE` | Run `git commit FILE` on `FILES` in the corresponding repositories |\n| `git ws commit -m MESSAGE` | Run `git commit` repositories with changes |\n| `git ws checkout FILES` | Run `git checkout FILE` on `FILES` in the corresponding repositories |\n| `git ws checkout` | Checkout git revision specified as in the manifest(s) (clone them if needed) |\n\n#### Run Commands on all repositories\n\n| Command | Description |\n| --- | --- |\n| `git ws push` | Run `git push` on all repositories (in reverse order) |\n| `git ws fetch` | Run `git fetch` on all repositories |\n| `git ws rebase` | Run `git rebase` on all repositories |\n| `git ws pull` | Run `git pull` on all repositories |\n| `git ws diff` | Run `git diff` on all repositories |\n| `git ws git CMD` | Run `git CMD` on all repositories |\n| `git ws foreach CMD` | Run `CMD` on all repositories |\n\n#### Other\n\n| Command | Description |\n| --- | --- |\n| `git ws manifest freeze`   | Print The Resolved Manifest With SHAs For All Project Revisions. |\n| `git ws manifest path`     | Print Path to Main Manifest File. |\n| `git ws manifest paths`    | Print Paths to ALL Manifest Files. |\n| `git ws manifest resolve`  | Print The Manifest With All Projects And All Their Dependencies. |\n| `git ws manifest upgrade`  | Update Manifest To Latest Version. |\n| `git ws manifest validate` | Validate The Current Manifest, Exiting With An Error On Issues. |\n| `git ws info main-path`      | Print Path to Main Git Clone. |\n| `git ws info project-paths`  | Print Paths to all git clones. |\n| `git ws info workspace-path` | Print Path to Workspace. |\n| `git ws info dep-tree` | Print Dependency Tree. |\n| `git ws info dep-tree --dot \\| dot -Tpng > dep-tree.png` | Draw Dependency Diagramm (needs [graphviz](https://graphviz.org)) |\n\n\n## 🐍 Python API\n\nGit Workspace is written in Python. Besides the `git ws` command line tool, there is also an API which you can use to further automate workspace creation and maintenance. If you are interested, have a look into the [API documentation](https://git-ws.readthedocs.io/en/latest/api/gitws.html).\n\n\n## 🤝 Alternatives\n\nBefore writing Git Workspace, we investigates several other existing tools in the hope they would fulfil out needs. In particular, we looked into the following tools and methodologies which are widely used to organize large projects:\n\n- [`git submodules`](https://git-scm.com/book/en/v2/Git-Tools-Submodules).\n- Google\'s [repo](https://gerrit.googlesource.com/git-repo/) tool.\n- The [`west`](https://docs.zephyrproject.org/latest/develop/west/index.html) tool developed in the scope of [Zephyr](https://www.zephyrproject.org/).\n- Leaving the pure `git` domain, one can also use a package manager like [`conan`](https://conan.io/).\n- And lastly, there are also approaches to still pack everything into a large so called *monorepo*.\n\nUnfortunately, none of the tools we tested really satisfied us. But hey, as we are developers - *why not starting our own tool for the purpose?*\n\nAnd that\'s what we did - Git Workspace is a our tool for managing a large workspace consisting of several smaller `git` projects. Here is how it compares to the other tools we evaluated:\n\n\n|                           | `git submodules` | `repo` | `west` | *Monorepos* | `git ws` |\n| ------------------------- | ---------------- | ------ | ------ | ----------- | --------- |\n| Reusable Components       | ✅               | ✅     | ✅     | ➖          | ✅        |\n| Ease of Use               | ➖               | ✅     | ✅     | ✅          | ✅        |\n| Editable Components       | ➖               | ✅     | ➖     | ✅          | ✅        |\n| Freezing Configurations   | ✅               | ✅     | ✅     | ✅          | ✅        |\n| Transitive Dependencies   | ➖               | ➖     | ✅     | ➖          | ✅        |\n| Relative Dependency Paths | ✅               | ✅     | ➖     | ➖          | ✅        |\n| Branches as dependencies  | ➖               | ✅     | ✅     | ➖          | ✅        |\n\n👉 Please note that our view on the various features might be biased. As we did, always look at all the options available to you before deciding for one tool or the other. While the other tools in comparison did not model what we needed for our workflow, they might just be what you are looking for.\n\nIf you want to learn more, have a look into the [documentation](https://git-ws.readthedocs.io/en/latest/manual/why.html).\n\n',
-    'author': 'c0fec0de',
-    'author_email': 'c0fec0de@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+* [Installation](https://github.com/c0fec0de/git-ws#-installation)
+* [Usage](https://github.com/c0fec0de/git-ws#-usage)
+* [Getting Started](https://github.com/c0fec0de/git-ws#-getting-started)
+* [Cheat-Sheet](https://github.com/c0fec0de/git-ws#%EF%B8%8F-cheat-sheet)
+* [Python API](https://github.com/c0fec0de/git-ws#-python-api)
+* [Alternatives](https://github.com/c0fec0de/git-ws#-alternatives)
+
+Git Workspace is a lightweight tool for creating and managing *workspaces* consisting of several interdependent `git` repositories. Starting from a *main repository*, Git Workspace discovers dependencies specified in a *manifest file*, fetching any specified required repositories and assembling them into a single workspace.
+
+![Workspace](https://github.com/c0fec0de/git-ws/raw/main/docs/images/workspace.png)
+
+👉 You can read more about the used [nomenclature](https://git-ws.readthedocs.io/en/latest/manual/nomenclature.html) in the [documentation](https://git-ws.readthedocs.io/en/latest/index.html).
+
+
+
+## 📦 Installation
+
+Git Workspace is written in Python and - as usual - installing it is pretty easy:
+
+```bash
+pip install git-ws
+```
+
+And that's it! Ideally, if your project also uses Python, we recommend adding Git Workspace as a dependency to it as well so that you can track the exact version of it together with your other dependencies. For example, if you use `poetry`, add it by running
+
+```bash
+# Add Git Workspace as a development dependency:
+poetry add --group dev git-ws
+```
+
+For testing you can try:
+
+```bash
+git ws --version
+```
+
+
+## 📔 Usage
+
+Git Workspace is integrated into git `git ws` - this is what you will be using most of the time.
+
+#### The Manifest
+
+Let's assume we have a project called `myapp`, which requires a library `mylib` that is maintained in another `git` repository. In order to use this project with Git Workspace, `myapp` needs to provide a so called *manifest*. A Git Workspace manifest is a simple [TOML](https://toml.io/) file - by default called `git-ws.toml` in the project's root folder - which defines the dependencies a project has as well as some other meta information. A minimal manifest for our project could look like this:
+
+```toml
+[[dependencies]]
+name = "mylib"
+url = "git@github.com:example/mylib.git"
+revision = "v2.3.4"
+```
+
+If `myapp` and `mylib` are stored on the same server (side-by-side), then the manifest can even be simpler:
+
+```toml
+[[dependencies]]
+name = "mylib"
+revision = "v2.3.4"
+```
+
+The project will be searched via a relative path (which is either `../mylib` or `../mylib.git` depending on the main repository's URL). Relative paths are in general useful as they allow using the same protocol for the main repository as well as any of its dependencies.
+
+See the [Manifest Documentation](https://git-ws.readthedocs.io/en/latest/manual/manifest.html) for any further details on available options.
+
+#### The Initial Clone
+
+To build a workspace from a project prepared like that, simply clone it via `git ws`:
+
+```bash
+cd $HOME/Projects
+git ws clone --update git@github.com:example/myapp.git
+```
+
+👉 Without the `--update` option, only the main repository will be fetched.
+
+The above will clone the app repository and also the library side-by-side:
+
+```bash
+ls -a myapp/
+# Should print something like
+.
+..
+.git-ws
+myapp
+mylib
+```
+
+As you can see, besides the two repositories we wanted, there is also a hidden `.git-ws` folder where the tool stores the needed configuration data.
+
+The [`git ws clone` documentation](https://git-ws.readthedocs.io/en/latest/manual/command-line-interface/workspace-management.html#git-ws-clone) describes all options.
+
+#### Initialization
+
+Sometimes there are use cases where using `git ws clone` cannot be used. For example, when you set up your manifest for the first time or when a CI/CD system creates the initial clone of the main repository, you may need a way to fetch the remaining projects. This can be done by simply running the following **within** the main project:
+
+```bash
+git ws init --update
+```
+
+👉 As with `git ws clone`, without the `--update`, no dependencies will be fetched.
+
+This command initializes the workspace and just needs to run once.
+Changes to the manifest require an update operation (see next section) but no re-initialization.
+
+#### Updating
+
+Another important use case is keeping a workspace up-to-date. Let's say you pull in an update in the main repository, which in turn might cause changes in the manifest to be pulled in as well. Updating the existing workspace is as simple as
+
+```bash
+# Update the workspace (main and all dependent repositories):
+git ws update
+
+# Alternatively, run `git rebase` instead of `git pull` in dependencies:
+git ws update --rebase
+```
+
+#### Non-Git Main Projects
+
+`git ws` can leave the manifest version control to any other version control system (Subversion, VCS, DesignSync, etc.).
+Just manage the manifest file `git-ws.toml` within the version control system of your choice.
+Run `git ws init --update` or `git ws init --update -M path/to/git-ws.toml` in the intended workspace directory.
+
+👉 As before, without the `--update`, no dependencies will be fetched.
+
+**Inside** a git clone, `git ws init` uses the actual git project as the *main project* of the workspace.
+**Outside** a git clone, `git ws init` initializes a workspace *without* a *main project*.
+
+👉 There are just two drawbacks of a workspace without a main project:
+
+1. `git ws tag` has no main project to tag and will fail. Please use [`git ws manifest freeze`](https://git-ws.readthedocs.io/en/latest/manual/command-line-interface/manifest.html#git-ws-manifest-freeze).
+2. Relative URLs are not supported, as there is no URL to be relative to. Please use `remotes`:
+
+```toml
+[[remotes]]
+name = "main"
+url-base = "git@github.example.com:your-group"
+
+[[dependencies]]
+name = "dep1"
+remote = "main"
+```
+
+## 👍 Getting Started
+
+Please ensure a proper [installation](https://github.com/c0fec0de/git-ws#-installation).
+
+Lets take a clone of an example project, which does not use ``git ws`` yet.
+
+```bash
+mkdir -p $HOME/Projects/Example-Workspace
+cd $HOME/Projects/Example-Workspace
+git clone https://github.com/c0fec0de/git-ws-example-one.git
+# Cloning into 'git-ws-example-one'...
+# remote: Enumerating objects: 3, done.
+# remote: Counting objects: 100% (3/3), done.
+# remote: Compressing objects: 100% (2/2), done.
+# remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
+# Receiving objects: 100% (3/3), done.
+```
+
+Now you should have one git clone in your workspace directory. Let's use it as *main project*.
+At first, we need a manifest file ``git-ws.toml``.
+
+```bash
+cd git-ws-example-one
+git ws manifest create
+# Manifest 'git-ws.toml' created.
+git add git-ws.toml
+```
+
+Now, we need to initialize the workspace
+
+```bash
+git ws init
+# ===== . (MAIN 'git-ws-example-one') =====
+# Workspace initialized at '..'.
+# Please continue with:
+#
+#     git ws update
+#
+```
+
+The parent directory became the ``git ws`` *workspace directory* .
+The actual git clone is the *main project* now.
+``git ws`` suggests to run ``git ws update``.
+You can try, but nothing will happen yet, as the manifest is quite empty.
+
+Let's add our first dependency ``git-ws-example-lib``, which is located on the same git server.
+You can manually edit the manifest file ``git-ws.toml``, or you just run
+
+```bash
+git ws dep add git-ws-example-lib
+```
+
+Feel free to inspect the ``git-ws.toml`` file.
+``git ws update`` will now apply the manifest changes and pull the new dependency:
+
+
+```bash
+git ws update
+# ===== . (MAIN 'git-ws-example-one', revision='main') =====
+# Pulling branch 'main'.
+# Already up to date.
+# ===== ../git-ws-example-lib ('git-ws-example-lib') =====
+# git-ws WARNING Clone git-ws-example-lib has no revision!
+# Cloning 'https://github.com/c0fec0de/git-ws-example-lib.git'.
+# Cloning into '../git-ws-example-lib'...
+# remote: Enumerating objects: 3, done.
+# remote: Counting objects: 100% (3/3), done.
+# remote: Compressing objects: 100% (2/2), done.
+# remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
+# Receiving objects: 100% (3/3), done.
+```
+
+Please note the warning:
+
+```bash
+# git-ws WARNING Clone git-ws-example-lib has no revision!
+```
+
+It is strongly recommended to specify a default revision for all dependencies. The command
+
+```bash
+git ws default revision main
+```
+
+solves that for you. Any successive ``git ws update`` is now free of this warning:
+
+```
+===== . (MAIN 'git-ws-example-one', revision='main') =====
+Pulling branch 'main'.
+Already up to date.
+===== ../git-ws-example-lib ('git-ws-example-lib', revision='main') =====
+Pulling branch 'main'.
+Already up to date.
+```
+
+Now you can add, commit and push your changes to the ``git-ws.toml`` file.
+Other colleagues should use now:
+
+```bash
+cd $HOME/Projects
+git ws clone --update YOUR-REPO-URL
+
+# OR
+
+cd $HOME/Projects/Workspace
+git clone YOUR-REPO-URL
+cd <directory>
+git ws init --update
+```
+
+``git ws status`` shows all changes within all git clones in the workspace.
+``git ws add`` runs likewise the ``git add`` operation in the associated git clones.
+Please see the next section for an overview of all commands.
+
+
+## 🕹️ Cheat-Sheet
+
+#### Initialization
+
+| Command | Description |
+| --- | --- |
+| `git ws clone URL` | Clone git repository from `URL` as main repository and initialize Git Workspace |
+| `git ws init` (**inside** a git clone) | Initialize Git Workspace at parent directory. Use current git clone as main repository |
+| `git ws init` (**outside** a git clone) | Initialize Git Workspace at current directory. No main repository. |
+| `git ws manifest create` | Create well documented, empty manifest |
+
+#### Basic
+
+| Command | Description |
+| --- | --- |
+| `git ws update` | Pull latest changes on main repository and all dependent repositories (clone them if needed) |
+| `git ws update --rebase` | Same as above, but fetch and rebase instead of pull |
+| `git ws status` | Run `git status` on all repositories (displayed paths include the actual clone path) |
+| `git ws add FILES` | Run `git add FILE` on `FILES` in the corresponding repositories |
+| `git ws reset FILES` | Run `git reset FILE` on `FILES` in the corresponding repositories. Undo `git add` |
+| `git ws commit FILES -m MESSAGE` | Run `git commit FILE` on `FILES` in the corresponding repositories |
+| `git ws commit -m MESSAGE` | Run `git commit` repositories with changes |
+| `git ws checkout FILES` | Run `git checkout FILE` on `FILES` in the corresponding repositories |
+| `git ws checkout` | Checkout git revision specified as in the manifest(s) (clone them if needed) |
+
+#### Run Commands on all repositories
+
+| Command | Description |
+| --- | --- |
+| `git ws push` | Run `git push` on all repositories (in reverse order) |
+| `git ws fetch` | Run `git fetch` on all repositories |
+| `git ws rebase` | Run `git rebase` on all repositories |
+| `git ws pull` | Run `git pull` on all repositories |
+| `git ws diff` | Run `git diff` on all repositories |
+| `git ws git CMD` | Run `git CMD` on all repositories |
+| `git ws foreach CMD` | Run `CMD` on all repositories |
+
+#### Other
+
+| Command | Description |
+| --- | --- |
+| `git ws manifest freeze`   | Print The Resolved Manifest With SHAs For All Project Revisions. |
+| `git ws manifest path`     | Print Path to Main Manifest File. |
+| `git ws manifest paths`    | Print Paths to ALL Manifest Files. |
+| `git ws manifest resolve`  | Print The Manifest With All Projects And All Their Dependencies. |
+| `git ws manifest upgrade`  | Update Manifest To Latest Version. |
+| `git ws manifest validate` | Validate The Current Manifest, Exiting With An Error On Issues. |
+| `git ws info main-path`      | Print Path to Main Git Clone. |
+| `git ws info project-paths`  | Print Paths to all git clones. |
+| `git ws info workspace-path` | Print Path to Workspace. |
+| `git ws info dep-tree` | Print Dependency Tree. |
+| `git ws info dep-tree --dot \| dot -Tpng > dep-tree.png` | Draw Dependency Diagramm (needs [graphviz](https://graphviz.org)) |
+
+
+See the [command-line interface documentation](https://git-ws.readthedocs.io/en/latest/manual/command-line-interface/index.html) for any further details.
+
+
+## 🐍 Python API
+
+Git Workspace is written in Python. Besides the `git ws` command line tool, there is also an API which you can use to further automate workspace creation and maintenance. If you are interested, have a look into the [API documentation](https://git-ws.readthedocs.io/en/latest/api/gitws.html).
+
+
+## 🤝 Alternatives
+
+Before writing Git Workspace, we investigated several other existing tools in the hope they would fulfil our needs. In particular, we looked into the following tools and methodologies which are widely used to organize large projects:
+
+- [`git submodules`](https://git-scm.com/book/en/v2/Git-Tools-Submodules).
+- Google's [repo](https://gerrit.googlesource.com/git-repo/) tool.
+- The [`west`](https://docs.zephyrproject.org/latest/develop/west/index.html) tool developed in the scope of [Zephyr](https://www.zephyrproject.org/).
+- Leaving the pure `git` domain, one can also use a package manager like [`conan`](https://conan.io/).
+- And lastly, there are also approaches to still pack everything into a large, so called *monorepo*.
+
+Unfortunately, none of the tools we tested really satisfied us. But hey, as we are developers - *why not start our own tool for the purpose?*
+
+And that's what we did - Git Workspace is our tool for managing a large workspace consisting of several smaller `git` projects. Here is how it compares to the other tools we evaluated:
+
+
+|                           | `git submodules` | `repo` | `west` | *Monorepos* | `git ws` |
+| ------------------------- | ---------------- | ------ | ------ | ----------- | --------- |
+| Reusable Components       | ✅               | ✅     | ✅     | ➖          | ✅        |
+| Ease of Use               | ➖               | ✅     | ✅     | ✅          | ✅        |
+| Editable Components       | ➖               | ✅     | ➖     | ✅          | ✅        |
+| Freezing Configurations   | ✅               | ✅     | ✅     | ✅          | ✅        |
+| Transitive Dependencies   | ➖               | ➖     | ✅     | ➖          | ✅        |
+| Relative Dependency Paths | ✅               | ✅     | ➖     | ➖          | ✅        |
+| Branches as dependencies  | ➖               | ✅     | ✅     | ➖          | ✅        |
+
+👉 Please note that our view on the various features might be biased. As we did, always look at all the options available to you before deciding on one tool or the other. While the other tools in comparison did not model what we needed for our workflow, they might just be what you are looking for.
+
+If you want to learn more, have a look into [Why We Started Git Workspace](https://git-ws.readthedocs.io/en/latest/manual/why.html).
 
 
-setup(**setup_kwargs)
```

