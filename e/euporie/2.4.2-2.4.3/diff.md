# Comparing `tmp/euporie-2.4.2.tar.gz` & `tmp/euporie-2.4.3.tar.gz`

## Comparing `euporie-2.4.2.tar` & `euporie-2.4.3.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/console/__init__.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/console/__main__.py
--rw-r--r--   0        0        0     7667 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/console/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/console/py.typed
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/console/tabs/__init__.py
--rw-r--r--   0        0        0    23533 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/console/tabs/console.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/__init__.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/__main__.py
--rw-r--r--   0        0        0    40124 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/app.py
--rw-r--r--   0        0        0    46884 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/border.py
--rw-r--r--   0        0        0     8252 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/commands.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/completion.py
--rw-r--r--   0        0        0    21438 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/config.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/current.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/data_structures.py
--rw-r--r--   0        0        0     8064 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/filters.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/format.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/history.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/io.py
--rw-r--r--   0        0        0    41091 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/kernel.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/keys.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/launch.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/lexers.py
--rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/log.py
--rw-r--r--   0        0        0    21206 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/margins.py
--rw-r--r--   0        0        0     7946 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/path.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/processors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/py.typed
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/pygments.py
--rw-r--r--   0        0        0    65039 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/reference.py
--rw-r--r--   0        0        0    16527 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/renderer.py
--rw-r--r--   0        0        0    30922 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/style.py
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/suggest.py
--rw-r--r--   0        0        0    14686 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/terminal.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/utils.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/validation.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/comm/__init__.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/comm/base.py
--rw-r--r--   0        0        0    52707 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/comm/ipywidgets.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/comm/registry.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/convert/__init__.py
--rw-r--r--   0        0        0     8732 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/convert/core.py
--rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/convert/utils.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/convert/formats/__init__.py
--rw-r--r--   0        0        0    13561 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/convert/formats/ansi.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/convert/formats/base64.py
--rw-r--r--   0        0        0     4965 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/convert/formats/common.py
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/convert/formats/formatted_text.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/convert/formats/html.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/convert/formats/jpeg.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/convert/formats/markdown.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/convert/formats/pdf.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/convert/formats/pil.py
--rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/convert/formats/png.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/convert/formats/rich.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/convert/formats/sixel.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/formatted_text/__init__.py
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/formatted_text/ansi.py
--rw-r--r--   0        0        0   144060 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/formatted_text/html.py
--rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/formatted_text/markdown.py
--rw-r--r--   0        0        0    41140 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/formatted_text/table.py
--rw-r--r--   0        0        0    27819 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/formatted_text/utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/key_binding/__init__.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/key_binding/key_processor.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/key_binding/micro_state.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/key_binding/registry.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/key_binding/utils.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/key_binding/vi_state.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/key_binding/bindings/__init__.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/key_binding/bindings/completion.py
--rw-r--r--   0        0        0    28624 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/key_binding/bindings/micro.py
--rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/key_binding/bindings/mouse.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/tabs/__init__.py
--rw-r--r--   0        0        0    13546 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/tabs/base.py
--rw-r--r--   0        0        0    15648 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/tabs/notebook.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/__init__.py
--rw-r--r--   0        0        0    29874 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/cell.py
--rw-r--r--   0        0        0    15742 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/cell_outputs.py
--rw-r--r--   0        0        0    22153 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/decor.py
--rw-r--r--   0        0        0    32257 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/dialog.py
--rw-r--r--   0        0        0    49787 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/display.py
--rw-r--r--   0        0        0    19842 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/file_browser.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/formatted_text_area.py
--rw-r--r--   0        0        0    82382 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/forms.py
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/inputs.py
--rw-r--r--   0        0        0    20678 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/layout.py
--rw-r--r--   0        0        0    30676 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/menu.py
--rw-r--r--   0        0        0    42512 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/page.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/pager.py
--rw-r--r--   0        0        0    10814 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/palette.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/search_bar.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/status_bar.py
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/core/widgets/tree.py
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/data/desktop/euporie-console.desktop
--rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/data/desktop/euporie-notebook.desktop
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/hub/__init__.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/hub/__main__.py
--rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/hub/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/hub/py.typed
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/notebook/__init__.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/notebook/__main__.py
--rw-r--r--   0        0        0    20398 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/notebook/app.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/notebook/current.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/notebook/enums.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/notebook/filters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/notebook/py.typed
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/notebook/tabs/__init__.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/notebook/tabs/display.py
--rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/notebook/tabs/edit.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/notebook/tabs/json.py
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/notebook/tabs/log.py
--rw-r--r--   0        0        0    41796 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/notebook/tabs/notebook.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/notebook/widgets/__init__.py
--rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/notebook/widgets/side_bar.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/preview/__init__.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/preview/__main__.py
--rw-r--r--   0        0        0     8769 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/preview/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/preview/py.typed
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/preview/tabs/__init__.py
--rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/preview/tabs/notebook.py
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/web/tabs/web.py
--rw-r--r--   0        0        0    19186 2020-02-02 00:00:00.000000 euporie-2.4.2/euporie/web/widgets/webview.py
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 euporie-2.4.2/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 euporie-2.4.2/LICENSE
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 euporie-2.4.2/README.rst
--rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 euporie-2.4.2/pyproject.toml
--rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 euporie-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/console/__init__.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/console/__main__.py
+-rw-r--r--   0        0        0     7667 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/console/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/console/py.typed
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/console/tabs/__init__.py
+-rw-r--r--   0        0        0    23533 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/console/tabs/console.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/__init__.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/__main__.py
+-rw-r--r--   0        0        0    40124 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/app.py
+-rw-r--r--   0        0        0    46884 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/border.py
+-rw-r--r--   0        0        0     8252 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/commands.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/completion.py
+-rw-r--r--   0        0        0    21438 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/config.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/current.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/data_structures.py
+-rw-r--r--   0        0        0     8064 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/filters.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/format.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/history.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/io.py
+-rw-r--r--   0        0        0    41091 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/kernel.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/keys.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/launch.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/lexers.py
+-rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/log.py
+-rw-r--r--   0        0        0    21206 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/margins.py
+-rw-r--r--   0        0        0     7946 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/path.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/processors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/py.typed
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/pygments.py
+-rw-r--r--   0        0        0    65039 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/reference.py
+-rw-r--r--   0        0        0    16527 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/renderer.py
+-rw-r--r--   0        0        0    30972 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/style.py
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/suggest.py
+-rw-r--r--   0        0        0    14686 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/terminal.py
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/utils.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/validation.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/comm/__init__.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/comm/base.py
+-rw-r--r--   0        0        0    52707 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/comm/ipywidgets.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/comm/registry.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/convert/__init__.py
+-rw-r--r--   0        0        0     8732 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/convert/core.py
+-rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/convert/utils.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/convert/formats/__init__.py
+-rw-r--r--   0        0        0    13561 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/convert/formats/ansi.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/convert/formats/base64.py
+-rw-r--r--   0        0        0     4965 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/convert/formats/common.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/convert/formats/formatted_text.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/convert/formats/html.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/convert/formats/jpeg.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/convert/formats/markdown.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/convert/formats/pdf.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/convert/formats/pil.py
+-rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/convert/formats/png.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/convert/formats/rich.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/convert/formats/sixel.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/formatted_text/__init__.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/formatted_text/ansi.py
+-rw-r--r--   0        0        0   144060 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/formatted_text/html.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/formatted_text/markdown.py
+-rw-r--r--   0        0        0    41140 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/formatted_text/table.py
+-rw-r--r--   0        0        0    27819 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/formatted_text/utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/key_binding/__init__.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/key_binding/key_processor.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/key_binding/micro_state.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/key_binding/registry.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/key_binding/utils.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/key_binding/vi_state.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/key_binding/bindings/__init__.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/key_binding/bindings/completion.py
+-rw-r--r--   0        0        0    28624 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/key_binding/bindings/micro.py
+-rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/key_binding/bindings/mouse.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/tabs/__init__.py
+-rw-r--r--   0        0        0    13546 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/tabs/base.py
+-rw-r--r--   0        0        0    15648 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/tabs/notebook.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/__init__.py
+-rw-r--r--   0        0        0    29874 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/cell.py
+-rw-r--r--   0        0        0    15742 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/cell_outputs.py
+-rw-r--r--   0        0        0    22153 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/decor.py
+-rw-r--r--   0        0        0    32257 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/dialog.py
+-rw-r--r--   0        0        0    49787 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/display.py
+-rw-r--r--   0        0        0    19842 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/file_browser.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/formatted_text_area.py
+-rw-r--r--   0        0        0    82382 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/forms.py
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/inputs.py
+-rw-r--r--   0        0        0    20678 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/layout.py
+-rw-r--r--   0        0        0    30676 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/menu.py
+-rw-r--r--   0        0        0    42512 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/page.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/pager.py
+-rw-r--r--   0        0        0    10814 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/palette.py
+-rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/search_bar.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/status_bar.py
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/core/widgets/tree.py
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/data/desktop/euporie-console.desktop
+-rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/data/desktop/euporie-notebook.desktop
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/hub/__init__.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/hub/__main__.py
+-rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/hub/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/hub/py.typed
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/notebook/__init__.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/notebook/__main__.py
+-rw-r--r--   0        0        0    20398 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/notebook/app.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/notebook/current.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/notebook/enums.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/notebook/filters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/notebook/py.typed
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/notebook/tabs/__init__.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/notebook/tabs/display.py
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/notebook/tabs/edit.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/notebook/tabs/json.py
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/notebook/tabs/log.py
+-rw-r--r--   0        0        0    41796 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/notebook/tabs/notebook.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/notebook/widgets/__init__.py
+-rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/notebook/widgets/side_bar.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/preview/__init__.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/preview/__main__.py
+-rw-r--r--   0        0        0     8769 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/preview/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/preview/py.typed
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/preview/tabs/__init__.py
+-rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/preview/tabs/notebook.py
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/web/tabs/web.py
+-rw-r--r--   0        0        0    19186 2020-02-02 00:00:00.000000 euporie-2.4.3/euporie/web/widgets/webview.py
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 euporie-2.4.3/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 euporie-2.4.3/LICENSE
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 euporie-2.4.3/README.rst
+-rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 euporie-2.4.3/pyproject.toml
+-rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 euporie-2.4.3/PKG-INFO
```

### Comparing `euporie-2.4.2/euporie/console/app.py` & `euporie-2.4.3/euporie/console/app.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/console/tabs/console.py` & `euporie-2.4.3/euporie/console/tabs/console.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/app.py` & `euporie-2.4.3/euporie/core/app.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/border.py` & `euporie-2.4.3/euporie/core/border.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/commands.py` & `euporie-2.4.3/euporie/core/commands.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/completion.py` & `euporie-2.4.3/euporie/core/completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,9 +37,10 @@
     ) -> AsyncGenerator[Completion, None]:
         """Retrieve completions from a :class:`Kernel`."""
         for kwargs in await self.kernel.complete_(
             code=document.text,
             cursor_pos=document.cursor_position,
         ):
             if completion_type := kwargs.get("display_meta"):
