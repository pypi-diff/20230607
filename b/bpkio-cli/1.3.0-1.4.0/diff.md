# Comparing `tmp/bpkio_cli-1.3.0.tar.gz` & `tmp/bpkio_cli-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpkio_cli-1.3.0.tar", max compression
+gzip compressed data, was "bpkio_cli-1.4.0.tar", max compression
```

## Comparing `bpkio_cli-1.3.0.tar` & `bpkio_cli-1.4.0.tar`

### file list

```diff
@@ -1,67 +1,68 @@
--rw-r--r--   0        0        0        0 2023-03-28 20:04:37.409875 bpkio_cli-1.3.0/README.md
--rw-r--r--   0        0        0       22 2023-06-05 14:47:30.710905 bpkio_cli-1.3.0/bpkio_cli/__init__.py
--rw-r--r--   0        0        0     3812 2023-05-24 04:05:57.379943 bpkio_cli-1.3.0/bpkio_cli/app.py
--rw-r--r--   0        0        0       91 2023-04-29 21:05:12.410693 bpkio_cli-1.3.0/bpkio_cli/click_mods/__init__.py
--rw-r--r--   0        0        0      771 2023-05-24 04:19:18.738931 bpkio_cli-1.3.0/bpkio_cli/click_mods/default_last_command.py
--rw-r--r--   0        0        0     5145 2023-06-01 09:13:30.452845 bpkio_cli-1.3.0/bpkio_cli/click_mods/group_rest_resource.py
--rw-r--r--   0        0        0     1747 2023-03-23 13:12:03.515867 bpkio_cli-1.3.0/bpkio_cli/click_mods/option_eat_all.py
--rw-r--r--   0        0        0      599 2023-05-21 21:17:36.965795 bpkio_cli-1.3.0/bpkio_cli/click_options/__init__.py
--rw-r--r--   0        0        0      848 2023-05-17 22:07:10.594805 bpkio_cli-1.3.0/bpkio_cli/click_options/admin.py
--rw-r--r--   0        0        0      355 2023-05-12 19:07:07.722647 bpkio_cli-1.3.0/bpkio_cli/click_options/json.py
--rw-r--r--   0        0        0      958 2023-05-12 07:26:58.744571 bpkio_cli-1.3.0/bpkio_cli/click_options/list.py
--rw-r--r--   0        0        0      933 2023-04-27 14:26:01.185185 bpkio_cli-1.3.0/bpkio_cli/click_options/poll.py
--rw-r--r--   0        0        0      851 2023-05-23 10:02:17.547439 bpkio_cli-1.3.0/bpkio_cli/click_options/read.py
--rw-r--r--   0        0        0     1183 2023-04-27 14:26:01.185667 bpkio_cli-1.3.0/bpkio_cli/click_options/search.py
--rw-r--r--   0        0        0      445 2023-05-04 18:13:29.662132 bpkio_cli-1.3.0/bpkio_cli/click_options/table.py
--rw-r--r--   0        0        0     1161 2023-05-22 16:50:12.003620 bpkio_cli-1.3.0/bpkio_cli/click_options/urls.py
--rw-r--r--   0        0        0      656 2023-05-21 21:48:40.162730 bpkio_cli-1.3.0/bpkio_cli/commands/__init__.py
--rw-r--r--   0        0        0      751 2023-05-21 21:49:06.651917 bpkio_cli-1.3.0/bpkio_cli/commands/addons.py
--rw-r--r--   0        0        0     4878 2023-06-01 13:43:54.231560 bpkio_cli-1.3.0/bpkio_cli/commands/configure.py
--rw-r--r--   0        0        0     1758 2023-04-28 08:13:42.029805 bpkio_cli-1.3.0/bpkio_cli/commands/consumption.py
--rw-r--r--   0        0        0     4388 2023-05-23 21:27:26.436574 bpkio_cli-1.3.0/bpkio_cli/commands/creators/ad_insertion.py
--rw-r--r--   0        0        0     7930 2023-05-23 21:19:19.179090 bpkio_cli-1.3.0/bpkio_cli/commands/creators/sources.py
--rw-r--r--   0        0        0     4064 2023-05-22 08:49:01.223413 bpkio_cli-1.3.0/bpkio_cli/commands/creators/virtual_channel.py
--rw-r--r--   0        0        0     8808 2023-05-21 21:14:37.474798 bpkio_cli-1.3.0/bpkio_cli/commands/creators/virtual_channel_populate.py
--rw-r--r--   0        0        0      761 2023-05-21 21:14:37.453890 bpkio_cli-1.3.0/bpkio_cli/commands/hello.py
--rw-r--r--   0        0        0     1251 2023-05-21 21:14:37.453903 bpkio_cli-1.3.0/bpkio_cli/commands/memory.py
--rw-r--r--   0        0        0     3118 2023-05-21 21:14:37.453880 bpkio_cli-1.3.0/bpkio_cli/commands/package.py
--rw-r--r--   0        0        0     9969 2023-05-23 22:13:49.593225 bpkio_cli-1.3.0/bpkio_cli/commands/profiles.py
--rw-r--r--   0        0        0     2700 2023-05-21 20:35:26.716484 bpkio_cli-1.3.0/bpkio_cli/commands/recorder.py
--rw-r--r--   0        0        0     3669 2023-06-01 13:42:32.164671 bpkio_cli-1.3.0/bpkio_cli/commands/services.py
--rw-r--r--   0        0        0     7952 2023-06-01 13:44:49.316974 bpkio_cli-1.3.0/bpkio_cli/commands/sources.py
--rw-r--r--   0        0        0    18465 2023-06-02 14:22:43.378526 bpkio_cli-1.3.0/bpkio_cli/commands/template_crud.py
--rw-r--r--   0        0        0     7306 2023-05-21 21:17:10.206971 bpkio_cli-1.3.0/bpkio_cli/commands/template_crud_slots.py
--rw-r--r--   0        0        0      332 2023-04-28 08:33:05.100937 bpkio_cli-1.3.0/bpkio_cli/commands/tenants.py
--rw-r--r--   0        0        0     5477 2023-05-22 16:05:47.390346 bpkio_cli-1.3.0/bpkio_cli/commands/url.py
--rw-r--r--   0        0        0      359 2023-04-28 08:33:22.939414 bpkio_cli-1.3.0/bpkio_cli/commands/users.py
--rw-r--r--   0        0        0     1036 2023-05-22 17:10:47.554934 bpkio_cli-1.3.0/bpkio_cli/core/app_context.py
--rw-r--r--   0        0        0     3753 2023-05-24 04:10:19.009730 bpkio_cli-1.3.0/bpkio_cli/core/config_provider.py
--rw-r--r--   0        0        0      135 2023-04-20 16:43:38.934392 bpkio_cli-1.3.0/bpkio_cli/core/exceptions.py
--rw-r--r--   0        0        0     2565 2023-05-24 04:11:25.852254 bpkio_cli-1.3.0/bpkio_cli/core/initialize.py
--rw-r--r--   0        0        0     1718 2023-04-07 16:07:08.180945 bpkio_cli-1.3.0/bpkio_cli/core/logger.py
--rw-r--r--   0        0        0     8783 2023-05-19 21:18:11.983457 bpkio_cli-1.3.0/bpkio_cli/core/packager.py
--rw-r--r--   0        0        0     8775 2023-05-22 09:50:46.909212 bpkio_cli-1.3.0/bpkio_cli/core/resource_recorder.py
--rw-r--r--   0        0        0     2204 2023-05-21 21:15:26.397241 bpkio_cli-1.3.0/bpkio_cli/core/resource_trail.py
--rw-r--r--   0        0        0     5128 2023-05-16 19:08:30.137349 bpkio_cli-1.3.0/bpkio_cli/core/response_handler.py
--rw-r--r--   0        0        0     1234 2023-05-21 20:37:15.106665 bpkio_cli-1.3.0/bpkio_cli/core/session_recorder.py
--rw-r--r--   0        0        0      395 2023-05-21 21:21:56.973900 bpkio_cli-1.3.0/bpkio_cli/utils/__init__.py
--rw-r--r--   0        0        0     2288 2023-05-12 07:34:26.643986 bpkio_cli-1.3.0/bpkio_cli/utils/arrays.py
--rw-r--r--   0        0        0     1358 2023-05-19 19:23:50.776214 bpkio_cli-1.3.0/bpkio_cli/utils/datetimes.py
--rw-r--r--   0        0        0     1828 2023-05-21 21:21:56.974288 bpkio_cli-1.3.0/bpkio_cli/utils/editor.py
--rw-r--r--   0        0        0      476 2023-05-19 16:10:53.950053 bpkio_cli-1.3.0/bpkio_cli/utils/inquirer_defaults.py
--rw-r--r--   0        0        0      136 2023-04-14 20:15:18.159888 bpkio_cli-1.3.0/bpkio_cli/utils/json.py
--rw-r--r--   0        0        0      567 2023-04-29 21:58:38.435162 bpkio_cli-1.3.0/bpkio_cli/utils/profile_maker.py
--rw-r--r--   0        0        0     8758 2023-06-02 14:32:29.030983 bpkio_cli-1.3.0/bpkio_cli/utils/url_builders.py
--rw-r--r--   0        0        0      861 2023-05-22 14:30:20.340741 bpkio_cli-1.3.0/bpkio_cli/utils/urls.py
--rw-r--r--   0        0        0     1034 2023-05-24 04:10:59.495781 bpkio_cli-1.3.0/bpkio_cli/writers/breadcrumbs.py
--rw-r--r--   0        0        0     1404 2023-05-02 20:19:18.033992 bpkio_cli-1.3.0/bpkio_cli/writers/colorizer.py
--rw-r--r--   0        0        0     4503 2023-05-23 20:32:04.036975 bpkio_cli-1.3.0/bpkio_cli/writers/content_display.py
--rw-r--r--   0        0        0      840 2023-04-26 12:03:04.848088 bpkio_cli-1.3.0/bpkio_cli/writers/diff.py
--rw-r--r--   0        0        0      152 2023-04-26 12:03:04.848777 bpkio_cli-1.3.0/bpkio_cli/writers/formatter.py
--rw-r--r--   0        0        0     4533 2023-05-09 10:21:54.315733 bpkio_cli-1.3.0/bpkio_cli/writers/hls_formatter.py
--rw-r--r--   0        0        0      714 2023-05-21 21:21:56.975414 bpkio_cli-1.3.0/bpkio_cli/writers/json_formatter.py
--rw-r--r--   0        0        0     1674 2023-05-22 15:17:28.335555 bpkio_cli-1.3.0/bpkio_cli/writers/players.py
--rw-r--r--   0        0        0     1865 2023-05-12 07:26:12.170387 bpkio_cli-1.3.0/bpkio_cli/writers/tables.py
--rw-r--r--   0        0        0     5205 2023-04-26 12:03:04.849885 bpkio_cli-1.3.0/bpkio_cli/writers/xml_formatter.py
--rw-r--r--   0        0        0     1220 2023-06-05 14:47:30.709930 bpkio_cli-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      929 1970-01-01 00:00:00.000000 bpkio_cli-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 14:52:28.912688 bpkio_cli-1.4.0/README.md
+-rw-r--r--   0        0        0       22 2023-06-07 15:39:48.699204 bpkio_cli-1.4.0/bpkio_cli/__init__.py
+-rw-r--r--   0        0        0     3871 2023-06-07 13:10:56.410462 bpkio_cli-1.4.0/bpkio_cli/app.py
+-rw-r--r--   0        0        0       91 2023-06-05 14:52:28.913801 bpkio_cli-1.4.0/bpkio_cli/click_mods/__init__.py
+-rw-r--r--   0        0        0      771 2023-06-05 14:52:28.914515 bpkio_cli-1.4.0/bpkio_cli/click_mods/default_last_command.py
+-rw-r--r--   0        0        0     5145 2023-06-05 14:52:28.915057 bpkio_cli-1.4.0/bpkio_cli/click_mods/group_rest_resource.py
+-rw-r--r--   0        0        0     1747 2023-06-05 14:52:28.915564 bpkio_cli-1.4.0/bpkio_cli/click_mods/option_eat_all.py
+-rw-r--r--   0        0        0      599 2023-06-05 14:52:28.916268 bpkio_cli-1.4.0/bpkio_cli/click_options/__init__.py
+-rw-r--r--   0        0        0      848 2023-06-05 14:52:28.916749 bpkio_cli-1.4.0/bpkio_cli/click_options/admin.py
+-rw-r--r--   0        0        0      355 2023-06-05 14:52:28.917214 bpkio_cli-1.4.0/bpkio_cli/click_options/json.py
+-rw-r--r--   0        0        0      958 2023-06-05 14:52:28.917874 bpkio_cli-1.4.0/bpkio_cli/click_options/list.py
+-rw-r--r--   0        0        0      933 2023-06-05 14:52:28.918220 bpkio_cli-1.4.0/bpkio_cli/click_options/poll.py
+-rw-r--r--   0        0        0      845 2023-06-06 10:33:40.520475 bpkio_cli-1.4.0/bpkio_cli/click_options/read.py
+-rw-r--r--   0        0        0     1183 2023-06-05 14:52:28.919379 bpkio_cli-1.4.0/bpkio_cli/click_options/search.py
+-rw-r--r--   0        0        0      445 2023-06-05 14:52:28.919891 bpkio_cli-1.4.0/bpkio_cli/click_options/table.py
+-rw-r--r--   0        0        0     1161 2023-06-05 14:52:28.920409 bpkio_cli-1.4.0/bpkio_cli/click_options/urls.py
+-rw-r--r--   0        0        0      656 2023-06-05 14:52:28.920820 bpkio_cli-1.4.0/bpkio_cli/commands/__init__.py
+-rw-r--r--   0        0        0      751 2023-06-05 14:52:28.921064 bpkio_cli-1.4.0/bpkio_cli/commands/addons.py
+-rw-r--r--   0        0        0     5246 2023-06-07 13:11:32.107723 bpkio_cli-1.4.0/bpkio_cli/commands/configure.py
+-rw-r--r--   0        0        0     1766 2023-06-07 08:50:23.685205 bpkio_cli-1.4.0/bpkio_cli/commands/consumption.py
+-rw-r--r--   0        0        0     4379 2023-06-05 19:39:32.652087 bpkio_cli-1.4.0/bpkio_cli/commands/creators/ad_insertion.py
+-rw-r--r--   0        0        0     7921 2023-06-05 19:39:32.652047 bpkio_cli-1.4.0/bpkio_cli/commands/creators/sources.py
+-rw-r--r--   0        0        0     4055 2023-06-05 19:39:32.651893 bpkio_cli-1.4.0/bpkio_cli/commands/creators/virtual_channel.py
+-rw-r--r--   0        0        0     8799 2023-06-05 19:39:32.651985 bpkio_cli-1.4.0/bpkio_cli/commands/creators/virtual_channel_populate.py
+-rw-r--r--   0        0        0      761 2023-06-05 14:52:28.924009 bpkio_cli-1.4.0/bpkio_cli/commands/hello.py
+-rw-r--r--   0        0        0     1251 2023-06-05 14:52:28.924268 bpkio_cli-1.4.0/bpkio_cli/commands/memory.py
+-rw-r--r--   0        0        0     3444 2023-06-07 13:33:49.992001 bpkio_cli-1.4.0/bpkio_cli/commands/package.py
+-rw-r--r--   0        0        0    10213 2023-06-07 15:09:40.408861 bpkio_cli-1.4.0/bpkio_cli/commands/profiles.py
+-rw-r--r--   0        0        0     2700 2023-06-05 14:52:28.925148 bpkio_cli-1.4.0/bpkio_cli/commands/recorder.py
+-rw-r--r--   0        0        0     3669 2023-06-05 14:52:28.925467 bpkio_cli-1.4.0/bpkio_cli/commands/services.py
+-rw-r--r--   0        0        0     5728 2023-06-06 14:52:14.895415 bpkio_cli-1.4.0/bpkio_cli/commands/sources.py
+-rw-r--r--   0        0        0    18471 2023-06-06 10:33:54.312903 bpkio_cli-1.4.0/bpkio_cli/commands/template_crud.py
+-rw-r--r--   0        0        0     7306 2023-06-05 14:52:28.926463 bpkio_cli-1.4.0/bpkio_cli/commands/template_crud_slots.py
+-rw-r--r--   0        0        0      332 2023-06-05 14:52:28.926844 bpkio_cli-1.4.0/bpkio_cli/commands/tenants.py
+-rw-r--r--   0        0        0     5477 2023-06-05 14:52:28.927171 bpkio_cli-1.4.0/bpkio_cli/commands/url.py
+-rw-r--r--   0        0        0      359 2023-06-05 14:52:28.927398 bpkio_cli-1.4.0/bpkio_cli/commands/users.py
+-rw-r--r--   0        0        0     1036 2023-06-05 14:52:28.927822 bpkio_cli-1.4.0/bpkio_cli/core/app_context.py
+-rw-r--r--   0        0        0     3753 2023-06-05 14:52:28.928412 bpkio_cli-1.4.0/bpkio_cli/core/config_provider.py
+-rw-r--r--   0        0        0      135 2023-06-05 14:52:28.928924 bpkio_cli-1.4.0/bpkio_cli/core/exceptions.py
+-rw-r--r--   0        0        0     2565 2023-06-05 14:52:28.929158 bpkio_cli-1.4.0/bpkio_cli/core/initialize.py
+-rw-r--r--   0        0        0     1718 2023-06-05 14:52:28.929630 bpkio_cli-1.4.0/bpkio_cli/core/logger.py
+-rw-r--r--   0        0        0     8332 2023-06-07 15:35:22.116286 bpkio_cli-1.4.0/bpkio_cli/core/packager.py
+-rw-r--r--   0        0        0     9358 2023-06-07 13:33:12.629695 bpkio_cli-1.4.0/bpkio_cli/core/resource_recorder.py
+-rw-r--r--   0        0        0     2204 2023-06-05 14:52:28.930943 bpkio_cli-1.4.0/bpkio_cli/core/resource_trail.py
+-rw-r--r--   0        0        0     5128 2023-06-05 14:52:28.931598 bpkio_cli-1.4.0/bpkio_cli/core/response_handler.py
+-rw-r--r--   0        0        0     1234 2023-06-05 14:52:28.931905 bpkio_cli-1.4.0/bpkio_cli/core/session_recorder.py
+-rw-r--r--   0        0        0      395 2023-06-05 14:52:28.932292 bpkio_cli-1.4.0/bpkio_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2288 2023-06-05 14:52:28.932584 bpkio_cli-1.4.0/bpkio_cli/utils/arrays.py
+-rw-r--r--   0        0        0     1358 2023-06-05 14:52:28.932885 bpkio_cli-1.4.0/bpkio_cli/utils/datetimes.py
+-rw-r--r--   0        0        0     1828 2023-06-05 14:52:28.933224 bpkio_cli-1.4.0/bpkio_cli/utils/editor.py
+-rw-r--r--   0        0        0      494 2023-06-05 19:39:43.849589 bpkio_cli-1.4.0/bpkio_cli/utils/inquirer.py
+-rw-r--r--   0        0        0      136 2023-06-05 14:52:28.933905 bpkio_cli-1.4.0/bpkio_cli/utils/json.py
+-rw-r--r--   0        0        0      567 2023-06-05 14:52:28.934214 bpkio_cli-1.4.0/bpkio_cli/utils/profile_maker.py
+-rw-r--r--   0        0        0    11802 2023-06-06 06:32:34.505189 bpkio_cli-1.4.0/bpkio_cli/utils/url_builders.py
+-rw-r--r--   0        0        0      861 2023-06-05 14:52:28.934866 bpkio_cli-1.4.0/bpkio_cli/utils/urls.py
+-rw-r--r--   0        0        0     1034 2023-06-05 14:52:28.935214 bpkio_cli-1.4.0/bpkio_cli/writers/breadcrumbs.py
+-rw-r--r--   0        0        0     1667 2023-06-06 07:59:33.797067 bpkio_cli-1.4.0/bpkio_cli/writers/colorizer.py
+-rw-r--r--   0        0        0     5213 2023-06-06 14:37:01.564679 bpkio_cli-1.4.0/bpkio_cli/writers/content_display.py
+-rw-r--r--   0        0        0      840 2023-06-05 14:52:28.936348 bpkio_cli-1.4.0/bpkio_cli/writers/diff.py
+-rw-r--r--   0        0        0      751 2023-06-06 10:33:05.139814 bpkio_cli-1.4.0/bpkio_cli/writers/formatter.py
+-rw-r--r--   0        0        0     5364 2023-06-06 14:30:13.177404 bpkio_cli-1.4.0/bpkio_cli/writers/hls_formatter.py
+-rw-r--r--   0        0        0      714 2023-06-05 14:52:28.938409 bpkio_cli-1.4.0/bpkio_cli/writers/json_formatter.py
+-rw-r--r--   0        0        0     1665 2023-06-05 19:39:32.651931 bpkio_cli-1.4.0/bpkio_cli/writers/players.py
+-rw-r--r--   0        0        0     1631 2023-06-06 14:40:13.522055 bpkio_cli-1.4.0/bpkio_cli/writers/scte35.py
+-rw-r--r--   0        0        0     1865 2023-06-05 14:52:28.939530 bpkio_cli-1.4.0/bpkio_cli/writers/tables.py
+-rw-r--r--   0        0        0     5368 2023-06-06 10:21:02.754933 bpkio_cli-1.4.0/bpkio_cli/writers/xml_formatter.py
+-rw-r--r--   0        0        0     1243 2023-06-07 15:39:48.698279 bpkio_cli-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 bpkio_cli-1.4.0/PKG-INFO
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/app.py` & `bpkio_cli-1.4.0/bpkio_cli/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,25 +73,25 @@
 def bic(ctx, tenant, log_level, log_sdk, use_cache, use_prompts):
     if log_level or LOG_LEVEL:
         set_console_logging_level(
             log_level or LOG_LEVEL, include_sdk=log_sdk or LOG_SDK
         )
 
     requires_api = True
