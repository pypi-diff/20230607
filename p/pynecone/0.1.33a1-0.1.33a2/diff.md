# Comparing `tmp/pynecone-0.1.33a1.tar.gz` & `tmp/pynecone-0.1.33a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynecone-0.1.33a1.tar", max compression
+gzip compressed data, was "pynecone-0.1.33a2.tar", max compression
```

## Comparing `pynecone-0.1.33a1.tar` & `pynecone-0.1.33a2.tar`

### file list

```diff
@@ -1,169 +1,171 @@
--rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.33a1/LICENSE
--rw-r--r--   0        0        0     7876 2023-05-18 00:14:14.758659 pynecone-0.1.33a1/README.md
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.33a1/pynecone/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1340 2023-06-03 03:13:15.297910 pynecone-0.1.33a1/pynecone/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.33a1/pynecone/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.33a1/pynecone/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.33a1/pynecone/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      183 2023-05-15 02:04:07.604358 pynecone-0.1.33a1/pynecone/.templates/jinja/app/pcconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-05-15 02:04:07.604515 pynecone-0.1.33a1/pynecone/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-05-18 18:33:16.414872 pynecone-0.1.33a1/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-05-15 02:04:07.604642 pynecone-0.1.33a1/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     2558 2023-06-06 03:55:08.648087 pynecone-0.1.33a1/pynecone/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-05-22 21:40:04.765805 pynecone-0.1.33a1/pynecone/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0       38 2023-05-15 02:04:07.604905 pynecone-0.1.33a1/pynecone/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.33a1/pynecone/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   257247 2023-05-26 18:45:47.401731 pynecone-0.1.33a1/pynecone/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-05-26 18:45:47.402096 pynecone-0.1.33a1/pynecone/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.33a1/pynecone/.templates/web/next.config.js
--rw-r--r--   0        0        0      995 2023-06-01 03:15:26.563786 pynecone-0.1.33a1/pynecone/.templates/web/package.json
--rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.33a1/pynecone/.templates/web/pages/404.js
--rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.33a1/pynecone/.templates/web/pages/_app.js
--rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.33a1/pynecone/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0     8262 2023-06-06 03:55:08.648388 pynecone-0.1.33a1/pynecone/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1448 2023-06-01 03:12:11.084175 pynecone-0.1.33a1/pynecone/__init__.py
--rw-r--r--   0        0        0    20112 2023-06-06 03:56:12.966996 pynecone-0.1.33a1/pynecone/app.py
--rw-r--r--   0        0        0     2524 2023-05-18 00:14:14.759391 pynecone-0.1.33a1/pynecone/base.py
--rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.33a1/pynecone/compiler/__init__.py
--rw-r--r--   0        0        0     6688 2023-06-06 03:55:08.649189 pynecone-0.1.33a1/pynecone/compiler/compiler.py
--rw-r--r--   0        0        0     2565 2023-05-15 02:04:07.607300 pynecone-0.1.33a1/pynecone/compiler/templates.py
--rw-r--r--   0        0        0     7761 2023-06-01 00:32:59.071818 pynecone-0.1.33a1/pynecone/compiler/utils.py
--rw-r--r--   0        0        0     7062 2023-06-06 03:55:08.649644 pynecone-0.1.33a1/pynecone/components/__init__.py
--rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.33a1/pynecone/components/base/__init__.py
--rw-r--r--   0        0        0      727 2023-05-15 02:04:07.607680 pynecone-0.1.33a1/pynecone/components/base/bare.py
--rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.33a1/pynecone/components/base/body.py
--rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.33a1/pynecone/components/base/document.py
--rw-r--r--   0        0        0      265 2023-05-15 02:04:07.607851 pynecone-0.1.33a1/pynecone/components/base/head.py
--rw-r--r--   0        0        0      930 2023-05-15 02:04:07.607989 pynecone-0.1.33a1/pynecone/components/base/link.py
--rw-r--r--   0        0        0     1340 2023-05-15 02:04:07.608303 pynecone-0.1.33a1/pynecone/components/base/meta.py
--rw-r--r--   0        0        0    24243 2023-06-01 00:32:59.072142 pynecone-0.1.33a1/pynecone/components/component.py
--rw-r--r--   0        0        0      496 2023-05-26 18:45:47.404646 pynecone-0.1.33a1/pynecone/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      334 2023-05-15 02:04:07.608726 pynecone-0.1.33a1/pynecone/components/datadisplay/badge.py
--rw-r--r--   0        0        0     2513 2023-05-15 02:04:07.608840 pynecone-0.1.33a1/pynecone/components/datadisplay/code.py
--rw-r--r--   0        0        0     4033 2023-05-15 02:04:07.608953 pynecone-0.1.33a1/pynecone/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      537 2023-05-15 02:04:07.609045 pynecone-0.1.33a1/pynecone/components/datadisplay/divider.py
--rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.33a1/pynecone/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1430 2023-05-15 02:04:07.609140 pynecone-0.1.33a1/pynecone/components/datadisplay/list.py
--rw-r--r--   0        0        0     2157 2023-05-15 02:04:07.609232 pynecone-0.1.33a1/pynecone/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5793 2023-05-26 18:45:47.405454 pynecone-0.1.33a1/pynecone/components/datadisplay/table.py
--rw-r--r--   0        0        0     2188 2023-05-26 18:45:47.406072 pynecone-0.1.33a1/pynecone/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-05-26 18:45:47.406587 pynecone-0.1.33a1/pynecone/components/disclosure/__init__.py
--rw-r--r--   0        0        0     2941 2023-05-15 02:04:07.609439 pynecone-0.1.33a1/pynecone/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2777 2023-05-15 02:04:07.609534 pynecone-0.1.33a1/pynecone/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1741 2023-05-26 18:45:47.406922 pynecone-0.1.33a1/pynecone/components/disclosure/transition.py
--rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.33a1/pynecone/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.33a1/pynecone/components/feedback/__init__.py
--rw-r--r--   0        0        0     1571 2023-05-15 02:04:07.609649 pynecone-0.1.33a1/pynecone/components/feedback/alert.py
--rw-r--r--   0        0        0     1905 2023-05-15 02:04:07.609745 pynecone-0.1.33a1/pynecone/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      879 2023-05-15 02:04:07.609838 pynecone-0.1.33a1/pynecone/components/feedback/progress.py
--rw-r--r--   0        0        0     1785 2023-05-15 02:04:07.609925 pynecone-0.1.33a1/pynecone/components/feedback/skeleton.py
--rw-r--r--   0        0        0      678 2023-05-15 02:04:07.610013 pynecone-0.1.33a1/pynecone/components/feedback/spinner.py
--rw-r--r--   0        0        0     1308 2023-06-06 03:55:08.649928 pynecone-0.1.33a1/pynecone/components/forms/__init__.py
--rw-r--r--   0        0        0     1765 2023-05-15 17:32:17.392510 pynecone-0.1.33a1/pynecone/components/forms/button.py
--rw-r--r--   0        0        0     2454 2023-05-18 00:14:14.760429 pynecone-0.1.33a1/pynecone/components/forms/checkbox.py
--rw-r--r--   0        0        0      578 2023-05-18 00:14:14.760629 pynecone-0.1.33a1/pynecone/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0      243 2023-06-06 03:55:08.650277 pynecone-0.1.33a1/pynecone/components/forms/date_picker.py
--rw-r--r--   0        0        0      277 2023-06-06 03:55:08.650792 pynecone-0.1.33a1/pynecone/components/forms/date_time_picker.py
--rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.760816 pynecone-0.1.33a1/pynecone/components/forms/editable.py
--rw-r--r--   0        0        0      243 2023-06-01 00:48:48.431001 pynecone-0.1.33a1/pynecone/components/forms/email.py
--rw-r--r--   0        0        0     2996 2023-05-26 18:45:47.407573 pynecone-0.1.33a1/pynecone/components/forms/form.py
--rw-r--r--   0        0        0      802 2023-05-15 02:04:07.610729 pynecone-0.1.33a1/pynecone/components/forms/iconbutton.py
--rw-r--r--   0        0        0     2880 2023-05-18 00:14:14.761287 pynecone-0.1.33a1/pynecone/components/forms/input.py
--rw-r--r--   0        0        0    12667 2023-06-03 03:13:18.319215 pynecone-0.1.33a1/pynecone/components/forms/multiselect.py
--rw-r--r--   0        0        0     3897 2023-05-18 00:14:14.761460 pynecone-0.1.33a1/pynecone/components/forms/numberinput.py
--rw-r--r--   0        0        0      253 2023-05-15 02:04:07.611101 pynecone-0.1.33a1/pynecone/components/forms/password.py
--rw-r--r--   0        0        0     2670 2023-05-18 00:14:14.761619 pynecone-0.1.33a1/pynecone/components/forms/pininput.py
--rw-r--r--   0        0        0     3043 2023-05-18 00:14:14.761823 pynecone-0.1.33a1/pynecone/components/forms/radio.py
--rw-r--r--   0        0        0     2853 2023-05-18 00:14:14.761962 pynecone-0.1.33a1/pynecone/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3522 2023-06-03 03:13:18.320175 pynecone-0.1.33a1/pynecone/components/forms/select.py
--rw-r--r--   0        0        0     3124 2023-05-18 00:14:14.762261 pynecone-0.1.33a1/pynecone/components/forms/slider.py
--rw-r--r--   0        0        0     1552 2023-05-18 00:14:14.762398 pynecone-0.1.33a1/pynecone/components/forms/switch.py
--rw-r--r--   0        0        0     1531 2023-05-18 00:14:14.762541 pynecone-0.1.33a1/pynecone/components/forms/textarea.py
--rw-r--r--   0        0        0     2915 2023-05-18 00:14:14.762683 pynecone-0.1.33a1/pynecone/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.33a1/pynecone/components/graphing/__init__.py
--rw-r--r--   0        0        0     1357 2023-05-15 02:04:07.613685 pynecone-0.1.33a1/pynecone/components/graphing/plotly.py
--rw-r--r--   0        0        0    17360 2023-05-15 02:04:07.613960 pynecone-0.1.33a1/pynecone/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-05-22 21:39:53.010163 pynecone-0.1.33a1/pynecone/components/layout/__init__.py
--rw-r--r--   0        0        0      324 2023-05-15 02:04:07.614167 pynecone-0.1.33a1/pynecone/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      769 2023-05-15 02:04:07.614311 pynecone-0.1.33a1/pynecone/components/layout/box.py
--rw-r--r--   0        0        0     2859 2023-05-22 21:39:53.010378 pynecone-0.1.33a1/pynecone/components/layout/card.py
--rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.33a1/pynecone/components/layout/center.py
--rw-r--r--   0        0        0     3844 2023-05-18 00:14:14.762938 pynecone-0.1.33a1/pynecone/components/layout/cond.py
--rw-r--r--   0        0        0      363 2023-05-15 02:04:07.614634 pynecone-0.1.33a1/pynecone/components/layout/container.py
--rw-r--r--   0        0        0      656 2023-05-15 02:04:07.614740 pynecone-0.1.33a1/pynecone/components/layout/flex.py
--rw-r--r--   0        0        0     3167 2023-05-26 18:45:47.408238 pynecone-0.1.33a1/pynecone/components/layout/foreach.py
--rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.33a1/pynecone/components/layout/fragment.py
--rw-r--r--   0        0        0     2418 2023-05-15 02:04:07.614987 pynecone-0.1.33a1/pynecone/components/layout/grid.py
--rw-r--r--   0        0        0      979 2023-05-30 04:03:19.236282 pynecone-0.1.33a1/pynecone/components/layout/html.py
--rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.33a1/pynecone/components/layout/responsive.py
--rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.33a1/pynecone/components/layout/spacer.py
--rw-r--r--   0        0        0      995 2023-05-15 02:04:07.615111 pynecone-0.1.33a1/pynecone/components/layout/stack.py
--rw-r--r--   0        0        0     1471 2023-05-15 02:04:07.615242 pynecone-0.1.33a1/pynecone/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.33a1/pynecone/components/libs/__init__.py
--rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.33a1/pynecone/components/libs/chakra.py
--rw-r--r--   0        0        0     1391 2023-06-01 03:15:26.564372 pynecone-0.1.33a1/pynecone/components/libs/react_player.py
--rw-r--r--   0        0        0      240 2023-06-01 03:15:26.564561 pynecone-0.1.33a1/pynecone/components/media/__init__.py
--rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564687 pynecone-0.1.33a1/pynecone/components/media/audio.py
--rw-r--r--   0        0        0     1524 2023-05-18 00:14:14.763360 pynecone-0.1.33a1/pynecone/components/media/avatar.py
--rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.33a1/pynecone/components/media/icon.py
--rw-r--r--   0        0        0     1774 2023-06-01 03:15:26.564867 pynecone-0.1.33a1/pynecone/components/media/image.py
--rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564984 pynecone-0.1.33a1/pynecone/components/media/video.py
--rw-r--r--   0        0        0      282 2023-06-06 03:55:08.651124 pynecone-0.1.33a1/pynecone/components/navigation/__init__.py
--rw-r--r--   0        0        0     2023 2023-05-15 02:04:07.615856 pynecone-0.1.33a1/pynecone/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0      753 2023-06-06 03:56:12.967444 pynecone-0.1.33a1/pynecone/components/navigation/link.py
--rw-r--r--   0        0        0      530 2023-05-15 02:04:07.616129 pynecone-0.1.33a1/pynecone/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      507 2023-05-15 02:04:07.616229 pynecone-0.1.33a1/pynecone/components/navigation/nextlink.py
--rw-r--r--   0        0        0      887 2023-06-06 03:55:08.651436 pynecone-0.1.33a1/pynecone/components/overlay/__init__.py
--rw-r--r--   0        0        0     5027 2023-05-18 00:14:14.763711 pynecone-0.1.33a1/pynecone/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     1016 2023-06-06 03:55:08.651780 pynecone-0.1.33a1/pynecone/components/overlay/banner.py
--rw-r--r--   0        0        0     4681 2023-05-18 00:14:14.763867 pynecone-0.1.33a1/pynecone/components/overlay/drawer.py
--rw-r--r--   0        0        0     5530 2023-05-18 00:14:14.764021 pynecone-0.1.33a1/pynecone/components/overlay/menu.py
--rw-r--r--   0        0        0     4917 2023-05-18 00:14:14.764177 pynecone-0.1.33a1/pynecone/components/overlay/modal.py
--rw-r--r--   0        0        0     5688 2023-05-18 00:14:14.764341 pynecone-0.1.33a1/pynecone/components/overlay/popover.py
--rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.764530 pynecone-0.1.33a1/pynecone/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.33a1/pynecone/components/tags/__init__.py
--rw-r--r--   0        0        0      451 2023-05-15 02:04:07.617454 pynecone-0.1.33a1/pynecone/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2306 2023-05-15 02:04:07.617560 pynecone-0.1.33a1/pynecone/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5018 2023-05-18 00:14:14.764773 pynecone-0.1.33a1/pynecone/components/tags/tag.py
--rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.33a1/pynecone/components/tags/tagless.py
--rw-r--r--   0        0        0      304 2023-06-01 00:32:59.073257 pynecone-0.1.33a1/pynecone/components/typography/__init__.py
--rw-r--r--   0        0        0      282 2023-05-15 02:04:07.617958 pynecone-0.1.33a1/pynecone/components/typography/heading.py
--rw-r--r--   0        0        0      682 2023-06-01 00:32:59.073664 pynecone-0.1.33a1/pynecone/components/typography/highlight.py
--rw-r--r--   0        0        0     3460 2023-06-03 03:13:18.321195 pynecone-0.1.33a1/pynecone/components/typography/markdown.py
--rw-r--r--   0        0        0      337 2023-05-15 02:04:07.618372 pynecone-0.1.33a1/pynecone/components/typography/span.py
--rw-r--r--   0        0        0      306 2023-05-15 02:04:07.618520 pynecone-0.1.33a1/pynecone/components/typography/text.py
--rw-r--r--   0        0        0     6858 2023-06-06 03:55:08.652315 pynecone-0.1.33a1/pynecone/config.py
--rw-r--r--   0        0        0    10169 2023-06-06 03:55:08.652752 pynecone-0.1.33a1/pynecone/constants.py
--rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.33a1/pynecone/el/__init__.py
--rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.33a1/pynecone/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.33a1/pynecone/el/constants/html.py
--rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.33a1/pynecone/el/constants/pynecone.py
--rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.33a1/pynecone/el/constants/react.py
--rw-r--r--   0        0        0     1320 2023-06-06 03:56:12.968362 pynecone-0.1.33a1/pynecone/el/element.py
--rw-r--r--   0        0        0   108518 2023-05-15 02:04:07.619552 pynecone-0.1.33a1/pynecone/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2667 2023-05-15 02:04:07.619858 pynecone-0.1.33a1/pynecone/el/precompile.py
--rw-r--r--   0        0        0    10977 2023-06-03 03:13:18.321601 pynecone-0.1.33a1/pynecone/event.py
--rw-r--r--   0        0        0      113 2023-05-15 02:04:07.620772 pynecone-0.1.33a1/pynecone/middleware/__init__.py
--rw-r--r--   0        0        0     1738 2023-05-15 02:04:07.621034 pynecone-0.1.33a1/pynecone/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1167 2023-05-15 02:04:07.621188 pynecone-0.1.33a1/pynecone/middleware/middleware.py
--rw-r--r--   0        0        0     2085 2023-06-01 03:12:11.086155 pynecone-0.1.33a1/pynecone/model.py
--rw-r--r--   0        0        0     8431 2023-06-01 03:12:42.958684 pynecone-0.1.33a1/pynecone/pc.py
--rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.33a1/pynecone/py.typed
--rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.33a1/pynecone/route.py
--rw-r--r--   0        0        0    30953 2023-06-06 03:55:08.653419 pynecone-0.1.33a1/pynecone/state.py
--rw-r--r--   0        0        0     1060 2023-05-15 02:04:07.621889 pynecone-0.1.33a1/pynecone/style.py
--rw-r--r--   0        0        0       26 2023-05-15 02:04:07.622076 pynecone-0.1.33a1/pynecone/utils/__init__.py
--rw-r--r--   0        0        0     7451 2023-06-01 03:12:42.959046 pynecone-0.1.33a1/pynecone/utils/build.py
--rw-r--r--   0        0        0     1759 2023-05-15 02:04:07.622587 pynecone-0.1.33a1/pynecone/utils/console.py
--rw-r--r--   0        0        0     5229 2023-06-01 03:12:42.959181 pynecone-0.1.33a1/pynecone/utils/exec.py
--rw-r--r--   0        0        0    11859 2023-06-01 03:15:26.565621 pynecone-0.1.33a1/pynecone/utils/format.py
--rw-r--r--   0        0        0      587 2023-05-15 02:04:07.623144 pynecone-0.1.33a1/pynecone/utils/imports.py
--rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.33a1/pynecone/utils/path_ops.py
--rw-r--r--   0        0        0    10033 2023-05-17 03:31:04.698132 pynecone-0.1.33a1/pynecone/utils/prerequisites.py
--rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.33a1/pynecone/utils/processes.py
--rw-r--r--   0        0        0     2397 2023-05-15 02:04:07.623496 pynecone-0.1.33a1/pynecone/utils/telemetry.py
--rw-r--r--   0        0        0     4806 2023-06-01 03:15:26.565774 pynecone-0.1.33a1/pynecone/utils/types.py
--rw-r--r--   0        0        0     2634 2023-05-15 02:04:07.623722 pynecone-0.1.33a1/pynecone/utils/watch.py
--rw-r--r--   0        0        0    30928 2023-05-18 00:14:14.766310 pynecone-0.1.33a1/pynecone/vars.py
--rw-r--r--   0        0        0     1825 2023-06-06 03:56:37.113710 pynecone-0.1.33a1/pyproject.toml
--rw-r--r--   0        0        0     9462 1970-01-01 00:00:00.000000 pynecone-0.1.33a1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.33a2/LICENSE
+-rw-r--r--   0        0        0     7876 2023-05-18 00:14:14.758659 pynecone-0.1.33a2/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.33a2/pynecone/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1340 2023-06-07 06:32:06.269060 pynecone-0.1.33a2/pynecone/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.33a2/pynecone/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.33a2/pynecone/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.33a2/pynecone/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      183 2023-05-15 02:04:07.604358 pynecone-0.1.33a2/pynecone/.templates/jinja/app/pcconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-05-15 02:04:07.604515 pynecone-0.1.33a2/pynecone/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-05-18 18:33:16.414872 pynecone-0.1.33a2/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-05-15 02:04:07.604642 pynecone-0.1.33a2/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     2554 2023-06-07 06:28:05.215601 pynecone-0.1.33a2/pynecone/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-05-22 21:40:04.765805 pynecone-0.1.33a2/pynecone/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0       38 2023-05-15 02:04:07.604905 pynecone-0.1.33a2/pynecone/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.33a2/pynecone/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   257247 2023-05-26 18:45:47.401731 pynecone-0.1.33a2/pynecone/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-05-26 18:45:47.402096 pynecone-0.1.33a2/pynecone/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.33a2/pynecone/.templates/web/next.config.js
+-rw-r--r--   0        0        0      995 2023-06-01 03:15:26.563786 pynecone-0.1.33a2/pynecone/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.33a2/pynecone/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.33a2/pynecone/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.33a2/pynecone/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0     8480 2023-06-07 06:21:32.940912 pynecone-0.1.33a2/pynecone/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1490 2023-06-07 06:05:03.874348 pynecone-0.1.33a2/pynecone/__init__.py
+-rw-r--r--   0        0        0      320 2023-06-07 06:05:03.874470 pynecone-0.1.33a2/pynecone/admin.py
+-rw-r--r--   0        0        0    21105 2023-06-07 06:21:03.890579 pynecone-0.1.33a2/pynecone/app.py
+-rw-r--r--   0        0        0     2524 2023-05-18 00:14:14.759391 pynecone-0.1.33a2/pynecone/base.py
+-rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.33a2/pynecone/compiler/__init__.py
+-rw-r--r--   0        0        0     6688 2023-06-07 06:05:03.875477 pynecone-0.1.33a2/pynecone/compiler/compiler.py
+-rw-r--r--   0        0        0     2642 2023-06-07 06:26:49.090764 pynecone-0.1.33a2/pynecone/compiler/templates.py
+-rw-r--r--   0        0        0     7761 2023-06-01 00:32:59.071818 pynecone-0.1.33a2/pynecone/compiler/utils.py
+-rw-r--r--   0        0        0     7346 2023-06-07 06:05:03.875765 pynecone-0.1.33a2/pynecone/components/__init__.py
+-rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.33a2/pynecone/components/base/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-15 02:04:07.607680 pynecone-0.1.33a2/pynecone/components/base/bare.py
+-rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.33a2/pynecone/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.33a2/pynecone/components/base/document.py
+-rw-r--r--   0        0        0      265 2023-05-15 02:04:07.607851 pynecone-0.1.33a2/pynecone/components/base/head.py
+-rw-r--r--   0        0        0      930 2023-05-15 02:04:07.607989 pynecone-0.1.33a2/pynecone/components/base/link.py
+-rw-r--r--   0        0        0     1340 2023-05-15 02:04:07.608303 pynecone-0.1.33a2/pynecone/components/base/meta.py
+-rw-r--r--   0        0        0    24243 2023-06-01 00:32:59.072142 pynecone-0.1.33a2/pynecone/components/component.py
+-rw-r--r--   0        0        0      496 2023-05-26 18:45:47.404646 pynecone-0.1.33a2/pynecone/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      334 2023-05-15 02:04:07.608726 pynecone-0.1.33a2/pynecone/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     2513 2023-05-15 02:04:07.608840 pynecone-0.1.33a2/pynecone/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4033 2023-05-15 02:04:07.608953 pynecone-0.1.33a2/pynecone/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      537 2023-05-15 02:04:07.609045 pynecone-0.1.33a2/pynecone/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.33a2/pynecone/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1430 2023-05-15 02:04:07.609140 pynecone-0.1.33a2/pynecone/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2157 2023-05-15 02:04:07.609232 pynecone-0.1.33a2/pynecone/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5793 2023-05-26 18:45:47.405454 pynecone-0.1.33a2/pynecone/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2188 2023-05-26 18:45:47.406072 pynecone-0.1.33a2/pynecone/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-05-26 18:45:47.406587 pynecone-0.1.33a2/pynecone/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     2941 2023-05-15 02:04:07.609439 pynecone-0.1.33a2/pynecone/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2777 2023-05-15 02:04:07.609534 pynecone-0.1.33a2/pynecone/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1741 2023-05-26 18:45:47.406922 pynecone-0.1.33a2/pynecone/components/disclosure/transition.py
+-rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.33a2/pynecone/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.33a2/pynecone/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1571 2023-05-15 02:04:07.609649 pynecone-0.1.33a2/pynecone/components/feedback/alert.py
+-rw-r--r--   0        0        0     1905 2023-05-15 02:04:07.609745 pynecone-0.1.33a2/pynecone/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      879 2023-05-15 02:04:07.609838 pynecone-0.1.33a2/pynecone/components/feedback/progress.py
+-rw-r--r--   0        0        0     1785 2023-05-15 02:04:07.609925 pynecone-0.1.33a2/pynecone/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      678 2023-05-15 02:04:07.610013 pynecone-0.1.33a2/pynecone/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1308 2023-06-07 06:05:03.876023 pynecone-0.1.33a2/pynecone/components/forms/__init__.py
+-rw-r--r--   0        0        0     1765 2023-05-15 17:32:17.392510 pynecone-0.1.33a2/pynecone/components/forms/button.py
+-rw-r--r--   0        0        0     2454 2023-05-18 00:14:14.760429 pynecone-0.1.33a2/pynecone/components/forms/checkbox.py
+-rw-r--r--   0        0        0      578 2023-05-18 00:14:14.760629 pynecone-0.1.33a2/pynecone/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      243 2023-06-07 06:05:03.876332 pynecone-0.1.33a2/pynecone/components/forms/date_picker.py
+-rw-r--r--   0        0        0      277 2023-06-07 06:05:03.876514 pynecone-0.1.33a2/pynecone/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.760816 pynecone-0.1.33a2/pynecone/components/forms/editable.py
+-rw-r--r--   0        0        0      243 2023-06-01 00:48:48.431001 pynecone-0.1.33a2/pynecone/components/forms/email.py
+-rw-r--r--   0        0        0     2996 2023-05-26 18:45:47.407573 pynecone-0.1.33a2/pynecone/components/forms/form.py
+-rw-r--r--   0        0        0      802 2023-05-15 02:04:07.610729 pynecone-0.1.33a2/pynecone/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     2880 2023-05-18 00:14:14.761287 pynecone-0.1.33a2/pynecone/components/forms/input.py
+-rw-r--r--   0        0        0    12667 2023-06-07 06:05:03.876768 pynecone-0.1.33a2/pynecone/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3897 2023-05-18 00:14:14.761460 pynecone-0.1.33a2/pynecone/components/forms/numberinput.py
+-rw-r--r--   0        0        0      253 2023-05-15 02:04:07.611101 pynecone-0.1.33a2/pynecone/components/forms/password.py
+-rw-r--r--   0        0        0     2670 2023-05-18 00:14:14.761619 pynecone-0.1.33a2/pynecone/components/forms/pininput.py
+-rw-r--r--   0        0        0     3043 2023-05-18 00:14:14.761823 pynecone-0.1.33a2/pynecone/components/forms/radio.py
+-rw-r--r--   0        0        0     2853 2023-05-18 00:14:14.761962 pynecone-0.1.33a2/pynecone/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3522 2023-06-07 06:05:03.877157 pynecone-0.1.33a2/pynecone/components/forms/select.py
+-rw-r--r--   0        0        0     3124 2023-05-18 00:14:14.762261 pynecone-0.1.33a2/pynecone/components/forms/slider.py
+-rw-r--r--   0        0        0     1552 2023-05-18 00:14:14.762398 pynecone-0.1.33a2/pynecone/components/forms/switch.py
+-rw-r--r--   0        0        0     1531 2023-05-18 00:14:14.762541 pynecone-0.1.33a2/pynecone/components/forms/textarea.py
+-rw-r--r--   0        0        0     2915 2023-05-18 00:14:14.762683 pynecone-0.1.33a2/pynecone/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.33a2/pynecone/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1357 2023-05-15 02:04:07.613685 pynecone-0.1.33a2/pynecone/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17360 2023-05-15 02:04:07.613960 pynecone-0.1.33a2/pynecone/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-05-22 21:39:53.010163 pynecone-0.1.33a2/pynecone/components/layout/__init__.py
+-rw-r--r--   0        0        0      324 2023-05-15 02:04:07.614167 pynecone-0.1.33a2/pynecone/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      769 2023-05-15 02:04:07.614311 pynecone-0.1.33a2/pynecone/components/layout/box.py
+-rw-r--r--   0        0        0     2859 2023-05-22 21:39:53.010378 pynecone-0.1.33a2/pynecone/components/layout/card.py
+-rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.33a2/pynecone/components/layout/center.py
+-rw-r--r--   0        0        0     3844 2023-05-18 00:14:14.762938 pynecone-0.1.33a2/pynecone/components/layout/cond.py
+-rw-r--r--   0        0        0      363 2023-05-15 02:04:07.614634 pynecone-0.1.33a2/pynecone/components/layout/container.py
+-rw-r--r--   0        0        0      656 2023-05-15 02:04:07.614740 pynecone-0.1.33a2/pynecone/components/layout/flex.py
+-rw-r--r--   0        0        0     3167 2023-05-26 18:45:47.408238 pynecone-0.1.33a2/pynecone/components/layout/foreach.py
+-rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.33a2/pynecone/components/layout/fragment.py
+-rw-r--r--   0        0        0     2418 2023-05-15 02:04:07.614987 pynecone-0.1.33a2/pynecone/components/layout/grid.py
+-rw-r--r--   0        0        0      979 2023-05-30 04:03:19.236282 pynecone-0.1.33a2/pynecone/components/layout/html.py
+-rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.33a2/pynecone/components/layout/responsive.py
+-rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.33a2/pynecone/components/layout/spacer.py
+-rw-r--r--   0        0        0      995 2023-05-15 02:04:07.615111 pynecone-0.1.33a2/pynecone/components/layout/stack.py
+-rw-r--r--   0        0        0     1471 2023-05-15 02:04:07.615242 pynecone-0.1.33a2/pynecone/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.33a2/pynecone/components/libs/__init__.py
+-rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.33a2/pynecone/components/libs/chakra.py
+-rw-r--r--   0        0        0     1391 2023-06-01 03:15:26.564372 pynecone-0.1.33a2/pynecone/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-06-01 03:15:26.564561 pynecone-0.1.33a2/pynecone/components/media/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564687 pynecone-0.1.33a2/pynecone/components/media/audio.py
+-rw-r--r--   0        0        0     1524 2023-05-18 00:14:14.763360 pynecone-0.1.33a2/pynecone/components/media/avatar.py
+-rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.33a2/pynecone/components/media/icon.py
+-rw-r--r--   0        0        0     1774 2023-06-01 03:15:26.564867 pynecone-0.1.33a2/pynecone/components/media/image.py
+-rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564984 pynecone-0.1.33a2/pynecone/components/media/video.py
+-rw-r--r--   0        0        0      450 2023-06-07 06:05:03.877519 pynecone-0.1.33a2/pynecone/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2023 2023-05-15 02:04:07.615856 pynecone-0.1.33a2/pynecone/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0      746 2023-06-07 06:05:03.877899 pynecone-0.1.33a2/pynecone/components/navigation/link.py
+-rw-r--r--   0        0        0      530 2023-05-15 02:04:07.616129 pynecone-0.1.33a2/pynecone/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      507 2023-05-15 02:04:07.616229 pynecone-0.1.33a2/pynecone/components/navigation/nextlink.py
+-rw-r--r--   0        0        0     2842 2023-06-07 06:05:03.878280 pynecone-0.1.33a2/pynecone/components/navigation/stepper.py
+-rw-r--r--   0        0        0      887 2023-06-07 06:05:03.878625 pynecone-0.1.33a2/pynecone/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5027 2023-05-18 00:14:14.763711 pynecone-0.1.33a2/pynecone/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1016 2023-06-07 06:05:03.878806 pynecone-0.1.33a2/pynecone/components/overlay/banner.py
+-rw-r--r--   0        0        0     4681 2023-05-18 00:14:14.763867 pynecone-0.1.33a2/pynecone/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5530 2023-05-18 00:14:14.764021 pynecone-0.1.33a2/pynecone/components/overlay/menu.py
+-rw-r--r--   0        0        0     4917 2023-05-18 00:14:14.764177 pynecone-0.1.33a2/pynecone/components/overlay/modal.py
+-rw-r--r--   0        0        0     5688 2023-06-07 04:31:19.747990 pynecone-0.1.33a2/pynecone/components/overlay/popover.py
+-rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.764530 pynecone-0.1.33a2/pynecone/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.33a2/pynecone/components/tags/__init__.py
+-rw-r--r--   0        0        0      451 2023-05-15 02:04:07.617454 pynecone-0.1.33a2/pynecone/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2306 2023-05-15 02:04:07.617560 pynecone-0.1.33a2/pynecone/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5018 2023-05-18 00:14:14.764773 pynecone-0.1.33a2/pynecone/components/tags/tag.py
+-rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.33a2/pynecone/components/tags/tagless.py
+-rw-r--r--   0        0        0      304 2023-06-01 00:32:59.073257 pynecone-0.1.33a2/pynecone/components/typography/__init__.py
+-rw-r--r--   0        0        0      282 2023-05-15 02:04:07.617958 pynecone-0.1.33a2/pynecone/components/typography/heading.py
+-rw-r--r--   0        0        0      682 2023-06-01 00:32:59.073664 pynecone-0.1.33a2/pynecone/components/typography/highlight.py
+-rw-r--r--   0        0        0     3460 2023-06-07 06:05:03.879093 pynecone-0.1.33a2/pynecone/components/typography/markdown.py
+-rw-r--r--   0        0        0      337 2023-05-15 02:04:07.618372 pynecone-0.1.33a2/pynecone/components/typography/span.py
+-rw-r--r--   0        0        0      306 2023-05-15 02:04:07.618520 pynecone-0.1.33a2/pynecone/components/typography/text.py
+-rw-r--r--   0        0        0     7021 2023-06-07 06:05:03.879346 pynecone-0.1.33a2/pynecone/config.py
+-rw-r--r--   0        0        0    10219 2023-06-07 06:21:32.941182 pynecone-0.1.33a2/pynecone/constants.py
+-rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.33a2/pynecone/el/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.33a2/pynecone/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.33a2/pynecone/el/constants/html.py
+-rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.33a2/pynecone/el/constants/pynecone.py
+-rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.33a2/pynecone/el/constants/react.py
+-rw-r--r--   0        0        0     1320 2023-06-07 06:05:03.879903 pynecone-0.1.33a2/pynecone/el/element.py
+-rw-r--r--   0        0        0   108518 2023-05-15 02:04:07.619552 pynecone-0.1.33a2/pynecone/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2667 2023-05-15 02:04:07.619858 pynecone-0.1.33a2/pynecone/el/precompile.py
+-rw-r--r--   0        0        0    10977 2023-06-07 06:05:03.880324 pynecone-0.1.33a2/pynecone/event.py
+-rw-r--r--   0        0        0      113 2023-05-15 02:04:07.620772 pynecone-0.1.33a2/pynecone/middleware/__init__.py
+-rw-r--r--   0        0        0     1738 2023-05-15 02:04:07.621034 pynecone-0.1.33a2/pynecone/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1167 2023-05-15 02:04:07.621188 pynecone-0.1.33a2/pynecone/middleware/middleware.py
+-rw-r--r--   0        0        0     2581 2023-06-07 06:05:03.880790 pynecone-0.1.33a2/pynecone/model.py
+-rw-r--r--   0        0        0     8515 2023-06-07 06:05:03.881000 pynecone-0.1.33a2/pynecone/pc.py
+-rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.33a2/pynecone/py.typed
+-rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.33a2/pynecone/route.py
+-rw-r--r--   0        0        0    30945 2023-06-07 06:21:32.941558 pynecone-0.1.33a2/pynecone/state.py
+-rw-r--r--   0        0        0     1060 2023-05-15 02:04:07.621889 pynecone-0.1.33a2/pynecone/style.py
+-rw-r--r--   0        0        0       26 2023-05-15 02:04:07.622076 pynecone-0.1.33a2/pynecone/utils/__init__.py
+-rw-r--r--   0        0        0     7394 2023-06-07 06:21:13.591977 pynecone-0.1.33a2/pynecone/utils/build.py
+-rw-r--r--   0        0        0     1759 2023-05-15 02:04:07.622587 pynecone-0.1.33a2/pynecone/utils/console.py
+-rw-r--r--   0        0        0     5229 2023-06-01 03:12:42.959181 pynecone-0.1.33a2/pynecone/utils/exec.py
+-rw-r--r--   0        0        0    11859 2023-06-01 03:15:26.565621 pynecone-0.1.33a2/pynecone/utils/format.py
+-rw-r--r--   0        0        0      587 2023-05-15 02:04:07.623144 pynecone-0.1.33a2/pynecone/utils/imports.py
+-rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.33a2/pynecone/utils/path_ops.py
+-rw-r--r--   0        0        0    11355 2023-06-07 06:05:03.882688 pynecone-0.1.33a2/pynecone/utils/prerequisites.py
+-rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.33a2/pynecone/utils/processes.py
+-rw-r--r--   0        0        0     2397 2023-05-15 02:04:07.623496 pynecone-0.1.33a2/pynecone/utils/telemetry.py
+-rw-r--r--   0        0        0     4806 2023-06-01 03:15:26.565774 pynecone-0.1.33a2/pynecone/utils/types.py
+-rw-r--r--   0        0        0     2634 2023-05-15 02:04:07.623722 pynecone-0.1.33a2/pynecone/utils/watch.py
+-rw-r--r--   0        0        0    30928 2023-05-18 00:14:14.766310 pynecone-0.1.33a2/pynecone/vars.py
+-rw-r--r--   0        0        0     1852 2023-06-07 06:37:30.531853 pynecone-0.1.33a2/pyproject.toml
+-rw-r--r--   0        0        0     9511 1970-01-01 00:00:00.000000 pynecone-0.1.33a2/PKG-INFO
```

### Comparing `pynecone-0.1.33a1/LICENSE` & `pynecone-0.1.33a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/README.md` & `pynecone-0.1.33a2/README.md`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/.templates/apps/counter/counter.py` & `pynecone-0.1.33a2/pynecone/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/.templates/apps/default/default.py` & `pynecone-0.1.33a2/pynecone/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/.templates/assets/favicon.ico` & `pynecone-0.1.33a2/pynecone/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/.templates/jinja/web/pages/index.js.jinja2` & `pynecone-0.1.33a2/pynecone/.templates/jinja/web/pages/index.js.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
           ...{{const.result}}.{{const.state}},
           events: [...{{state_name}}.{{const.events}}, ...{{const.result}}.{{const.events}}],
         })
 
         {{const.result|react_setter}}({
           {{const.state}}: null,
           {{const.events}}: [],
-          {{const.processing}}: {{const.result}}.{{const.processing}},
+          {{const.processing}}: !{{const.result}}.{{const.final}},
         })
       }
 
       await updateState({{state_name}}, {{state_name|react_setter}}, {{const.result}}, {{const.result|react_setter}}, {{const.router}}, {{const.socket}}.current)
     }
     if (focusRef.current)
       focusRef.current.focus();
```

