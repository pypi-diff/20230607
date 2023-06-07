# Comparing `tmp/jax-relax-0.1.5.tar.gz` & `tmp/jax-relax-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-relax-0.1.5.tar", last modified: Sat May 20 00:54:43 2023, max compression
+gzip compressed data, was "jax-relax-0.1.6.tar", last modified: Wed Jun  7 15:18:42 2023, max compression
```

## Comparing `jax-relax-0.1.5.tar` & `jax-relax-0.1.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-20 00:54:43.023699 jax-relax-0.1.5/
--rw-r--r--   0 birk      (1000) birk      (1000)     2381 2023-01-17 02:27:26.000000 jax-relax-0.1.5/CONTRIBUTING.md
--rw-r--r--   0 birk      (1000) birk      (1000)    11558 2023-01-17 02:27:26.000000 jax-relax-0.1.5/LICENSE
--rw-r--r--   0 birk      (1000) birk      (1000)      116 2023-01-17 02:27:26.000000 jax-relax-0.1.5/MANIFEST.in
--rw-r--r--   0 birk      (1000) birk      (1000)     3371 2023-05-20 00:54:43.023699 jax-relax-0.1.5/PKG-INFO
--rw-r--r--   0 birk      (1000) birk      (1000)     2608 2023-05-13 23:13:26.000000 jax-relax-0.1.5/README.md
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-20 00:54:43.023699 jax-relax-0.1.5/jax_relax.egg-info/
--rw-r--r--   0 birk      (1000) birk      (1000)     3371 2023-05-20 00:54:42.000000 jax-relax-0.1.5/jax_relax.egg-info/PKG-INFO
--rw-r--r--   0 birk      (1000) birk      (1000)      820 2023-05-20 00:54:42.000000 jax-relax-0.1.5/jax_relax.egg-info/SOURCES.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-05-20 00:54:42.000000 jax-relax-0.1.5/jax_relax.egg-info/dependency_links.txt
--rw-r--r--   0 birk      (1000) birk      (1000)       32 2023-05-20 00:54:42.000000 jax-relax-0.1.5/jax_relax.egg-info/entry_points.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-01-17 02:38:00.000000 jax-relax-0.1.5/jax_relax.egg-info/not-zip-safe
--rw-r--r--   0 birk      (1000) birk      (1000)      217 2023-05-20 00:54:42.000000 jax-relax-0.1.5/jax_relax.egg-info/requires.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        6 2023-05-20 00:54:42.000000 jax-relax-0.1.5/jax_relax.egg-info/top_level.txt
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-20 00:54:43.023699 jax-relax-0.1.5/relax/
--rw-r--r--   0 birk      (1000) birk      (1000)       21 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)     3855 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/_ckpt_manager.py
--rw-r--r--   0 birk      (1000) birk      (1000)    84243 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/_modidx.py
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-20 00:54:43.023699 jax-relax-0.1.5/relax/data/
--rw-r--r--   0 birk      (1000) birk      (1000)      117 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/data/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)     7842 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/data/loader.py
--rw-r--r--   0 birk      (1000) birk      (1000)    19548 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/data/module.py
--rw-r--r--   0 birk      (1000) birk      (1000)     9776 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/data/scm.py
--rw-r--r--   0 birk      (1000) birk      (1000)     6199 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/docs.py
--rw-r--r--   0 birk      (1000) birk      (1000)    19678 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/evaluate.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1341 2023-05-03 15:57:46.000000 jax-relax-0.1.5/relax/import_essentials.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1985 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/logger.py
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-20 00:54:43.023699 jax-relax-0.1.5/relax/methods/
--rw-r--r--   0 birk      (1000) birk      (1000)      361 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)     2319 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/base.py
--rw-r--r--   0 birk      (1000) birk      (1000)    11822 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/cchvae.py
--rw-r--r--   0 birk      (1000) birk      (1000)    14314 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/clue.py
--rw-r--r--   0 birk      (1000) birk      (1000)    12640 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/counternet.py
--rw-r--r--   0 birk      (1000) birk      (1000)     6125 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/diverse.py
--rw-r--r--   0 birk      (1000) birk      (1000)     9245 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/proto.py
--rw-r--r--   0 birk      (1000) birk      (1000)     6893 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/sphere.py
--rw-r--r--   0 birk      (1000) birk      (1000)    11617 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/vaecf.py
--rw-r--r--   0 birk      (1000) birk      (1000)     3699 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/vanilla.py
--rw-r--r--   0 birk      (1000) birk      (1000)     9921 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/module.py
--rw-r--r--   0 birk      (1000) birk      (1000)     4797 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/plots.py
--rw-r--r--   0 birk      (1000) birk      (1000)     4938 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/trainer.py
--rw-r--r--   0 birk      (1000) birk      (1000)     8433 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/utils.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1130 2023-05-20 00:52:05.000000 jax-relax-0.1.5/settings.ini
--rw-r--r--   0 birk      (1000) birk      (1000)       38 2023-05-20 00:54:43.023699 jax-relax-0.1.5/setup.cfg
--rw-r--r--   0 birk      (1000) birk      (1000)     2603 2023-05-03 15:57:46.000000 jax-relax-0.1.5/setup.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-06-07 15:18:42.520000 jax-relax-0.1.6/
+-rw-r--r--   0 birk      (1000) birk      (1000)     2348 2022-12-18 21:09:02.000000 jax-relax-0.1.6/CONTRIBUTING.md
+-rw-r--r--   0 birk      (1000) birk      (1000)    11357 2022-12-18 21:09:02.000000 jax-relax-0.1.6/LICENSE
+-rw-r--r--   0 birk      (1000) birk      (1000)      111 2022-12-18 21:09:02.000000 jax-relax-0.1.6/MANIFEST.in
+-rw-r--r--   0 birk      (1000) birk      (1000)     3371 2023-06-07 15:18:42.520000 jax-relax-0.1.6/PKG-INFO
+-rw-r--r--   0 birk      (1000) birk      (1000)     2530 2023-05-18 22:24:40.000000 jax-relax-0.1.6/README.md
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-06-07 15:18:42.510000 jax-relax-0.1.6/jax_relax.egg-info/
+-rw-r--r--   0 birk      (1000) birk      (1000)     3371 2023-06-07 15:18:42.000000 jax-relax-0.1.6/jax_relax.egg-info/PKG-INFO
+-rw-r--r--   0 birk      (1000) birk      (1000)      820 2023-06-07 15:18:42.000000 jax-relax-0.1.6/jax_relax.egg-info/SOURCES.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-06-07 15:18:42.000000 jax-relax-0.1.6/jax_relax.egg-info/dependency_links.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)       32 2023-06-07 15:18:42.000000 jax-relax-0.1.6/jax_relax.egg-info/entry_points.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)        1 2022-12-19 10:47:31.000000 jax-relax-0.1.6/jax_relax.egg-info/not-zip-safe
+-rw-r--r--   0 birk      (1000) birk      (1000)      217 2023-06-07 15:18:42.000000 jax-relax-0.1.6/jax_relax.egg-info/requires.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)        6 2023-06-07 15:18:42.000000 jax-relax-0.1.6/jax_relax.egg-info/top_level.txt
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-06-07 15:18:42.520000 jax-relax-0.1.6/relax/
+-rw-r--r--   0 birk      (1000) birk      (1000)       21 2023-06-07 15:17:38.000000 jax-relax-0.1.6/relax/__init__.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     3855 2023-06-07 15:17:37.000000 jax-relax-0.1.6/relax/_ckpt_manager.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    85879 2023-06-07 15:17:38.000000 jax-relax-0.1.6/relax/_modidx.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-06-07 15:18:42.520000 jax-relax-0.1.6/relax/data/
+-rw-r--r--   0 birk      (1000) birk      (1000)      115 2023-06-07 15:17:38.000000 jax-relax-0.1.6/relax/data/__init__.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     7842 2023-06-07 15:17:37.000000 jax-relax-0.1.6/relax/data/loader.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    19552 2023-06-07 15:17:37.000000 jax-relax-0.1.6/relax/data/module.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     9776 2023-06-07 15:17:37.000000 jax-relax-0.1.6/relax/data/scm.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     6199 2023-06-07 15:17:37.000000 jax-relax-0.1.6/relax/docs.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    22165 2023-06-07 15:17:38.000000 jax-relax-0.1.6/relax/evaluate.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     1305 2023-05-03 17:16:11.000000 jax-relax-0.1.6/relax/import_essentials.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     1985 2023-06-07 15:17:37.000000 jax-relax-0.1.6/relax/logger.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-06-07 15:18:42.520000 jax-relax-0.1.6/relax/methods/
+-rw-r--r--   0 birk      (1000) birk      (1000)      353 2023-06-07 15:17:38.000000 jax-relax-0.1.6/relax/methods/__init__.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     2319 2023-06-07 15:17:37.000000 jax-relax-0.1.6/relax/methods/base.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    11922 2023-06-07 15:17:37.000000 jax-relax-0.1.6/relax/methods/cchvae.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    14362 2023-06-07 15:17:38.000000 jax-relax-0.1.6/relax/methods/clue.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    12742 2023-06-07 15:17:37.000000 jax-relax-0.1.6/relax/methods/counternet.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     6150 2023-06-07 15:17:37.000000 jax-relax-0.1.6/relax/methods/diverse.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     9245 2023-06-07 15:17:37.000000 jax-relax-0.1.6/relax/methods/proto.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     6893 2023-06-07 15:17:37.000000 jax-relax-0.1.6/relax/methods/sphere.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    11654 2023-06-07 15:17:38.000000 jax-relax-0.1.6/relax/methods/vaecf.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     3699 2023-06-07 15:17:37.000000 jax-relax-0.1.6/relax/methods/vanilla.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     9921 2023-06-07 15:17:37.000000 jax-relax-0.1.6/relax/module.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     4797 2023-06-07 15:17:38.000000 jax-relax-0.1.6/relax/plots.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     4938 2023-06-07 15:17:37.000000 jax-relax-0.1.6/relax/trainer.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     8441 2023-06-07 15:17:37.000000 jax-relax-0.1.6/relax/utils.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     1130 2023-06-07 15:17:37.000000 jax-relax-0.1.6/settings.ini
+-rw-r--r--   0 birk      (1000) birk      (1000)       38 2023-06-07 15:18:42.520000 jax-relax-0.1.6/setup.cfg
+-rw-r--r--   0 birk      (1000) birk      (1000)     2546 2023-05-03 17:16:11.000000 jax-relax-0.1.6/setup.py
```

### Comparing `jax-relax-0.1.5/CONTRIBUTING.md` & `jax-relax-0.1.6/CONTRIBUTING.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# How to contribute
-
-## How to get started
-
-Before anything else, please install the git hooks that run automatic scripts during each commit and merge to strip the notebooks of superfluous metadata (and avoid merge conflicts). After cloning the repository, run the following command inside it:
-```
-nbdev_install_git_hooks
-```
-
-## Did you find a bug?
-
-* Ensure the bug was not already reported by searching on GitHub under Issues.
-* If you're unable to find an open issue addressing the problem, open a new one. Be sure to include a title and clear description, as much relevant information as possible, and a code sample or an executable test case demonstrating the expected behavior that is not occurring.
-* Be sure to add the complete error messages.
-
-#### Did you write a patch that fixes a bug?
-
-* Open a new GitHub pull request with the patch.
-* Ensure that your PR includes a test that fails without your patch, and pass with it.
-* Ensure the PR description clearly describes the problem and solution. Include the relevant issue number if applicable.
-
-## PR submission guidelines
-
-* Keep each PR focused. While it's more convenient, do not combine several unrelated fixes together. Create as many branches as needing to keep each PR focused.
-* Do not mix style changes/fixes with "functional" changes. It's very difficult to review such PRs and it most likely get rejected.
-* Do not add/remove vertical whitespace. Preserve the original style of the file you edit as much as you can.
-* Do not turn an already submitted PR into your development playground. If after you submitted PR, you discovered that more work is needed - close the PR, do the required work and then submit a new PR. Otherwise each of your commits requires attention from maintainers of the project.
-* If, however, you submitted a PR and received a request for changes, you should proceed with commits inside that PR, so that the maintainer can see the incremental fixes and won't need to review the whole PR again. In the exception case where you realize it'll take many many commits to complete the requests, then it's probably best to close the PR, do the work and then submit it again. Use common sense where you'd choose one way over another.
-
-## Do you want to contribute to the documentation?
-
-* Docs are automatically created from the notebooks in the nbs folder.
-
+# How to contribute
+
+## How to get started
+
+Before anything else, please install the git hooks that run automatic scripts during each commit and merge to strip the notebooks of superfluous metadata (and avoid merge conflicts). After cloning the repository, run the following command inside it:
+```
+nbdev_install_git_hooks
+```
+
+## Did you find a bug?
+
+* Ensure the bug was not already reported by searching on GitHub under Issues.
+* If you're unable to find an open issue addressing the problem, open a new one. Be sure to include a title and clear description, as much relevant information as possible, and a code sample or an executable test case demonstrating the expected behavior that is not occurring.
+* Be sure to add the complete error messages.
+
+#### Did you write a patch that fixes a bug?
+
+* Open a new GitHub pull request with the patch.
+* Ensure that your PR includes a test that fails without your patch, and pass with it.
+* Ensure the PR description clearly describes the problem and solution. Include the relevant issue number if applicable.
+
+## PR submission guidelines
+
+* Keep each PR focused. While it's more convenient, do not combine several unrelated fixes together. Create as many branches as needing to keep each PR focused.
+* Do not mix style changes/fixes with "functional" changes. It's very difficult to review such PRs and it most likely get rejected.
+* Do not add/remove vertical whitespace. Preserve the original style of the file you edit as much as you can.
+* Do not turn an already submitted PR into your development playground. If after you submitted PR, you discovered that more work is needed - close the PR, do the required work and then submit a new PR. Otherwise each of your commits requires attention from maintainers of the project.
+* If, however, you submitted a PR and received a request for changes, you should proceed with commits inside that PR, so that the maintainer can see the incremental fixes and won't need to review the whole PR again. In the exception case where you realize it'll take many many commits to complete the requests, then it's probably best to close the PR, do the work and then submit it again. Use common sense where you'd choose one way over another.
+
+## Do you want to contribute to the documentation?
+
+* Docs are automatically created from the notebooks in the nbs folder.
+
```

### Comparing `jax-relax-0.1.5/LICENSE` & `jax-relax-0.1.6/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `jax-relax-0.1.5/PKG-INFO` & `jax-relax-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-relax
-Version: 0.1.5
+Version: 0.1.6
 Summary: Jax-based Recourse Explanation Library
 Home-page: https://github.com/birkhoffg/relax/tree/master/
 Author: BirkhoffG
 Author-email: 26811230+BirkhoffG@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: Jax,Recourse,Explanation,Interpretability,Machine Learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jax-relax-0.1.5/README.md` & `jax-relax-0.1.6/README.md`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-ReLax
