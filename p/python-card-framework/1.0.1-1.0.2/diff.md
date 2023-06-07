# Comparing `tmp/python-card-framework-1.0.1.tar.gz` & `tmp/python-card-framework-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-card-framework-1.0.1.tar", last modified: Wed Jun  7 16:05:07 2023, max compression
+gzip compressed data, was "python-card-framework-1.0.2.tar", last modified: Wed Jun  7 16:52:31 2023, max compression
```

## Comparing `python-card-framework-1.0.1.tar` & `python-card-framework-1.0.2.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-07 16:05:07.929379 python-card-framework-1.0.1/
--rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)    11357 2022-06-28 20:30:54.000000 python-card-framework-1.0.1/LICENSE
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2778 2023-06-07 16:05:07.929379 python-card-framework-1.0.1/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2256 2022-10-27 14:17:49.000000 python-card-framework-1.0.1/README.md
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-07 16:05:07.921379 python-card-framework-1.0.1/card_framework/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5111 2022-11-14 18:42:27.000000 python-card-framework-1.0.1/card_framework/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)    13557 2022-11-14 16:19:34.000000 python-card-framework-1.0.1/card_framework/__init_test.py
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-07 16:05:07.925379 python-card-framework-1.0.1/card_framework/v2/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      593 2022-07-12 21:22:00.000000 python-card-framework-1.0.1/card_framework/v2/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1179 2022-11-11 21:07:48.000000 python-card-framework-1.0.1/card_framework/v2/action_response.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1293 2022-11-11 21:07:56.000000 python-card-framework-1.0.1/card_framework/v2/action_status.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3768 2022-11-11 21:08:05.000000 python-card-framework-1.0.1/card_framework/v2/annotation.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2121 2022-11-09 20:10:13.000000 python-card-framework-1.0.1/card_framework/v2/annotation_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3321 2022-11-11 21:08:38.000000 python-card-framework-1.0.1/card_framework/v2/attachment.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2327 2022-11-11 20:49:35.000000 python-card-framework-1.0.1/card_framework/v2/card.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      927 2022-11-11 21:09:09.000000 python-card-framework-1.0.1/card_framework/v2/card_action.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      941 2022-11-11 21:09:53.000000 python-card-framework-1.0.1/card_framework/v2/card_fixed_footer.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1898 2022-11-11 21:10:45.000000 python-card-framework-1.0.1/card_framework/v2/card_header.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2636 2022-07-13 21:37:01.000000 python-card-framework-1.0.1/card_framework/v2/card_header_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2332 2022-11-11 14:53:40.000000 python-card-framework-1.0.1/card_framework/v2/card_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1061 2022-11-11 21:11:01.000000 python-card-framework-1.0.1/card_framework/v2/dialog_action.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1051 2022-11-14 15:13:46.000000 python-card-framework-1.0.1/card_framework/v2/enums.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2041 2022-11-11 20:08:40.000000 python-card-framework-1.0.1/card_framework/v2/message.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1022 2022-11-09 22:37:58.000000 python-card-framework-1.0.1/card_framework/v2/message_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1564 2022-11-11 21:11:36.000000 python-card-framework-1.0.1/card_framework/v2/section.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3846 2022-11-09 21:44:42.000000 python-card-framework-1.0.1/card_framework/v2/section_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1378 2022-11-11 21:11:45.000000 python-card-framework-1.0.1/card_framework/v2/space.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1043 2022-11-11 21:11:50.000000 python-card-framework-1.0.1/card_framework/v2/user.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1242 2022-11-14 15:19:31.000000 python-card-framework-1.0.1/card_framework/v2/widget.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1589 2022-11-14 15:20:57.000000 python-card-framework-1.0.1/card_framework/v2/widget_test.py
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-07 16:05:07.929379 python-card-framework-1.0.1/card_framework/v2/widgets/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      592 2022-07-12 20:43:49.000000 python-card-framework-1.0.1/card_framework/v2/widgets/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1410 2022-11-11 20:52:08.000000 python-card-framework-1.0.1/card_framework/v2/widgets/action.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1200 2022-11-11 20:53:02.000000 python-card-framework-1.0.1/card_framework/v2/widgets/button.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1070 2022-11-11 20:52:19.000000 python-card-framework-1.0.1/card_framework/v2/widgets/button_list.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2571 2022-10-27 13:44:49.000000 python-card-framework-1.0.1/card_framework/v2/widgets/button_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1717 2022-11-11 20:53:35.000000 python-card-framework-1.0.1/card_framework/v2/widgets/color.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1270 2022-07-13 16:19:12.000000 python-card-framework-1.0.1/card_framework/v2/widgets/color_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1285 2023-06-07 15:55:33.000000 python-card-framework-1.0.1/card_framework/v2/widgets/date_time_picker.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2108 2023-06-07 15:56:04.000000 python-card-framework-1.0.1/card_framework/v2/widgets/date_time_picker_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2292 2022-11-11 20:54:50.000000 python-card-framework-1.0.1/card_framework/v2/widgets/decorated_text.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      652 2022-11-09 21:41:16.000000 python-card-framework-1.0.1/card_framework/v2/widgets/divider.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      785 2022-07-12 20:58:55.000000 python-card-framework-1.0.1/card_framework/v2/widgets/divider_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2476 2022-11-11 20:55:50.000000 python-card-framework-1.0.1/card_framework/v2/widgets/grid.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3308 2022-11-14 15:24:38.000000 python-card-framework-1.0.1/card_framework/v2/widgets/icon.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1899 2022-10-27 13:44:20.000000 python-card-framework-1.0.1/card_framework/v2/widgets/icon_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1088 2022-11-11 21:00:51.000000 python-card-framework-1.0.1/card_framework/v2/widgets/image.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1846 2022-11-09 22:09:39.000000 python-card-framework-1.0.1/card_framework/v2/widgets/image_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2474 2022-11-11 21:01:51.000000 python-card-framework-1.0.1/card_framework/v2/widgets/on_click.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3189 2022-08-30 15:19:59.000000 python-card-framework-1.0.1/card_framework/v2/widgets/on_click_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1117 2022-11-11 21:04:56.000000 python-card-framework-1.0.1/card_framework/v2/widgets/open_link.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1310 2022-11-11 21:05:13.000000 python-card-framework-1.0.1/card_framework/v2/widgets/selection_input.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      864 2022-11-11 21:05:36.000000 python-card-framework-1.0.1/card_framework/v2/widgets/selection_item.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      955 2022-11-11 21:05:52.000000 python-card-framework-1.0.1/card_framework/v2/widgets/suggestions.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1796 2022-11-11 21:06:19.000000 python-card-framework-1.0.1/card_framework/v2/widgets/switch_control.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1396 2022-11-11 21:06:39.000000 python-card-framework-1.0.1/card_framework/v2/widgets/text_input.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2862 2022-09-01 19:48:26.000000 python-card-framework-1.0.1/card_framework/v2/widgets/text_input_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      979 2022-11-11 21:07:34.000000 python-card-framework-1.0.1/card_framework/v2/widgets/text_paragraph.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1262 2022-11-10 20:06:50.000000 python-card-framework-1.0.1/card_framework/v2/widgets/text_paragraph_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      807 2023-06-07 15:20:23.000000 python-card-framework-1.0.1/pyproject.toml
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-07 16:05:07.929379 python-card-framework-1.0.1/python_card_framework.egg-info/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2778 2023-06-07 16:05:07.000000 python-card-framework-1.0.1/python_card_framework.egg-info/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2159 2023-06-07 16:05:07.000000 python-card-framework-1.0.1/python_card_framework.egg-info/SOURCES.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-07 16:05:07.000000 python-card-framework-1.0.1/python_card_framework.egg-info/dependency_links.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       42 2023-06-07 16:05:07.000000 python-card-framework-1.0.1/python_card_framework.egg-info/requires.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       15 2023-06-07 16:05:07.000000 python-card-framework-1.0.1/python_card_framework.egg-info/top_level.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-07 16:05:07.929379 python-card-framework-1.0.1/setup.cfg
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-07 16:52:31.814729 python-card-framework-1.0.2/
+-rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)    11357 2022-06-28 20:30:54.000000 python-card-framework-1.0.2/LICENSE
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2779 2023-06-07 16:52:31.814729 python-card-framework-1.0.2/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2257 2023-06-07 16:51:51.000000 python-card-framework-1.0.2/README.md
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-07 16:52:31.806729 python-card-framework-1.0.2/card_framework/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5111 2022-11-14 18:42:27.000000 python-card-framework-1.0.2/card_framework/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)    13557 2022-11-14 16:19:34.000000 python-card-framework-1.0.2/card_framework/__init_test.py
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-07 16:52:31.810729 python-card-framework-1.0.2/card_framework/v2/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      593 2022-07-12 21:22:00.000000 python-card-framework-1.0.2/card_framework/v2/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1179 2022-11-11 21:07:48.000000 python-card-framework-1.0.2/card_framework/v2/action_response.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1293 2022-11-11 21:07:56.000000 python-card-framework-1.0.2/card_framework/v2/action_status.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3768 2022-11-11 21:08:05.000000 python-card-framework-1.0.2/card_framework/v2/annotation.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2121 2022-11-09 20:10:13.000000 python-card-framework-1.0.2/card_framework/v2/annotation_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3321 2022-11-11 21:08:38.000000 python-card-framework-1.0.2/card_framework/v2/attachment.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2327 2022-11-11 20:49:35.000000 python-card-framework-1.0.2/card_framework/v2/card.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      927 2022-11-11 21:09:09.000000 python-card-framework-1.0.2/card_framework/v2/card_action.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      941 2022-11-11 21:09:53.000000 python-card-framework-1.0.2/card_framework/v2/card_fixed_footer.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1898 2022-11-11 21:10:45.000000 python-card-framework-1.0.2/card_framework/v2/card_header.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2636 2022-07-13 21:37:01.000000 python-card-framework-1.0.2/card_framework/v2/card_header_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2332 2022-11-11 14:53:40.000000 python-card-framework-1.0.2/card_framework/v2/card_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1061 2022-11-11 21:11:01.000000 python-card-framework-1.0.2/card_framework/v2/dialog_action.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1051 2022-11-14 15:13:46.000000 python-card-framework-1.0.2/card_framework/v2/enums.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2041 2022-11-11 20:08:40.000000 python-card-framework-1.0.2/card_framework/v2/message.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1022 2022-11-09 22:37:58.000000 python-card-framework-1.0.2/card_framework/v2/message_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1564 2022-11-11 21:11:36.000000 python-card-framework-1.0.2/card_framework/v2/section.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3846 2022-11-09 21:44:42.000000 python-card-framework-1.0.2/card_framework/v2/section_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1378 2022-11-11 21:11:45.000000 python-card-framework-1.0.2/card_framework/v2/space.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1043 2022-11-11 21:11:50.000000 python-card-framework-1.0.2/card_framework/v2/user.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1242 2022-11-14 15:19:31.000000 python-card-framework-1.0.2/card_framework/v2/widget.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1589 2022-11-14 15:20:57.000000 python-card-framework-1.0.2/card_framework/v2/widget_test.py
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-07 16:52:31.814729 python-card-framework-1.0.2/card_framework/v2/widgets/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      592 2022-07-12 20:43:49.000000 python-card-framework-1.0.2/card_framework/v2/widgets/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1410 2022-11-11 20:52:08.000000 python-card-framework-1.0.2/card_framework/v2/widgets/action.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1200 2022-11-11 20:53:02.000000 python-card-framework-1.0.2/card_framework/v2/widgets/button.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1070 2022-11-11 20:52:19.000000 python-card-framework-1.0.2/card_framework/v2/widgets/button_list.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2571 2022-10-27 13:44:49.000000 python-card-framework-1.0.2/card_framework/v2/widgets/button_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1717 2022-11-11 20:53:35.000000 python-card-framework-1.0.2/card_framework/v2/widgets/color.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1270 2022-07-13 16:19:12.000000 python-card-framework-1.0.2/card_framework/v2/widgets/color_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2117 2023-06-07 16:51:51.000000 python-card-framework-1.0.2/card_framework/v2/widgets/columns.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6540 2023-06-07 16:51:51.000000 python-card-framework-1.0.2/card_framework/v2/widgets/columns_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1285 2023-06-07 15:55:33.000000 python-card-framework-1.0.2/card_framework/v2/widgets/date_time_picker.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2108 2023-06-07 15:56:04.000000 python-card-framework-1.0.2/card_framework/v2/widgets/date_time_picker_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2292 2022-11-11 20:54:50.000000 python-card-framework-1.0.2/card_framework/v2/widgets/decorated_text.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      652 2022-11-09 21:41:16.000000 python-card-framework-1.0.2/card_framework/v2/widgets/divider.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      785 2022-07-12 20:58:55.000000 python-card-framework-1.0.2/card_framework/v2/widgets/divider_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2476 2022-11-11 20:55:50.000000 python-card-framework-1.0.2/card_framework/v2/widgets/grid.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3308 2022-11-14 15:24:38.000000 python-card-framework-1.0.2/card_framework/v2/widgets/icon.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1899 2022-10-27 13:44:20.000000 python-card-framework-1.0.2/card_framework/v2/widgets/icon_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1088 2022-11-11 21:00:51.000000 python-card-framework-1.0.2/card_framework/v2/widgets/image.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1846 2022-11-09 22:09:39.000000 python-card-framework-1.0.2/card_framework/v2/widgets/image_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2474 2022-11-11 21:01:51.000000 python-card-framework-1.0.2/card_framework/v2/widgets/on_click.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3189 2022-08-30 15:19:59.000000 python-card-framework-1.0.2/card_framework/v2/widgets/on_click_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1117 2022-11-11 21:04:56.000000 python-card-framework-1.0.2/card_framework/v2/widgets/open_link.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1310 2022-11-11 21:05:13.000000 python-card-framework-1.0.2/card_framework/v2/widgets/selection_input.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      864 2022-11-11 21:05:36.000000 python-card-framework-1.0.2/card_framework/v2/widgets/selection_item.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      955 2022-11-11 21:05:52.000000 python-card-framework-1.0.2/card_framework/v2/widgets/suggestions.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1796 2022-11-11 21:06:19.000000 python-card-framework-1.0.2/card_framework/v2/widgets/switch_control.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1396 2022-11-11 21:06:39.000000 python-card-framework-1.0.2/card_framework/v2/widgets/text_input.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2862 2022-09-01 19:48:26.000000 python-card-framework-1.0.2/card_framework/v2/widgets/text_input_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      979 2022-11-11 21:07:34.000000 python-card-framework-1.0.2/card_framework/v2/widgets/text_paragraph.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1262 2022-11-10 20:06:50.000000 python-card-framework-1.0.2/card_framework/v2/widgets/text_paragraph_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      807 2023-06-07 16:51:51.000000 python-card-framework-1.0.2/pyproject.toml
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-07 16:52:31.814729 python-card-framework-1.0.2/python_card_framework.egg-info/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2779 2023-06-07 16:52:31.000000 python-card-framework-1.0.2/python_card_framework.egg-info/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2238 2023-06-07 16:52:31.000000 python-card-framework-1.0.2/python_card_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-07 16:52:31.000000 python-card-framework-1.0.2/python_card_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       42 2023-06-07 16:52:31.000000 python-card-framework-1.0.2/python_card_framework.egg-info/requires.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       15 2023-06-07 16:52:31.000000 python-card-framework-1.0.2/python_card_framework.egg-info/top_level.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-07 16:52:31.814729 python-card-framework-1.0.2/setup.cfg
```

### Comparing `python-card-framework-1.0.1/LICENSE` & `python-card-framework-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/PKG-INFO` & `python-card-framework-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-card-framework
-Version: 1.0.1
+Version: 1.0.2
 Summary: API for rendering Chat App Card json.
 Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/google/python-card-framework
 Project-URL: Bug Tracker, https://github.com/google/python-card-framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,15 @@
 
 The exact JSON that is being rendered can be found in the official Google
 Developer Docs pages here: https://developers.google.com/chat/api/reference/rest/v1/spaces.messages?hl=en
 
 ## Intention
 
 In order to generate or send messages from a chat application to the user, the