+                completion_type = completion_type.replace(" ", "-")
                 kwargs["style"] = f"class:completion-{completion_type}"
             yield Completion(**kwargs)
```

### Comparing `euporie-2.4.2/euporie/core/config.py` & `euporie-2.4.3/euporie/core/config.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/current.py` & `euporie-2.4.3/euporie/core/current.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/data_structures.py` & `euporie-2.4.3/euporie/core/data_structures.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/filters.py` & `euporie-2.4.3/euporie/core/filters.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/format.py` & `euporie-2.4.3/euporie/core/format.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/history.py` & `euporie-2.4.3/euporie/core/history.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/io.py` & `euporie-2.4.3/euporie/core/io.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/kernel.py` & `euporie-2.4.3/euporie/core/kernel.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/keys.py` & `euporie-2.4.3/euporie/core/keys.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/launch.py` & `euporie-2.4.3/euporie/core/launch.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/lexers.py` & `euporie-2.4.3/euporie/core/lexers.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/log.py` & `euporie-2.4.3/euporie/core/log.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/margins.py` & `euporie-2.4.3/euporie/core/margins.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/path.py` & `euporie-2.4.3/euporie/core/path.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/processors.py` & `euporie-2.4.3/euporie/core/processors.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/pygments.py` & `euporie-2.4.3/euporie/core/pygments.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/reference.py` & `euporie-2.4.3/euporie/core/reference.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/renderer.py` & `euporie-2.4.3/euporie/core/renderer.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/style.py` & `euporie-2.4.3/euporie/core/style.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,14 +457,15 @@
         "menu completion-function": "fg:#005faf",
         "menu completion-class": "fg:#008700",
         "menu completion-statement": "fg:#5f0000",
         "menu completion-instance": "fg:#d75f00",
         "menu completion-module": "fg:#d70000",
         "menu completion-magic": "fg:#888888",
         "menu completion-path": "fg:#aa8800",