### Comparing `pynecone-0.1.33a1/pynecone/.templates/jinja/web/pages/utils.js.jinja2` & `pynecone-0.1.33a2/pynecone/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/.templates/web/bun.lockb` & `pynecone-0.1.33a2/pynecone/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/.templates/web/package.json` & `pynecone-0.1.33a2/pynecone/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/.templates/web/pages/_app.js` & `pynecone-0.1.33a2/pynecone/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/.templates/web/styles/code/prism.js` & `pynecone-0.1.33a2/pynecone/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/.templates/web/utils/state.js` & `pynecone-0.1.33a2/pynecone/.templates/web/utils/state.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,18 @@
 // State management for Pynecone web apps.
 import axios from "axios";
 import io from "socket.io-client";
 import JSON5 from "json5";
 import env from "env.json";
 
+// Endpoint URLs.
 const PINGURL = env.pingUrl
 const EVENTURL = env.eventUrl
 const UPLOADURL = env.uploadUrl
+
 // Global variable to hold the token.
 let token;
 
 // Key for the token in the session storage.
 const TOKEN_KEY = "token";
 
 // Dictionary holding component references.
@@ -126,21 +128,30 @@
     }
 
     return false;
 };
 
 /**
  * Process an event off the event queue.
- * @param queue_event The current event
+ * @param event The current event
  * @param state The state with the event queue.
  * @param setResult The function to set the result.
  */