-messages ust be formed of valid JSON objects. In the event that the message is
+messages must be formed of valid JSON objects. In the event that the message is
 malformed, a simple 'Chat App not responding' message is returned. This leads
 to the developer having to insert large blocks of JSON in their Python code,
 much of which is boiler-plate and can easily lead to hard to find cut and paste
 errors.
 
 As a result this library of objects has been created to alleviate the problem.
 The developer can now create and manipulate first-class Python objects which
```

### Comparing `python-card-framework-1.0.1/README.md` & `python-card-framework-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 The exact JSON that is being rendered can be found in the official Google
 Developer Docs pages here: https://developers.google.com/chat/api/reference/rest/v1/spaces.messages?hl=en
 
 ## Intention
 
 In order to generate or send messages from a chat application to the user, the
-messages ust be formed of valid JSON objects. In the event that the message is
+messages must be formed of valid JSON objects. In the event that the message is
 malformed, a simple 'Chat App not responding' message is returned. This leads
 to the developer having to insert large blocks of JSON in their Python code,
 much of which is boiler-plate and can easily lead to hard to find cut and paste
 errors.
 
 As a result this library of objects has been created to alleviate the problem.
 The developer can now create and manipulate first-class Python objects which
```

### Comparing `python-card-framework-1.0.1/card_framework/__init__.py` & `python-card-framework-1.0.2/card_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/__init_test.py` & `python-card-framework-1.0.2/card_framework/__init_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/__init__.py` & `python-card-framework-1.0.2/card_framework/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/action_response.py` & `python-card-framework-1.0.2/card_framework/v2/action_response.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/action_status.py` & `python-card-framework-1.0.2/card_framework/v2/action_status.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/annotation.py` & `python-card-framework-1.0.2/card_framework/v2/annotation.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/annotation_test.py` & `python-card-framework-1.0.2/card_framework/v2/annotation_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/attachment.py` & `python-card-framework-1.0.2/card_framework/v2/attachment.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/card.py` & `python-card-framework-1.0.2/card_framework/v2/card.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/card_action.py` & `python-card-framework-1.0.2/card_framework/v2/card_action.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/card_fixed_footer.py` & `python-card-framework-1.0.2/card_framework/v2/card_fixed_footer.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/card_header.py` & `python-card-framework-1.0.2/card_framework/v2/card_header.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/card_header_test.py` & `python-card-framework-1.0.2/card_framework/v2/card_header_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/card_test.py` & `python-card-framework-1.0.2/card_framework/v2/card_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/dialog_action.py` & `python-card-framework-1.0.2/card_framework/v2/dialog_action.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/enums.py` & `python-card-framework-1.0.2/card_framework/v2/enums.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/message.py` & `python-card-framework-1.0.2/card_framework/v2/message.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/message_test.py` & `python-card-framework-1.0.2/card_framework/v2/message_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/section.py` & `python-card-framework-1.0.2/card_framework/v2/section.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/section_test.py` & `python-card-framework-1.0.2/card_framework/v2/section_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/space.py` & `python-card-framework-1.0.2/card_framework/v2/space.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/user.py` & `python-card-framework-1.0.2/card_framework/v2/user.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widget.py` & `python-card-framework-1.0.2/card_framework/v2/widget.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widget_test.py` & `python-card-framework-1.0.2/card_framework/v2/widget_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/__init__.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/action.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/action.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/button.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/button.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/button_list.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/button_list.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/button_test.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/button_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/color.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/color.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/color_test.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/color_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/date_time_picker.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/date_time_picker.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/date_time_picker_test.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/date_time_picker_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/decorated_text.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/decorated_text.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/divider.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/divider.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/divider_test.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/divider_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/grid.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/grid.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/icon.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/icon.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/icon_test.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/icon_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/image.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/image.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/image_test.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/image_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/on_click.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/on_click.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/on_click_test.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/on_click_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/open_link.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/open_link.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/selection_input.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/selection_input.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/selection_item.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/selection_item.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/suggestions.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/suggestions.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/switch_control.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/switch_control.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/text_input.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/text_input.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/text_input_test.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/text_input_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/text_paragraph.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/text_paragraph.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/card_framework/v2/widgets/text_paragraph_test.py` & `python-card-framework-1.0.2/card_framework/v2/widgets/text_paragraph_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.1/pyproject.toml` & `python-card-framework-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-card-framework"
-version = "1.0.1"
+version = "1.0.2"
 authors = [{ name = "David Harcombe", email = "david.harcombe@gmail.com" }]
 description = "API for rendering Chat App Card json."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
  "Programming Language :: Python :: 3",
  "Operating System :: OS Independent",