-    if ctx.invoked_subcommand in ["init", "config", "record"]:
+    if ctx.invoked_subcommand in ["init", "configure", "record"]:
         requires_api = False
 
     app_context = initialize(
         tenant=tenant,
         use_cache=use_cache,
         use_prompts=use_prompts,
         requires_api=requires_api,
     )
 
-    if app_context:
+    if app_context and ctx.invoked_subcommand not in ["init", "configure"]:
         display_tenant_info(app_context.tenant)
 
     # TODO - validate the token in the initialisation of BroadpeakApi
     ctx.obj = app_context
 
     @ctx.call_on_close
     def close_cleanly():
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/click_mods/default_last_command.py` & `bpkio_cli-1.4.0/bpkio_cli/click_mods/default_last_command.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/click_mods/group_rest_resource.py` & `bpkio_cli-1.4.0/bpkio_cli/click_mods/group_rest_resource.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/click_mods/option_eat_all.py` & `bpkio_cli-1.4.0/bpkio_cli/click_mods/option_eat_all.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/click_options/__init__.py` & `bpkio_cli-1.4.0/bpkio_cli/click_options/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/click_options/admin.py` & `bpkio_cli-1.4.0/bpkio_cli/click_options/admin.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/click_options/list.py` & `bpkio_cli-1.4.0/bpkio_cli/click_options/list.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/click_options/poll.py` & `bpkio_cli-1.4.0/bpkio_cli/click_options/poll.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/click_options/read.py` & `bpkio_cli-1.4.0/bpkio_cli/click_options/read.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,18 +9,18 @@
         "--raw",
         is_flag=True,
         type=bool,
         default=False,
         help="Get the raw content, unchanged",
     )
     @click.option(
-        "--top", type=int, default=None, help="Only display the first N lines"
+        "--top", type=int, default=0, help="Only display the first N lines"
     )
     @click.option(
-        "--tail", type=int, default=None, help="Only display the last N lines"
+        "--tail", type=int, default=0, help="Only display the last N lines"
     )
     @click.option(
         "--pager/--no-pager",
         type=bool,
         is_flag=True,
         default=None,
         help="Display through a pager (to allow scrolling). If the flag is not set, a pager will automatically be used if the content is too long to fit on screen",
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/click_options/search.py` & `bpkio_cli-1.4.0/bpkio_cli/click_options/search.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/click_options/urls.py` & `bpkio_cli-1.4.0/bpkio_cli/click_options/urls.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/commands/__init__.py` & `bpkio_cli-1.4.0/bpkio_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/commands/addons.py` & `bpkio_cli-1.4.0/bpkio_cli/commands/addons.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/commands/configure.py` & `bpkio_cli-1.4.0/bpkio_cli/commands/configure.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import click
 import cloup
 from bpkio_api.api import DEFAULT_FQDN, BroadpeakIoApi
 from bpkio_api.credential_provider import TenantProfileProvider
 from InquirerPy import inquirer
 
+from bpkio_cli.click_mods.option_eat_all import OptionEatAll
 from bpkio_cli.commands.hello import hello
 from bpkio_cli.core.config_provider import ConfigProvider
 from bpkio_cli.core.initialize import initialize
 from bpkio_cli.core.response_handler import ResponseHandler
 
 
 # Command: INIT
@@ -60,19 +61,29 @@
 @click.pass_obj
 def tenants(obj):
     pass
 
 
 # Command: LIST
 @tenants.command(help="List the tenants previously configured", aliases=["ls"])
-def list():
+@click.option(
+    "-s",
+    "--sort",
+    "sort_fields",
+    cls=OptionEatAll,
+    type=tuple,
+    help="List of fields used to sort the list. Append ':desc' to sort in descending order",
+)
+def list(sort_fields):
     cp = TenantProfileProvider()
     tenants = cp.list_tenants()
     ResponseHandler().treat_list_resources(
-        resources=tenants, select_fields=["label", "id", "fqdn"]
+        resources=tenants,
+        select_fields=["label", "id", "fqdn"],
+        sort_fields=sort_fields,
     )
 
 
 # Command: SWITCH
 @tenants.command(help="Switch the tenant used for subsequent invocations")
 @click.argument("tenant", required=False)
 @click.pass_context
@@ -107,14 +118,15 @@
         validate=lambda candidate: BroadpeakIoApi.is_valid_api_key_format(candidate),
         invalid_message="Invalid API Key",
     ).execute()
     fqdn = inquirer.text(
         message="Application domain name",
         default=DEFAULT_FQDN,
         validate=lambda url: BroadpeakIoApi.is_correct_entrypoint(url, api_key),
+        filter=lambda url: BroadpeakIoApi.normalise_fqdn(url),
         invalid_message=(
             "This URL does not appear to be a broadpeak.io application, "
             "or your API key does not give you access to it"
         ),
     ).execute()
 
     # Test the API key by initialising the API with it
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/commands/consumption.py` & `bpkio_cli-1.4.0/bpkio_cli/commands/consumption.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         return
 
     else:
         ranges = get_utc_date_ranges(from_time=start, to_time=end, unit=by)
         data = []
         for start, end in ranges:
             # data.append(obj.api.consumption.retrieve(start, end, tenant))