-================
-
-<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
-
-![Python](https://img.shields.io/pypi/pyversions/jax-relax.svg) ![CI
-status](https://github.com/BirkhoffG/ReLax/actions/workflows/test.yaml/badge.svg)
-![Docs](https://github.com/BirkhoffG/ReLax/actions/workflows/deploy.yaml/badge.svg)
-![pypi](https://img.shields.io/pypi/v/jax-relax.svg) ![GitHub
-License](https://img.shields.io/github/license/BirkhoffG/ReLax.svg)
-
-[**Overview**](#overview) \| [**Installation**](#installation) \|
-[**Tutorials**](https://birkhoffg.github.io/ReLax/tutorials/getting_started.html)
-\| [**Documentation**](https://birkhoffg.github.io/ReLax/) \| [**Citing
-ReLax**](#citing-relax)
-
-## Overview
-
-`ReLax` (**Re**course Explanation **L**ibrary in J**ax**) is a library
-built on top of `jax` to generate counterfactual and recourse
-explanations for Machine Learning algorithms. By leveraging
-*vectorization* though `vmap`/`pmap` and *just-in-time* compilation in
-[jax](https://jax.readthedocs.io/en/latest/) (a high-performance
-auto-differentiation library). `ReLax` offers massive speed improvements
-in generating individual (or local) explanations for predictions made by
-Machine Learning algorithms.
-
-Some of the key features are as follows:
-
-- 🏃 **Fast** recourse generation via `jax.jit`, `jax.vmap`/`jax.pmap`.
-
-- 🚀 **Accelerated** over `cpu`, `gpu`, `tpu`.
-
-- 🪓 **Comprehensive** set of recourse methods implemented for
-  benchmarking.
-
-- 👐 **Customizable** API to enable the building of entire modeling
-
-- and interpretation pipelines for new recourse algorithms.
-
-## Installation
-
-The latest `ReLax` release can directly be installed from PyPI:
-
-``` bash
-pip install jax-relax
-```
-
-or installed directly from the repository:
-
-``` bash
-pip install git+https://github.com/BirkhoffG/ReLax.git 
-```
-
-To futher unleash the power of accelerators (i.e., GPU/TPU), we suggest
-to first install this library via `pip install jax-relax`. Then, follow
-steps in the [official install
-guidelines](https://github.com/google/jax#installation) to install the
-right version for GPU or TPU.
-
-## An Example of using `ReLax`
-
-See [Getting Started with
-ReLax](https://birkhoffg.github.io/ReLax/tutorials/getting_started.html).
-
-## Citing `ReLax`
-
-To cite this repository:
-
-``` latex
-@software{relax2023github,
-  author = {Hangzhi Guo and Xinchang Xiong and Amulya Yadav},
-  title = {{R}e{L}ax: Recourse Explanation Library in Jax},
-  url = {http://github.com/birkhoffg/ReLax},
-  version = {0.1.0},
-  year = {2023},
-}
-```
+ReLax
+================
+
+<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
+
+![Python](https://img.shields.io/pypi/pyversions/jax-relax.svg) ![CI
+status](https://github.com/BirkhoffG/ReLax/actions/workflows/test.yaml/badge.svg)
+![Docs](https://github.com/BirkhoffG/ReLax/actions/workflows/deploy.yaml/badge.svg)
+![pypi](https://img.shields.io/pypi/v/jax-relax.svg) ![GitHub
+License](https://img.shields.io/github/license/BirkhoffG/ReLax.svg)
+
+[**Overview**](#overview) \| [**Installation**](#installation) \|
+[**Tutorials**](https://birkhoffg.github.io/ReLax/tutorials/getting_started.html)
+\| [**Documentation**](https://birkhoffg.github.io/ReLax/) \| [**Citing
+ReLax**](#citing-relax)
+
+## Overview
+
+`ReLax` (**Re**course Explanation **L**ibrary in J**ax**) is a library
+built on top of `jax` to generate counterfactual and recourse
+explanations for Machine Learning algorithms. By leveraging
+*vectorization* though `vmap`/`pmap` and *just-in-time* compilation in
+[jax](https://jax.readthedocs.io/en/latest/) (a high-performance
+auto-differentiation library). `ReLax` offers massive speed improvements
+in generating individual (or local) explanations for predictions made by
+Machine Learning algorithms.
+
+Some of the key features are as follows:
+
+- 🏃 **Fast** recourse generation via `jax.jit`, `jax.vmap`/`jax.pmap`.
+
+- 🚀 **Accelerated** over `cpu`, `gpu`, `tpu`.
+
+- 🪓 **Comprehensive** set of recourse methods implemented for
+  benchmarking.
+
+- 👐 **Customizable** API to enable the building of entire modeling
+
+- and interpretation pipelines for new recourse algorithms.
+
+## Installation
+
+The latest `ReLax` release can directly be installed from PyPI:
+
+``` bash
+pip install jax-relax
+```
+
+or installed directly from the repository:
+
+``` bash
+pip install git+https://github.com/BirkhoffG/ReLax.git 
+```
+
+To futher unleash the power of accelerators (i.e., GPU/TPU), we suggest
+to first install this library via `pip install jax-relax`. Then, follow
+steps in the [official install
+guidelines](https://github.com/google/jax#installation) to install the
+right version for GPU or TPU.
+
+## An Example of using `ReLax`
+
+See [Getting Started with
+ReLax](https://birkhoffg.github.io/ReLax/tutorials/getting_started.html).
+
+## Citing `ReLax`
+
+To cite this repository:
+
+``` latex
+@software{relax2023github,
+  author = {Hangzhi Guo and Xinchang Xiong and Amulya Yadav},
+  title = {{R}e{L}ax: Recourse Explanation Library in Jax},
+  url = {http://github.com/birkhoffg/ReLax},
+  version = {0.1.0},
+  year = {2023},
+}
+```
```

### Comparing `jax-relax-0.1.5/jax_relax.egg-info/PKG-INFO` & `jax-relax-0.1.6/jax_relax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-relax
-Version: 0.1.5
+Version: 0.1.6
 Summary: Jax-based Recourse Explanation Library
 Home-page: https://github.com/birkhoffg/relax/tree/master/
 Author: BirkhoffG
 Author-email: 26811230+BirkhoffG@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: Jax,Recourse,Explanation,Interpretability,Machine Learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jax-relax-0.1.5/jax_relax.egg-info/SOURCES.txt` & `jax-relax-0.1.6/jax_relax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.5/relax/_ckpt_manager.py` & `jax-relax-0.1.6/relax/_ckpt_manager.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.5/relax/_modidx.py` & `jax-relax-0.1.6/relax/_modidx.py`

 * *Files 5% similar despite different names*

```diff
@@ -212,14 +212,26 @@
             'relax.evaluate': { 'relax.evaluate.BaseEvalMetrics': ('evaluate.html#baseevalmetrics', 'relax/evaluate.py'),
                                 'relax.evaluate.BaseEvalMetrics.__call__': ('evaluate.html#baseevalmetrics.__call__', 'relax/evaluate.py'),
                                 'relax.evaluate.BaseEvalMetrics.__init__': ('evaluate.html#baseevalmetrics.__init__', 'relax/evaluate.py'),
                                 'relax.evaluate.BaseEvalMetrics.__str__': ('evaluate.html#baseevalmetrics.__str__', 'relax/evaluate.py'),
                                 'relax.evaluate.BaseGenerationStrategy': ('evaluate.html#basegenerationstrategy', 'relax/evaluate.py'),
                                 'relax.evaluate.BaseGenerationStrategy.__call__': ( 'evaluate.html#basegenerationstrategy.__call__',
                                                                                     'relax/evaluate.py'),
+                                'relax.evaluate.BatchedPmapGenerationStrategy': ( 'evaluate.html#batchedpmapgenerationstrategy',
+                                                                                  'relax/evaluate.py'),
+                                'relax.evaluate.BatchedPmapGenerationStrategy.__call__': ( 'evaluate.html#batchedpmapgenerationstrategy.__call__',
+                                                                                           'relax/evaluate.py'),
+                                'relax.evaluate.BatchedPmapGenerationStrategy.__init__': ( 'evaluate.html#batchedpmapgenerationstrategy.__init__',
+                                                                                           'relax/evaluate.py'),
+                                'relax.evaluate.BatchedVmapGenerationStrategy': ( 'evaluate.html#batchedvmapgenerationstrategy',
+                                                                                  'relax/evaluate.py'),
+                                'relax.evaluate.BatchedVmapGenerationStrategy.__call__': ( 'evaluate.html#batchedvmapgenerationstrategy.__call__',
+                                                                                           'relax/evaluate.py'),
+                                'relax.evaluate.BatchedVmapGenerationStrategy.__init__': ( 'evaluate.html#batchedvmapgenerationstrategy.__init__',
+                                                                                           'relax/evaluate.py'),
                                 'relax.evaluate.Explanation': ('evaluate.html#explanation', 'relax/evaluate.py'),
                                 'relax.evaluate.Explanation.__post_init__': ( 'evaluate.html#explanation.__post_init__',
                                                                               'relax/evaluate.py'),
                                 'relax.evaluate.IterativeGenerationStrategy': ( 'evaluate.html#iterativegenerationstrategy',
                                                                                 'relax/evaluate.py'),
                                 'relax.evaluate.IterativeGenerationStrategy.__call__': ( 'evaluate.html#iterativegenerationstrategy.__call__',
                                                                                          'relax/evaluate.py'),
@@ -256,14 +268,15 @@
                                 'relax.evaluate.Validity.__init__': ('evaluate.html#validity.__init__', 'relax/evaluate.py'),
                                 'relax.evaluate.VmapGenerationStrategy': ('evaluate.html#vmapgenerationstrategy', 'relax/evaluate.py'),
                                 'relax.evaluate.VmapGenerationStrategy.__call__': ( 'evaluate.html#vmapgenerationstrategy.__call__',
                                                                                     'relax/evaluate.py'),
                                 'relax.evaluate._AuxPredFn': ('evaluate.html#_auxpredfn', 'relax/evaluate.py'),
                                 'relax.evaluate._AuxPredFn.__call__': ('evaluate.html#_auxpredfn.__call__', 'relax/evaluate.py'),
                                 'relax.evaluate._AuxPredFn.__init__': ('evaluate.html#_auxpredfn.__init__', 'relax/evaluate.py'),
+                                'relax.evaluate._batched_generation': ('evaluate.html#_batched_generation', 'relax/evaluate.py'),
                                 'relax.evaluate._check_aux_pred_fn_args': ('evaluate.html#_check_aux_pred_fn_args', 'relax/evaluate.py'),
                                 'relax.evaluate._check_pred_fn': ('evaluate.html#_check_pred_fn', 'relax/evaluate.py'),
                                 'relax.evaluate._compute_acc': ('evaluate.html#_compute_acc', 'relax/evaluate.py'),
                                 'relax.evaluate._compute_manifold_dist': ('evaluate.html#_compute_manifold_dist', 'relax/evaluate.py'),
                                 'relax.evaluate._compute_proximity': ('evaluate.html#_compute_proximity', 'relax/evaluate.py'),
                                 'relax.evaluate._compute_spar': ('evaluate.html#_compute_spar', 'relax/evaluate.py'),
                                 'relax.evaluate._compute_val': ('evaluate.html#_compute_val', 'relax/evaluate.py'),
```

### Comparing `jax-relax-0.1.5/relax/data/loader.py` & `jax-relax-0.1.6/relax/data/loader.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.5/relax/data/module.py` & `jax-relax-0.1.6/relax/data/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
             continuous_col_names=self._configs.continous_cols,
             cat_arrays=self._cat_arrays,
         )
         
         # prepare train & test
         train_test_tuple = train_test_split(X, y, shuffle=False)
         train_X, test_X, train_y, test_y = map(
-             lambda x: x.astype(float), train_test_tuple
+             lambda x: x.astype(np.single), train_test_tuple
          )
         if self._configs.sample_frac:
             train_size = int(len(train_X) * self._configs.sample_frac)
             train_X, train_y = train_X[:train_size], train_y[:train_size]
         
         self._train_dataset = ArrayDataset(train_X, train_y)
         self._val_dataset = ArrayDataset(test_X, test_y)
```

### Comparing `jax-relax-0.1.5/relax/data/scm.py` & `jax-relax-0.1.6/relax/data/scm.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.5/relax/docs.py` & `jax-relax-0.1.6/relax/docs.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.5/relax/evaluate.py` & `jax-relax-0.1.6/relax/evaluate.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from .methods.counternet import CounterNet
 from copy import deepcopy
 from sklearn.neighbors import NearestNeighbors
 from fastcore.test import test_fail
 
 # %% auto 0
 __all__ = ['CFExplanationResults', 'METRICS_CALLABLE', 'METRICS', 'DEFAULT_METRICS', 'Explanation', 'BaseGenerationStrategy',
-           'IterativeGenerationStrategy', 'VmapGenerationStrategy', 'PmapGenerationStrategy', 'StrategyFactory',
+           'IterativeGenerationStrategy', 'VmapGenerationStrategy', 'PmapGenerationStrategy',
+           'BatchedVmapGenerationStrategy', 'BatchedPmapGenerationStrategy', 'StrategyFactory',
            'generate_cf_explanations', 'BaseEvalMetrics', 'PredictiveAccuracy', 'Validity', 'Proximity', 'Sparsity',
            'ManifoldDist', 'Runtime', 'compute_so_validity', 'compute_so_proximity', 'compute_so_sparsity',
            'evaluate_cfs', 'benchmark_cfs']
 
 # %% ../nbs/06_evaluate.ipynb 4
 @dataclass
 class Explanation:
@@ -126,15 +127,80 @@
         X_padded = _pad_divisible_X(X, self.n_devices)
         partial_fn = partial(fn, pred_fn=pred_fn, **kwargs)
         cfs = jax.pmap(jax.vmap(partial_fn))(X_padded)
         cfs = cfs.reshape(-1, *cfs.shape[2:])
         cfs = cfs[:X.shape[0]]
         return cfs
 
-# %% ../nbs/06_evaluate.ipynb 19
+# %% ../nbs/06_evaluate.ipynb 14
+def _batched_generation(
+    gs_fn: Callable, # Generation strategy function
+    cf_fn: Callable, # Function to generate cf for a single input
+    X: jnp.ndarray, # Input instances to be explained
+    pred_fn: Callable[[Array], Array],
+    batch_size: int,
+    **kwargs
+) -> Array: # Generated counterfactual explanations
+    """Batched generation of counterfactuals."""
+    
+    assert X.ndim == 2, f"X must be a 2D array, got {X.ndim}D array"
+    x_shape = X.shape
+    batch_size = min(batch_size, x_shape[0])
+    # pad X to be divisible by batch_size
+    pad_size = batch_size - (X.shape[0] % batch_size)
+    X = jnp.pad(X, ((0, pad_size), (0, 0)))
+    X = X.reshape(-1, batch_size, *x_shape[1:])
+    # generate cfs via lax.map
+    gs_fn_partial = lambda x: gs_fn(cf_fn, x, pred_fn=pred_fn, **kwargs)
+    cfs = lax.map(gs_fn_partial, X)
+    cfs = cfs.reshape(-1, *x_shape[1:])[:x_shape[0]]
+    return cfs
+
+# %% ../nbs/06_evaluate.ipynb 15
+class BatchedVmapGenerationStrategy(BaseGenerationStrategy):
+    """Auto-batching for generate counterfactuals via `jax.vmap`."""
+    def __init__(self, batch_size: int):
+        self.batch_size = batch_size
+
+    def __call__(
+        self, 
+        fn: Callable, # Function to generate cf for a single input
+        X: jnp.ndarray, # Input instances to be explained
+        pred_fn: Callable[[Array], Array],
+        **kwargs
+    ) -> Array: # Generated counterfactual explanations
+        vmap_g = VmapGenerationStrategy()    
+        cfs = _batched_generation(
+            vmap_g, fn, X, pred_fn, self.batch_size, **kwargs
+        )
+        return cfs
+
+
+# %% ../nbs/06_evaluate.ipynb 16
+class BatchedPmapGenerationStrategy(BaseGenerationStrategy):
+    """Auto-batching for generate counterfactuals via `jax.vmap`."""
+    def __init__(self, batch_size: int, n_devices: int = None):
+        self.batch_size = batch_size
+        self.n_devices = n_devices
+
+    def __call__(
+        self, 
+        fn: Callable, # Function to generate cf for a single input
+        X: jnp.ndarray, # Input instances to be explained
+        pred_fn: Callable[[Array], Array],
+        **kwargs
+    ) -> Array: # Generated counterfactual explanations
+        pmap_g = PmapGenerationStrategy(self.n_devices)
+        cfs = _batched_generation(
+            pmap_g, fn, X, pred_fn, self.batch_size, **kwargs
+        )
+        return cfs
+
+
+# %% ../nbs/06_evaluate.ipynb 25
 class StrategyFactory(object):
     """Factory class for Parallelism Strategy."""
 
     __strategy_map = {
         'iter': IterativeGenerationStrategy(),
         'vmap': VmapGenerationStrategy(),
         'pmap': PmapGenerationStrategy(),
@@ -154,15 +220,15 @@
         if isinstance(strategy, BaseGenerationStrategy):
             return strategy
         elif isinstance(strategy, str) and strategy in cls.__strategy_map:
             return cls.__strategy_map[strategy]
         else:
             raise ValueError(f"Invalid strategy: {strategy}")
 
-# %% ../nbs/06_evaluate.ipynb 22
+# %% ../nbs/06_evaluate.ipynb 28
 def _validate_configs(
     cf_module: BaseCFModule,
     datamodule: TabularDataModule,
     pred_fn: Callable[[jnp.DeviceArray], jnp.DeviceArray] = None,
     t_configs=None
 ):
     if (pred_fn is None) and (not isinstance(cf_module, BasePredFnCFModule)):
@@ -186,15 +252,15 @@
 ):
     if not cf_module._is_module_trained():
         print(f'{type(cf_module).__name__} contains parametric models. '
             'Starts training before generating explanations...')
         cf_module.train(datamodule, t_configs, pred_fn=pred_fn)
     return cf_module
 
-# %% ../nbs/06_evaluate.ipynb 23
+# %% ../nbs/06_evaluate.ipynb 29
 def _check_aux_pred_fn_args(pred_fn_args: dict | None):
     if pred_fn_args is None:
         return dict()
     elif isinstance(pred_fn_args, dict):
         return pred_fn_args
     else:
         raise ValueError(f'`pred_fn_args` should be a `dict`,',
@@ -225,15 +291,15 @@
                     f"and `{type(cf_module).__name__}` has not attribute `pred_fn`."
             )
     elif isinstance(cf_module, BasePredFnCFModule):
         # override pred_fn if `cf_module` has `pred_fn`
         pred_fn = cf_module.pred_fn
     return pred_fn
 
-# %% ../nbs/06_evaluate.ipynb 24
+# %% ../nbs/06_evaluate.ipynb 30
 def generate_cf_explanations(
     cf_module: BaseCFModule, # CF Explanation Module
     datamodule: TabularDataModule, # Data Module
     pred_fn: callable = None, # Predictive function
     strategy: str | BaseGenerationStrategy = 'vmap', # Parallelism Strategy for generating CFs
     t_configs: TrainingConfigs = None, # training configs for `BaseParametricCFModule`
     pred_fn_args: dict = None # auxiliary arguments for `pred_fn` 
@@ -251,30 +317,30 @@
         cf_module = _train_parametric_module(
             cf_module, datamodule, t_configs=t_configs, pred_fn=pred_fn
         )
     X, _ = datamodule.test_dataset[:]
 
     strategy = StrategyFactory.get_strategy(strategy)
     current_time = time.time()
-    cfs = strategy(cf_module.generate_cf, X, pred_fn=pred_fn)
+    cfs = strategy(cf_module.generate_cf, X, pred_fn=pred_fn).block_until_ready()
     total_time = time.time() - current_time
 
     # check pred_fn
     pred_fn = _check_pred_fn(pred_fn, cf_module)
 
     return Explanation(
         cf_name=cf_module.name,
         data_module=datamodule,
         cfs=cfs,
         total_time=total_time,
         pred_fn=pred_fn,
     )
 
 
-# %% ../nbs/06_evaluate.ipynb 32
+# %% ../nbs/06_evaluate.ipynb 38
 class BaseEvalMetrics(ABC):
     """Base evaluation metrics class."""
 
     def __init__(self, name: str = None):
         if name is None: name = type(self).__name__
         self.name = name
 
@@ -285,138 +351,138 @@
                 "EvalMetrics must have a name. Add the following as the first line in your "
                 f"__init__ method:\n\nsuper({self.__name__}, self).__init__()")
         return self.name
 
     def __call__(self, cf_explanations: Explanation) -> Any:
         raise NotImplementedError
 
-# %% ../nbs/06_evaluate.ipynb 33
+# %% ../nbs/06_evaluate.ipynb 39
 def _compute_acc(
     input: jnp.DeviceArray, # input dim: [N, k]
     label: jnp.DeviceArray, # label dim: [N] or [N, 1]
     pred_fn: Callable[[jnp.DeviceArray], jnp.DeviceArray]
 ) -> float:
     y_pred = pred_fn(input).reshape(-1, 1).round()
     label = label.reshape(-1, 1)
     return accuracy(y_pred, label).item()
 
-# %% ../nbs/06_evaluate.ipynb 35
+# %% ../nbs/06_evaluate.ipynb 41
 class PredictiveAccuracy(BaseEvalMetrics):
     """Compute the accuracy of the predict function."""
     
     def __init__(self, name: str = "accuracy"):
         super().__init__(name=name)
 
     def __call__(self, cf_explanations: Explanation) -> float:
         X, y = cf_explanations.data_module.test_dataset[:]
         return _compute_acc(X, y, cf_explanations.pred_fn)
 
-# %% ../nbs/06_evaluate.ipynb 37
+# %% ../nbs/06_evaluate.ipynb 43
 def _compute_val(
     input: jnp.DeviceArray, # input dim: [N, k]
     cfs: jnp.DeviceArray, # cfs dim: [N, k]
     pred_fn: Callable[[jnp.DeviceArray], jnp.DeviceArray]
 ):
     y_pred = pred_fn(input).reshape(-1, 1).round()
     y_prime = jnp.ones_like(y_pred) - y_pred
     cf_y = pred_fn(cfs).reshape(-1, 1).round()
     return accuracy(y_prime, cf_y).item()
 
-# %% ../nbs/06_evaluate.ipynb 39
+# %% ../nbs/06_evaluate.ipynb 45
 class Validity(BaseEvalMetrics):
     """Compute fraction of input instances on which CF explanation methods output valid CF examples."""
     
     def __init__(self, name: str = "validity"):
         super().__init__(name=name)
     
     def __call__(self, cf_explanations: Explanation) -> float:
         X, _ = cf_explanations.data_module.test_dataset[:]
         return _compute_val(
             X, cf_explanations.cfs, cf_explanations.pred_fn
         )
 
-# %% ../nbs/06_evaluate.ipynb 40
+# %% ../nbs/06_evaluate.ipynb 46
 def _compute_proximity(
     inputs: jnp.DeviceArray, # input dim: [N, k]
     cfs: jnp.DeviceArray, # cfs dim: [N, k]
 ):
     prox = jnp.linalg.norm(inputs - cfs, ord=1, axis=1).mean()
     return prox.item()
 
-# %% ../nbs/06_evaluate.ipynb 42
+# %% ../nbs/06_evaluate.ipynb 48
 class Proximity(BaseEvalMetrics):
     """Compute L1 norm distance between input datasets and CF examples divided by the number of features."""
     def __init__(self, name: str = "proximity"):
         super().__init__(name=name)
     
     def __call__(self, cf_explanations: Explanation) -> float:
         X, _ = cf_explanations.data_module.test_dataset[:]
         return _compute_proximity(X, cf_explanations.cfs)
 
-# %% ../nbs/06_evaluate.ipynb 43
+# %% ../nbs/06_evaluate.ipynb 49
 def _compute_spar(
     input: jnp.DeviceArray,
     cfs: jnp.DeviceArray,
     cat_idx: int
 ):
     # calculate sparsity
     cat_sparsity = proximity(input[:, cat_idx:], cfs[:, cat_idx:]) / 2
     cont_sparsity = jnp.linalg.norm(
         jnp.abs(input[:, :cat_idx] - cfs[:, :cat_idx]), ord=0, axis=1
     ).mean()
     return (cont_sparsity + cat_sparsity).item()
 
 
-# %% ../nbs/06_evaluate.ipynb 44
+# %% ../nbs/06_evaluate.ipynb 50
 class Sparsity(BaseEvalMetrics):
     """Compute the number of feature changes between input datasets and CF examples."""
 
     def __init__(self, name: str = "sparsity"):
         super().__init__(name=name)
     
     def __call__(self, cf_explanations: Explanation) -> float:
         X, _ = cf_explanations.data_module.test_dataset[:]
         return _compute_spar(X, cf_explanations.cfs, cf_explanations.cat_idx)
 
-# %% ../nbs/06_evaluate.ipynb 45
+# %% ../nbs/06_evaluate.ipynb 51
 def _compute_manifold_dist(
     input: jnp.DeviceArray,
     cfs: jnp.DeviceArray,
     n_neighbors: int = 1,
     p: int = 2
 ):
     knn = NearestNeighbors(n_neighbors=n_neighbors, p=p)
     knn.fit(input)
     nearest_dist, nearest_points = knn.kneighbors(cfs, 1, return_distance=True)
     return jnp.mean(nearest_dist).item()
 
-# %% ../nbs/06_evaluate.ipynb 46
+# %% ../nbs/06_evaluate.ipynb 52
 class ManifoldDist(BaseEvalMetrics):
     """Compute the L1 distance to the n-nearest neighbor for all CF examples."""
     def __init__(self, n_neighbors: int = 1, p: int = 2, name: str = "manifold_dist"):
         super().__init__(name=name)
         self.n_neighbors = n_neighbors
         self.p = p
         
     def __call__(self, cf_explanations: Explanation) -> float:
         X, _ = cf_explanations.data_module.test_dataset[:]
         return _compute_manifold_dist(
             X, cf_explanations.cfs, self.n_neighbors, self.p
         )
 
-# %% ../nbs/06_evaluate.ipynb 47
+# %% ../nbs/06_evaluate.ipynb 53
 class Runtime(BaseEvalMetrics):
     """Get the running time to generate CF examples."""
     def __init__(self, name: str = "runtime"):
         super().__init__(name=name)
     
     def __call__(self, cf_explanations: Explanation) -> float:
         return cf_explanations.total_time
 
-# %% ../nbs/06_evaluate.ipynb 49
+# %% ../nbs/06_evaluate.ipynb 55
 def _create_second_order_cfs(cf_results: CFExplanationResults, threshold: float = 2.0):
     X, y = cf_results.data_module.test_dataset[:]
     cfs = cf_results.cfs
     scaler = cf_results.data_module.normalizer
     cat_idx = cf_results.data_module.cat_idx
 
     # get normalized threshold = threshold / (max - min)
@@ -455,15 +521,15 @@
     cfs_hat = _create_second_order_cfs(cf_results, threshold)
     cf_results_so = deepcopy(cf_results)
     cf_results_so.cfs = cfs_hat
     compute_sparsity = Sparsity()
     return compute_sparsity(cf_results_so)
 
 
-# %% ../nbs/06_evaluate.ipynb 51
+# %% ../nbs/06_evaluate.ipynb 57
 def fake_explanations():
     """Generate sudo explanations for testing."""
     from relax.data import load_data
 
     dm = load_data("adult")
     X, y = dm.test_dataset[:]
     cfs = X
@@ -471,15 +537,15 @@
     pred_fn = lambda x: jax.random.bernoulli(jax.random.PRNGKey(0), 0.5, (x.shape[0], 1)).astype(float)
     assert y.shape == pred_fn(X).shape
     return Explanation(
         cf_name='sudo', data_module=dm, cfs=cfs, pred_fn=pred_fn, total_time=0.0, dataset_name=dn
     )
 
 
-# %% ../nbs/06_evaluate.ipynb 52
+# %% ../nbs/06_evaluate.ipynb 58
 # METRICS = dict(
 #     acc=PredictiveAccuracy(),
 #     accuracy=PredictiveAccuracy(),
 #     validity=Validity(),
 #     proximity=Proximity(),
 #     runtime=Runtime(),
 #     manifold_dist=ManifoldDist(),
@@ -497,15 +563,15 @@
     ManifoldDist(),
 ]
 
 METRICS = { m.name: m for m in METRICS_CALLABLE }
 
 DEFAULT_METRICS = ["acc", "validity", "proximity"]
 
-# %% ../nbs/06_evaluate.ipynb 54
+# %% ../nbs/06_evaluate.ipynb 60
 def _get_metric(metric: str | BaseEvalMetrics, cf_exp: Explanation):
     if isinstance(metric, str):
         if metric not in METRICS.keys():
             raise ValueError(f"'{metric}' is not supported. Must be one of {METRICS.keys()}")
         res = METRICS[metric](cf_exp)
     elif callable(metric):
         # f(cf_exp) not supported for now
@@ -515,15 +581,15 @@
     else:
         raise ValueError(f"{type(metric).__name__} is not supported as a metric.")
     
     if isinstance(res, jnp.ndarray) and res.shape == (1,):
         res = res.item()
     return res
 
-# %% ../nbs/06_evaluate.ipynb 56
+# %% ../nbs/06_evaluate.ipynb 62
 def evaluate_cfs(
     cf_exp: Explanation, # CF Explanations
     metrics: Iterable[Union[str, BaseEvalMetrics]] = None, # A list of Metrics. Can be `str` or a subclass of `BaseEvalMetrics`
     return_dict: bool = True, # return a dictionary or not (default: True)
     return_df: bool = False # return a pandas Dataframe or not (default: False)
 ):
     cf_name = cf_exp.cf_name
@@ -539,15 +605,15 @@
     result_df = pd.DataFrame.from_dict(result_dict, orient="index")
     
     if return_dict and return_df:
         return (result_dict, result_df)
     elif return_dict or return_df:
         return result_df if return_df else result_dict
 
-# %% ../nbs/06_evaluate.ipynb 58
+# %% ../nbs/06_evaluate.ipynb 64
 def benchmark_cfs(
     cf_results_list: Iterable[CFExplanationResults],
     metrics: Optional[Iterable[str]] = None,
 ):
     dfs = [
         evaluate_cfs(
             cf_exp=cf_results, metrics=metrics, return_dict=False, return_df=True
```

### Comparing `jax-relax-0.1.5/relax/logger.py` & `jax-relax-0.1.6/relax/logger.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.5/relax/methods/base.py` & `jax-relax-0.1.6/relax/methods/base.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.5/relax/methods/cchvae.py` & `jax-relax-0.1.6/relax/methods/cchvae.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,18 @@
     lr = 0.001
 
 # %% ../../nbs/methods/06_cchvae.ipynb 6
 class CHVAE(BaseTrainingModule):
     def __init__(self, m_config: Dict):
         self.save_hyperparameters(m_config)
         self.m_config = validate_configs(m_config, CHVAEConfigs)
-        self.opt = optax.adam(self.m_config.lr)
+        self.opt = optax.chain(
+            optax.adaptive_grad_clip(0.05),
+            optax.adam(self.m_config.lr)
+        )
 
     def init_net_opt(self, dm, key):
         X, _ = dm.train_dataset[:128]
         encoded_size = self.m_config.enc_sizes[-1]
         Z = jnp.ones((X.shape[0], encoded_size))
 
         self.encoder = make_hk_module(
@@ -220,32 +223,31 @@
     z_rep = z.reshape(1, -1)
     rng_key, _ = jrand.split(rng_key)
     # candidate_cf = jnp.array(x, copy=True)
     candidate_cf = jnp.ones_like(x) * jnp.inf
     state = (0, candidate_cf, rng_key) # (count, candidate_cf, rng_key)
     # count, candidate_cf, rng_key = jax.lax.while_loop(cond_fn, body_fn, state)
     count, candidate_cf, rng_key = lax.fori_loop(0, max_steps, body_fn, state)
-    # while cond_fn(state):
-    #     count, candidate_cf, rng_key = body_fn(state)
-    # print(count)
+    # if `inf` is found, return the original input
+    candidate_cf = jnp.where(jnp.isinf(candidate_cf), x, candidate_cf)
     return candidate_cf
 
 # %% ../../nbs/methods/06_cchvae.ipynb 9
 class CCHVAEConfigs(BaseParser):
     enc_sizes: List[int] = Field(
         [20, 16, 14, 12], description="Encoder hidden sizes"
     ) 
     dec_sizes: List[int] = Field(
         [12, 14, 16, 20], description="Decoder hidden sizes"
     )
     encoded_size: int = Field(5, description="Encoded size")
     lr: float = Field(0.001, description="Learning rate")
     max_steps: int = Field(100, description="Max steps")
     n_search_samples: int = Field(300, description="Number of generated candidate counterfactuals.")
-    step_size: float = Field(1, description="Step size")
+    step_size: float = Field(0.1, description="Step size")
     seed: int = Field(0, description="Seed for random number generator")
 
 # %% ../../nbs/methods/06_cchvae.ipynb 10
 class CCHVAE(BaseCFModule, BaseParametricCFModule):
     params: Tuple[hk.Params, hk.Params] = None
     module: CHVAE
     name: str = 'C-CHVAE'
```

### Comparing `jax-relax-0.1.5/relax/methods/clue.py` & `jax-relax-0.1.6/relax/methods/clue.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,17 +344,18 @@
 # %% ../../nbs/methods/08_clue.ipynb 10
 class CLUE(BaseCFModule, BaseParametricCFModule):
     params: Tuple[hk.Params, hk.Params] = None
     module: VAEGaussCat
     name: str = 'CLUE'
 
     def __init__(self, m_config: Dict | CLUEConfigs = None):
-        if m_config is None: m_config = CLUEConfigs()
-        self.m_config = m_config
-        self.module = VAEGaussCat(m_config.dict())
+        if m_config is None:
+            m_config = CLUEConfigs()
+        self.m_config = validate_configs(m_config, CLUEConfigs)
+        self.module = VAEGaussCat(self.m_config.dict())
         self.rng_key = random.PRNGKey(self.m_config.seed)
 
     def _is_module_trained(self) -> bool:
         return not (self.params is None)
     
     def train(
         self,
```

### Comparing `jax-relax-0.1.5/relax/methods/counternet.py` & `jax-relax-0.1.6/relax/methods/counternet.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,29 +14,31 @@
 __all__ = ['CounterNetModel', 'partition_trainable_params', 'project_immutable_features', 'CounterNetTrainingModuleConfigs',
            'CounterNetTrainingModule', 'CounterNetConfigs', 'CounterNet']
 
 # %% ../../nbs/methods/04_counternet.ipynb 5
 class CounterNetModelConfigs(BaseParser):
     """Configurator of `CounterNetModel`."""
 
-    enc_sizes: List[int] = Field(description='Encoder sizes.')
-    dec_sizes: List[int] = Field(description='Predictor sizes.')
-    exp_sizes: List[int] = Field(description='CF generator sizes.')
+    enc_sizes: List[int] = Field([50,10], description='Encoder sizes.')
+    dec_sizes: List[int] = Field([10], description='Predictor sizes.')
+    exp_sizes: List[int] = Field([50, 50], description='CF generator sizes.')
     dropout_rate: float = Field(0.3, description='Dropout rate.')
 
 # %% ../../nbs/methods/04_counternet.ipynb 6
 class CounterNetModel(hk.Module):
     """CounterNet Model"""
     def __init__(
         self,
         m_config: Dict | CounterNetModelConfigs,  # Model configs which contain configs in `CounterNetModelConfigs`.
         name: str = None,  # Name of the module.
     ):
         """CounterNet model architecture."""
         super().__init__(name=name)
+        if m_config is None:
+            m_config = CounterNetModelConfigs()
         self.configs = validate_configs(m_config, CounterNetModelConfigs)
 
     def __call__(self, x: jnp.ndarray, is_training: bool = True) -> jnp.ndarray:
         input_shape = x.shape[-1]
         # encoder
         z = MLP(self.configs.enc_sizes, self.configs.dropout_rate, name="Encoder")(
             x, is_training
```

### Comparing `jax-relax-0.1.5/relax/methods/diverse.py` & `jax-relax-0.1.6/relax/methods/diverse.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     lambda_: float,  #  loss = validity_loss + lambda_params * cost
     key: jax.random.PRNGKey,
     projection_fn: Callable,
     regularization_fn: Callable
 ) -> jnp.DeviceArray:  # return `cf` shape: (k,)
     @jit
     def loss_fn_1(cf_y: Array, y_prime: Array):
-        return jnp.mean(hinge_loss(input=cf_y, target=y_prime))
+        return optax.l2_loss(cf_y.mean(axis=0, keepdims=True), y_prime).mean()
 
     @jit
     def loss_fn_2(x: Array, cf: Array):
         return jnp.mean(jnp.abs(cf - x))
 
     @partial(jit, static_argnums=(1,))
     def loss_fn_3(cfs: jnp.DeviceArray, n_cfs: int):
@@ -98,28 +98,28 @@
         y_prime = 1.0 - y_pred
         cf_y = pred_fn(cf)
 
         loss_1 = loss_fn_1(cf_y, y_prime)
         loss_2 = loss_fn_2(x, cf)
         loss_3 = loss_fn_3(cf, n_cfs)
         loss_4 = loss_fn_4(x, cfs)
-        return loss_1 + loss_2 + loss_3 + loss_4
+        return loss_1 + 0.01 * loss_2 + loss_3 + 0.1 * loss_4
 
     @loop_tqdm(n_steps)
     def gen_cf_step(
         i, cf_opt_state: Tuple[Array, optax.OptState]
     ) -> Tuple[Array, optax.OptState]:
         cf, opt_state = cf_opt_state
         cf_grads = jax.grad(loss_fn)(cf, x, pred_fn)
         cf, opt_state = grad_update(cf_grads, cf, opt_state, opt)
         return cf, opt_state
 
     key, subkey = jax.random.split(key)
     cfs = jax.random.normal(key, shape=(n_cfs, x.shape[-1]))
-    opt = optax.rmsprop(lr)
+    opt = optax.adam(lr)
     opt_state = opt.init(cfs)
     cfs, opt_state = lax.fori_loop(0, n_steps, gen_cf_step, (cfs, opt_state))
     # for _ in tqdm(range(n_steps)):
     #     cfs, opt_state = gen_cf_step(x, cfs, opt_state)
     cf = projection_fn(x, cfs[:1, :], hard=True)
     return cf
```

### Comparing `jax-relax-0.1.5/relax/methods/proto.py` & `jax-relax-0.1.6/relax/methods/proto.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.5/relax/methods/sphere.py` & `jax-relax-0.1.6/relax/methods/sphere.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.5/relax/methods/vaecf.py` & `jax-relax-0.1.6/relax/methods/vaecf.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,16 +257,16 @@
     params: Tuple[hk.Params, hk.Params] = None
     module: VAECFModule
     name: str = 'VAECF'
 
     def __init__(self, m_config: Dict | VAECFConfigs = None):
         if m_config is None:
             m_config = VAECFConfigs()
-        self.m_config = m_config
-        self.module = VAECFModule(m_config.dict())
+        self.m_config = validate_configs(m_config, VAECFConfigs)
+        self.module = VAECFModule(self.m_config.dict())
 
     def _is_module_trained(self) -> bool:
         return not (self.params is None)
     
     def train(
         self, 
         datamodule: TabularDataModule, # data module
```

### Comparing `jax-relax-0.1.5/relax/methods/vanilla.py` & `jax-relax-0.1.6/relax/methods/vanilla.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.5/relax/module.py` & `jax-relax-0.1.6/relax/module.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.5/relax/plots.py` & `jax-relax-0.1.6/relax/plots.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.5/relax/trainer.py` & `jax-relax-0.1.6/relax/trainer.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.5/relax/utils.py` & `jax-relax-0.1.6/relax/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 # %% ../nbs/00_utils.ipynb 42
 def grad_update(
     grads: Dict[str, jnp.ndarray],
     params: hk.Params,
     opt_state: optax.OptState,
     opt: optax.GradientTransformation,
 ) -> Tuple[hk.Params, optax.OptState]:
-    updates, opt_state = opt.update(grads, opt_state)
+    updates, opt_state = opt.update(grads, opt_state, params)
     upt_params = optax.apply_updates(params, updates)
     return upt_params, opt_state
 
 
 # %% ../nbs/00_utils.ipynb 43
 def check_cat_info(method):
     def inner(cf_module, *args, **kwargs):
```

### Comparing `jax-relax-0.1.5/settings.ini` & `jax-relax-0.1.6/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = birkhoffg
 description = Jax-based Recourse Explanation Library
 keywords = Jax, Recourse, Explanation, Interpretability, Machine Learning
 author = BirkhoffG
 author_email = 26811230+BirkhoffG@users.noreply.github.com
 copyright = Birkhoff Guo
 branch = master
-version = 0.1.5
+version = 0.1.6
 min_python = 3.8
 audience = Developers
 language = English
 custom_sidebar = true
 license = apache2
 status = 2
 requirements = matplotlib seaborn scikit-learn>=1.0.2,<1.4.0 pandas nbdev jupyter dm-haiku test_tube jax[cpu] tqdm optax pydantic>=1.9.0,<2 deprecation networkx jax-tqdm
```

### Comparing `jax-relax-0.1.5/setup.py` & `jax-relax-0.1.6/setup.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from pkg_resources import parse_version
-from configparser import ConfigParser
-import setuptools
-assert parse_version(setuptools.__version__)>=parse_version('36.2')
-
-# note: all settings are in settings.ini; edit there, not here
-config = ConfigParser(delimiters=['='])
-config.read('settings.ini')
-cfg = config['DEFAULT']
-
-cfg_keys = 'version description keywords author author_email'.split()
-expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
-for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
-setup_cfg = {o:cfg[o] for o in cfg_keys}
-
-licenses = {
-    'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
-    'mit': ('MIT License', 'OSI Approved :: MIT License'),
-    'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
-    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
-    'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
-}
-statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
-    '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
-py_versions = '3.6 3.7 3.8 3.9 3.10 3.11'.split()
-
-requirements = cfg.get('requirements','').split()
-if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
-min_python = cfg['min_python']
-lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
-dev_requirements = (cfg.get('dev_requirements') or '').split()
-
-setuptools.setup(
-    name = cfg['lib_name'],
-    license = lic[0],
-    classifiers = [
-        'Development Status :: ' + statuses[int(cfg['status'])],
-        'Intended Audience :: ' + cfg['audience'].title(),
-        'Natural Language :: ' + cfg['language'].title(),
-    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
-    url = cfg['git_url'],
-    packages = setuptools.find_packages(),
-    include_package_data = True,
-    install_requires = requirements,
-    extras_require={ 'dev': dev_requirements },
-    dependency_links = cfg.get('dep_links','').split(),
-    python_requires  = '>=' + cfg['min_python'],
-    long_description = open('README.md').read(),
-    long_description_content_type = 'text/markdown',
-    zip_safe = False,
-    entry_points = {
-        'console_scripts': cfg.get('console_scripts','').split(),
-        'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
-    },
-    **setup_cfg)
-
-
+from pkg_resources import parse_version
+from configparser import ConfigParser
+import setuptools
+assert parse_version(setuptools.__version__)>=parse_version('36.2')
+
+# note: all settings are in settings.ini; edit there, not here
+config = ConfigParser(delimiters=['='])
+config.read('settings.ini')
+cfg = config['DEFAULT']
+
+cfg_keys = 'version description keywords author author_email'.split()
+expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
+for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
+setup_cfg = {o:cfg[o] for o in cfg_keys}
+
+licenses = {
+    'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
+    'mit': ('MIT License', 'OSI Approved :: MIT License'),
+    'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
+    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
+    'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
+}
+statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
+    '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
+py_versions = '3.6 3.7 3.8 3.9 3.10 3.11'.split()
+
+requirements = cfg.get('requirements','').split()
+if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
+min_python = cfg['min_python']
+lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
+dev_requirements = (cfg.get('dev_requirements') or '').split()
+
+setuptools.setup(
+    name = cfg['lib_name'],
+    license = lic[0],
+    classifiers = [
+        'Development Status :: ' + statuses[int(cfg['status'])],
+        'Intended Audience :: ' + cfg['audience'].title(),
+        'Natural Language :: ' + cfg['language'].title(),
+    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
+    url = cfg['git_url'],
+    packages = setuptools.find_packages(),
+    include_package_data = True,
+    install_requires = requirements,
+    extras_require={ 'dev': dev_requirements },
+    dependency_links = cfg.get('dep_links','').split(),
+    python_requires  = '>=' + cfg['min_python'],
+    long_description = open('README.md').read(),
+    long_description_content_type = 'text/markdown',
+    zip_safe = False,
+    entry_points = {
+        'console_scripts': cfg.get('console_scripts','').split(),
+        'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
+    },
+    **setup_cfg)
+
+
```