```

### Comparing `python-card-framework-1.0.1/python_card_framework.egg-info/PKG-INFO` & `python-card-framework-1.0.2/python_card_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-card-framework
-Version: 1.0.1
+Version: 1.0.2
 Summary: API for rendering Chat App Card json.
 Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/google/python-card-framework
 Project-URL: Bug Tracker, https://github.com/google/python-card-framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,15 @@
 
 The exact JSON that is being rendered can be found in the official Google
 Developer Docs pages here: https://developers.google.com/chat/api/reference/rest/v1/spaces.messages?hl=en
 
 ## Intention
 
 In order to generate or send messages from a chat application to the user, the
-messages ust be formed of valid JSON objects. In the event that the message is
+messages must be formed of valid JSON objects. In the event that the message is
 malformed, a simple 'Chat App not responding' message is returned. This leads
 to the developer having to insert large blocks of JSON in their Python code,
 much of which is boiler-plate and can easily lead to hard to find cut and paste
 errors.
 
 As a result this library of objects has been created to alleviate the problem.
 The developer can now create and manipulate first-class Python objects which
```

### Comparing `python-card-framework-1.0.1/python_card_framework.egg-info/SOURCES.txt` & `python-card-framework-1.0.2/python_card_framework.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 card_framework/v2/widgets/__init__.py
 card_framework/v2/widgets/action.py
 card_framework/v2/widgets/button.py
 card_framework/v2/widgets/button_list.py
 card_framework/v2/widgets/button_test.py
 card_framework/v2/widgets/color.py
 card_framework/v2/widgets/color_test.py
+card_framework/v2/widgets/columns.py
+card_framework/v2/widgets/columns_test.py
 card_framework/v2/widgets/date_time_picker.py
 card_framework/v2/widgets/date_time_picker_test.py
 card_framework/v2/widgets/decorated_text.py
 card_framework/v2/widgets/divider.py
 card_framework/v2/widgets/divider_test.py
 card_framework/v2/widgets/grid.py
 card_framework/v2/widgets/icon.py
```