-            data.append(obj.api.consumption.retrieve(start, end))
+            data.append(obj.api.consumption.retrieve(start, end, tenant))
 
         obj.response_handler.treat_list_resources(
             data,
             select_fields=[
                 "tenantId",
                 "startTime",
                 "endTime",
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/commands/creators/ad_insertion.py` & `bpkio_cli-1.4.0/bpkio_cli/commands/creators/ad_insertion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 import cloup
 import InquirerPy.inquirer as inquirer
 from bpkio_api.models import AdInsertionServiceIn, SourceType
 
-import bpkio_cli.utils.inquirer_defaults as inqdef
+import bpkio_cli.utils.inquirer as inqdef
 from bpkio_cli.core.app_context import AppContext
 
 
 def create_ad_insertion_service_command():
     # COMMAND: CREATE
     @cloup.command(help="Create a (simple) Ad Insertion service")
     @click.pass_obj
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/commands/creators/sources.py` & `bpkio_cli-1.4.0/bpkio_cli/commands/creators/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     LiveSourceIn,
     SlateSourceIn,
     SourceType,
 )
 from InquirerPy import inquirer
 from InquirerPy.base.control import Choice
 
-import bpkio_cli.utils.inquirer_defaults as inqdef
+import bpkio_cli.utils.inquirer as inqdef
 from bpkio_cli.core.app_context import AppContext
 
 
 @cloup.command(
     help="Create a Source from just a URL. "
     "The CLI will work out what type of Source it is and create it accordingly"
 )
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/commands/creators/virtual_channel.py` & `bpkio_cli-1.4.0/bpkio_cli/commands/creators/virtual_channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 import cloup
 import InquirerPy.inquirer as inquirer
 from bpkio_api.models import SourceType, VirtualChannelServiceIn
 
-import bpkio_cli.utils.inquirer_defaults as inqdef
+import bpkio_cli.utils.inquirer as inqdef
 from bpkio_cli.core.app_context import AppContext
 
 
 def create_virtual_channel_service_command():
     # COMMAND: CREATE
     @cloup.command(help="Create a (simple) Virtual Channel service")
     @click.pass_obj
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/commands/creators/virtual_channel_populate.py` & `bpkio_cli-1.4.0/bpkio_cli/commands/creators/virtual_channel_populate.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     LiveSourceIn,
     SourceType,
     VirtualChannelService,
     VirtualChannelSlotIn,
     VirtualChannelSlotType,
 )
 