-export const applyRestEvent = async (queue_event, state, setResult) => {
-    if (queue_event.handler == "uploadFiles") {
-        await uploadFiles(state, setResult, queue_event.name);
+export const applyRestEvent = async (event, state, setResult) => {
+    let eventSent = false;
+    if (event.handler == "uploadFiles") {
+        eventSent = await uploadFiles(state, setResult, event.name);
+    }
+    if (!eventSent) {
+        // If no event was sent, set processing to false and return.
+        setResult({
+            ...state,
+            final: true,
+            processing: false
+        });
     }
 };
 
 /**
  * Process an event off the event queue.
  * @param state The state with the event queue.
  * @param setState The function to set the state.
@@ -165,30 +176,31 @@
     // Set processing to true to block other events from being processed.
     setResult({
         ...result,
         processing: true
     });
 
     // Pop the next event off the queue and apply it.
-    const queue_event = state.events.shift();
+    const event = state.events.shift();
     // Set new events to avoid reprocessing the same event.
     setState({
         ...state,
         events: state.events
     });
 
     // Process events with handlers via REST and all others via websockets.
-    if (queue_event.handler) {
-        await applyRestEvent(queue_event, state, setResult);
+    if (event.handler) {
+        await applyRestEvent(event, state, setResult);
     } else {
-        const eventSent = await applyEvent(queue_event, router, socket);
+        const eventSent = await applyEvent(event, router, socket);
         if (!eventSent) {
             // If no event was sent, set processing to false and return.
             setResult({
                 ...state,
+                final: true,
                 processing: false
             });
         }
     }
 };
 
 /**
@@ -208,18 +220,18 @@
     result,
     setResult,
     router,
     transports,
     setNotConnected
 ) => {
     // Get backend URL object from the endpoint
-    const endpoint_url = new URL(EVENTURL);
+    const endpoint = new URL(EVENTURL);
     // Create the socket.
     socket.current = io(EVENTURL, {
-        path: endpoint_url["pathname"],
+        path: endpoint["pathname"],
         transports: transports,
         autoUnref: false,
     });
 
     // Once the socket is open, hydrate the page.
     socket.current.on("connect", () => {
         updateState(state, setState, result, setResult, router, socket.current);
@@ -231,17 +243,18 @@
     });
 
     // On each received message, apply the delta and set the result.
     socket.current.on("event", function(update) {
         update = JSON5.parse(update);
         applyDelta(state, update.delta);
         setResult({
-            processing: update.processing,
             state: state,
             events: update.events,
+            final: update.final,
+            processing: true,
         });
     });
 };
 
 /**
  * Upload files to the server.
  *
@@ -251,15 +264,15 @@
  * @param endpoint The endpoint to upload to.
  */
 export const uploadFiles = async (state, setResult, handler) => {
     const files = state.files;
 
     // return if there's no file to upload
     if (files.length == 0) {
-        return;
+        return false;
     }
 
     const headers = {
         "Content-Type": files[0].type,
     };
     const formdata = new FormData();
 
@@ -276,19 +289,22 @@
     await axios.post(UPLOADURL, formdata, headers).then((response) => {
         // Apply the delta and set the result.
         const update = response.data;
         applyDelta(state, update.delta);
 
         // Set processing to false and return.
         setResult({
-            processing: false,
             state: state,
             events: update.events,
+            final: true,
+            processing: false,
         });
     });
+
+    return true;
 };
 
 /**
  * Create an event object.
  * @param name The name of the event.
  * @param payload The payload of the event.
  * @param use_websocket Whether the event uses websocket.
```

### Comparing `pynecone-0.1.33a1/pynecone/__init__.py` & `pynecone-0.1.33a2/pynecone/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 Anything imported here will be available in the default Pynecone import as `pc.*`.
 To signal to typecheckers that something should be reexported, 
 we use the Flask "import name as name" syntax.
 """
 
 from . import el as el
+from .admin import AdminDash as AdminDash
 from .app import App as App
 from .app import UploadFile as UploadFile
 from .base import Base as Base
 from .compiler.utils import get_asset_path
 from .components import *
 from .components.component import custom_component as memo
 from .components.graphing.victory import data as data
```

### Comparing `pynecone-0.1.33a1/pynecone/app.py` & `pynecone-0.1.33a2/pynecone/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,19 @@
     Type,
     Union,
 )
 
 from fastapi import FastAPI, UploadFile
 from fastapi.middleware import cors
 from socketio import ASGIApp, AsyncNamespace, AsyncServer
+from starlette_admin.contrib.sqla.admin import Admin
+from starlette_admin.contrib.sqla.view import ModelView
 
 from pynecone import constants
+from pynecone.admin import AdminDash
 from pynecone.base import Base
 from pynecone.compiler import compiler
 from pynecone.compiler import utils as compiler_utils
 from pynecone.components.component import Component, ComponentStyle
 from pynecone.config import get_config
 from pynecone.event import Event, EventHandler
 from pynecone.middleware import HydrateMiddleware, Middleware
@@ -72,14 +75,17 @@
 
     # Middleware to add to the app.
     middleware: List[Middleware] = []
 
     # List of event handlers to trigger when a page loads.
     load_events: Dict[str, List[EventHandler]] = {}
 
+    # Admin dashboard
+    admin_dash: Optional[AdminDash] = None
+
     # The component to render if there is a connection error to the server.
     connect_error_component: Optional[Component] = None
 
     def __init__(self, *args, **kwargs):
         """Initialize the app.
 
         Args:
@@ -122,14 +128,17 @@
 
         # Register the event namespace with the socket.
         self.sio.register_namespace(event_namespace)
 
         # Mount the socket app with the API.
         self.api.mount(str(constants.Endpoint.EVENT), self.socket_app)
 
+        # Set up the admin dash.
+        self.setup_admin_dash()
+
     def __repr__(self) -> str:
         """Get the string representation of the app.
 
         Returns:
             The string representation of the app.
         """
         return f"<App state={self.state.__name__}>"
@@ -385,14 +394,33 @@
         ):
             self.pages[froute(constants.ROOT_404)] = component
         if not any(
             page.startswith("[...") or page.startswith("[[...") for page in self.pages
         ):
             self.pages[froute(constants.SLUG_404)] = component
 
+    def setup_admin_dash(self):
+        """Setup the admin dash."""
+        # Get the config.
+        config = get_config()
+        if config.enable_admin and config.admin_dash and config.admin_dash.models:
+            # Build the admin dashboard
+            admin = (
+                config.admin_dash.admin
+                if config.admin_dash.admin
+                else Admin(
+                    engine=Model.get_db_engine(),
+                    title="Pynecone Admin Dashboard",
+                    logo_url="https://pynecone.io/logo.png",
+                )
+            )
+            for model in config.admin_dash.models:
+                admin.add_view(ModelView(model))
+            admin.mount_to(self.api)
+
     def compile(self):
         """Compile the app and output it to the pages folder."""
         for render, kwargs in DECORATED_ROUTES:
             self.add_page(render, **kwargs)
 
         # Get the env mode.
         config = get_config()
```

### Comparing `pynecone-0.1.33a1/pynecone/base.py` & `pynecone-0.1.33a2/pynecone/base.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/compiler/compiler.py` & `pynecone-0.1.33a2/pynecone/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/compiler/templates.py` & `pynecone-0.1.33a2/pynecone/compiler/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,20 @@
         self.globals["const"] = {
             "socket": constants.SOCKET,
             "result": constants.RESULT,
             "router": constants.ROUTER,
             "event_endpoint": constants.Endpoint.EVENT.name,
             "events": constants.EVENTS,
             "state": constants.STATE,
+            "final": constants.FINAL,
             "processing": constants.PROCESSING,
             "initial_result": {
                 constants.STATE: None,
                 constants.EVENTS: [],
+                constants.FINAL: True,
                 constants.PROCESSING: False,
             },
             "color_mode": constants.COLOR_MODE,
             "toggle_color_mode": constants.TOGGLE_COLOR_MODE,
             "use_color_mode": constants.USE_COLOR_MODE,
             "hydrate": constants.HYDRATE,
             "db_url": constants.DB_URL,
```

### Comparing `pynecone-0.1.33a1/pynecone/compiler/utils.py` & `pynecone-0.1.33a2/pynecone/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/__init__.py` & `pynecone-0.1.33a2/pynecone/components/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,14 +179,23 @@
 breadcrumb_item = BreadcrumbItem.create
 breadcrumb_link = BreadcrumbLink.create
 breadcrumb_separator = BreadcrumbSeparator.create
 link = Link.create
 link_box = LinkBox.create
 link_overlay = LinkOverlay.create
 next_link = NextLink.create
+step = Step.create
+step_description = StepDescription.create
+step_icon = StepIcon.create
+step_indicator = StepIndicator.create
+step_number = StepNumber.create
+step_separator = StepSeparator.create
+step_status = StepStatus.create
+step_title = StepTitle.create
+stepper = Stepper.create
 alert_dialog = AlertDialog.create
 alert_dialog_body = AlertDialogBody.create
 alert_dialog_content = AlertDialogContent.create
 alert_dialog_footer = AlertDialogFooter.create
 alert_dialog_header = AlertDialogHeader.create
 alert_dialog_overlay = AlertDialogOverlay.create
 drawer = Drawer.create
```

### Comparing `pynecone-0.1.33a1/pynecone/components/base/bare.py` & `pynecone-0.1.33a2/pynecone/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/base/document.py` & `pynecone-0.1.33a2/pynecone/components/base/document.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/base/link.py` & `pynecone-0.1.33a2/pynecone/components/base/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/base/meta.py` & `pynecone-0.1.33a2/pynecone/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/component.py` & `pynecone-0.1.33a2/pynecone/components/component.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/datadisplay/code.py` & `pynecone-0.1.33a2/pynecone/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/datadisplay/datatable.py` & `pynecone-0.1.33a2/pynecone/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/datadisplay/divider.py` & `pynecone-0.1.33a2/pynecone/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/datadisplay/list.py` & `pynecone-0.1.33a2/pynecone/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/datadisplay/stat.py` & `pynecone-0.1.33a2/pynecone/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/datadisplay/table.py` & `pynecone-0.1.33a2/pynecone/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/datadisplay/tag.py` & `pynecone-0.1.33a2/pynecone/components/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/disclosure/accordion.py` & `pynecone-0.1.33a2/pynecone/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/disclosure/tabs.py` & `pynecone-0.1.33a2/pynecone/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/disclosure/transition.py` & `pynecone-0.1.33a2/pynecone/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/feedback/alert.py` & `pynecone-0.1.33a2/pynecone/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/feedback/circularprogress.py` & `pynecone-0.1.33a2/pynecone/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/feedback/progress.py` & `pynecone-0.1.33a2/pynecone/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/feedback/skeleton.py` & `pynecone-0.1.33a2/pynecone/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/feedback/spinner.py` & `pynecone-0.1.33a2/pynecone/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/__init__.py` & `pynecone-0.1.33a2/pynecone/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/button.py` & `pynecone-0.1.33a2/pynecone/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/checkbox.py` & `pynecone-0.1.33a2/pynecone/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/copytoclipboard.py` & `pynecone-0.1.33a2/pynecone/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/editable.py` & `pynecone-0.1.33a2/pynecone/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/form.py` & `pynecone-0.1.33a2/pynecone/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/iconbutton.py` & `pynecone-0.1.33a2/pynecone/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/input.py` & `pynecone-0.1.33a2/pynecone/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/multiselect.py` & `pynecone-0.1.33a2/pynecone/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/numberinput.py` & `pynecone-0.1.33a2/pynecone/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/pininput.py` & `pynecone-0.1.33a2/pynecone/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/radio.py` & `pynecone-0.1.33a2/pynecone/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/rangeslider.py` & `pynecone-0.1.33a2/pynecone/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/select.py` & `pynecone-0.1.33a2/pynecone/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/slider.py` & `pynecone-0.1.33a2/pynecone/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/switch.py` & `pynecone-0.1.33a2/pynecone/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/textarea.py` & `pynecone-0.1.33a2/pynecone/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/forms/upload.py` & `pynecone-0.1.33a2/pynecone/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/graphing/plotly.py` & `pynecone-0.1.33a2/pynecone/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/graphing/victory.py` & `pynecone-0.1.33a2/pynecone/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/layout/__init__.py` & `pynecone-0.1.33a2/pynecone/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/layout/box.py` & `pynecone-0.1.33a2/pynecone/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/layout/card.py` & `pynecone-0.1.33a2/pynecone/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/layout/cond.py` & `pynecone-0.1.33a2/pynecone/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/layout/flex.py` & `pynecone-0.1.33a2/pynecone/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/layout/foreach.py` & `pynecone-0.1.33a2/pynecone/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/layout/grid.py` & `pynecone-0.1.33a2/pynecone/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/layout/html.py` & `pynecone-0.1.33a2/pynecone/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/layout/responsive.py` & `pynecone-0.1.33a2/pynecone/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/layout/stack.py` & `pynecone-0.1.33a2/pynecone/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/layout/wrap.py` & `pynecone-0.1.33a2/pynecone/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/libs/react_player.py` & `pynecone-0.1.33a2/pynecone/components/libs/react_player.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/media/avatar.py` & `pynecone-0.1.33a2/pynecone/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/media/icon.py` & `pynecone-0.1.33a2/pynecone/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/media/image.py` & `pynecone-0.1.33a2/pynecone/components/media/image.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/navigation/breadcrumb.py` & `pynecone-0.1.33a2/pynecone/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/navigation/link.py` & `pynecone-0.1.33a2/pynecone/components/navigation/link.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,8 +23,8 @@
     # What the link renders to.
     as_: Var[str] = BaseVar.create("{NextLink}", is_local=False)  # type: ignore
 
     # If true, the link will open in new tab.
     is_external: Var[bool]
 
     def _get_imports(self) -> imports.ImportDict:
-        return {**super()._get_imports(), **NextLink(href=self.href)._get_imports()}
+        return {**super()._get_imports(), **NextLink.create()._get_imports()}
```

### Comparing `pynecone-0.1.33a1/pynecone/components/navigation/linkoverlay.py` & `pynecone-0.1.33a2/pynecone/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/overlay/__init__.py` & `pynecone-0.1.33a2/pynecone/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/overlay/alertdialog.py` & `pynecone-0.1.33a2/pynecone/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/overlay/banner.py` & `pynecone-0.1.33a2/pynecone/components/overlay/banner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/overlay/drawer.py` & `pynecone-0.1.33a2/pynecone/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/overlay/menu.py` & `pynecone-0.1.33a2/pynecone/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/overlay/modal.py` & `pynecone-0.1.33a2/pynecone/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/overlay/popover.py` & `pynecone-0.1.33a2/pynecone/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/overlay/tooltip.py` & `pynecone-0.1.33a2/pynecone/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/tags/iter_tag.py` & `pynecone-0.1.33a2/pynecone/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/tags/tag.py` & `pynecone-0.1.33a2/pynecone/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/tags/tagless.py` & `pynecone-0.1.33a2/pynecone/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/typography/highlight.py` & `pynecone-0.1.33a2/pynecone/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/components/typography/markdown.py` & `pynecone-0.1.33a2/pynecone/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/config.py` & `pynecone-0.1.33a2/pynecone/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import sys
 import urllib.parse
 from typing import List, Optional
 
 from dotenv import load_dotenv
 
 from pynecone import constants
+from pynecone.admin import AdminDash
 from pynecone.base import Base
 
 
 class DBConfig(Base):
     """Database config."""
 
     engine: str
@@ -169,14 +170,20 @@
 
     # Disable bun.
     disable_bun: bool = False
 
     # Additional frontend packages to install.
     frontend_packages: List[str] = []
 
+    # Enable the admin dash.
+    enable_admin: bool = False
+
+    # The Admin Dash
+    admin_dash: Optional[AdminDash] = None
+
     # Backend transport methods.
     backend_transports: Optional[
         constants.Transports
     ] = constants.Transports.WEBSOCKET_POLLING
 
     # List of origins that are allowed to connect to the backend API.
     cors_allowed_origins: Optional[list] = constants.CORS_ALLOWED_ORIGINS
```

### Comparing `pynecone-0.1.33a1/pynecone/constants.py` & `pynecone-0.1.33a2/pynecone/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,16 @@
 API_VAR = "api"
 # The name of the router variable.
 ROUTER = "router"
 # The name of the socket variable.
 SOCKET = "socket"
 # The name of the variable to hold API results.
 RESULT = "result"
+# The name of the final variable.
+FINAL = "final"
 # The name of the process variable.
 PROCESSING = "processing"
 # The name of the state variable.
 STATE = "state"
 # The name of the events variable.
 EVENTS = "events"
 # The name of the initial hydrate event.
```

### Comparing `pynecone-0.1.33a1/pynecone/el/constants/html.py` & `pynecone-0.1.33a2/pynecone/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/el/constants/pynecone.py` & `pynecone-0.1.33a2/pynecone/el/constants/pynecone.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/el/constants/react.py` & `pynecone-0.1.33a2/pynecone/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/el/element.py` & `pynecone-0.1.33a2/pynecone/el/element.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/el/elements/__init__.py` & `pynecone-0.1.33a2/pynecone/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/el/precompile.py` & `pynecone-0.1.33a2/pynecone/el/precompile.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/event.py` & `pynecone-0.1.33a2/pynecone/event.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/middleware/hydrate_middleware.py` & `pynecone-0.1.33a2/pynecone/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/middleware/middleware.py` & `pynecone-0.1.33a2/pynecone/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/model.py` & `pynecone-0.1.33a2/pynecone/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,17 +14,22 @@
     Returns:
         The database engine.
 
     Raises:
         ValueError: If the database url is None.
     """
     url = get_config().db_url
+    enable_admin = get_config().enable_admin
     if not url:
         raise ValueError("No database url in config")
-    return sqlmodel.create_engine(url, echo=False)
+    return sqlmodel.create_engine(
+        url,
+        echo=False,
+        connect_args={"check_same_thread": False} if enable_admin else {},
+    )
 
 
 class Model(Base, sqlmodel.SQLModel):
     """Base class to define a table in the database."""
 
     # The primary key for the table.
     id: Optional[int] = sqlmodel.Field(primary_key=True)
@@ -54,14 +59,23 @@
 
     @staticmethod
     def create_all():
         """Create all the tables."""
         engine = get_engine()
         sqlmodel.SQLModel.metadata.create_all(engine)
 
+    @staticmethod
+    def get_db_engine():
+        """Get the database engine.
+
+        Returns:
+            The database engine.
+        """
+        return get_engine()
+
     @classmethod
     @property
     def select(cls):
         """Select rows from the table.
 
         Returns:
             The select statement.
@@ -74,11 +88,17 @@
 
     Args:
         url: The database url.
 
     Returns:
         A database session.
     """
+    enable_admin = get_config().enable_admin
     if url is not None:
-        return sqlmodel.Session(sqlmodel.create_engine(url))
+        return sqlmodel.Session(
+            sqlmodel.create_engine(
+                url,
+                connect_args={"check_same_thread": False} if enable_admin else {},
+            ),
+        )
     engine = get_engine()
     return sqlmodel.Session(engine)
```

### Comparing `pynecone-0.1.33a1/pynecone/pc.py` & `pynecone-0.1.33a2/pynecone/pc.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,17 @@
         )
         raise typer.Exit()
 
     # Get the app module.
     console.rule("[bold]Starting Pynecone App")
     app = prerequisites.get_app()
 
+    # Check the admin dashboard settings.
+    prerequisites.check_admin_settings()
+
     # Get the frontend and backend commands, based on the environment.
     frontend_cmd = backend_cmd = None
     if env == constants.Env.DEV:
         frontend_cmd, backend_cmd = exec.run_frontend, exec.run_backend
     if env == constants.Env.PROD:
         frontend_cmd, backend_cmd = exec.run_frontend_prod, exec.run_backend_prod
     assert frontend_cmd and backend_cmd, "Invalid env"
```

### Comparing `pynecone-0.1.33a1/pynecone/route.py` & `pynecone-0.1.33a2/pynecone/route.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/state.py` & `pynecone-0.1.33a2/pynecone/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -651,23 +651,23 @@
             payload=event.payload,
         )
 
         # Clean the state before processing the event.
         self.clean()
 
         # Run the event generator and return state updates.
-        async for events, processing in event_iter:
+        async for events, final in event_iter:
             # Fix the returned events.
             events = fix_events(events, event.token)  # type: ignore
 
             # Get the delta after processing the event.
             delta = self.get_delta()
 
             # Yield the state update.
-            yield StateUpdate(delta=delta, events=events, processing=processing)
+            yield StateUpdate(delta=delta, events=events, final=final)
 
             # Clean the state to prepare for the next event.
             self.clean()
 
     async def _process_event(
         self, handler: EventHandler, state: State, payload: Dict
     ) -> AsyncIterator[Tuple[Optional[List[EventSpec]], bool]]:
@@ -677,15 +677,15 @@
             handler: Eventhandler to process.
             state: State to process the handler.
             payload: The event payload.
 
         Yields:
             Tuple containing:
                 0: The state update after processing the event.
-                1: Whether the event is being processed.
+                1: Whether the event is the final event.
         """
         # Get the function to process the event.
         fn = functools.partial(handler.fn, state)
 
         # Wrap the function in a try/except block.
         try:
             # Handle async functions.
@@ -695,32 +695,32 @@
             # Handle regular functions.
             else:
                 events = fn(**payload)
 
             # Handle async generators.
             if inspect.isasyncgen(events):
                 async for event in events:
-                    yield event, True
-                yield None, False
+                    yield event, False
+                yield None, True
 
             # Handle regular generators.
             elif inspect.isgenerator(events):
                 for event in events:
-                    yield event, True
-                yield None, False
+                    yield event, False
+                yield None, True
 
             # Handle regular event chains.
             else:
-                yield events, False
+                yield events, True
 
         # If an error occurs, throw a window alert.
         except Exception:
             error = traceback.format_exc()
             print(error)
-            yield [window_alert("An error occurred. See logs for details.")], False
+            yield [window_alert("An error occurred. See logs for details.")], True
 
     def _always_dirty_computed_vars(self) -> Set[str]:
         """The set of ComputedVars that always need to be recalculated.
 
         Returns:
             Set of all ComputedVar in this state where cache=False
         """
@@ -877,16 +877,16 @@
 
     # The state delta.
     delta: Delta = {}
 
     # Events to be added to the event queue.
     events: List[Event] = []
 
-    # Whether the event is still processing.
-    processing: bool = False
+    # Whether this is the final state update for the event.
+    final: bool = True
 
 
 class StateManager(Base):
     """A class to manage many client states."""
 
     # The state class to use.
     state: Type[State] = DefaultState
```

### Comparing `pynecone-0.1.33a1/pynecone/style.py` & `pynecone-0.1.33a2/pynecone/style.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/utils/build.py` & `pynecone-0.1.33a2/pynecone/utils/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,15 +204,14 @@
     # Initialize the web directory if it doesn't exist.
     web_dir = prerequisites.create_web_directory(root)
 
     # Install frontend packages.
     prerequisites.install_frontend_packages(web_dir)
 
     # Copy asset files to public folder.
-    path_ops.mkdir(str(root / constants.WEB_ASSETS_DIR))
     path_ops.cp(
         src=str(root / constants.APP_ASSETS_DIR),
         dest=str(root / constants.WEB_ASSETS_DIR),
     )
 
     # set the environment variables in client(env.json)
     set_environment_variables()
```

### Comparing `pynecone-0.1.33a1/pynecone/utils/console.py` & `pynecone-0.1.33a2/pynecone/utils/console.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/utils/exec.py` & `pynecone-0.1.33a2/pynecone/utils/exec.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/utils/format.py` & `pynecone-0.1.33a2/pynecone/utils/format.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/utils/imports.py` & `pynecone-0.1.33a2/pynecone/utils/imports.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/utils/path_ops.py` & `pynecone-0.1.33a2/pynecone/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/utils/prerequisites.py` & `pynecone-0.1.33a2/pynecone/utils/prerequisites.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import json
 import os
 import platform
 import re
 import subprocess
 import sys
+from datetime import datetime
 from pathlib import Path
 from types import ModuleType
 from typing import Optional
 
 import typer
 from packaging import version
 from redis import Redis
@@ -330,7 +331,34 @@
         Whether the app is using the latest template.
     """
     if not os.path.exists(constants.PCVERSION_APP_FILE):
         return False
     with open(constants.PCVERSION_APP_FILE) as f:  # type: ignore
         app_version = json.load(f)["version"]
     return app_version == constants.VERSION
+
+
+def check_admin_settings():
+    """Check if admin settings are set and valid for logging in cli app."""
+    admin_enabled = get_config().enable_admin
+    admin_dash = get_config().admin_dash
+    current_time = datetime.now()
+    if admin_enabled and admin_dash:
+        if not admin_dash.models:
+            console.print(
+                f"[yellow][Admin Dashboard][/yellow] :megaphone: Admin dashboard enabled, but no models defined in [bold magenta]pcconfig.py[/bold magenta]. Time: {current_time}"
+            )
+        else:
+            console.print(
+                f"[yellow][Admin Dashboard][/yellow] Admin enabled, building admin dashboard. Time: {current_time}"
+            )
+            console.print(
+                "Admin dashboard running at: [bold green]http://localhost:8000/admin[/bold green]"
+            )
+    elif admin_enabled:
+        console.print(
+            f"[yellow][Admin Dashboard][/yellow] :megaphone: Admin enabled, but no admin dashboard defined in [bold magenta]pcconfig.py[/bold magenta]. Time: {current_time}"
+        )
+    elif admin_dash:
+        console.print(
+            f"[yellow][Admin Dashboard][/yellow] :megaphone: Admin dashboard defined, but admin is not enabled in [bold magenta]pcconfig.py[/bold magenta]. Time: {current_time}"
+        )
```

### Comparing `pynecone-0.1.33a1/pynecone/utils/processes.py` & `pynecone-0.1.33a2/pynecone/utils/processes.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/utils/telemetry.py` & `pynecone-0.1.33a2/pynecone/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/utils/types.py` & `pynecone-0.1.33a2/pynecone/utils/types.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/utils/watch.py` & `pynecone-0.1.33a2/pynecone/utils/watch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pynecone/vars.py` & `pynecone-0.1.33a2/pynecone/vars.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a1/pyproject.toml` & `pynecone-0.1.33a2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynecone"
-version = "0.1.33a1"
+version = "0.1.33a2"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
@@ -37,14 +37,15 @@
 redis = "^4.3.5"
 rich = "^13.0.0"
 sqlmodel = "^0.0.8"
 typer = "0.4.2"
 uvicorn = "^0.20.0"
 watchdog = "^2.3.1"
 websockets = "^10.4"
+starlette-admin = "^0.9.0"
 python-dotenv = "^0.13.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 pytest-mock = "^3.10.0"
 pyright = "^1.1.229"
 darglint = "^1.8.1"
```

### Comparing `pynecone-0.1.33a1/PKG-INFO` & `pynecone-0.1.33a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone
-Version: 0.1.33a1
+Version: 0.1.33a2
 Summary: Web apps in pure Python.
 Home-page: https://pynecone.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
@@ -26,14 +26,15 @@
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: python-dotenv (>=0.13.0,<0.14.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: python-socketio (>=5.7.0,<6.0.0)
 Requires-Dist: redis (>=4.3.5,<5.0.0)
 Requires-Dist: rich (>=13.0.0,<14.0.0)
 Requires-Dist: sqlmodel (>=0.0.8,<0.0.9)
+Requires-Dist: starlette-admin (>=0.9.0,<0.10.0)
 Requires-Dist: typer (==0.4.2)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
 Requires-Dist: watchdog (>=2.3.1,<3.0.0)
 Requires-Dist: websockets (>=10.4,<11.0)
 Project-URL: Documentation, https://pynecone.io/docs/getting-started/introduction
 Project-URL: Repository, https://github.com/pynecone-io/pynecone
 Description-Content-Type: text/markdown
```

