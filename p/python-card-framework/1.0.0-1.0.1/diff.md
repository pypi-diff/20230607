# Comparing `tmp/python-card-framework-1.0.0.tar.gz` & `tmp/python-card-framework-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-card-framework-1.0.0.tar", last modified: Fri Nov 11 21:17:23 2022, max compression
+gzip compressed data, was "python-card-framework-1.0.1.tar", last modified: Wed Jun  7 16:05:07 2023, max compression
```

## Comparing `python-card-framework-1.0.0.tar` & `python-card-framework-1.0.1.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-x---   0 davidharcombe (261421) primarygroup (89939)        0 2022-11-11 21:17:23.142934 python-card-framework-1.0.0/
--rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)    11357 2022-06-28 20:30:54.000000 python-card-framework-1.0.0/LICENSE
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     2906 2022-11-11 21:17:23.142934 python-card-framework-1.0.0/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2256 2022-10-27 14:17:49.000000 python-card-framework-1.0.0/README.md
-drwxr-x---   0 davidharcombe (261421) primarygroup (89939)        0 2022-11-11 21:17:23.122934 python-card-framework-1.0.0/card_framework/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5073 2022-11-11 21:12:11.000000 python-card-framework-1.0.0/card_framework/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)    13920 2022-11-11 20:48:12.000000 python-card-framework-1.0.0/card_framework/__init_test.py
-drwxr-x---   0 davidharcombe (261421) primarygroup (89939)        0 2022-11-11 21:17:23.130934 python-card-framework-1.0.0/card_framework/v2/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      593 2022-07-12 21:22:00.000000 python-card-framework-1.0.0/card_framework/v2/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1179 2022-11-11 21:07:48.000000 python-card-framework-1.0.0/card_framework/v2/action_response.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1293 2022-11-11 21:07:56.000000 python-card-framework-1.0.0/card_framework/v2/action_status.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3768 2022-11-11 21:08:05.000000 python-card-framework-1.0.0/card_framework/v2/annotation.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2121 2022-11-09 20:10:13.000000 python-card-framework-1.0.0/card_framework/v2/annotation_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3321 2022-11-11 21:08:38.000000 python-card-framework-1.0.0/card_framework/v2/attachment.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2327 2022-11-11 20:49:35.000000 python-card-framework-1.0.0/card_framework/v2/card.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      927 2022-11-11 21:09:09.000000 python-card-framework-1.0.0/card_framework/v2/card_action.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      941 2022-11-11 21:09:53.000000 python-card-framework-1.0.0/card_framework/v2/card_fixed_footer.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1898 2022-11-11 21:10:45.000000 python-card-framework-1.0.0/card_framework/v2/card_header.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2636 2022-07-13 21:37:01.000000 python-card-framework-1.0.0/card_framework/v2/card_header_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2332 2022-11-11 14:53:40.000000 python-card-framework-1.0.0/card_framework/v2/card_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1061 2022-11-11 21:11:01.000000 python-card-framework-1.0.0/card_framework/v2/dialog_action.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1117 2022-11-09 16:53:48.000000 python-card-framework-1.0.0/card_framework/v2/enums.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2041 2022-11-11 20:08:40.000000 python-card-framework-1.0.0/card_framework/v2/message.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1022 2022-11-09 22:37:58.000000 python-card-framework-1.0.0/card_framework/v2/message_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1564 2022-11-11 21:11:36.000000 python-card-framework-1.0.0/card_framework/v2/section.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3846 2022-11-09 21:44:42.000000 python-card-framework-1.0.0/card_framework/v2/section_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1378 2022-11-11 21:11:45.000000 python-card-framework-1.0.0/card_framework/v2/space.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1043 2022-11-11 21:11:50.000000 python-card-framework-1.0.0/card_framework/v2/user.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1242 2022-11-09 22:07:01.000000 python-card-framework-1.0.0/card_framework/v2/widget.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1251 2022-11-09 21:44:05.000000 python-card-framework-1.0.0/card_framework/v2/widget_test.py
-drwxr-x---   0 davidharcombe (261421) primarygroup (89939)        0 2022-11-11 21:17:23.138934 python-card-framework-1.0.0/card_framework/v2/widgets/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      592 2022-07-12 20:43:49.000000 python-card-framework-1.0.0/card_framework/v2/widgets/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1410 2022-11-11 20:52:08.000000 python-card-framework-1.0.0/card_framework/v2/widgets/action.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1200 2022-11-11 20:53:02.000000 python-card-framework-1.0.0/card_framework/v2/widgets/button.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1070 2022-11-11 20:52:19.000000 python-card-framework-1.0.0/card_framework/v2/widgets/button_list.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2571 2022-10-27 13:44:49.000000 python-card-framework-1.0.0/card_framework/v2/widgets/button_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1717 2022-11-11 20:53:35.000000 python-card-framework-1.0.0/card_framework/v2/widgets/color.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1270 2022-07-13 16:19:12.000000 python-card-framework-1.0.0/card_framework/v2/widgets/color_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2292 2022-11-11 20:54:50.000000 python-card-framework-1.0.0/card_framework/v2/widgets/decorated_text.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      652 2022-11-09 21:41:16.000000 python-card-framework-1.0.0/card_framework/v2/widgets/divider.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      785 2022-07-12 20:58:55.000000 python-card-framework-1.0.0/card_framework/v2/widgets/divider_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2476 2022-11-11 20:55:50.000000 python-card-framework-1.0.0/card_framework/v2/widgets/grid.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3312 2022-11-11 21:01:00.000000 python-card-framework-1.0.0/card_framework/v2/widgets/icon.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1899 2022-10-27 13:44:20.000000 python-card-framework-1.0.0/card_framework/v2/widgets/icon_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1088 2022-11-11 21:00:51.000000 python-card-framework-1.0.0/card_framework/v2/widgets/image.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1846 2022-11-09 22:09:39.000000 python-card-framework-1.0.0/card_framework/v2/widgets/image_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2474 2022-11-11 21:01:51.000000 python-card-framework-1.0.0/card_framework/v2/widgets/on_click.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3189 2022-08-30 15:19:59.000000 python-card-framework-1.0.0/card_framework/v2/widgets/on_click_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1117 2022-11-11 21:04:56.000000 python-card-framework-1.0.0/card_framework/v2/widgets/open_link.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1310 2022-11-11 21:05:13.000000 python-card-framework-1.0.0/card_framework/v2/widgets/selection_input.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      864 2022-11-11 21:05:36.000000 python-card-framework-1.0.0/card_framework/v2/widgets/selection_item.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      955 2022-11-11 21:05:52.000000 python-card-framework-1.0.0/card_framework/v2/widgets/suggestions.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1796 2022-11-11 21:06:19.000000 python-card-framework-1.0.0/card_framework/v2/widgets/switch_control.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1396 2022-11-11 21:06:39.000000 python-card-framework-1.0.0/card_framework/v2/widgets/text_input.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2862 2022-09-01 19:48:26.000000 python-card-framework-1.0.0/card_framework/v2/widgets/text_input_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      979 2022-11-11 21:07:34.000000 python-card-framework-1.0.0/card_framework/v2/widgets/text_paragraph.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1262 2022-11-10 20:06:50.000000 python-card-framework-1.0.0/card_framework/v2/widgets/text_paragraph_test.py
-drwxr-x---   0 davidharcombe (261421) primarygroup (89939)        0 2022-11-11 21:17:23.142934 python-card-framework-1.0.0/python_card_framework.egg-info/
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     2906 2022-11-11 21:17:23.000000 python-card-framework-1.0.0/python_card_framework.egg-info/PKG-INFO
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     2100 2022-11-11 21:17:23.000000 python-card-framework-1.0.0/python_card_framework.egg-info/SOURCES.txt
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)        1 2022-11-11 21:17:23.000000 python-card-framework-1.0.0/python_card_framework.egg-info/dependency_links.txt
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)        1 2022-10-12 16:32:20.000000 python-card-framework-1.0.0/python_card_framework.egg-info/not-zip-safe
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)       42 2022-11-11 21:17:23.000000 python-card-framework-1.0.0/python_card_framework.egg-info/requires.txt
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)       15 2022-11-11 21:17:23.000000 python-card-framework-1.0.0/python_card_framework.egg-info/top_level.txt
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)       38 2022-11-11 21:17:23.142934 python-card-framework-1.0.0/setup.cfg
--rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)     1925 2022-11-11 21:12:27.000000 python-card-framework-1.0.0/setup.py
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-07 16:05:07.929379 python-card-framework-1.0.1/
+-rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)    11357 2022-06-28 20:30:54.000000 python-card-framework-1.0.1/LICENSE
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2778 2023-06-07 16:05:07.929379 python-card-framework-1.0.1/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2256 2022-10-27 14:17:49.000000 python-card-framework-1.0.1/README.md
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-07 16:05:07.921379 python-card-framework-1.0.1/card_framework/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5111 2022-11-14 18:42:27.000000 python-card-framework-1.0.1/card_framework/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)    13557 2022-11-14 16:19:34.000000 python-card-framework-1.0.1/card_framework/__init_test.py
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-07 16:05:07.925379 python-card-framework-1.0.1/card_framework/v2/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      593 2022-07-12 21:22:00.000000 python-card-framework-1.0.1/card_framework/v2/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1179 2022-11-11 21:07:48.000000 python-card-framework-1.0.1/card_framework/v2/action_response.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1293 2022-11-11 21:07:56.000000 python-card-framework-1.0.1/card_framework/v2/action_status.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3768 2022-11-11 21:08:05.000000 python-card-framework-1.0.1/card_framework/v2/annotation.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2121 2022-11-09 20:10:13.000000 python-card-framework-1.0.1/card_framework/v2/annotation_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3321 2022-11-11 21:08:38.000000 python-card-framework-1.0.1/card_framework/v2/attachment.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2327 2022-11-11 20:49:35.000000 python-card-framework-1.0.1/card_framework/v2/card.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      927 2022-11-11 21:09:09.000000 python-card-framework-1.0.1/card_framework/v2/card_action.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      941 2022-11-11 21:09:53.000000 python-card-framework-1.0.1/card_framework/v2/card_fixed_footer.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1898 2022-11-11 21:10:45.000000 python-card-framework-1.0.1/card_framework/v2/card_header.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2636 2022-07-13 21:37:01.000000 python-card-framework-1.0.1/card_framework/v2/card_header_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2332 2022-11-11 14:53:40.000000 python-card-framework-1.0.1/card_framework/v2/card_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1061 2022-11-11 21:11:01.000000 python-card-framework-1.0.1/card_framework/v2/dialog_action.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1051 2022-11-14 15:13:46.000000 python-card-framework-1.0.1/card_framework/v2/enums.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2041 2022-11-11 20:08:40.000000 python-card-framework-1.0.1/card_framework/v2/message.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1022 2022-11-09 22:37:58.000000 python-card-framework-1.0.1/card_framework/v2/message_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1564 2022-11-11 21:11:36.000000 python-card-framework-1.0.1/card_framework/v2/section.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3846 2022-11-09 21:44:42.000000 python-card-framework-1.0.1/card_framework/v2/section_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1378 2022-11-11 21:11:45.000000 python-card-framework-1.0.1/card_framework/v2/space.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1043 2022-11-11 21:11:50.000000 python-card-framework-1.0.1/card_framework/v2/user.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1242 2022-11-14 15:19:31.000000 python-card-framework-1.0.1/card_framework/v2/widget.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1589 2022-11-14 15:20:57.000000 python-card-framework-1.0.1/card_framework/v2/widget_test.py
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-07 16:05:07.929379 python-card-framework-1.0.1/card_framework/v2/widgets/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      592 2022-07-12 20:43:49.000000 python-card-framework-1.0.1/card_framework/v2/widgets/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1410 2022-11-11 20:52:08.000000 python-card-framework-1.0.1/card_framework/v2/widgets/action.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1200 2022-11-11 20:53:02.000000 python-card-framework-1.0.1/card_framework/v2/widgets/button.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1070 2022-11-11 20:52:19.000000 python-card-framework-1.0.1/card_framework/v2/widgets/button_list.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2571 2022-10-27 13:44:49.000000 python-card-framework-1.0.1/card_framework/v2/widgets/button_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1717 2022-11-11 20:53:35.000000 python-card-framework-1.0.1/card_framework/v2/widgets/color.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1270 2022-07-13 16:19:12.000000 python-card-framework-1.0.1/card_framework/v2/widgets/color_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1285 2023-06-07 15:55:33.000000 python-card-framework-1.0.1/card_framework/v2/widgets/date_time_picker.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2108 2023-06-07 15:56:04.000000 python-card-framework-1.0.1/card_framework/v2/widgets/date_time_picker_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2292 2022-11-11 20:54:50.000000 python-card-framework-1.0.1/card_framework/v2/widgets/decorated_text.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      652 2022-11-09 21:41:16.000000 python-card-framework-1.0.1/card_framework/v2/widgets/divider.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      785 2022-07-12 20:58:55.000000 python-card-framework-1.0.1/card_framework/v2/widgets/divider_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2476 2022-11-11 20:55:50.000000 python-card-framework-1.0.1/card_framework/v2/widgets/grid.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3308 2022-11-14 15:24:38.000000 python-card-framework-1.0.1/card_framework/v2/widgets/icon.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1899 2022-10-27 13:44:20.000000 python-card-framework-1.0.1/card_framework/v2/widgets/icon_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1088 2022-11-11 21:00:51.000000 python-card-framework-1.0.1/card_framework/v2/widgets/image.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1846 2022-11-09 22:09:39.000000 python-card-framework-1.0.1/card_framework/v2/widgets/image_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2474 2022-11-11 21:01:51.000000 python-card-framework-1.0.1/card_framework/v2/widgets/on_click.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3189 2022-08-30 15:19:59.000000 python-card-framework-1.0.1/card_framework/v2/widgets/on_click_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1117 2022-11-11 21:04:56.000000 python-card-framework-1.0.1/card_framework/v2/widgets/open_link.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1310 2022-11-11 21:05:13.000000 python-card-framework-1.0.1/card_framework/v2/widgets/selection_input.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      864 2022-11-11 21:05:36.000000 python-card-framework-1.0.1/card_framework/v2/widgets/selection_item.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      955 2022-11-11 21:05:52.000000 python-card-framework-1.0.1/card_framework/v2/widgets/suggestions.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1796 2022-11-11 21:06:19.000000 python-card-framework-1.0.1/card_framework/v2/widgets/switch_control.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1396 2022-11-11 21:06:39.000000 python-card-framework-1.0.1/card_framework/v2/widgets/text_input.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2862 2022-09-01 19:48:26.000000 python-card-framework-1.0.1/card_framework/v2/widgets/text_input_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      979 2022-11-11 21:07:34.000000 python-card-framework-1.0.1/card_framework/v2/widgets/text_paragraph.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1262 2022-11-10 20:06:50.000000 python-card-framework-1.0.1/card_framework/v2/widgets/text_paragraph_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      807 2023-06-07 15:20:23.000000 python-card-framework-1.0.1/pyproject.toml
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-07 16:05:07.929379 python-card-framework-1.0.1/python_card_framework.egg-info/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2778 2023-06-07 16:05:07.000000 python-card-framework-1.0.1/python_card_framework.egg-info/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2159 2023-06-07 16:05:07.000000 python-card-framework-1.0.1/python_card_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-07 16:05:07.000000 python-card-framework-1.0.1/python_card_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       42 2023-06-07 16:05:07.000000 python-card-framework-1.0.1/python_card_framework.egg-info/requires.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       15 2023-06-07 16:05:07.000000 python-card-framework-1.0.1/python_card_framework.egg-info/top_level.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-07 16:05:07.929379 python-card-framework-1.0.1/setup.cfg
```

### Comparing `python-card-framework-1.0.0/LICENSE` & `python-card-framework-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/PKG-INFO` & `python-card-framework-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Metadata-Version: 2.1
 Name: python-card-framework