+        "menu completion-dict-key": "fg:#ddbb00",
         "menu selection completion-keyword": f"fg:{ColorPaletteColor('#d700af').lighter(0.75)}",
         "menu selection completion-function": f"fg:{ColorPaletteColor('#005faf').lighter(0.75)}",
         "menu selection completion-class": f"fg:{ColorPaletteColor('#008700').lighter(0.75)}",
         "menu selection completion-statement": f"fg:{ColorPaletteColor('#5f0000').lighter(0.75)}",
         "menu selection completion-instance": f"fg:{ColorPaletteColor('#d75f00').lighter(0.75)}",
         "menu selection completion-module": f"fg:{ColorPaletteColor('#d70000').lighter(0.75)}",
         "menu selection completion-magic": f"fg:{ColorPaletteColor('#888888').lighter(0.75)}",
```

### Comparing `euporie-2.4.2/euporie/core/suggest.py` & `euporie-2.4.3/euporie/core/suggest.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/terminal.py` & `euporie-2.4.3/euporie/core/terminal.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/utils.py` & `euporie-2.4.3/euporie/core/utils.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/validation.py` & `euporie-2.4.3/euporie/core/validation.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/comm/base.py` & `euporie-2.4.3/euporie/core/comm/base.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/comm/ipywidgets.py` & `euporie-2.4.3/euporie/core/comm/ipywidgets.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/comm/registry.py` & `euporie-2.4.3/euporie/core/comm/registry.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/convert/core.py` & `euporie-2.4.3/euporie/core/convert/core.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/convert/utils.py` & `euporie-2.4.3/euporie/core/convert/utils.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/convert/formats/ansi.py` & `euporie-2.4.3/euporie/core/convert/formats/ansi.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/convert/formats/base64.py` & `euporie-2.4.3/euporie/core/convert/formats/base64.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/convert/formats/common.py` & `euporie-2.4.3/euporie/core/convert/formats/common.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/convert/formats/formatted_text.py` & `euporie-2.4.3/euporie/core/convert/formats/formatted_text.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/convert/formats/html.py` & `euporie-2.4.3/euporie/core/convert/formats/html.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/convert/formats/markdown.py` & `euporie-2.4.3/euporie/core/convert/formats/markdown.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/convert/formats/pil.py` & `euporie-2.4.3/euporie/core/convert/formats/pil.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/convert/formats/png.py` & `euporie-2.4.3/euporie/core/convert/formats/png.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/convert/formats/rich.py` & `euporie-2.4.3/euporie/core/convert/formats/rich.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/convert/formats/sixel.py` & `euporie-2.4.3/euporie/core/convert/formats/sixel.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/formatted_text/ansi.py` & `euporie-2.4.3/euporie/core/formatted_text/ansi.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/formatted_text/html.py` & `euporie-2.4.3/euporie/core/formatted_text/html.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/formatted_text/markdown.py` & `euporie-2.4.3/euporie/core/formatted_text/markdown.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/formatted_text/table.py` & `euporie-2.4.3/euporie/core/formatted_text/table.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/formatted_text/utils.py` & `euporie-2.4.3/euporie/core/formatted_text/utils.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/key_binding/key_processor.py` & `euporie-2.4.3/euporie/core/key_binding/key_processor.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/key_binding/micro_state.py` & `euporie-2.4.3/euporie/core/key_binding/micro_state.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/key_binding/registry.py` & `euporie-2.4.3/euporie/core/key_binding/registry.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/key_binding/utils.py` & `euporie-2.4.3/euporie/core/key_binding/utils.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/key_binding/vi_state.py` & `euporie-2.4.3/euporie/core/key_binding/vi_state.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/key_binding/bindings/completion.py` & `euporie-2.4.3/euporie/core/key_binding/bindings/completion.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/key_binding/bindings/micro.py` & `euporie-2.4.3/euporie/core/key_binding/bindings/micro.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/key_binding/bindings/mouse.py` & `euporie-2.4.3/euporie/core/key_binding/bindings/mouse.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/tabs/base.py` & `euporie-2.4.3/euporie/core/tabs/base.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/tabs/notebook.py` & `euporie-2.4.3/euporie/core/tabs/notebook.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/widgets/cell.py` & `euporie-2.4.3/euporie/core/widgets/cell.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/widgets/cell_outputs.py` & `euporie-2.4.3/euporie/core/widgets/cell_outputs.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/widgets/decor.py` & `euporie-2.4.3/euporie/core/widgets/decor.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/widgets/dialog.py` & `euporie-2.4.3/euporie/core/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/widgets/display.py` & `euporie-2.4.3/euporie/core/widgets/display.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/widgets/file_browser.py` & `euporie-2.4.3/euporie/core/widgets/file_browser.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/widgets/formatted_text_area.py` & `euporie-2.4.3/euporie/core/widgets/formatted_text_area.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/widgets/forms.py` & `euporie-2.4.3/euporie/core/widgets/forms.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/widgets/inputs.py` & `euporie-2.4.3/euporie/core/widgets/inputs.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/widgets/layout.py` & `euporie-2.4.3/euporie/core/widgets/layout.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/widgets/menu.py` & `euporie-2.4.3/euporie/core/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/widgets/page.py` & `euporie-2.4.3/euporie/core/widgets/page.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/widgets/pager.py` & `euporie-2.4.3/euporie/core/widgets/pager.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/widgets/palette.py` & `euporie-2.4.3/euporie/core/widgets/palette.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/widgets/search_bar.py` & `euporie-2.4.3/euporie/core/widgets/search_bar.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/widgets/status_bar.py` & `euporie-2.4.3/euporie/core/widgets/status_bar.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/core/widgets/tree.py` & `euporie-2.4.3/euporie/core/widgets/tree.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/hub/app.py` & `euporie-2.4.3/euporie/hub/app.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/notebook/app.py` & `euporie-2.4.3/euporie/notebook/app.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/notebook/filters.py` & `euporie-2.4.3/euporie/notebook/filters.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/notebook/tabs/display.py` & `euporie-2.4.3/euporie/notebook/tabs/display.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/notebook/tabs/edit.py` & `euporie-2.4.3/euporie/notebook/tabs/edit.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/notebook/tabs/json.py` & `euporie-2.4.3/euporie/notebook/tabs/json.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/notebook/tabs/log.py` & `euporie-2.4.3/euporie/notebook/tabs/log.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/notebook/tabs/notebook.py` & `euporie-2.4.3/euporie/notebook/tabs/notebook.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/notebook/widgets/side_bar.py` & `euporie-2.4.3/euporie/notebook/widgets/side_bar.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/preview/app.py` & `euporie-2.4.3/euporie/preview/app.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/preview/tabs/notebook.py` & `euporie-2.4.3/euporie/preview/tabs/notebook.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/web/tabs/web.py` & `euporie-2.4.3/euporie/web/tabs/web.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/euporie/web/widgets/webview.py` & `euporie-2.4.3/euporie/web/widgets/webview.py`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/.gitignore` & `euporie-2.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/LICENSE` & `euporie-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/README.rst` & `euporie-2.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/pyproject.toml` & `euporie-2.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `euporie-2.4.2/PKG-INFO` & `euporie-2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: euporie
-Version: 2.4.2
+Version: 2.4.3
 Summary: Euporie is a suite of terminal applications for interacting with Jupyter kernels
 Project-URL: Documentation, https://euporie.readthedocs.io/en/latest
 Project-URL: Issues, https://github.com/joouha/euporie/issues
 Project-URL: Source, https://github.com/joouha/euporie
 Project-URL: Changelog, https://euporie.readthedocs.io/en/latest/pages/changelog.html
 Author-email: Josiah Outram Halstead <josiah@halstead.email>
 License-File: LICENSE
```