-import bpkio_cli.utils.inquirer_defaults as inqdef
+import bpkio_cli.utils.inquirer as inqdef
 from bpkio_cli.core.app_context import AppContext
 from bpkio_cli.utils.datetimes import (
     parse_date_expression_as_utc,
     parse_duration_expression,
 )
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/commands/hello.py` & `bpkio_cli-1.4.0/bpkio_cli/commands/hello.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/commands/memory.py` & `bpkio_cli-1.4.0/bpkio_cli/commands/memory.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/commands/package.py` & `bpkio_cli-1.4.0/bpkio_cli/commands/package.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,35 +27,41 @@
     default="$",
     required=False,
 )
 @cloup.option("-o", "--output", type=click.File("w"), required=False, default=None)
 @click.pass_obj
 def make(obj: AppContext, ref: str, output):
     if ref == "$":
-        resources = inquirer.checkbox(
+        resources = inquirer.fuzzy(
             message="What (top-level) resources do you want to include in the package?  ",
             choices=[
                 Choice(s, name=summary(s, with_class=True), enabled=(i == 0))
-                for i, s in enumerate(obj.cache.list_resources())
+                for i, s in enumerate(obj.cache.list_resources(models_only=True))
             ],
+            multiselect=True,
+            keybindings={"toggle": [{"key": "right"}]},
+            long_instruction="Keyboard: right arrow = select/unselect",
         ).execute()
 
     if ref == "@":
         list = inquirer.select(
             message="What list of resources to use?  ",
             multiselect=False,
             choices=[
                 Choice(lst, name=k, enabled=(i == 0))
                 for i, (k, lst) in enumerate(obj.cache.list_lists().items())
             ],
         ).execute()
 
-        resources = inquirer.checkbox(
+        resources = inquirer.fuzzy(
             message="What (top-level) resources do you want to include in the package?  ",
             choices=[Choice(s, name=summary(s, with_class=True)) for s in list],
+            multiselect=True,
+            keybindings={"toggle": [{"key": "right"}]},
+            long_instruction="Keyboard: right arrow = select/unselect",
         ).execute()
 
     if resources:
         package_resources(resources, obj.api, output)
 
 
 def package_resources(resources, api, output: click.File):
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/commands/profiles.py` & `bpkio_cli-1.4.0/bpkio_cli/commands/profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,27 @@
         admin_api = BroadpeakIoApi(tenant=admin_tenant)
         return admin_api.transcoding_profiles
 
 
 def get_profile_resource(tenant=None):
     ctx = click.get_current_context()
     id = ctx.obj.resources.last()
-    return ctx.obj.api.transcoding_profiles.retrieve(id, tenantId=tenant)
+    return ctx.obj.api.transcoding_profiles.retrieve(id, tenant_id=tenant)
+
+
+def create_profile_as_admin(profile, tenant=None, upsert=False):
+    if tenant:
+        profile.tenantId = tenant
+
+    # set the correct context to create the API
+    endpoint = get_admin_endpoint()
+    if upsert:
+        return endpoint.upsert(profile=profile, if_exists="retrieve", tenant_id=tenant)
+    else:
+        return endpoint.create(profile=profile)
 
 
 # # --- TRANSCODING PROFILES Group
 @cloup.group(
     cls=ApiResourceGroup,
     aliases=["prf", "profiles", "transcoding-profile"],
     show_subcommand_aliases=True,
@@ -91,15 +103,15 @@
 def lst(obj, json, select_fields, sort_fields, tenant):
     SessionRecorder.record(
         SessionSection(
             title="List of Transcoding Profiles", description="This is for a test"
         )
     )
 
-    profiles = obj.api.transcoding_profiles.list(tenantId=tenant)
+    profiles = obj.api.transcoding_profiles.list(tenant_id=tenant)
 
     obj.response_handler.treat_list_resources(
         profiles,
         select_fields=select_fields,
         sort_fields=sort_fields,
         json=json,
     )
@@ -170,15 +182,15 @@
 
         if content_only:
             profile = profile.json_content
 
         obj.response_handler.treat_single_resource(profile, json=True)
 
     except Exception:
-        profiles = obj.api.transcoding_profiles.list(tenantId=tenant)
+        profiles = obj.api.transcoding_profiles.list(tenant_id=tenant)
         if content_only:
             # TODO - Dirty code. Needs resolving, maybe at level of the SDK
             bare_profiles = []
             for profile in profiles:
                 new_pro = j.loads(profile.json())
                 new_pro["_expanded_content"] = profile.json_content
                 bare_profiles.append(new_pro)
@@ -225,36 +237,32 @@
 # --- CREATE Command
 @cloup.command(help="[ADMIN] Create a Transcoding Profile")
 @bic_options.tenant(required=True)
 @cloup.option("--from", "from_file", type=click.File("r"), required=False, default=None)
 @cloup.option("--name", type=str, required=False, default=None)
 @click.pass_obj
 def create(obj: AppContext, tenant: int, from_file, name: str):
-    # set the correct context to create the API
-    endpoint = get_admin_endpoint()
-
     # get the content of the profile
     if from_file:
         content = j.loads(from_file.read())
     else:
         content = get_profile_skeleton()
 
     payload = edit_payload(content, is_json=True)
     if not is_json(payload):
         raise ValueError("The content of the profile is not valid JSON")
 
     if not name:
         name = inquirer.text(message="Name: ").execute()
 
     # build the profile object for creation
-    tpro = TranscodingProfileIn(content=payload, name=name, tenantId=None)
-    if tenant:
-        tpro.tenantId = tenant
+    tpro = TranscodingProfileIn(content=payload, name=name, tenant_id=None)
+
+    out_profile = create_profile_as_admin(tpro, tenant)
 
-    out_profile = endpoint.create(profile=tpro)
     obj.response_handler.treat_single_resource(out_profile)
 
 
 # --- UPDATE Command
 @cloup.command(aliases=["put"], help="[ADMIN] Update a Transcoding Profile")
 @click.option(
     "-c",
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/commands/recorder.py` & `bpkio_cli-1.4.0/bpkio_cli/commands/recorder.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/commands/services.py` & `bpkio_cli-1.4.0/bpkio_cli/commands/services.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/commands/template_crud.py` & `bpkio_cli-1.4.0/bpkio_cli/commands/template_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,16 +354,16 @@
         def read(
             obj: AppContext,
             sub: int,
             url: str,
             fqdn: str,
             table: bool,
             raw: bool,
-            top: bool,
-            tail: bool,
+            top: int = 0,
+            tail: int = 0,
             header: bool = True,
             pager: bool = False,
         ):
             resource = retrieve_resource()
             handler = get_content_handler(
                 resource, replacement_fqdn=fqdn, extra_url=url, subplaylist_index=sub
             )
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/commands/template_crud_slots.py` & `bpkio_cli-1.4.0/bpkio_cli/commands/template_crud_slots.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/commands/url.py` & `bpkio_cli-1.4.0/bpkio_cli/commands/url.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/core/app_context.py` & `bpkio_cli-1.4.0/bpkio_cli/core/app_context.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/core/config_provider.py` & `bpkio_cli-1.4.0/bpkio_cli/core/config_provider.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/core/initialize.py` & `bpkio_cli-1.4.0/bpkio_cli/core/initialize.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/core/logger.py` & `bpkio_cli-1.4.0/bpkio_cli/core/logger.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/core/packager.py` & `bpkio_cli-1.4.0/bpkio_cli/core/packager.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 import bpkio_api.mappings as mappings
 import bpkio_api.models as models
 from bpkio_api.endpoints.enums import UpsertOperationType
 from bpkio_api.models.common import summary
 from pydantic import BaseModel
 
+from bpkio_cli.commands.profiles import create_profile_as_admin
+
 logger = logging.getLogger(__name__)
 
 
 class ResourcePackager:
     def __init__(self, api) -> None:
         self.api = api
         self.resources: List[models.BaseResource] = []
@@ -170,28 +172,19 @@
                 in_obj.name = in_obj.name + " " + self._suffix
 
             # Create it
             try:
                 message = ""
                 endpoint = mappings.model_to_endpoint(self.api, model=model)
 
-                # Special handling for objects that require admin access. We just check whether they exist (by name)
-                if instruction["model"] in ("TranscodingProfileIn"):
-                    resource_name = instruction["payload"]["name"]
-                    existing_resources = endpoint.search(
-                        value=resource_name, field="name"
+                # Special handling for objects that require admin access.
+                if instruction["model"] == "TranscodingProfileIn":
+                    (resource, status) = create_profile_as_admin(
+                        in_obj, self.api.get_tenant_id(), upsert=True
                     )
-                    if not len(existing_resources):
-                        raise Exception(
-                            f"The {instruction['model']} with name '{resource_name}' must "
-                            "already exist and cannot be automatically created by this script"
-                        )
-                    else:
-                        resource = existing_resources[0]
-                        status = 0
                 else:
                     if hasattr(endpoint, "upsert"):
                         (resource, status) = endpoint.upsert(
                             in_obj, if_exists="retrieve"
                         )
                     elif hasattr(endpoint, "create"):
                         resource = endpoint.create(in_obj)
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/core/resource_recorder.py` & `bpkio_cli-1.4.0/bpkio_cli/core/resource_recorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import pickle
 import re
 import tempfile
 from typing import List
 
+from pydantic import BaseModel
+
 from bpkio_cli.core.exceptions import BroadpeakIoCliError
 from bpkio_cli.core.logger import get_child_logger
 
 logger = get_child_logger(__name__)
 
 
 class ResourceRecorder:
@@ -154,17 +156,20 @@
             return list[position].id
         except IndexError:
             raise RecorderCacheError(
                 f"The list of resources of type {type_.__name__} currently "
                 f"in cache only contains {len(list)} resources"
             )
 
-    def list_resources(self):
+    def list_resources(self, models_only=False):
         """Return a list of all resources in the cache"""
-        return self._cache_singles.values()
+        resources = self._cache_singles.values()
+        if models_only:
+            resources = [r for r in resources if isinstance(r, BaseModel)]
+        return resources
 
     def list_lists(self):
         """Return a list of all lists in the cache"""
         return self._cache_lists
 
     def record_metadata(self, item, key, value):
         """Records metadata against an item"""
@@ -180,15 +185,25 @@
     def get_metadata(self, item, key):
         """Returns the metadata for an item"""
         item_key = item.summary
         if item_key in self._cache_metadata:
             lst: MoveToFrontList = self._cache_metadata[item_key].get(key)
             if lst:
                 return lst.values()
+        return None
 
+    def remove_metadata(self, item, key, value):
+        """Removes metadata for an item"""
+        item_key = item.summary
+        if item_key in self._cache_metadata:
+            lst: MoveToFrontList = self._cache_metadata[item_key].get(key)
+            if lst:
+                lst.remove(value)
+                self._cache_metadata[item_key][key] = lst
+                return lst
         return None
 
     def list_metadata(self):
         """Return a list of all metadata in the cache"""
         return self._cache_metadata
 
     def sort_resources_by_most_recently_accessed(self, original_list):
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/core/resource_trail.py` & `bpkio_cli-1.4.0/bpkio_cli/core/resource_trail.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/core/response_handler.py` & `bpkio_cli-1.4.0/bpkio_cli/core/response_handler.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/core/session_recorder.py` & `bpkio_cli-1.4.0/bpkio_cli/core/session_recorder.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/utils/arrays.py` & `bpkio_cli-1.4.0/bpkio_cli/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/utils/datetimes.py` & `bpkio_cli-1.4.0/bpkio_cli/utils/datetimes.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/utils/editor.py` & `bpkio_cli-1.4.0/bpkio_cli/utils/editor.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/utils/profile_maker.py` & `bpkio_cli-1.4.0/bpkio_cli/utils/profile_maker.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/utils/url_builders.py` & `bpkio_cli-1.4.0/bpkio_cli/utils/url_builders.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,19 +10,21 @@
     AssetCatalogSourceIn,
     BaseResource,
     SourceIn,
     SourceType,
     VirtualChannelService,
 )
 
-import bpkio_cli.utils.inquirer_defaults as inqdef
+import bpkio_cli.utils.inquirer as inqdef
 from bpkio_cli.core.app_context import AppContext
 from bpkio_cli.utils.urls import add_query_parameters, validate_ipv4_or_domain
 
 NEW = "-- add new --"
+DELETED = "__DELETED__"
+UNSET = "__UNSET__"
 
 
 def get_source_handler(
     source: SourceIn, extra_url: Optional[str], subplaylist_index: Optional[int]
 ) -> ContentHandler:
     if isinstance(source, AssetCatalogSourceIn):
         # Ask for extra portion of URL if it wasn't supplied
@@ -124,98 +126,159 @@
     obj: AppContext = click.get_current_context().obj
 
     section_title_shown = False
 
     metadata_cache = obj.cache
     filled_params = dict()
     params = adserver.queries
+
     if params:
         params = params.split("&")
         for p in params:
             parts = p.split("=")
             if len(parts) == 2:
                 (k, val) = parts
             else:
                 k = (parts[0],)
                 val = "=".join(parts[1:])
 
             if val.startswith("$arg_"):
                 input_param = val.replace("$arg_", "")
+                # determine output param name
+                if for_service:
+                    param_to_fill = input_param
+                else:
+                    param_to_fill = k
+
                 cached_values = metadata_cache.get_metadata(adserver, input_param)
 
                 if k in existing_params:
                     cached_values.insert(0, existing_params[k])
 
-                input_val = ""
+                input_val = UNSET
 
                 if obj.config.get("use_prompts"):
                     if not section_title_shown:
                         click.secho(
                             "\nQuery params to pass to the ad server", fg="white"
                         )
                         section_title_shown = True
 
-                    if cached_values:
-                        input_val = inquirer.select(
-                            message=f"Parameter '{input_param}'",
-                            choices=cached_values + [NEW],
-                            multiselect=False,
-                            default=cached_values[0],
-                            **inqdef.select_markers(),
-                        ).execute()
-
-                    if not cached_values:
-                        input_val = inquirer.text(
-                            message=f"Parameter '{input_param}'", **inqdef.markers(0)
-                        ).execute()
-
-                    if input_val == NEW:
-                        input_val = inquirer.text(
-                            message="New value: ", **inqdef.markers(1)
-                        ).execute()
+                    while input_val in [DELETED, UNSET]:
+                        if cached_values:
+                            input_val_prompt = inquirer.select(
+                                message=f"Parameter '{input_param}': ",
+                                choices=cached_values + [NEW],
+                                multiselect=False,
+                                default=cached_values[0],
+                                long_instruction="Key bindings: 'd' = delete the selected value | "
+                                "'ctrl-s' = skip all prompts, using last or default value",
+                                **inqdef.select_markers(),
+                            )
+
+                            @input_val_prompt.register_kb("d")
+                            def _handle_delete(event):
+                                choice_value = input_val_prompt.result_value
+
+                                metadata_cache.remove_metadata(
+                                    adserver, input_param, choice_value
+                                )
+                                event.app.exit(result=DELETED)
+
+                            @input_val_prompt.register_kb("c-s")
+                            def _handle_skip_all(event):
+                                choice_value = input_val_prompt.result_value
+
+                                obj.config.set_temporary("use_prompts", False)
+                                click.secho(choice_value, fg="bright_blue")
+                                event.app.exit(result=choice_value)
+
+                            input_val = input_val_prompt.execute()
+
+                        if not cached_values:
+                            input_val_prompt = inquirer.text(
+                                message=f"Parameter '{input_param}'",
+                                **inqdef.markers(0),
+                                long_instruction="Key bindings: 'ctrl-s' = skip all prompts, using last or default value",
+                            )
+
+                            @input_val_prompt.register_kb("c-s")
+                            def _handle_skip_all(event):
+                                obj.config.set_temporary("use_prompts", False)
+                                event.app.exit(result="")
+
+                            input_val = input_val_prompt.execute()
+
+                        if input_val == NEW:
+                            input_val = inquirer.text(
+                                message="New value: ", **inqdef.markers(1)
+                            ).execute()
 
                 else:
                     if cached_values:
                         input_val = cached_values[0]
                     else:
-                        input_val = val
+                        input_val = ""
 
-                if for_service:
-                    filled_params[input_param] = input_val
-                else:
-                    filled_params[k] = input_val
+                    click.secho(f"> Parameter '{input_param}': ", fg="white", nl=False)
+                    click.secho(input_val, fg="blue", bold=True)
+
+                filled_params[param_to_fill] = input_val
 
-                metadata_cache.record_metadata(adserver, input_param, input_val)
+                if input_val is not None and input_val != "":
+                    metadata_cache.record_metadata(adserver, input_param, input_val)
     return filled_params
 
 
 def ask_for_asset_catalog_sub_path(source: AssetCatalogSourceIn):
     extra_url = source.assetSample
 
     obj = click.get_current_context().obj
 
     metadata_cache = obj.cache
     cached_values = metadata_cache.get_metadata(source, "subPath")
 
+    extra_url = UNSET
+
     if obj.config.get("use_prompts"):
-        if cached_values:
-            extra_url = inquirer.select(
-                message="Sub-path",
-                choices=cached_values + [NEW],
-                multiselect=False,
-                default=cached_values[0],
-                **inqdef.select_markers(),
-            ).execute()
-
-        if not cached_values or extra_url == NEW:
-            extra_url = inquirer.text(
-                message="Sub-path (defaulting to the asset sample, if empty)",
-                default=source.assetSample,
-                **inqdef.markers(),
-            ).execute()
+        while extra_url in [UNSET, DELETED]:
+            if cached_values:
+                extra_url_prompt = inquirer.select(
+                    message="Sub-path",
+                    choices=cached_values + [NEW],
+                    multiselect=False,
+                    default=cached_values[0],
+                    long_instruction="Keyboard: 'd' = delete the selected value | "
+                    "'ctrl-s' = skip all prompts, using last or default value",
+                    **inqdef.select_markers(),
+                )
+
+                @extra_url_prompt.register_kb("d")
+                def _handle_delete(event):
+                    choice_value = extra_url_prompt.result_value
+
+                    metadata_cache.remove_metadata(source, "subPath", choice_value)
+                    event.app.exit(result=DELETED)
+
+                @extra_url_prompt.register_kb("c-s")
+                def _handle_skip_all(event):
+                    choice_value = extra_url_prompt.result_value
+                    obj.config.set_temporary("use_prompts", False)
+                    click.secho(choice_value, fg="bright_blue")
+
+                    event.app.exit(result=choice_value)
+
+                extra_url = extra_url_prompt.execute()
+
+            if not cached_values or extra_url == NEW:
+                extra_url = inquirer.text(
+                    message="Sub-path (defaulting to the asset sample, if empty)",
+                    default=source.assetSample,
+                    **inqdef.markers(),
+                ).execute()
 
     else:
         if cached_values:
             extra_url = cached_values[0]
         else:
             extra_url = source.assetSample
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/utils/urls.py` & `bpkio_cli-1.4.0/bpkio_cli/utils/urls.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/writers/breadcrumbs.py` & `bpkio_cli-1.4.0/bpkio_cli/writers/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/writers/colorizer.py` & `bpkio_cli-1.4.0/bpkio_cli/writers/colorizer.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,15 +45,27 @@
         return click.style(text, fg="yellow", italic=True)
 
     @staticmethod
     def url2(text):
         return click.style(text, fg="green", italic=True, underline=True)
 
     @staticmethod
-    def make_separator(text: Optional[str] = None, length: Optional[int] = None):
+    def expand(text):
+        return click.style(text, fg="bright_black", italic=True)
+
+    @staticmethod
+    def make_separator(
+        text: Optional[str] = None, length: Optional[int] = None, mode=None
+    ):
         if text:
             dashes = "-" * len(text)
         else:
             if not length:
                 length = 30
             dashes = "-" * length
+
+        if mode == "xml":
+            dashes = f"<!-- {dashes} -->"
+        if mode == "hls":
+            dashes = f"## {dashes}"
+
         return Colorizer.high3(dashes)
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/writers/content_display.py` & `bpkio_cli-1.4.0/bpkio_cli/writers/content_display.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,38 @@
+import math
 import os
 import shutil
 import time
 from datetime import datetime
 from typing import Optional
 
 import bpkio_api.helpers.handlers as handlers
 import click
 
 from bpkio_cli.core.exceptions import BroadpeakIoCliError
 from bpkio_cli.writers.diff import generate_diff
+from bpkio_cli.writers.formatter import OutputFormatter
 from bpkio_cli.writers.hls_formatter import HLSFormatter
 from bpkio_cli.writers.tables import display_table
 from bpkio_cli.writers.xml_formatter import XMLFormatter
 
 
 # ---- Shared Functions ----
 def display_content(
     handler: handlers.ContentHandler,
     max: int,
     interval: int,
     table: bool = False,
     raw: bool = False,
     diff: bool = False,
-    top: bool = False,
-    tail: bool = False,
+    top: int = 0,
+    tail: int = 0,
     clear: bool = False,
     header: bool = True,
-    pager: bool = False,
+    pager: bool = None,
 ):
     """Fetches the content of the URL associated with ID"""
     previous_content = None
 
     terminal_size = shutil.get_terminal_size().lines
 
     counter = max
@@ -77,36 +79,50 @@
                     raise BroadpeakIoCliError(
                         "No summary functionality implemented for this type of resource"
                     )
                 displayed = True
 
             if not displayed:
                 content = "No content to display"
+
                 match handler:
                     case handlers.XMLHandler():
                         formatter = XMLFormatter(handler=handler)
-                        content = formatter.format("raw" if raw else "standard")
+                        content = formatter.format(
+                            "raw" if raw else "standard", top=top, tail=tail
+                        )
 
                     case handlers.HLSHandler():
                         formatter = HLSFormatter(handler=handler)
                         content = formatter.format(
                             "raw" if raw else "standard", top=top, tail=tail
                         )
 
                 _show_redirect(handler.url, handler.original_url)
 
                 if previous_content and diff:
                     content_to_display = generate_diff(previous_content, content)
                 else:
                     content_to_display = content
 
+                # use a pager - including if content is too long to fit on screen
                 if pager or (
-                    pager is None and content_to_display.count("\n") > terminal_size - 5
+                    pager is None
+                    and len(content_to_display.splitlines()) > terminal_size - 5
                 ):
-                    click.echo_via_pager(content_to_display)
+                    # Avoid pager if polling
+                    if max != 1 and top == 0 and tail == 0:
+                        content_to_display = OutputFormatter.trim(
+                            content_to_display,
+                            top=math.floor((terminal_size - 5) / 2),
+                            tail=math.floor((terminal_size - 5) / 2),
+                        )
+                        click.echo(content_to_display)
+                    else:
+                        click.echo_via_pager(content_to_display)
                 else:
                     click.echo(content_to_display)
 
                 previous_content = content
 
             if counter == 1:
                 break
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/writers/diff.py` & `bpkio_cli-1.4.0/bpkio_cli/writers/diff.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/writers/json_formatter.py` & `bpkio_cli-1.4.0/bpkio_cli/writers/json_formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/writers/players.py` & `bpkio_cli-1.4.0/bpkio_cli/writers/players.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import click
 from InquirerPy import inquirer
 
 from bpkio_cli.core.config_provider import ConfigProvider
-from bpkio_cli.utils.inquirer_defaults import select_markers
+from bpkio_cli.utils.inquirer import select_markers
 
 
 class StreamPlayer:
     def __init__(self):
         self.config_provider = ConfigProvider()
         self._player_templates = None
```

### Comparing `bpkio_cli-1.3.0/bpkio_cli/writers/tables.py` & `bpkio_cli-1.4.0/bpkio_cli/writers/tables.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.3.0/bpkio_cli/writers/xml_formatter.py` & `bpkio_cli-1.4.0/bpkio_cli/writers/xml_formatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,26 +9,29 @@
 
 
 class XMLFormatter(OutputFormatter):
     def __init__(self, handler: XMLHandler) -> None:
         super().__init__()
         self.handler = handler
 
-    def format(self, mode="standard"):
+    def format(self, mode="standard", top: int = 0, tail: int = 0):
         match mode:
             case "raw":
-                return self.raw()
+                output = self.raw()
             case "standard":
-                return self.pretty_print()
+                output = self.pretty_print()
+
+        output = self.trim(output, top, tail)
+        return output
 
     def raw(self):
         # Pretty-print the XML using the ElementTree's tostring() method
         # return etree.tostring(self.handler.xml_document, pretty_print=True)
 
-        return self.handler.content
+        return self.handler.content.decode()
 
     def pretty_print(self):
         """Pretty-print the XML with colored output
 
         Returns:
             str
         """
@@ -59,15 +62,17 @@
                     lambda m: ns_mappings.get(m.group(1), m.group(0)),
                     tag,
                 )
             resolved_tag = tag
 
             # Add a line if there are multiple periods
             if resolved_tag == "Period" and position > 0:
-                result += CL.make_separator(length=150) + "\n" + indent * level
+                result += (
+                    CL.make_separator(length=150, mode="xml") + "\n" + indent * level
+                )
 
             # Start the opening tag
             result = result + "<"
 
             # Color-code the element tag name
             tag = CL.node(tag)
```

### Comparing `bpkio_cli-1.3.0/pyproject.toml` & `bpkio_cli-1.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 [tool.poetry]
 name = "bpkio-cli"
-version = "1.3.0"
+version = "1.4.0"
 description = "A command line interface to the broadpeak.io APIs, with additional helpers"
 authors = ["Fabre Lambeau <fabre.lambeau@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "bpkio_cli" }]
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poetry-dynamic-versioning.substitution]
 files = ["*/__init__.py", "*/__version__.py", "*/_version.py"]
 
 [tool.poetry.dependencies]
-bpkio-python-sdk = "^1.2.0"
+bpkio-python-sdk = "^1.3.0"
 python = "^3.10"
 click = "^8.1.3"
 colorama = "^0.4.6"
 # inquirerpy = { git = "https://github.com/kazhala/InquirerPy" }
 inquirerpy = "^0.3.4"
 tabulate = "^0.9.0"
 arrow = "^1.2.3"
 dateparser = "^1.1.8"
 setuptools = "^67.6.1"
 cloup = "^2.0.0.post1"
 diskcache = "^5.4.0"
 pygments = "^2.15.1"
 pytimeparse = "^1.1.8"
+threefive = "^2.3.95"
 
 [tool.poetry.scripts]
 bic = "bpkio_cli.app:safe_entry_point"
 bic-debug = "bpkio_cli.app:debug_entry_point"
 
 [tool.poetry.group.dev.dependencies]
 bpkio-python-sdk = { path = "../bpkio-python-sdk", develop = true }
```

### Comparing `bpkio_cli-1.3.0/PKG-INFO` & `bpkio_cli-1.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: bpkio-cli
-Version: 1.3.0
+Version: 1.4.0
 Summary: A command line interface to the broadpeak.io APIs, with additional helpers
 Author: Fabre Lambeau
 Author-email: fabre.lambeau@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
-Requires-Dist: bpkio-python-sdk (>=1.2.0,<2.0.0)
+Requires-Dist: bpkio-python-sdk (>=1.3.0,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cloup (>=2.0.0.post1,<3.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
 Requires-Dist: diskcache (>=5.4.0,<6.0.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
 Requires-Dist: pytimeparse (>=1.1.8,<2.0.0)
 Requires-Dist: setuptools (>=67.6.1,<68.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: threefive (>=2.3.95,<3.0.0)
 Description-Content-Type: text/markdown
```