-Version: 1.0.0
+Version: 1.0.1
 Summary: API for rendering Chat App Card json.
-Home-page: https://github.com/google/python-card-framework
-Author: David Harcombe
-Author-email: davidharcombe@google.com
+Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: License :: OSI Approved :: Apache Software License
+Project-URL: Homepage, https://github.com/google/python-card-framework
+Project-URL: Bug Tracker, https://github.com/google/python-card-framework/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Card Framework
 
 This is a library designed to allow Python developers to treat the Chat API
@@ -76,9 +71,7 @@
                     image_url='https://source.unsplash.com/featured320x180?nature&sig=8')
 card = Card(header=header, sections=[Section(widgets=widgets)])
 
 return Message(cards=[card]).render()
 ```
 
 which will return the correct JSON.
-
-
```

### Comparing `python-card-framework-1.0.0/README.md` & `python-card-framework-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/__init__.py` & `python-card-framework-1.0.1/card_framework/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,67 +12,64 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import dataclasses
 import enum
 import inspect
+from operator import contains
 from typing import Any, Callable, Mapping
 
 import dataclasses_json
 import stringcase
 
 
-def lazy_property(f: Callable):
-  """Decorator that makes a property lazy-evaluated.
-
-  Args:
-    f: the function to convert to a lazy property.
-  """
-  attr_name = '_lazy_' + f.__name__
-
-  @property
-  def _lazy_property(self) -> Any:
-    if not hasattr(self, attr_name):
-      setattr(self, attr_name, f(self))
-    return getattr(self, attr_name)
-  return _lazy_property
-
-
-def field(default: Any = None, default_factory: Any = None,
+def __field(default: Any = None, default_factory: Any = None,
           **metadata) -> dataclasses.Field:
   return (
       dataclasses.field(
           default_factory=default_factory,
           metadata=dataclasses_json.config(**metadata)
       ) if default_factory
       else dataclasses.field(default=default,
                              metadata=dataclasses_json.config(**metadata))
   )
 
 
-def metadata(base: Mapping[str, Any], **custom) -> Mapping[str, Any]:
+def merge_metadata(base: Mapping[str, Any], **custom) -> Mapping[str, Any]:
+  """Merges metadata with supplied metadata keys.
+
+  This is different from a plain dict.update() as it removes keys defined as
+  `None` allowing any dataclass default behaviour to reassert itself.
+
+  Args:
+      base (Mapping[str, Any]): the base metadata
+      **custom (Any): the list of named metadata parameters to add/edit/remove
+
+  Returns:
+      Mapping[str, Any]: the merged metadata
+  """
   for key in custom:
     if not custom[key] and key in base:
       del base[key]
 
     elif custom[key]:
-      base.update({key: custom[key]})
+      base |= {key: custom[key]}
 
   return base
 
 
 def standard_field(default: Any = None, default_factory: Any = None,
                    **kwargs) -> dataclasses.Field:
-  base = metadata({
+  base = merge_metadata({
       'letter_case': dataclasses_json.LetterCase.CAMEL,
       'exclude': lambda x: not x
   }, **kwargs)
 
-  return field(default=default, default_factory=default_factory, **base)
+  return __field(default=default, default_factory=default_factory, **base)
 
 
 def enum_field(default: Any = None, **kwargs) -> dataclasses.Field:
   base = {'encoder': lambda x: x.name if x else None, **kwargs}
 
   return standard_field(default=default, **base)
 
@@ -87,15 +84,15 @@
   base = {'encoder': lambda x: [__value(f) or f for f in x], **kwargs}
 
   return standard_field(default_factory=default_factory, **base)
 
 
 class AutoNumber(enum.Enum):
   def __repr__(self):
-    return f'{self.__class__.__name__}, {self.name}'
+    return f'{self.name}'
 
   def __new__(cls, *args, **kwargs):
     value = len(cls.__members__) + 1
     obj = object.__new__(cls)
     obj._value_ = value
     return obj
 
@@ -154,15 +151,15 @@
         Mapping[str, Any]: the json representation of the widget
     """
     if getattr(self, '__SUPPRESS_TAG__', False):
       return self.to_dict()
 
     render = {
         (getattr(self, '__OVERRIDE_TAG__', False) or
-          stringcase.camelcase(self.__class__.__name__)): self.to_dict()}
+         stringcase.camelcase(self.__class__.__name__)): self.to_dict()}
     properties = inspect.getmembers(self.__class__,
                                     lambda v: isinstance(v, property))
     for (name, value) in properties:
       if widget_value := value.fget(self):
         render[stringcase.camelcase(name)] = widget_value
 
     return render
```

### Comparing `python-card-framework-1.0.0/card_framework/__init_test.py` & `python-card-framework-1.0.1/card_framework/__init_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,78 +11,63 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import unittest
 from dataclasses import Field, dataclass
-from typing import List
+from typing import Callable, List
 
 from dataclasses_json import dataclass_json
 
 from card_framework import *
 from card_framework.v2.action_response import ActionResponse
 from card_framework.v2.action_status import ActionStatus
 
 
-class LazyPropertyTest(unittest.TestCase):
-  class Foo(object):
-    @lazy_property
-    def thing(self) -> str:
-      return 'lazy'
-
-  def test_lazy_thing(self):
-    foo = LazyPropertyTest.Foo()
-    self.assertFalse(hasattr(foo, 'lazy_thing'))
-    self.assertEqual('lazy', foo.thing)
-    self.assertTrue(hasattr(foo, '_lazy_thing'))
-    with self.assertRaises(AttributeError):
-      foo.thing = 'bar'
-
-
 class TestEnum(enum.Enum):
   ONE = enum.auto()
   TWO = enum.auto()
 
 
 class MetadataTest(unittest.TestCase):
   def test_simple_update(self) -> None:
     base = {'pirate': 'Westley'}
 
-    updated = metadata(base=base, pirate='Dread Pirate Roberts')
+    updated =merge_metadata(base=base, pirate='Dread Pirate Roberts')
 
     self.assertDictEqual(updated, {'pirate': 'Dread Pirate Roberts'})
 
   def test_remove(self) -> None:
     base = {'pirate': 'Dread Pirate Roberts', 'swordsman': 'Inigo Montoya'}
 
-    updated = metadata(base=base, swordsman=None)
+    updated = merge_metadata(base=base, swordsman=None)
 
     self.assertDictEqual(updated, {'pirate': 'Dread Pirate Roberts'})
 
   def test_add(self) -> None:
     base = {'pirate': 'Dread Pirate Roberts', }
 
-    updated = metadata(base=base, swordsman='Inigo Montoya')
+    updated = merge_metadata(base=base, swordsman='Inigo Montoya')
 
     self.assertDictEqual(updated, {'pirate': 'Dread Pirate Roberts',
                                    'swordsman': 'Inigo Montoya'})
 
   def test_add_and_remove(self) -> None:
     base = {'pirate': 'Dread Pirate Roberts', 'strongman': 'Fezzik'}
 
-    updated = metadata(base=base, swordsman='Inigo Montoya', strongman=None)
+    updated = merge_metadata(base=base, swordsman='Inigo Montoya', strongman=None)
 
     self.assertDictEqual(updated, {'pirate': 'Dread Pirate Roberts',
                                    'swordsman': 'Inigo Montoya'})
 
   def test_add_update_and_remove(self) -> None:
     base = {'pirate': 'Westley', 'strongman': 'Fezzik'}
 
-    updated = metadata(base=base, swordsman='Inigo Montoya', strongman=None,
+    updated = merge_metadata(base=base, swordsman='Inigo Montoya', strongman=None,
                        pirate='Dread Pirate Roberts')
 
     self.assertDictEqual(updated, {'pirate': 'Dread Pirate Roberts',
                                    'swordsman': 'Inigo Montoya'})
 
 
 class StandardFieldTest(unittest.TestCase):
```

### Comparing `python-card-framework-1.0.0/card_framework/v2/__init__.py` & `python-card-framework-1.0.1/card_framework/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/action_response.py` & `python-card-framework-1.0.1/card_framework/v2/action_response.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/action_status.py` & `python-card-framework-1.0.1/card_framework/v2/action_status.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/annotation.py` & `python-card-framework-1.0.1/card_framework/v2/annotation.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/annotation_test.py` & `python-card-framework-1.0.1/card_framework/v2/annotation_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/attachment.py` & `python-card-framework-1.0.1/card_framework/v2/attachment.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/card.py` & `python-card-framework-1.0.1/card_framework/v2/card.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/card_action.py` & `python-card-framework-1.0.1/card_framework/v2/card_action.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/card_fixed_footer.py` & `python-card-framework-1.0.1/card_framework/v2/card_fixed_footer.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/card_header.py` & `python-card-framework-1.0.1/card_framework/v2/card_header.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/card_header_test.py` & `python-card-framework-1.0.1/card_framework/v2/card_header_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/card_test.py` & `python-card-framework-1.0.1/card_framework/v2/card_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/dialog_action.py` & `python-card-framework-1.0.1/card_framework/v2/dialog_action.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/enums.py` & `python-card-framework-1.0.1/card_framework/v2/enums.py`

 * *Files 19% similar despite different names*

```diff
@@ -29,16 +29,11 @@
   SQUARE = ()
   CIRCLE = ()
 
 
 class HorizontalAlignment(AutoNumber):
   """HorizontalAlignment
   """
+  HORIZONTAL_ALIGNMENT_UNSPECIFIED = ()
   START = ()
   CENTER = ()
   END = ()
-
-  def __str__(self) -> str:
-    return self.name
-
-  def __repr__(self) -> str:
-    return str(self.name)
```

### Comparing `python-card-framework-1.0.0/card_framework/v2/message.py` & `python-card-framework-1.0.1/card_framework/v2/message.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/message_test.py` & `python-card-framework-1.0.1/card_framework/v2/message_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/section.py` & `python-card-framework-1.0.1/card_framework/v2/section.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/section_test.py` & `python-card-framework-1.0.1/card_framework/v2/section_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/space.py` & `python-card-framework-1.0.1/card_framework/v2/space.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/user.py` & `python-card-framework-1.0.1/card_framework/v2/user.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widget.py` & `python-card-framework-1.0.1/card_framework/v2/widget.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widget_test.py` & `python-card-framework-1.0.1/card_framework/v2/widget_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,7 +35,16 @@
 
   def test_valid_widget_render(self) -> None:
     widget = ValidWidget()
     widget.camel_case_property = 'Inigo Montoya'
     self.assertDictEqual(
         widget.render(),
         {'validWidget': {'camelCaseProperty': 'Inigo Montoya'}})
+
+  def test_aligned_widget_render(self) -> None:
+    widget = ValidWidget()
+    widget.camel_case_property = 'Inigo Montoya'
+    widget.horizontal_alignment = HorizontalAlignment.END
+    self.assertDictEqual(
+        widget.render(),
+        {'horizontalAlignment': 'END',
+         'validWidget': {'camelCaseProperty': 'Inigo Montoya'}})
```

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/__init__.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/action.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/action.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/button.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/button.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/button_list.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/button_list.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/button_test.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/button_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/color.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/color.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/color_test.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/color_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/decorated_text.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/decorated_text.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/divider.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/divider.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/divider_test.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/divider_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/grid.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/grid.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/icon.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/icon.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     TICKET = ()
     TRAIN = ()
     VIDEO_CAMERA = ()
     VIDEO_PLAY = ()
 
   alt_text: Optional[str] = standard_field()
   icon_url: Optional[str] = standard_field()
-  image_type: Optional[ImageType] = standard_field()
+  image_type: Optional[ImageType] = enum_field()
   known_icon: Optional[KnownIcon] = enum_field()
 
   def __setattr__(self, __name: str, __value: Any) -> None:
     """Sets attributes.
 
     This is overridden to ensure that one and only one of action and open_link
     can be set. If an attempt is made to set both, the already set one will be
```

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/icon_test.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/icon_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/image.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/image.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/image_test.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/image_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/on_click.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/on_click.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/on_click_test.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/on_click_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/open_link.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/open_link.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/selection_input.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/selection_input.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/selection_item.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/selection_item.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/suggestions.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/suggestions.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/switch_control.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/switch_control.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/text_input.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/text_input.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/text_input_test.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/text_input_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/text_paragraph.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/text_paragraph.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/card_framework/v2/widgets/text_paragraph_test.py` & `python-card-framework-1.0.1/card_framework/v2/widgets/text_paragraph_test.py`

 * *Files identical despite different names*

### Comparing `python-card-framework-1.0.0/python_card_framework.egg-info/PKG-INFO` & `python-card-framework-1.0.1/python_card_framework.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Metadata-Version: 2.1
 Name: python-card-framework
-Version: 1.0.0
+Version: 1.0.1
 Summary: API for rendering Chat App Card json.
-Home-page: https://github.com/google/python-card-framework
-Author: David Harcombe
-Author-email: davidharcombe@google.com
+Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: License :: OSI Approved :: Apache Software License
+Project-URL: Homepage, https://github.com/google/python-card-framework
+Project-URL: Bug Tracker, https://github.com/google/python-card-framework/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Card Framework
 
 This is a library designed to allow Python developers to treat the Chat API
@@ -76,9 +71,7 @@
                     image_url='https://source.unsplash.com/featured320x180?nature&sig=8')
 card = Card(header=header, sections=[Section(widgets=widgets)])
 
 return Message(cards=[card]).render()
 ```
 
 which will return the correct JSON.
-
-
```

### Comparing `python-card-framework-1.0.0/python_card_framework.egg-info/SOURCES.txt` & `python-card-framework-1.0.1/python_card_framework.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 README.md
-setup.py
+pyproject.toml
 card_framework/__init__.py
 card_framework/__init_test.py
 card_framework/v2/__init__.py
 card_framework/v2/action_response.py
 card_framework/v2/action_status.py
 card_framework/v2/annotation.py
 card_framework/v2/annotation_test.py
@@ -28,14 +28,16 @@
 card_framework/v2/widgets/__init__.py
 card_framework/v2/widgets/action.py
 card_framework/v2/widgets/button.py
 card_framework/v2/widgets/button_list.py
 card_framework/v2/widgets/button_test.py
 card_framework/v2/widgets/color.py
 card_framework/v2/widgets/color_test.py
+card_framework/v2/widgets/date_time_picker.py
+card_framework/v2/widgets/date_time_picker_test.py
 card_framework/v2/widgets/decorated_text.py
 card_framework/v2/widgets/divider.py
 card_framework/v2/widgets/divider_test.py
 card_framework/v2/widgets/grid.py
 card_framework/v2/widgets/icon.py
 card_framework/v2/widgets/icon_test.py
 card_framework/v2/widgets/image.py
@@ -50,10 +52,9 @@
 card_framework/v2/widgets/text_input.py
 card_framework/v2/widgets/text_input_test.py
 card_framework/v2/widgets/text_paragraph.py
 card_framework/v2/widgets/text_paragraph_test.py
 python_card_framework.egg-info/PKG-INFO
 python_card_framework.egg-info/SOURCES.txt
 python_card_framework.egg-info/dependency_links.txt
-python_card_framework.egg-info/not-zip-safe
 python_card_framework.egg-info/requires.txt
 python_card_framework.egg-info/top_level.txt
```

