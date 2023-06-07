# Comparing `tmp/dimples-0.1.4.tar.gz` & `tmp/dimples-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimples-0.1.4.tar", last modified: Thu Feb 23 14:57:24 2023, max compression
+gzip compressed data, was "dist/dimples-0.1.5.tar", last modified: Wed Jun  7 17:09:33 2023, max compression
```

## Comparing `dimples-0.1.4.tar` & `dimples-0.1.5.tar`

### file list

```diff
@@ -1,139 +1,137 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2023-02-23 14:57:24.000000 dimples-0.1.4/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.1.4/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples/
--rw-r--r--   0 moky       (501) staff       (20)     7157 2023-02-23 13:42:13.000000 dimples-0.1.4/dimples/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples/client/
--rw-r--r--   0 moky       (501) staff       (20)     1945 2023-02-23 14:14:51.000000 dimples-0.1.4/dimples/client/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples/client/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2122 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/client/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3901 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/client/cpu/grp_expel.py
--rw-r--r--   0 moky       (501) staff       (20)     4006 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/client/cpu/grp_invite.py
--rw-r--r--   0 moky       (501) staff       (20)     3554 2023-02-23 11:18:06.000000 dimples-0.1.4/dimples/client/cpu/grp_query.py
--rw-r--r--   0 moky       (501) staff       (20)     3448 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/client/cpu/grp_quit.py
--rw-r--r--   0 moky       (501) staff       (20)     6373 2023-02-23 11:13:25.000000 dimples-0.1.4/dimples/client/cpu/grp_reset.py
--rw-r--r--   0 moky       (501) staff       (20)     5150 2023-02-23 14:17:47.000000 dimples-0.1.4/dimples/client/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     2948 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/client/cpu/history.py
--rw-r--r--   0 moky       (501) staff       (20)     1869 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/client/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/client/cpu/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)     5950 2023-02-23 14:12:55.000000 dimples-0.1.4/dimples/client/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples/client/network/
--rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.1.4/dimples/client/network/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6258 2023-02-23 14:14:03.000000 dimples-0.1.4/dimples/client/network/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8271 2023-02-23 14:19:16.000000 dimples-0.1.4/dimples/client/network/state.py
--rw-r--r--   0 moky       (501) staff       (20)     9531 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/client/network/transition.py
--rw-r--r--   0 moky       (501) staff       (20)     5291 2022-12-23 07:56:50.000000 dimples-0.1.4/dimples/client/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     6988 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/client/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5521 2023-02-23 14:13:41.000000 dimples-0.1.4/dimples/client/terminal.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples/common/
--rw-r--r--   0 moky       (501) staff       (20)     2103 2023-02-23 13:38:40.000000 dimples-0.1.4/dimples/common/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4228 2023-02-23 13:33:02.000000 dimples-0.1.4/dimples/common/ans.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples/common/dbi/
--rw-r--r--   0 moky       (501) staff       (20)     1945 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/common/dbi/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4000 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/common/dbi/account.py
--rw-r--r--   0 moky       (501) staff       (20)     2403 2022-12-13 10:56:52.000000 dimples-0.1.4/dimples/common/dbi/message.py
--rw-r--r--   0 moky       (501) staff       (20)     2597 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/common/dbi/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6995 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/common/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)    11170 2023-02-23 13:42:13.000000 dimples-0.1.4/dimples/common/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples/common/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     2536 2023-02-23 09:20:27.000000 dimples-0.1.4/dimples/common/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3237 2023-02-23 10:07:02.000000 dimples-0.1.4/dimples/common/protocol/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     5004 2022-12-23 07:24:37.000000 dimples-0.1.4/dimples/common/protocol/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4523 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/common/protocol/login.py
--rw-r--r--   0 moky       (501) staff       (20)     5191 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/common/protocol/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)     2501 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/common/protocol/report.py
--rw-r--r--   0 moky       (501) staff       (20)     3271 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/common/session.py
--rw-r--r--   0 moky       (501) staff       (20)     2813 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/common/transmitter.py
--rw-r--r--   0 moky       (501) staff       (20)     6122 2023-02-23 12:36:23.000000 dimples-0.1.4/dimples/config.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples/conn/
--rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.1.4/dimples/conn/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10213 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/conn/gate.py
--rw-r--r--   0 moky       (501) staff       (20)     9892 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/conn/gatekeeper.py
--rw-r--r--   0 moky       (501) staff       (20)    10305 2023-01-14 13:25:42.000000 dimples-0.1.4/dimples/conn/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     7851 2023-02-23 09:10:59.000000 dimples-0.1.4/dimples/conn/mtp.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples/conn/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/conn/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/conn/protocol/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     8254 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/conn/protocol/ws.py
--rw-r--r--   0 moky       (501) staff       (20)     5411 2023-02-23 09:10:59.000000 dimples-0.1.4/dimples/conn/queue.py
--rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.1.4/dimples/conn/seeker.py
--rw-r--r--   0 moky       (501) staff       (20)     5707 2023-01-14 15:58:29.000000 dimples-0.1.4/dimples/conn/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6991 2023-01-14 12:47:37.000000 dimples-0.1.4/dimples/conn/ws.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples/database/
--rw-r--r--   0 moky       (501) staff       (20)     2516 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/database/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     5981 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/database/account.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples/database/dos/
--rw-r--r--   0 moky       (501) staff       (20)     1748 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/database/dos/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4071 2022-12-22 17:59:17.000000 dimples-0.1.4/dimples/database/dos/base.py
--rw-r--r--   0 moky       (501) staff       (20)     3769 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/database/dos/document.py
--rw-r--r--   0 moky       (501) staff       (20)     3352 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/database/dos/group.py
--rw-r--r--   0 moky       (501) staff       (20)     3165 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/database/dos/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2680 2022-12-22 17:58:13.000000 dimples-0.1.4/dimples/database/dos/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     6447 2022-12-22 17:57:27.000000 dimples-0.1.4/dimples/database/dos/private.py
--rw-r--r--   0 moky       (501) staff       (20)     3741 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/database/dos/user.py
--rw-r--r--   0 moky       (501) staff       (20)     3097 2022-12-13 10:56:52.000000 dimples-0.1.4/dimples/database/message.py
--rw-r--r--   0 moky       (501) staff       (20)     3126 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/database/session.py
--rw-r--r--   0 moky       (501) staff       (20)     2972 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/database/t_cipherkey.py
--rw-r--r--   0 moky       (501) staff       (20)     3651 2023-01-14 12:27:17.000000 dimples-0.1.4/dimples/database/t_document.py
--rw-r--r--   0 moky       (501) staff       (20)     6874 2022-12-23 07:21:03.000000 dimples-0.1.4/dimples/database/t_group.py
--rw-r--r--   0 moky       (501) staff       (20)     3734 2022-12-23 07:21:03.000000 dimples-0.1.4/dimples/database/t_login.py
--rw-r--r--   0 moky       (501) staff       (20)     5144 2022-12-22 18:03:37.000000 dimples-0.1.4/dimples/database/t_message.py
--rw-r--r--   0 moky       (501) staff       (20)     3367 2022-12-23 07:21:03.000000 dimples-0.1.4/dimples/database/t_meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5386 2022-12-23 07:21:03.000000 dimples-0.1.4/dimples/database/t_private.py
--rw-r--r--   0 moky       (501) staff       (20)     2862 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/database/t_provider.py
--rw-r--r--   0 moky       (501) staff       (20)     4605 2022-12-22 18:01:59.000000 dimples-0.1.4/dimples/database/t_user.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples/edge/
--rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/edge/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    12760 2022-12-23 08:00:27.000000 dimples-0.1.4/dimples/edge/octopus.py
--rw-r--r--   0 moky       (501) staff       (20)     5517 2022-12-13 06:17:44.000000 dimples-0.1.4/dimples/edge/shared.py
--rw-r--r--   0 moky       (501) staff       (20)     2728 2022-12-13 06:17:44.000000 dimples-0.1.4/dimples/edge/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples/register/
--rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/register/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     9578 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/register/generate.py
--rw-r--r--   0 moky       (501) staff       (20)     7092 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/register/modify.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3880 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/register/run.py
--rw-r--r--   0 moky       (501) staff       (20)     1971 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/register/shared.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples/server/
--rw-r--r--   0 moky       (501) staff       (20)     2775 2023-02-23 09:37:38.000000 dimples-0.1.4/dimples/server/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples/server/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     1855 2023-02-23 09:37:38.000000 dimples-0.1.4/dimples/server/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2640 2023-02-23 10:54:44.000000 dimples-0.1.4/dimples/server/cpu/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     4787 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/server/cpu/document.py
--rw-r--r--   0 moky       (501) staff       (20)     3224 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/server/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     3859 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/server/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/server/cpu/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)     3089 2023-01-31 05:28:07.000000 dimples-0.1.4/dimples/server/cpu/report.py
--rw-r--r--   0 moky       (501) staff       (20)     6879 2022-12-13 10:59:06.000000 dimples-0.1.4/dimples/server/deliver.py
--rw-r--r--   0 moky       (501) staff       (20)     8893 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/server/delivering.py
--rw-r--r--   0 moky       (501) staff       (20)     7869 2023-02-23 13:19:19.000000 dimples-0.1.4/dimples/server/delivers.py
--rw-r--r--   0 moky       (501) staff       (20)     6073 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/server/dispatcher.py
--rw-r--r--   0 moky       (501) staff       (20)     4180 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/server/filter.py
--rw-r--r--   0 moky       (501) staff       (20)     8892 2023-02-23 13:42:13.000000 dimples-0.1.4/dimples/server/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     3287 2022-12-23 07:57:17.000000 dimples-0.1.4/dimples/server/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     5791 2023-02-23 11:39:56.000000 dimples-0.1.4/dimples/server/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     6433 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/server/push_info.py
--rw-r--r--   0 moky       (501) staff       (20)     6719 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/server/push_service.py
--rw-r--r--   0 moky       (501) staff       (20)     5680 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/server/pusher.py
--rw-r--r--   0 moky       (501) staff       (20)     7986 2023-01-14 12:19:38.000000 dimples-0.1.4/dimples/server/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/server/session_center.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples/station/
--rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.1.4/dimples/station/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4732 2022-12-23 07:58:49.000000 dimples-0.1.4/dimples/station/handler.py
--rw-r--r--   0 moky       (501) staff       (20)     8114 2023-02-23 13:34:51.000000 dimples-0.1.4/dimples/station/shared.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3784 2022-12-22 18:00:56.000000 dimples-0.1.4/dimples/station/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples/utils/
--rw-r--r--   0 moky       (501) staff       (20)     2568 2023-02-23 13:38:40.000000 dimples-0.1.4/dimples/utils/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6447 2022-12-22 12:24:04.000000 dimples-0.1.4/dimples/utils/cache.py
--rw-r--r--   0 moky       (501) staff       (20)     3292 2023-02-23 13:38:17.000000 dimples-0.1.4/dimples/utils/checker.py
--rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/utils/dos.py
--rw-r--r--   0 moky       (501) staff       (20)     2805 2022-12-28 05:23:15.000000 dimples-0.1.4/dimples/utils/log.py
--rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.1.4/dimples/utils/singleton.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     3304 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)      118 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples.egg-info/entry_points.txt
--rw-r--r--   0 moky       (501) staff       (20)      108 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        8 2023-02-23 14:57:24.000000 dimples-0.1.4/dimples.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2023-02-23 14:57:24.000000 dimples-0.1.4/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1675 2023-02-23 09:41:29.000000 dimples-0.1.4/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-07 17:09:33.000000 dimples-0.1.5/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.1.5/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/
+-rw-r--r--   0 moky       (501) staff       (20)     7071 2023-06-03 12:10:17.000000 dimples-0.1.5/dimples/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/client/
+-rw-r--r--   0 moky       (501) staff       (20)     1997 2023-06-03 11:38:39.000000 dimples-0.1.5/dimples/client/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/client/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2122 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/client/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4011 2023-06-02 18:30:20.000000 dimples-0.1.5/dimples/client/cpu/grp_expel.py
+-rw-r--r--   0 moky       (501) staff       (20)     4116 2023-06-02 18:31:07.000000 dimples-0.1.5/dimples/client/cpu/grp_invite.py
+-rw-r--r--   0 moky       (501) staff       (20)     3554 2023-02-23 11:18:06.000000 dimples-0.1.5/dimples/client/cpu/grp_query.py
+-rw-r--r--   0 moky       (501) staff       (20)     3558 2023-06-02 18:31:36.000000 dimples-0.1.5/dimples/client/cpu/grp_quit.py
+-rw-r--r--   0 moky       (501) staff       (20)     6498 2023-06-02 18:32:15.000000 dimples-0.1.5/dimples/client/cpu/grp_reset.py
+-rw-r--r--   0 moky       (501) staff       (20)     5150 2023-02-23 14:17:47.000000 dimples-0.1.5/dimples/client/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     2948 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/client/cpu/history.py
+-rw-r--r--   0 moky       (501) staff       (20)     1869 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/client/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/client/cpu/receipt.py
+-rw-r--r--   0 moky       (501) staff       (20)    16324 2023-06-02 17:03:56.000000 dimples-0.1.5/dimples/client/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     7713 2023-06-06 16:33:40.000000 dimples-0.1.5/dimples/client/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/client/network/
+-rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.1.5/dimples/client/network/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6258 2023-02-23 14:14:03.000000 dimples-0.1.5/dimples/client/network/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8302 2023-06-03 11:39:42.000000 dimples-0.1.5/dimples/client/network/state.py
+-rw-r--r--   0 moky       (501) staff       (20)     9531 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/client/network/transition.py
+-rw-r--r--   0 moky       (501) staff       (20)     6560 2023-06-06 16:21:36.000000 dimples-0.1.5/dimples/client/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     6988 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/client/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5521 2023-02-23 14:13:41.000000 dimples-0.1.5/dimples/client/terminal.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/common/
+-rw-r--r--   0 moky       (501) staff       (20)     2209 2023-06-06 13:30:28.000000 dimples-0.1.5/dimples/common/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4322 2023-06-02 08:44:29.000000 dimples-0.1.5/dimples/common/ans.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/common/dbi/
+-rw-r--r--   0 moky       (501) staff       (20)     2079 2023-06-04 17:02:25.000000 dimples-0.1.5/dimples/common/dbi/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6396 2023-06-02 10:33:41.000000 dimples-0.1.5/dimples/common/dbi/account.py
+-rw-r--r--   0 moky       (501) staff       (20)     2465 2023-06-02 07:39:55.000000 dimples-0.1.5/dimples/common/dbi/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     7819 2023-06-05 04:31:02.000000 dimples-0.1.5/dimples/common/dbi/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6739 2023-06-02 09:05:19.000000 dimples-0.1.5/dimples/common/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     6092 2023-06-06 13:27:51.000000 dimples-0.1.5/dimples/common/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     7918 2023-06-06 16:22:19.000000 dimples-0.1.5/dimples/common/packer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/common/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     2536 2023-02-23 09:20:27.000000 dimples-0.1.5/dimples/common/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3317 2023-06-02 08:06:32.000000 dimples-0.1.5/dimples/common/protocol/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     5004 2022-12-23 07:24:37.000000 dimples-0.1.5/dimples/common/protocol/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4523 2023-06-02 08:11:42.000000 dimples-0.1.5/dimples/common/protocol/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     6085 2023-06-02 08:40:15.000000 dimples-0.1.5/dimples/common/protocol/receipt.py
+-rw-r--r--   0 moky       (501) staff       (20)     2521 2023-06-02 08:42:45.000000 dimples-0.1.5/dimples/common/protocol/report.py
+-rw-r--r--   0 moky       (501) staff       (20)     4486 2023-06-04 16:41:38.000000 dimples-0.1.5/dimples/common/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6211 2023-06-03 12:24:47.000000 dimples-0.1.5/dimples/config.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/conn/
+-rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.1.5/dimples/conn/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10335 2023-06-07 13:23:28.000000 dimples-0.1.5/dimples/conn/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)     9892 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/conn/gatekeeper.py
+-rw-r--r--   0 moky       (501) staff       (20)    10305 2023-01-14 13:25:42.000000 dimples-0.1.5/dimples/conn/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     7851 2023-02-23 09:10:59.000000 dimples-0.1.5/dimples/conn/mtp.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/conn/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/conn/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/conn/protocol/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8254 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/conn/protocol/ws.py
+-rw-r--r--   0 moky       (501) staff       (20)     5411 2023-02-23 09:10:59.000000 dimples-0.1.5/dimples/conn/queue.py
+-rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.1.5/dimples/conn/seeker.py
+-rw-r--r--   0 moky       (501) staff       (20)     5726 2023-06-02 09:57:33.000000 dimples-0.1.5/dimples/conn/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6991 2023-01-14 12:47:37.000000 dimples-0.1.5/dimples/conn/ws.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/database/
+-rw-r--r--   0 moky       (501) staff       (20)     2560 2023-06-04 16:46:57.000000 dimples-0.1.5/dimples/database/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7000 2023-06-02 12:26:57.000000 dimples-0.1.5/dimples/database/account.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/database/dos/
+-rw-r--r--   0 moky       (501) staff       (20)     1808 2023-06-05 05:13:02.000000 dimples-0.1.5/dimples/database/dos/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4071 2022-12-22 17:59:17.000000 dimples-0.1.5/dimples/database/dos/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     3769 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/database/dos/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     4232 2023-06-02 10:30:44.000000 dimples-0.1.5/dimples/database/dos/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     3141 2023-06-02 11:02:33.000000 dimples-0.1.5/dimples/database/dos/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2680 2022-12-22 17:58:13.000000 dimples-0.1.5/dimples/database/dos/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5630 2023-06-02 11:04:20.000000 dimples-0.1.5/dimples/database/dos/private.py
+-rw-r--r--   0 moky       (501) staff       (20)     7961 2023-06-05 04:49:04.000000 dimples-0.1.5/dimples/database/dos/station.py
+-rw-r--r--   0 moky       (501) staff       (20)     5625 2023-06-02 11:01:02.000000 dimples-0.1.5/dimples/database/dos/user.py
+-rw-r--r--   0 moky       (501) staff       (20)     3097 2022-12-13 10:56:52.000000 dimples-0.1.5/dimples/database/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.1.5/dimples/database/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     2972 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/database/t_cipherkey.py
+-rw-r--r--   0 moky       (501) staff       (20)     3649 2023-06-05 05:32:38.000000 dimples-0.1.5/dimples/database/t_document.py
+-rw-r--r--   0 moky       (501) staff       (20)     7715 2023-06-05 05:41:56.000000 dimples-0.1.5/dimples/database/t_group.py
+-rw-r--r--   0 moky       (501) staff       (20)     3658 2023-06-05 05:34:19.000000 dimples-0.1.5/dimples/database/t_login.py
+-rw-r--r--   0 moky       (501) staff       (20)     5144 2022-12-22 18:03:37.000000 dimples-0.1.5/dimples/database/t_message.py
+-rw-r--r--   0 moky       (501) staff       (20)     3513 2023-06-05 05:36:10.000000 dimples-0.1.5/dimples/database/t_meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5589 2023-06-05 05:38:08.000000 dimples-0.1.5/dimples/database/t_private.py
+-rw-r--r--   0 moky       (501) staff       (20)     6647 2023-06-05 05:31:39.000000 dimples-0.1.5/dimples/database/t_station.py
+-rw-r--r--   0 moky       (501) staff       (20)     6455 2023-06-05 05:39:18.000000 dimples-0.1.5/dimples/database/t_user.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/edge/
+-rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/edge/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    12884 2023-06-05 09:19:20.000000 dimples-0.1.5/dimples/edge/octopus.py
+-rw-r--r--   0 moky       (501) staff       (20)     5594 2023-06-05 05:51:39.000000 dimples-0.1.5/dimples/edge/shared.py
+-rw-r--r--   0 moky       (501) staff       (20)     2726 2023-06-04 10:23:09.000000 dimples-0.1.5/dimples/edge/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/register/
+-rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/register/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     9516 2023-06-02 10:01:29.000000 dimples-0.1.5/dimples/register/generate.py
+-rw-r--r--   0 moky       (501) staff       (20)     7045 2023-06-02 10:02:10.000000 dimples-0.1.5/dimples/register/modify.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3880 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/register/run.py
+-rw-r--r--   0 moky       (501) staff       (20)     1971 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/register/shared.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/server/
+-rw-r--r--   0 moky       (501) staff       (20)     2561 2023-06-07 12:19:50.000000 dimples-0.1.5/dimples/server/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/server/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     1855 2023-02-23 09:37:38.000000 dimples-0.1.5/dimples/server/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2640 2023-02-23 10:54:44.000000 dimples-0.1.5/dimples/server/cpu/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     4781 2023-06-03 12:02:30.000000 dimples-0.1.5/dimples/server/cpu/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     3341 2023-04-14 16:24:15.000000 dimples-0.1.5/dimples/server/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     3853 2023-06-03 12:02:46.000000 dimples-0.1.5/dimples/server/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/server/cpu/receipt.py
+-rw-r--r--   0 moky       (501) staff       (20)     3089 2023-01-31 05:28:07.000000 dimples-0.1.5/dimples/server/cpu/report.py
+-rw-r--r--   0 moky       (501) staff       (20)    12938 2023-06-07 12:15:09.000000 dimples-0.1.5/dimples/server/dispatcher.py
+-rw-r--r--   0 moky       (501) staff       (20)    12456 2023-06-07 16:52:51.000000 dimples-0.1.5/dimples/server/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     7656 2023-06-07 15:42:18.000000 dimples-0.1.5/dimples/server/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     5791 2023-02-23 11:39:56.000000 dimples-0.1.5/dimples/server/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     6433 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/server/push_info.py
+-rw-r--r--   0 moky       (501) staff       (20)     6719 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/server/push_service.py
+-rw-r--r--   0 moky       (501) staff       (20)     5877 2023-06-07 13:18:30.000000 dimples-0.1.5/dimples/server/pusher.py
+-rw-r--r--   0 moky       (501) staff       (20)     7986 2023-01-14 12:19:38.000000 dimples-0.1.5/dimples/server/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/server/session_center.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/station/
+-rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.1.5/dimples/station/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4624 2023-06-07 12:21:10.000000 dimples-0.1.5/dimples/station/handler.py
+-rw-r--r--   0 moky       (501) staff       (20)     7087 2023-06-07 11:52:56.000000 dimples-0.1.5/dimples/station/shared.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3782 2023-06-04 10:23:09.000000 dimples-0.1.5/dimples/station/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples/utils/
+-rw-r--r--   0 moky       (501) staff       (20)     2568 2023-02-23 13:38:40.000000 dimples-0.1.5/dimples/utils/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6447 2022-12-22 12:24:04.000000 dimples-0.1.5/dimples/utils/cache.py
+-rw-r--r--   0 moky       (501) staff       (20)     4016 2023-06-02 18:00:31.000000 dimples-0.1.5/dimples/utils/checker.py
+-rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/utils/dos.py
+-rw-r--r--   0 moky       (501) staff       (20)     2805 2022-12-28 05:23:15.000000 dimples-0.1.5/dimples/utils/log.py
+-rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.1.5/dimples/utils/singleton.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:09:33.000000 dimples-0.1.5/dimples.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-07 17:09:32.000000 dimples-0.1.5/dimples.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     3247 2023-06-07 17:09:32.000000 dimples-0.1.5/dimples.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2023-06-07 17:09:32.000000 dimples-0.1.5/dimples.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)      118 2023-06-07 17:09:32.000000 dimples-0.1.5/dimples.egg-info/entry_points.txt
+-rw-r--r--   0 moky       (501) staff       (20)      108 2023-06-07 17:09:32.000000 dimples-0.1.5/dimples.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        8 2023-06-07 17:09:32.000000 dimples-0.1.5/dimples.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2023-06-07 17:09:33.000000 dimples-0.1.5/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1675 2023-06-02 06:58:43.000000 dimples-0.1.5/setup.py
```

### Comparing `dimples-0.1.4/PKG-INFO` & `dimples-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.1.4
+Version: 0.1.5
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.1.4/README.md` & `dimples-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/__init__.py` & `dimples-0.1.5/dimples/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,17 +80,14 @@
     'EntityType', 'MetaType',
     'Address', 'AddressFactory',
     'ID', 'IDFactory',
     'Meta', 'MetaFactory',
     'Document', 'DocumentFactory',
     'Visa', 'Bulletin',
 
-    'entity_is_user', 'entity_is_group', 'entity_is_broadcast',
-    'meta_has_seed',
-
     'BroadcastAddress', 'Identifier',
     'ANYWHERE', 'EVERYWHERE', 'ANYONE', 'EVERYONE', 'FOUNDER',
 
     #
     #   MingKeMing base extends
     #
     'BaseMeta',
```

### Comparing `dimples-0.1.4/dimples/client/__init__.py` & `dimples-0.1.5/dimples/client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 """
 
 from .cpu import *
 
 from .network import ClientSession
 from .network import SessionState
 
+from .group import GroupManager
 from .messenger import ClientMessenger
 from .packer import ClientMessagePacker
 from .processor import ClientMessageProcessor, ClientContentProcessorCreator
 from .terminal import Terminal
 
 
 __all__ = [
@@ -50,12 +51,13 @@
     'ReceiptCommandProcessor',
 
     #
     #   Client
     #
     'ClientSession', 'SessionState',
 
+    'GroupManager',
     'ClientMessenger',
     'ClientMessagePacker',
     'ClientMessageProcessor', 'ClientContentProcessorCreator',
     'Terminal',
 ]
```

### Comparing `dimples-0.1.4/dimples/client/cpu/__init__.py` & `dimples-0.1.5/dimples/client/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/client/cpu/grp_expel.py` & `dimples-0.1.5/dimples/client/cpu/grp_expel.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,11 +86,17 @@
             if item not in members:
                 continue
             # expelled member found
             remove_list.append(item)
             members.remove(item)
         # 2.3. do expel
         if len(remove_list) > 0:
-            if facebook.save_members(members=members, identifier=group):
+            man = group_manager()
+            if man.save_members(members=members, group=group):
                 content['removed'] = ID.revert(remove_list)
         # 3. response (no need to response this group command)
         return []
+
+
+def group_manager():
+    from ..group import GroupManager
+    return GroupManager()
```

### Comparing `dimples-0.1.4/dimples/client/cpu/grp_invite.py` & `dimples-0.1.5/dimples/client/cpu/grp_invite.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,11 +87,17 @@
             if item in members:
                 continue
             # new member found
             add_list.append(item)
             members.append(item)
         # 2.3. do invite
         if len(add_list) > 0:
-            if facebook.save_members(members=members, identifier=group):
+            man = group_manager()
+            if man.save_members(members=members, group=group):
                 content['added'] = ID.revert(add_list)
         # 3. response (no need to response this group command)
         return []
+
+
+def group_manager():
+    from ..group import GroupManager
+    return GroupManager()
```

### Comparing `dimples-0.1.4/dimples/client/cpu/grp_query.py` & `dimples-0.1.5/dimples/client/cpu/grp_query.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/client/cpu/grp_quit.py` & `dimples-0.1.5/dimples/client/cpu/grp_quit.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,10 +75,16 @@
             return self._respond_text(text=text, group=group)
         assistants = facebook.assistants(identifier=group)
         if assistants is not None and sender in assistants:
             return self._remove_assistant(content=content, msg=msg)
         # 2. remove sender from group members
         if sender in members:
             members.remove(sender)
-            facebook.save_members(members=members, identifier=group)
+            man = group_manager()
+            man.save_members(members=members, group=group)
         # 3. response (no need to response this group command)
         return []
+
+
+def group_manager():
+    from ..group import GroupManager
+    return GroupManager()
```

### Comparing `dimples-0.1.4/dimples/client/cpu/grp_reset.py` & `dimples-0.1.5/dimples/client/cpu/grp_reset.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,23 +68,24 @@
         facebook = self.facebook
         group = content.group
         # check whether the owner contained in the new members
         new_members = self.members(content=content)
         if new_members is None or len(new_members) == 0:
             text = self.STR_RESET_CMD_ERROR
             return self._respond_text(text=text, group=group)
+        man = group_manager()
         for item in new_members:
             if facebook.meta(identifier=item) is None:
                 # TODO: waiting for member's meta?
                 continue
-            elif not facebook.is_owner(member=item, group=group):
+            elif not man.is_owner(member=item, group=group):
                 # not owner, skip it
                 continue
             # it's a full list, save it now
-            if facebook.save_members(members=new_members, identifier=group):
+            if man.save_members(members=new_members, group=group):
                 if item != sender:
                     # NOTICE: to prevent counterfeit,
                     #         query the owner for newest member-list
                     self._query_owner(owner=item, group=group)
             # response (no need to respond this group command)
             return []
         # NOTICE: this is a partial member-list
@@ -133,14 +134,20 @@
         add_list = []
         for item in new_members:
             if item not in members:
                 # adding member found
                 add_list.append(item)
         # 2.4. do reset
         if len(add_list) > 0 or len(remove_list) > 0:
-            if facebook.save_members(members=new_members, identifier=group):
+            man = group_manager()
+            if man.save_members(members=new_members, group=group):
                 if len(add_list) > 0:
                     content['added'] = ID.revert(add_list)
                 if len(remove_list) > 0:
                     content['removed'] = ID.revert(remove_list)
         # 3. response (no need to response this group command)
         return []
+
+
+def group_manager():
+    from ..group import GroupManager
+    return GroupManager()
```

### Comparing `dimples-0.1.4/dimples/client/cpu/handshake.py` & `dimples-0.1.5/dimples/client/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/client/cpu/history.py` & `dimples-0.1.5/dimples/client/cpu/history.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/client/cpu/login.py` & `dimples-0.1.5/dimples/client/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/client/cpu/receipt.py` & `dimples-0.1.5/dimples/client/cpu/receipt.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/client/messenger.py` & `dimples-0.1.5/dimples/client/messenger.py`

 * *Files 22% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 
 from ..utils import QueryFrequencyChecker
 from ..common import HandshakeCommand, ReportCommand, LoginCommand
 from ..common import CommonMessenger
 
 from .network import ClientSession
 
+from .group import GroupManager
+
 
 class ClientMessenger(CommonMessenger):
 
     @property
     def session(self) -> ClientSession:
         sess = super().session
         assert isinstance(sess, ClientSession), 'session error: %s' % sess
@@ -77,65 +79,97 @@
             self.send_content(sender=None, receiver=srv_id, content=cmd, priority=-1)
 
     def handshake_success(self):
         """ callback for handshake success """
         # broadcast current documents after handshake success
         self.broadcast_document()
 
-    def broadcast_document(self):
-        """ broadcast meta & visa document to all stations """
-        facebook = self.facebook
-        current = facebook.current_user
-        identifier = current.identifier
-        meta = current.meta
-        visa = current.visa
-        cmd = DocumentCommand.response(identifier=identifier, meta=meta, document=visa)
-        # broadcast to everyone@everywhere
-        self.send_content(sender=identifier, receiver=EVERYONE, content=cmd, priority=1)
-
     def broadcast_login(self, sender: ID, user_agent: str):
         """ send login command to keep roaming """
         # get current station
-        session = self.session
-        station = session.station
-        assert sender.type != EntityType.STATION, \
-            'station (%s) would not login to another station: %s' % (sender, station)
+        station = self.session.station
+        assert sender.type != EntityType.STATION, 'station (%s) cannot login: %s' % (sender, station)
         # create login command
-        cmd = LoginCommand(identifier=sender)
-        cmd.agent = user_agent
-        cmd.station = station
+        command = LoginCommand(identifier=sender)
+        command.agent = user_agent
+        command.station = station
         # broadcast to everyone@everywhere
-        self.send_content(sender=sender, receiver=EVERYONE, content=cmd, priority=1)
+        self.send_content(sender=sender, receiver=EVERYONE, content=command, priority=1)
 
     def report_online(self, sender: ID = None):
         """ send report command to keep user online """
-        cmd = ReportCommand(title=ReportCommand.ONLINE)
-        self.send_content(sender=sender, receiver=Station.ANY, content=cmd, priority=1)
+        command = ReportCommand(title=ReportCommand.ONLINE)
+        self.send_content(sender=sender, receiver=Station.ANY, content=command, priority=1)
 
     def report_offline(self, sender: ID = None):
         """ Send report command to let user offline """
-        cmd = ReportCommand(title=ReportCommand.OFFLINE)
-        self.send_content(sender=sender, receiver=Station.ANY, content=cmd, priority=1)
+        command = ReportCommand(title=ReportCommand.OFFLINE)
+        self.send_content(sender=sender, receiver=Station.ANY, content=command, priority=1)
+
+    def broadcast_document(self, updated: bool = False):
+        """ broadcast meta & visa document to all stations """
+        facebook = self.facebook
+        user = facebook.current_user
+        assert user is not None, 'current user not found'
+        current = user.identifier
+        meta = user.meta
+        visa = user.visa
+        assert visa is not None, 'visa not found: %s' % user
+        command = DocumentCommand.response(identifier=current, meta=meta, document=visa)
+        # send to all contacts
+        contacts = facebook.contacts(identifier=current)
+        for item in contacts:
+            self.send_visa(sender=current, receiver=item, content=command, force=updated)
+        # broadcast to everyone@everywhere
+        self.send_visa(sender=current, receiver=EVERYONE, content=command, force=updated)
+
+    def send_visa(self, sender: Optional[ID], receiver: ID, content: DocumentCommand, force: bool = False):
+        checker = QueryFrequencyChecker()
+        if checker.document_response_expired(identifier=receiver, force=force):
+            self.info(msg='push visa to: %s' % receiver)
+            self.send_content(sender=sender, receiver=receiver, content=content, priority=1)
+        else:
+            # response not expired yet
+            self.debug(msg='document response not expired yet: %s' % receiver)
 
     # Override
-    def _query_meta(self, identifier: ID) -> bool:
+    def query_meta(self, identifier: ID) -> bool:
         checker = QueryFrequencyChecker()
         if not checker.meta_query_expired(identifier=identifier):
             # query not expired yet
             self.debug(msg='meta query not expired yet: %s' % identifier)
             return False
         self.info(msg='querying meta: %s from any station' % identifier)
-        cmd = MetaCommand.query(identifier=identifier)
-        self.send_content(sender=None, receiver=Station.ANY, content=cmd)
+        command = MetaCommand.query(identifier=identifier)
+        self.send_content(sender=None, receiver=Station.ANY, content=command, priority=1)
         return True
 
     # Override
-    def _query_document(self, identifier: ID) -> bool:
+    def query_document(self, identifier: ID) -> bool:
         checker = QueryFrequencyChecker()
         if not checker.document_query_expired(identifier=identifier):
             # query not expired yet
             self.debug(msg='document query not expired yet: %s' % identifier)
             return False
         self.info(msg='querying document: %s from any station' % identifier)
-        cmd = DocumentCommand.query(identifier=identifier)
-        self.send_content(sender=None, receiver=Station.ANY, content=cmd)
+        command = DocumentCommand.query(identifier=identifier)
+        self.send_content(sender=None, receiver=Station.ANY, content=command, priority=1)
+        return True
+
+    # Override
+    def query_members(self, identifier: ID) -> bool:
+        checker = QueryFrequencyChecker()
+        if not checker.members_query_expired(identifier=identifier):
+            # query not expired yet
+            self.debug(msg='members query not expired yet: %s' % identifier)
+            return False
+        self.info(msg='querying members: %s from any station' % identifier)
+        man = GroupManager()
+        assistants = man.assistants(identifier=identifier)
+        if assistants is None or len(assistants) == 0:
+            self.error(msg='group assistants not found: %s' % identifier)
+            return False
+        # querying members from bot
+        command = DocumentCommand.query(identifier=identifier)
+        for bot in assistants:
+            self.send_content(sender=None, receiver=bot, content=command, priority=1)
         return True
```

### Comparing `dimples-0.1.4/dimples/client/network/__init__.py` & `dimples-0.1.5/dimples/client/network/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/client/network/session.py` & `dimples-0.1.5/dimples/client/network/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/client/network/state.py` & `dimples-0.1.5/dimples/client/network/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
         docker = gate.get_docker(remote=session.remote_address, local=None, advance_party=[])
         if docker is None:
             return DockerStatus.ERROR
         else:
             return docker.status
 
 
+# noinspection PyAbstractClass
 class StateTransition(BaseTransition[StateMachine], ABC):
 
     # noinspection PyMethodMayBeStatic
     def is_expired(self, state, now: float) -> bool:
         assert isinstance(state, SessionState), 'state error: %s' % state
         return 0 < state.enter_time < (now - 30)
```

### Comparing `dimples-0.1.4/dimples/client/network/transition.py` & `dimples-0.1.5/dimples/client/network/transition.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/client/packer.py` & `dimples-0.1.5/dimples/client/packer.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,50 +26,68 @@
 """
     Common extensions for MessagePacker
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 from typing import Optional
 
 from dimsdk import SymmetricKey
+from dimsdk import ID
 from dimsdk import InstantMessage, SecureMessage, ReliableMessage
 from dimsdk import DocumentCommand
-from dimsdk import Messenger, MessagePacker
+from dimsdk import Messenger
 
 from ..utils import base64_encode, sha256
+from ..common import CommonFacebook, CommonMessagePacker
 
-from ..common import CommonFacebook, CommonMessenger
 
+class ClientMessagePacker(CommonMessagePacker):
 
-class ClientMessagePacker(MessagePacker):
-
-    @property
-    def facebook(self) -> CommonFacebook:
-        barrack = super().facebook
-        assert isinstance(barrack, CommonFacebook), 'facebook error: %s' % barrack
-        return barrack
+    # Override
+    def _check_instant_message_receiver(self, msg: InstantMessage) -> bool:
+        receiver = msg.receiver
+        if receiver.is_broadcast:
+            # broadcast message
+            return True
+        elif receiver.is_group:
+            # check group's meta & members
+            members = self._members(group=receiver)
+            if members is None:
+                # group not ready, suspend message for waiting meta/members
+                error = {
+                    'message': 'group not ready',
+                    'group': str(receiver),
+                }
+                self._suspend_instant_message(msg=msg, error=error)
+                return False
+            waiting = []
+            for item in members:
+                if self._visa_key(user=item) is not None:
+                    # member is OK
+                    continue
+                # meta not ready
+                waiting.append(item)
+            if len(waiting) > 0:
+                # member(s) not ready, suspend message for waiting document
+                error = {
+                    'message': 'encrypt keys not found',
+                    'group': str(receiver),
+                    'members': ID.revert(array=waiting),
+                }
+                self._suspend_instant_message(msg=msg, error=error)
+                return False
+            # receiver is OK
+            return True
+        # check user's meta & document
+        return super()._check_instant_message_receiver(msg=msg)
 
     # Override
     def serialize_message(self, msg: ReliableMessage) -> bytes:
         attach_key_digest(msg=msg, messenger=self.messenger)
         return super().serialize_message(msg=msg)
 
-    # Override
-    def deserialize_message(self, data: bytes) -> Optional[ReliableMessage]:
-        if data is None or len(data) < 2:
-            # message data error
-            return None
-        return super().deserialize_message(data=data)
-
-    # Override
-    def sign_message(self, msg: SecureMessage) -> ReliableMessage:
-        if isinstance(msg, ReliableMessage):
-            # already signed
-            return msg
-        return super().sign_message(msg=msg)
-
     # # Override
     # def encrypt_message(self, msg: InstantMessage) -> Optional[SecureMessage]:
     #     # make sure visa.key exists before encrypting message
     #     s_msg = super().encrypt_message(msg=msg)
     #     receiver = msg.receiver
     #     if receiver.is_group:
     #         # reuse group message keys
@@ -84,23 +102,36 @@
             return super().decrypt_message(msg=msg)
         except AssertionError as error:
             err_msg = '%s' % error
             # check exception thrown by DKD: chat.dim.dkd.EncryptedMessage.decrypt()
             if err_msg.find('failed to decrypt key in msg') < 0:
                 raise error
             # visa.key expired?
-            # send new visa to the sender
-            current = self.facebook.current_user
-            uid = current.identifier
-            visa = current.visa
+            # push new visa document to this message sender
+            facebook = get_facebook(packer=self)
+            user = facebook.current_user
+            current = user.identifier
+            visa = user.visa
             assert visa is not None and visa.valid, 'user visa error: %s' % current
-            cmd = DocumentCommand.response(document=visa, identifier=uid)
-            messenger = self.messenger
-            assert isinstance(messenger, CommonMessenger), 'messenger error: %s' % messenger
-            messenger.send_content(sender=uid, receiver=msg.sender, content=cmd)
+            command = DocumentCommand.response(document=visa, identifier=current)
+            messenger = get_messenger(packer=self)
+            messenger.send_visa(sender=current, receiver=msg.sender, content=command)
+
+
+def get_facebook(packer: CommonMessagePacker) -> CommonFacebook:
+    barrack = packer.facebook
+    assert isinstance(barrack, CommonFacebook), 'facebook error: %s' % barrack
+    return barrack
+
+
+def get_messenger(packer: CommonMessagePacker):
+    transceiver = packer.messenger
+    from .messenger import ClientMessenger
+    assert isinstance(transceiver, ClientMessenger), 'messenger error: %s' % transceiver
+    return transceiver
 
 
 def attach_key_digest(msg: ReliableMessage, messenger: Messenger):
     # check message delegate
     if msg.delegate is None:
         msg.delegate = messenger
     # check msg.key
```

### Comparing `dimples-0.1.4/dimples/client/processor.py` & `dimples-0.1.5/dimples/client/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/client/terminal.py` & `dimples-0.1.5/dimples/client/terminal.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/common/__init__.py` & `dimples-0.1.5/dimples/common/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
 from .protocol import *
 from .dbi import *
 
 from .ans import AddressNameServer
 from .facebook import CommonFacebook
 from .messenger import CommonMessenger
-from .transmitter import Transmitter
-from .session import Session
+from .packer import CommonMessagePacker
+from .session import Transmitter, Session
 
 
 __all__ = [
     #
     #   protocol
     #
     'HandshakeCommand', 'HandshakeState',
@@ -49,25 +49,27 @@
     'ReportCommand',
     'AnsCommand',
 
     #
     #   Database Interface
     #
     'PrivateKeyDBI', 'MetaDBI', 'DocumentDBI',
-    'UserDBI', 'GroupDBI',
+    'UserDBI', 'ContactDBI', 'GroupDBI',
     'AccountDBI',
 
-    'LoginDBI', 'ProviderDBI',
-    'SessionDBI',
-
     'ReliableMessageDBI', 'CipherKeyDBI',
     'MessageDBI',
 
+    'LoginDBI', 'ProviderDBI', 'StationDBI',
+    'SessionDBI',
+    'ProviderInfo', 'StationInfo',
+
     #
     #   common
     #
     'AddressNameServer',
     'CommonFacebook',
     'CommonMessenger',
+    'CommonMessagePacker',
     'Transmitter',
     'Session',
 ]
```

### Comparing `dimples-0.1.4/dimples/common/ans.py` & `dimples-0.1.5/dimples/common/ans.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,12 +109,13 @@
     def fix(self, records: Dict[str, str]) -> int:
         """ remove the keywords temporary before save new records """
         count = 0
         self.__reserved['assistant'] = False
         # self.__reserved['station'] = False
         for alias in records:
             identifier = ID.parse(identifier=records[alias])
+            assert identifier is not None, 'record error: %s => %s' % (alias, records[alias])
             if self.save(name=alias, identifier=identifier):
                 count += 1
         # self.__reserved['station'] = True
         self.__reserved['assistant'] = True
         return count
```

### Comparing `dimples-0.1.4/dimples/common/dbi/__init__.py` & `dimples-0.1.5/dimples/common/dbi/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,37 +26,39 @@
 """
     Database Interfaces
     ~~~~~~~~~~~~~~~~~~~
 
 """
 
 from .account import PrivateKeyDBI, MetaDBI, DocumentDBI
-from .account import UserDBI, GroupDBI
+from .account import UserDBI, ContactDBI, GroupDBI
 from .account import AccountDBI
 
 from .message import ReliableMessageDBI, CipherKeyDBI
 from .message import MessageDBI
 
-from .session import LoginDBI, ProviderDBI
+from .session import LoginDBI, ProviderDBI, StationDBI
 from .session import SessionDBI
+from .session import ProviderInfo, StationInfo
 
 
 __all__ = [
     #
     #   Account
     #
     'PrivateKeyDBI', 'MetaDBI', 'DocumentDBI',
-    'UserDBI', 'GroupDBI',
+    'UserDBI', 'ContactDBI', 'GroupDBI',
     'AccountDBI',
 
     #
     #   Message
     #
     'ReliableMessageDBI', 'CipherKeyDBI',
     'MessageDBI',
 
     #
     #   Session
     #
-    'LoginDBI', 'ProviderDBI',
+    'LoginDBI', 'ProviderDBI', 'StationDBI',
     'SessionDBI',
+    'ProviderInfo', 'StationInfo',
 ]
```

### Comparing `dimples-0.1.4/dimples/common/dbi/message.py` & `dimples-0.1.5/dimples/common/dbi/message.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,15 +49,17 @@
         raise NotImplemented
 
     @abstractmethod
     def remove_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
         raise NotImplemented
 
 
+# noinspection PyAbstractClass
 class CipherKeyDBI(CipherKeyDelegate, ABC):
     """ CipherKey Table """
     pass
 
 
+# noinspection PyAbstractClass
 class MessageDBI(ReliableMessageDBI, CipherKeyDBI, ABC):
     """ Message Database """
     pass
```

### Comparing `dimples-0.1.4/dimples/common/facebook.py` & `dimples-0.1.5/dimples/common/facebook.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     Barrack for cache entities
 """
 
 from typing import Optional, List
 
 from dimsdk import SignKey, DecryptKey
-from dimsdk import ID, Meta, Document, User, Group
+from dimsdk import ID, Meta, Document, User
 from dimsdk import Facebook
 
 from .dbi import AccountDBI
 
 
 class CommonFacebook(Facebook):
 
@@ -59,154 +59,148 @@
     #
     #   Super
     #
 
     @property  # Override
     def local_users(self) -> List[User]:
         db = self.database
-        users = []
         array = db.local_users()
         # 'users.js' empty?
         if array is None or len(array) == 0:
             current = self.__current
             return [] if current is None else [current]
         # create users
+        users = []
         for item in array:
+            assert self.private_key_for_signature(identifier=item) is not None, 'error: %s' % item
             usr = self.user(identifier=item)
             assert usr is not None, 'failed to create user: %s' % item
-            # assert self.private_key_for_signature(identifier=item) is not None
             users.append(usr)
         return users
 
     @property
     def current_user(self) -> Optional[User]:
         """ Get current user (for signing and sending message) """
         current = self.__current
         if current is None:
             # current = super().current_user
             users = self.local_users
             if users is not None and len(users) > 0:
                 current = users[0]
+                self.__current = current
         return current
 
     @current_user.setter
     def current_user(self, user: User):
+        if user.data_source is None:
+            user.data_source = self
         self.__current = user
 
     # Override
     def save_meta(self, meta: Meta, identifier: ID) -> bool:
         db = self.database
         return db.save_meta(meta=meta, identifier=identifier)
 
     # Override
     def save_document(self, document: Document) -> bool:
         db = self.database
         return db.save_document(document=document)
 
-    # Override
-    def save_members(self, members: List[ID], identifier: ID) -> bool:
-        db = self.database
-        return db.save_members(members=members, identifier=identifier)
+    # # Override
+    # def create_user(self, identifier: ID) -> Optional[User]:
+    #     if not identifier.is_broadcast:
+    #         if self.public_key_for_encryption(identifier=identifier) is None:
+    #             # visa.key not found
+    #             return None
+    #     return super().create_user(identifier=identifier)
+    #
+    # # Override
+    # def create_group(self, identifier: ID) -> Optional[Group]:
+    #     if not identifier.is_broadcast:
+    #         if self.meta(identifier=identifier) is None:
+    #             # meta not found
+    #             return None
+    #     return super().create_group(identifier=identifier)
 
-    def save_assistants(self, assistants: List[ID], identifier: ID) -> bool:
-        db = self.database
-        return db.save_assistants(assistants=assistants, identifier=identifier)
+    #
+    #   EntityDataSource
+    #
 
     # Override
-    def create_user(self, identifier: ID) -> Optional[User]:
-        if not identifier.is_broadcast:
-            if self.public_key_for_encryption(identifier=identifier) is None:
-                # visa.key not found
-                return None
-        return super().create_user(identifier=identifier)
+    def meta(self, identifier: ID) -> Optional[Meta]:
+        # if identifier.is_broadcast:
+        #     # broadcast ID has no meta
+        #     return None
+        db = self.database
+        return db.meta(identifier=identifier)
 
     # Override
-    def create_group(self, identifier: ID) -> Optional[Group]:
-        if not identifier.is_broadcast:
-            if self.meta(identifier=identifier) is None:
-                # meta not found
-                return None
-        return super().create_group(identifier=identifier)
+    def document(self, identifier: ID, doc_type: str = '*') -> Optional[Document]:
+        # if identifier.is_broadcast:
+        #     # broadcast ID has no document
+        #     return None
+        db = self.database
+        return db.document(identifier=identifier, doc_type=doc_type)
 
     #
     #   UserDataSource
     #
 
     # Override
     def contacts(self, identifier: ID) -> List[ID]:
         db = self.database
-        return db.contacts(identifier=identifier)
+        return db.contacts(user=identifier)
 
     # Override
     def private_keys_for_decryption(self, identifier: ID) -> List[DecryptKey]:
         db = self.database
-        return db.private_keys_for_decryption(identifier=identifier)
+        return db.private_keys_for_decryption(user=identifier)
 
     # Override
     def private_key_for_signature(self, identifier: ID) -> Optional[SignKey]:
         db = self.database
-        return db.private_key_for_signature(identifier=identifier)
+        return db.private_key_for_signature(user=identifier)
 
     # Override
     def private_key_for_visa_signature(self, identifier: ID) -> Optional[SignKey]:
         db = self.database
-        return db.private_key_for_visa_signature(identifier=identifier)
+        return db.private_key_for_visa_signature(user=identifier)
 
     #
     #    GroupDataSource
     #
 
     # Override
     def founder(self, identifier: ID) -> ID:
         db = self.database
-        user = db.founder(identifier=identifier)
+        user = db.founder(group=identifier)
         if user is not None:
             # got from database
             return user
         return super().founder(identifier=identifier)
 
     # Override
     def owner(self, identifier: ID) -> ID:
         db = self.database
-        user = db.owner(identifier=identifier)
+        user = db.owner(group=identifier)
         if user is not None:
             # got from database
             return user
         return super().owner(identifier=identifier)
 
     # Override
     def members(self, identifier: ID) -> Optional[List[ID]]:
         db = self.database
-        users = db.members(identifier=identifier)
+        users = db.members(group=identifier)
         if users is not None and len(users) > 0:
             # got from database
             return users
         return super().members(identifier=identifier)
 
     # Override
     def assistants(self, identifier: ID) -> Optional[List[ID]]:
         db = self.database
-        bots = db.assistants(identifier=identifier)
+        bots = db.assistants(group=identifier)
         if bots is not None and len(bots) > 0:
             # got from database
             return bots
         return super().assistants(identifier=identifier)
-
-    #
-    #   EntityDataSource
-    #
-
-    # Override
-    def meta(self, identifier: ID) -> Optional[Meta]:
-        # if identifier.is_broadcast:
-        #     # broadcast ID has no meta
-        #     return None
-        db = self.database
-        return db.meta(identifier=identifier)
-
-    # Override
-    def document(self, identifier: ID, doc_type: str = '*') -> Optional[Document]:
-        # if identifier.is_broadcast:
-        #     # broadcast ID has no document
-        #     return None
-        db = self.database
-        return db.document(identifier=identifier, doc_type=doc_type)
```

### Comparing `dimples-0.1.4/dimples/common/messenger.py` & `dimples-0.1.5/dimples/edge/octopus.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # ==============================================================================
 # MIT License
 #
-# Copyright (c) 2022 Albert Moky
+# Copyright (c) 2019 Albert Moky
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -20,265 +20,317 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 """
-    Common extensions for Messenger
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+    Octopus
+    ~~~~~~~
 
-    Transform and send message
+    Edges for neighbor stations
 """
 
+import threading
+import time
+import weakref
 from abc import ABC, abstractmethod
-from typing import Optional, Tuple
+from typing import Optional, List, Set
 
-from dimsdk import ID
-from dimsdk import InstantMessage, SecureMessage, ReliableMessage
-from dimsdk import Content, Envelope
-from dimsdk import GroupCommand
-from dimsdk import EntityDelegate, CipherKeyDelegate
-from dimsdk import Messenger, Packer, Processor
+from dimsdk import ContentType
+from dimsdk import EntityType, ID
+from dimsdk import ReliableMessage
 
 from ..utils import Logging
-from ..utils import QueryFrequencyChecker
+from ..utils import Runner
+from ..common import CommonFacebook
+from ..common import MessageDBI, SessionDBI
+from ..common import HandshakeCommand
+from ..conn.session import get_sig
 
-from .dbi import MessageDBI
+from ..client import ClientSession
+from ..client import ClientMessenger
+from ..client import ClientMessagePacker
+from ..client import ClientMessageProcessor
+from ..client import Terminal
 
-from .facebook import CommonFacebook
-from .transmitter import Transmitter
-from .session import Session
+from .shared import GlobalVariable
+from .shared import create_session
 
 
-class CommonMessenger(Messenger, Transmitter, Logging, ABC):
+class Octopus(Runner, Logging):
 
-    def __init__(self, session: Session, facebook: CommonFacebook, database: MessageDBI):
+    def __init__(self, shared: GlobalVariable, local_host: str = '127.0.0.1', local_port: int = 9394):
         super().__init__()
-        self.__session = session
-        self.__facebook = facebook
-        self.__database = database
-        self.__packer: Optional[Packer] = None
-        self.__processor: Optional[Processor] = None
-
-    @property  # Override
-    def packer(self) -> Packer:
-        return self.__packer
-
-    @packer.setter
-    def packer(self, delegate: Packer):
-        self.__packer = delegate
-
-    @property  # Override
-    def processor(self) -> Processor:
-        return self.__processor
-
-    @processor.setter
-    def processor(self, delegate: Processor):
-        self.__processor = delegate
+        self.__shared = shared
+        self.__inner = self.create_inner_terminal(host=local_host, port=local_port)
+        self.__outers: Set[Terminal] = set()
+        self.__outer_map = weakref.WeakValueDictionary()
+        self.__outer_lock = threading.Lock()
 
     @property
-    def database(self) -> MessageDBI:
-        return self.__database
+    def shared(self) -> GlobalVariable:
+        return self.__shared
 
-    @property  # Override
-    def key_cache(self) -> CipherKeyDelegate:
-        return self.__database
-
-    @property  # Override
-    def barrack(self) -> EntityDelegate:
-        return self.__facebook
+    @property
+    def database(self) -> SessionDBI:
+        return self.__shared.sdb
 
     @property
-    def facebook(self) -> CommonFacebook:
-        return self.__facebook
+    def inner_messenger(self) -> ClientMessenger:
+        terminal = self.__inner
+        return terminal.messenger
+
+    def get_outer_messenger(self, identifier: ID) -> Optional[ClientMessenger]:
+        with self.__outer_lock:
+            terminal = self.__outer_map.get(identifier)
+        if terminal is not None:
+            return terminal.messenger
+
+    def create_inner_terminal(self, host: str, port: int) -> Terminal:
+        shared = self.shared
+        session = create_session(facebook=shared.facebook, database=shared.sdb, host=host, port=port)
+        messenger = create_messenger(facebook=shared.facebook, database=shared.mdb,
+                                     session=session, messenger_class=InnerMessenger)
+        messenger.octopus = self
+        return create_terminal(messenger=messenger)
+
+    def create_outer_terminal(self, host: str, port: int) -> Terminal:
+        shared = self.shared
+        session = create_session(facebook=shared.facebook, database=shared.sdb, host=host, port=port)
+        messenger = create_messenger(facebook=shared.facebook, database=shared.mdb,
+                                     session=session, messenger_class=OuterMessenger)
+        messenger.octopus = self
+        return create_terminal(messenger=messenger)
+
+    def add_index(self, identifier: ID, terminal: Terminal):
+        with self.__outer_lock:
+            # self.__outers.add(terminal)
+            self.__outer_map[identifier] = terminal
+
+    def connect(self, host: str, port: int = 9394):
+        terminal = self.create_outer_terminal(host=host, port=port)
+        with self.__outer_lock:
+            self.__outers.add(terminal)
+
+    def start(self):
+        thread = threading.Thread(target=self.run)
+        thread.start()
+
+    # Override
+    def stop(self):
+        super().stop()
+        inner = self.__inner
+        if inner is not None:
+            inner.stop()
+        with self.__outer_lock:
+            outers = set(self.__outers)
+        for out in outers:
+            out.stop()
+
+    # Override
+    def _idle(self):
+        time.sleep(60)
+
+    # Override
+    def process(self) -> bool:
+        # get all neighbor stations
+        db = self.database
+        providers = db.all_providers()
+        assert len(providers) > 0, 'service provider not found'
+        gsp = providers[0].identifier
+        neighbors = db.all_stations(provider=gsp)
+        # get all outer terminals
+        with self.__outer_lock:
+            outers = set(self.__outers)
+        for out in outers:
+            # check station
+            station = out.session.station
+            host = station.host
+            port = station.port
+            for item in neighbors:
+                if item.port == port and item.host == host:
+                    # got
+                    neighbors.remove(item)
+                    break
+            if out.is_alive:
+                # outer terminal alive, ignore it
+                continue
+            # remove dead terminal
+            sid = station.identifier
+            with self.__outer_lock:
+                self.__outers.discard(out)
+                if sid is not None:
+                    self.__outer_map.pop(sid, None)
+        # check new neighbors
+        for item in neighbors:
+            host = item.host
+            port = item.port
+            self.info(msg='connecting neighbor station (%s:%d)' % (host, port))
+            self.connect(host=host, port=port)
+        return False
+
+    def income_message(self, msg: ReliableMessage, priority: int = 0) -> List[ReliableMessage]:
+        """ redirect message from remote station """
+        sig = get_sig(msg=msg)
+        messenger = self.inner_messenger
+        if messenger.send_reliable_message(msg=msg, priority=priority):
+            self.info(msg='redirected msg (%s) for receiver (%s)' % (sig, msg.receiver))
+        else:
+            self.error(msg='failed to redirect msg (%s) for receiver (%s)' % (sig, msg.receiver))
+        # no need to respond receipt for station
+        return []
+
+    def outgo_message(self, msg: ReliableMessage, priority: int = 0) -> List[ReliableMessage]:
+        """ redirect message to remote station """
+        target = ID.parse(identifier=msg.get('neighbor'))
+        if target is None:
+            # target station not found
+            self.info(msg='cannot get target station for receiver (%s)' % msg.receiver)
+            return []
+        messenger = self.get_outer_messenger(identifier=target)
+        if messenger is None:
+            # target station not my neighbor
+            self.info(msg='receiver (%s) is targeted to (%s), but not my neighbor' % (msg.receiver, target))
+            return []
+        msg.pop('neighbor', None)
+        if messenger.send_reliable_message(msg=msg, priority=priority):
+            sig = get_sig(msg=msg)
+            self.info(msg='redirected msg (%s) to target (%s) for receiver (%s)' % (sig, target, msg.receiver))
+            # no need to respond receipt for station
+            return []
+        sig = get_sig(msg=msg)
+        self.error(msg='failed to redirect msg (%s) to target (%s) for receiver (%s)' % (sig, target, msg.receiver))
+        return []
+
+
+class OctopusMessenger(ClientMessenger, ABC):
+    """ Messenger for processing message from remote station """
+
+    def __init__(self, session: ClientSession, facebook: CommonFacebook, database: MessageDBI):
+        super().__init__(session=session, facebook=facebook, database=database)
+        self.__terminal: Optional[weakref.ReferenceType] = None
+        self.__octopus: Optional[weakref.ReferenceType] = None
 
     @property
-    def session(self) -> Session:
-        return self.__session
+    def terminal(self) -> Terminal:
+        return self.__terminal()
 
-    @abstractmethod
-    def _query_meta(self, identifier: ID) -> bool:
-        """ request for meta with entity ID """
-        raise NotImplemented
+    @terminal.setter
+    def terminal(self, client: Terminal):
+        self.__terminal = weakref.ref(client)
 
-    @abstractmethod
-    def _query_document(self, identifier: ID) -> bool:
-        """ request for meta & visa document with entity ID """
-        raise NotImplemented
-
-    def _query_members(self, identifier: ID) -> bool:
-        """ request for group members with group ID """
-        checker = QueryFrequencyChecker()
-        if not checker.members_query_expired(identifier=identifier):
-            # query not expired yet
-            self.debug(msg='members query not expired yet: %s' % identifier)
-            return False
-        assert identifier.is_group, 'group ID error: %s' % identifier
-        group = self.facebook.group(identifier=identifier)
-        # request to group bots
-        assistants = group.assistants
-        if assistants is None or len(assistants) == 0:
-            self.error(msg='group assistants not found: %s' % identifier)
-            return False
-        self.info(msg='querying members of %s from assistants: %s' % (identifier, ID.revert(array=assistants)))
-        cmd = GroupCommand.query(group=identifier)
-        for bot in assistants:
-            self.send_content(sender=None, receiver=bot, content=cmd, priority=1)
-        return True
-
-    def _check_sender(self, msg: ReliableMessage) -> bool:
-        """ check whether msg.sender is ready """
-        sender = msg.sender
-        assert sender.is_user, 'sender error: %s' % sender
-        # check sender's meta & document
-        visa = msg.visa
-        if visa is not None:
-            # first handshake?
-            assert visa.identifier == sender, 'visa ID not match: %s => %s' % (sender, visa)
-            # assert Meta.match_id(meta=msg.meta, identifier=sender), 'meta error: %s' % msg
-            return True
+    @property
+    def octopus(self):
+        bot = self.__octopus()
+        assert isinstance(bot, Octopus), 'octopus error: %s' % bot
+        return bot
+
+    @octopus.setter
+    def octopus(self, bot):
+        self.__octopus = weakref.ref(bot)
+
+    @property
+    def local_station(self) -> ID:
         facebook = self.facebook
-        visa_key = facebook.public_key_for_encryption(identifier=sender)
-        if visa_key is not None:
-            # sender is OK
-            return True
-        if self._query_document(identifier=sender):
-            self.info(msg='querying document for sender: %s' % sender)
-        msg['error'] = {
-            'message': 'verify key not found',
-            'user': str(sender),
-        }
+        current = facebook.current_user
+        return current.identifier
 
-    def _check_receiver(self, msg: InstantMessage) -> bool:
-        """ check whether msg.receiver is ready """
+    def __is_handshaking(self, msg: ReliableMessage) -> bool:
+        """ check HandshakeCommand sent to this station """
         receiver = msg.receiver
-        if receiver.is_broadcast:
-            # broadcast message
-            return True
-        facebook = self.facebook
-        if receiver.is_user:
-            # check user's meta & document
-            visa_key = facebook.public_key_for_encryption(identifier=receiver)
-            if visa_key is None:
-                if self._query_document(identifier=receiver):
-                    self.info(msg='querying document for receiver: %s' % receiver)
-                msg['error'] = {
-                    'message': 'encrypt key not found',
-                    'user': str(receiver),
-                }
-                return False
-        else:
-            # check group's meta
-            meta = facebook.meta(identifier=receiver)
-            if meta is None:
-                if self._query_meta(identifier=receiver):
-                    self.info(msg='querying meta for group: %s' % receiver)
-                msg['error'] = {
-                    'message': 'group meta not found',
-                    'group': str(receiver),
-                }
-                return False
-            # check group members
-            members = facebook.members(identifier=receiver)
-            if members is None or len(members) == 0:
-                if self._query_members(identifier=receiver):
-                    self.info(msg='querying members for group: %s' % receiver)
-                msg['error'] = {
-                    'message': 'members not found',
-                    'group': str(receiver),
-                }
-                return False
-            waiting = set()
-            for item in members:
-                visa_key = facebook.public_key_for_encryption(identifier=item)
-                if visa_key is None:
-                    if self._query_document(identifier=item):
-                        self.info(msg='querying document for member: %s, group: %s' % (item, receiver))
-                    waiting.add(item)
-            if len(waiting) > 0:
-                msg['error'] = {
-                    'message': 'encrypt keys not found',
-                    'group': str(receiver),
-                    'members': ID.revert(array=waiting)
-                }
-                return False
-        # receiver is OK
-        return True
-
-    # # Override
-    # def serialize_key(self, key: Union[dict, SymmetricKey], msg: InstantMessage) -> Optional[bytes]:
-    #     # try to reuse message key
-    #     reused = key.get('reused')
-    #     if reused is not None:
-    #         if msg.receiver.is_group:
-    #             # reuse key for grouped message
-    #             return None
-    #         # remove before serialize key
-    #         key.pop('reused', None)
-    #     data = super().serialize_key(key=key, msg=msg)
-    #     if reused is not None:
-    #         # put it back
-    #         key['reused'] = reused
-    #     return data
+        if receiver.type != EntityType.STATION or receiver != self.local_station:
+            # not for this station
+            return False
+        if msg.type != ContentType.COMMAND:
+            # not a command
+            return False
+        i_msg = self.decrypt_message(msg=msg)
+        if i_msg is not None:
+            return isinstance(i_msg.content, HandshakeCommand)
 
     # Override
-    def encrypt_message(self, msg: InstantMessage) -> Optional[SecureMessage]:
-        if self._check_receiver(msg=msg):
-            return super().encrypt_message(msg=msg)
-        else:
-            # receiver not ready
-            self.warning(msg='receiver not ready: %s' % msg.receiver)
+    def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+        # check for HandshakeCommand
+        if self.__is_handshaking(msg=msg):
+            self.info(msg='receive handshaking: %s' % msg.sender)
+            return super().process_reliable_message(msg=msg)
+        # check for cycled message
+        if msg.receiver == msg.sender:
+            self.error(msg='drop cycled msg(type=%d): %s -> %s | from %s, traces: %s'
+                       % (msg.type, msg.sender, msg.receiver, get_remote_station(messenger=self), msg.get('traces')))
+            return []
+        # handshake accepted, redirecting message
+        sig = get_sig(msg=msg)
+        self.info(msg='redirect msg(type=%d, sig=%s): %s -> %s | from %s, traces: %s'
+                  % (msg.type, sig, msg.sender, msg.receiver, get_remote_station(messenger=self), msg.get('traces')))
+        return self.deliver_message(msg=msg)
+
+    @abstractmethod
+    def deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+        """ call octopus to redirect message """
+        pass
+
+
+def get_remote_station(messenger: ClientMessenger) -> ID:
+    session = messenger.session
+    station = session.station
+    return station.identifier
+
+
+class InnerMessenger(OctopusMessenger):
+    """ Messenger for local station """
 
     # Override
-    def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
-        if self._check_sender(msg=msg):
-            return super().verify_message(msg=msg)
-        else:
-            # sender not ready
-            self.warning(msg='sender not ready: %s' % msg.sender)
+    def deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+        priority = 0  # NORMAL
+        if msg.receiver.is_broadcast:
+            priority = 1  # SLOWER
+        octopus = self.octopus
+        return octopus.outgo_message(msg=msg, priority=priority)
+
 
-    #
-    #   Interfaces for Transmitting Message
-    #
+class OuterMessenger(OctopusMessenger):
+    """ Messenger for remote station """
 
     # Override
-    def send_content(self, sender: Optional[ID], receiver: ID, content: Content,
-                     priority: int = 0) -> Tuple[InstantMessage, Optional[ReliableMessage]]:
-        """ Send message content with priority """
-        # Application Layer should make sure user is already login before it send message to server.
-        # Application layer should put message into queue so that it will send automatically after user login
-        if sender is None:
-            current = self.facebook.current_user
-            assert current is not None, 'current user not set'
-            sender = current.identifier
-        env = Envelope.create(sender=sender, receiver=receiver)
-        i_msg = InstantMessage.create(head=env, body=content)
-        r_msg = self.send_instant_message(msg=i_msg, priority=priority)
-        return i_msg, r_msg
+    def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+        if msg.sender == self.local_station:
+            self.debug(msg='cycled message from this station: %s => %s' % (msg.sender, msg.receiver))
+            return []
+        return super().process_reliable_message(msg=msg)
 
     # Override
-    def send_instant_message(self, msg: InstantMessage, priority: int = 0) -> Optional[ReliableMessage]:
-        """ send instant message with priority """
-        # send message (secured + certified) to target station
-        s_msg = self.encrypt_message(msg=msg)
-        if s_msg is None:
-            # public key not found?
-            return None
-        r_msg = self.sign_message(msg=s_msg)
-        if r_msg is None:
-            # TODO: set msg.state = error
-            raise AssertionError('failed to sign message: %s' % s_msg)
-        if self.send_reliable_message(msg=r_msg, priority=priority):
-            return r_msg
-        # failed
+    def deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+        priority = 0  # NORMAL
+        if msg.receiver.is_broadcast:
+            priority = 1  # SLOWER
+        octopus = self.octopus
+        return octopus.income_message(msg=msg, priority=priority)
 
     # Override
-    def send_reliable_message(self, msg: ReliableMessage, priority: int = 0) -> bool:
-        """ send reliable message with priority """
-        # 1. serialize message
-        data = self.serialize_message(msg=msg)
-        assert data is not None, 'failed to serialize message: %s' % msg
-        # 2. call gate keeper to send the message data package
-        #    put message package into the waiting queue of current session
-        session = self.session
-        return session.queue_message_package(msg=msg, data=data, priority=priority)
+    def handshake_success(self):
+        super().handshake_success()
+        station = self.session.station
+        octopus = self.octopus
+        octopus.add_index(identifier=station.identifier, terminal=self.terminal)
+
+
+def create_messenger(facebook: CommonFacebook, database: MessageDBI,
+                     session: ClientSession, messenger_class) -> OctopusMessenger:
+    assert issubclass(messenger_class, OctopusMessenger), 'messenger class error: %s' % messenger_class
+    # 1. create messenger with session and MessageDB
+    messenger = messenger_class(session=session, facebook=facebook, database=database)
+    # 2. create packer, processor for messenger
+    #    they have weak references to facebook & messenger
+    messenger.packer = ClientMessagePacker(facebook=facebook, messenger=messenger)
+    messenger.processor = ClientMessageProcessor(facebook=facebook, messenger=messenger)
+    # 3. set weak reference to messenger
+    session.messenger = messenger
+    return messenger
+
+
+def create_terminal(messenger: OctopusMessenger) -> Terminal:
+    terminal = Terminal(messenger=messenger)
+    messenger.terminal = terminal
+    terminal.start()
+    return terminal
```

### Comparing `dimples-0.1.4/dimples/common/protocol/__init__.py` & `dimples-0.1.5/dimples/common/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/common/protocol/ans.py` & `dimples-0.1.5/dimples/common/protocol/report.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 #
 #   DIMP : Decentralized Instant Messaging Protocol
 #
-#                                Written in 2023 by Moky <albert.moky@gmail.com>
+#                                Written in 2020 by Moky <albert.moky@gmail.com>
 #
 # ==============================================================================
 # MIT License
 #
-# Copyright (c) 2023 Albert Moky
+# Copyright (c) 2020 Albert Moky
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -25,81 +25,58 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 """
-    ANS Protocol
-    ~~~~~~~~~~~~
+    Report Protocol
+    ~~~~~~~~~~~~~~~
 
-    Query/respond ANS records
+    Report for online/offline, ...
 """
 
-from typing import Optional, Union, Any, List, Dict
+from typing import Any, Dict
 
-from dimsdk import Command, BaseCommand
+from dimsdk import BaseCommand
 
 
-class AnsCommand(BaseCommand):
+class ReportCommand(BaseCommand):
     """
-        ANS Command
-        ~~~~~~~~~~~
+        Report Command
+        ~~~~~~~~~~~~~~
 
         data format: {
             type : 0x88,
             sn   : 123,
 
-            cmd     : "ans",
-            names   : "...",        // query with alias(es, separated by ' ')
-            records : {             // respond with record(s)
-                "{alias}": "{ID}",
-            }
+            cmd     : "report",
+            title   : "online",   // or "offline"
+            time    : 1234567890
         }
     """
 
-    ANS = 'ans'
+    REPORT = 'report'
 
-    def __init__(self, content: Dict[str, Any] = None, names: str = None):
+    ONLINE = 'online'
+    OFFLINE = 'offline'
+
+    def __init__(self, content: Dict[str, Any] = None, title: str = None):
         if content is None:
-            # create with names
-            super().__init__(cmd=AnsCommand.ANS)
-            if names is not None:
-                self['names'] = names
+            # create with title
+            super().__init__(cmd=ReportCommand.REPORT)
+            if title is not None:
+                self['title'] = title
         else:
             # create with command content
             super().__init__(content=content)
 
     #
-    #   ANS aliases
+    #   report title
     #
     @property
-    def names(self) -> Optional[List[str]]:
-        string = self.get('names')
-        if isinstance(string, str):
-            return string.split()
-
-    @property
-    def records(self) -> Optional[Dict[str, str]]:
-        return self.get('records')
-
-    @records.setter
-    def records(self, value: Dict[str, str]):
-        self['records'] = value
-
-    #
-    #   Factories
-    #
+    def title(self) -> str:
+        return self.get_str(key='title', default='')
 
-    @classmethod
-    def query(cls, names: Union[str, list]) -> Command:
-        if isinstance(names, list):
-            names = ' '.join(names)
-        return cls(names=names)
-
-    @classmethod
-    def response(cls, names: Union[str, list], records: Dict[str, str]) -> Command:
-        if isinstance(names, list):
-            names = ' '.join(names)
-        command = cls(names=names)
-        command.records = records
-        return command
+    @title.setter
+    def title(self, value: str):
+        self['title'] = value
```

### Comparing `dimples-0.1.4/dimples/common/protocol/handshake.py` & `dimples-0.1.5/dimples/common/protocol/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/common/protocol/login.py` & `dimples-0.1.5/dimples/common/protocol/login.py`

 * *Files 9% similar despite different names*

```diff
@@ -111,39 +111,39 @@
         else:
             self['agent'] = value
 
     #
     #   Server Info
     #
     @property
-    def station(self) -> Optional[dict]:
+    def station(self) -> Optional[Dict]:
         return self.get('station')
 
     @station.setter
-    def station(self, value: Union[dict, Station]):
+    def station(self, value: Union[Dict, Station]):
         if value is None:
             self.pop('station', None)
-        elif isinstance(value, dict):
+        elif isinstance(value, Dict):
             self['station'] = value
         else:
             assert isinstance(value, Station), 'station error: %s' % value
             self['station'] = {
                 'ID': str(value.identifier),
                 'host': value.host,
                 'port': value.port,
             }
 
     @property
-    def provider(self) -> Optional[dict]:
+    def provider(self) -> Optional[Dict]:
         return self.get('provider')
 
     @provider.setter
-    def provider(self, value: Union[dict, ServiceProvider]):
+    def provider(self, value: Union[Dict, ServiceProvider]):
         if value is None:
             self.pop('provider', None)
-        elif isinstance(value, dict):
+        elif isinstance(value, Dict):
             self['provider'] = value
         else:
             assert isinstance(value, ServiceProvider), 'SP error: %s' % value
             self['provider'] = {
                 'ID': str(value.identifier),
             }
```

### Comparing `dimples-0.1.4/dimples/common/protocol/receipt.py` & `dimples-0.1.5/dimples/common/protocol/receipt.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     ~~~~~~~~~~~~~~~~
 
     As receipt returned to sender to proofing the message's received
 """
 
 from typing import Optional, Union, Any, Dict
 
-from dimsdk import Envelope, ReliableMessage
+from dimsdk import Envelope, InstantMessage, ReliableMessage
 from dimsdk import BaseCommand
 
 from ...utils import base64_encode
 
 
 class ReceiptCommand(BaseCommand):
     """
@@ -99,35 +99,61 @@
     # -------- setters/getters
 
     @property
     def text(self) -> Optional[str]:
         return self.get('text')
 
     @property  # private
-    def origin(self) -> dict:
+    def origin(self) -> Optional[Dict]:
         return self.get('origin')
 
     @property
     def original_envelope(self) -> Optional[Envelope]:
         if self.__envelope is None:
             # origin: { sender: "...", receiver: "...", time: 0 }
             origin = self.origin
             if origin is not None and 'sender' in origin:
                 self.__envelope = Envelope.parse(envelope=origin)
         return self.__envelope
 
     @property
     def original_sn(self) -> int:
         origin = self.origin
-        return 0 if origin is None else origin.get('sn')
+        if origin is None:
+            return 0
+        sn = origin.get('sn')
+        return 0 if sn is None else sn
 
     @property
     def original_signature(self) -> Optional[str]:
         origin = self.origin
-        return None if origin is None else origin.get('signature')
+        if origin is None:
+            return None
+        return origin.get('signature')
+
+    def match_message(self, msg: InstantMessage) -> bool:
+        # check signature
+        sig1 = self.original_signature
+        if sig1 is not None:
+            # if contains signature, check it
+            sig2 = msg.get_str(key='signature')
+            if sig2 is not None:
+                if len(sig1) > 8:
+                    sig1 = sig1[-8:]
+                if len(sig2) > 8:
+                    sig2 = sig2[-8:]
+                return sig1 == sig2
+        # check envelope
+        env1 = self.original_envelope
+        if env1 is not None:
+            # if contains envelope, check it
+            return env1 == msg.envelope
+        # check serial number
+        # (only the original message's receiver can know this number)
+        return self.original_sn == msg.content.sn
 
     #
     #   Factory method
     #
 
     @classmethod
     def create(cls, text: str = None, msg: ReliableMessage = None):
```

### Comparing `dimples-0.1.4/dimples/common/protocol/report.py` & `dimples-0.1.5/dimples/common/protocol/ans.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 #
 #   DIMP : Decentralized Instant Messaging Protocol
 #
-#                                Written in 2020 by Moky <albert.moky@gmail.com>
+#                                Written in 2023 by Moky <albert.moky@gmail.com>
 #
 # ==============================================================================
 # MIT License
 #
-# Copyright (c) 2020 Albert Moky
+# Copyright (c) 2023 Albert Moky
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -25,58 +25,82 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 """
-    Report Protocol
-    ~~~~~~~~~~~~~~~
+    ANS Protocol
+    ~~~~~~~~~~~~
 
-    Report for online/offline, ...
+    Query/respond ANS records
 """
 
-from typing import Any, Dict
+from typing import Union, Any, List, Dict
 
-from dimsdk import BaseCommand
+from dimsdk import Command, BaseCommand
 
 
-class ReportCommand(BaseCommand):
+class AnsCommand(BaseCommand):
     """
-        Report Command
-        ~~~~~~~~~~~~~~
+        ANS Command
+        ~~~~~~~~~~~
 
         data format: {
             type : 0x88,
             sn   : 123,
 
-            cmd     : "report",
-            title   : "online",   // or "offline"
-            time    : 1234567890
+            cmd     : "ans",
+            names   : "...",        // query with alias(es, separated by ' ')
+            records : {             // respond with record(s)
+                "{alias}": "{ID}",
+            }
         }
     """
 
-    REPORT = 'report'
+    ANS = 'ans'
 
-    ONLINE = 'online'
-    OFFLINE = 'offline'
-
-    def __init__(self, content: Dict[str, Any] = None, title: str = None):
+    def __init__(self, content: Dict[str, Any] = None, names: str = None):
         if content is None:
-            # create with title
-            super().__init__(cmd=ReportCommand.REPORT)
-            if title is not None:
-                self['title'] = title
+            # create with names
+            super().__init__(cmd=AnsCommand.ANS)
+            if names is not None:
+                self['names'] = names
         else:
             # create with command content
             super().__init__(content=content)
 
     #
-    #   report title
+    #   ANS aliases
     #
     @property
-    def title(self) -> str:
-        return self.get('title')
+    def names(self) -> List[str]:
+        string = self.get_str('names')
+        return [] if string is None else string.split()
+
+    @property
+    def records(self) -> Dict[str, str]:
+        dictionary = self.get('records')
+        return {} if dictionary is None else dictionary
+
+    @records.setter
+    def records(self, value: Dict[str, str]):
+        """ get map for (name => ID string) """
+        self['records'] = value
+
+    #
+    #   Factories
+    #
 
-    @title.setter
-    def title(self, value: str):
-        self['title'] = value
+    @classmethod
+    def query(cls, names: Union[str, List[str]]) -> Command:
+        if isinstance(names, List):
+            names = ' '.join(names)
+        return cls(names=names)
+
+    @classmethod
+    def response(cls, names: Union[str, List[str]], records: Dict[str, str]) -> Command:
+        if isinstance(names, List):
+            names = ' '.join(names)
+        command = cls(names=names)
+        command.records = records
+        return command
```

### Comparing `dimples-0.1.4/dimples/common/session.py` & `dimples-0.1.5/dimples/database/t_cipherkey.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 # -*- coding: utf-8 -*-
-#
-#   DIM-SDK : Decentralized Instant Messaging Software Development Kit
-#
-#                                Written in 2021 by Moky <albert.moky@gmail.com>
-#
 # ==============================================================================
 # MIT License
 #
-# Copyright (c) 2021 Albert Moky
+# Copyright (c) 2022 Albert Moky
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -24,71 +19,58 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-from abc import ABC, abstractmethod
-from typing import Optional, Tuple
+import time
+from typing import Optional
+
+from dimsdk import ID, SymmetricKey
+from dimplugins import PlainKey
 
-from dimp import ID, ReliableMessage
+from ..utils import CacheManager
+from ..common import CipherKeyDBI
 
-from .dbi import SessionDBI
 
-from .transmitter import Transmitter
+class CipherKeyTable(CipherKeyDBI):
+    """ Implementations of CipherKeyDBI """
+
+    # noinspection PyUnusedLocal
+    def __init__(self, root: str = None, public: str = None, private: str = None):
+        super().__init__()
+        man = CacheManager()
+        self.__cipher_cache = man.get_pool(name='cipher')  # (ID, ID) => SymmetricKey
+
+    # noinspection PyMethodMayBeStatic
+    def show_info(self):
+        print('!!!      cipher key in memory only !!!')
+
+    #
+    #   CipherKey DBI
+    #
+
+    # Override
+    def cipher_key(self, sender: ID, receiver: ID, generate: bool = False) -> Optional[SymmetricKey]:
+        if receiver.is_broadcast:
+            return plain_key
+        now = time.time()
+        key, _ = self.__cipher_cache.fetch(key=(sender, receiver), now=now)
+        if key is None and generate:
+            # generate and cache it
+            key = SymmetricKey.generate(algorithm=SymmetricKey.AES)
+            assert key is not None, 'failed to generate symmetric key'
+            self.__cipher_cache.update(key=(sender, receiver), value=key, life_span=3600*24*7, now=now)
+        return key
+
+    # Override
+    def cache_cipher_key(self, key: SymmetricKey, sender: ID, receiver: ID):
+        if receiver.is_broadcast:
+            # no need to store cipher key for broadcast message
+            return False
+        now = time.time()
+        self.__cipher_cache.update(key=(sender, receiver), value=key, life_span=3600*24*7, now=now)
+        return True
 
 
-class Session(Transmitter, ABC):
-
-    @property
-    def database(self) -> SessionDBI:
-        """ Session Database """
-        raise NotImplemented
-
-    @property
-    def remote_address(self) -> Tuple[str, int]:
-        """ Remote (host, port) """
-        raise NotImplemented
-
-    @property
-    def key(self) -> Optional[str]:
-        """ Session Key """
-        raise NotImplemented
-
-    @property
-    def identifier(self) -> Optional[ID]:
-        """ Login User ID """
-        raise NotImplemented
-
-    def set_identifier(self, identifier: ID) -> bool:
-        """ Update ID and return True on changed """
-        raise NotImplemented
-
-    @property
-    def active(self) -> bool:
-        """ Session active """
-        raise NotImplemented
-
-    @abstractmethod
-    def set_active(self, active: bool, when: float = None):
-        """ Update active flag and return True on changed """
-        raise NotImplemented
-
-    def __str__(self) -> str:
-        clazz = self.__class__.__name__
-        return '<%s:%s %s|%s active=%s />' % (clazz, self.key, self.remote_address, self.identifier, self.active)
-
-    def __repr__(self) -> str:
-        clazz = self.__class__.__name__
-        return '<%s:%s %s|%s active=%s />' % (clazz, self.key, self.remote_address, self.identifier, self.active)
-
-    def queue_message_package(self, msg: ReliableMessage, data: bytes, priority: int = 0) -> bool:
-        """
-        Pack message into a waiting queue
-
-        :param msg:      network message
-        :param data:     serialized message
-        :param priority: smaller is faster
-        :return: False on error
-        """
-        raise NotImplemented
+plain_key = PlainKey()
```

### Comparing `dimples-0.1.4/dimples/common/transmitter.py` & `dimples-0.1.5/dimples/common/session.py`

 * *Files 24% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 from abc import ABC, abstractmethod
 from typing import Optional, Tuple
 
 from dimp import ID
 from dimp import Content
 from dimp import InstantMessage, ReliableMessage
 
+from .dbi import SessionDBI
+
 
 class Transmitter(ABC):
 
     @abstractmethod
     def send_content(self, sender: Optional[ID], receiver: ID, content: Content,
                      priority: int = 0) -> Tuple[InstantMessage, Optional[ReliableMessage]]:
         """
@@ -69,7 +71,63 @@
         Send reliable message with priority
 
         :param msg:      encrypted & signed message
         :param priority: smaller is faster
         :return: False on error
         """
         raise NotImplemented
+
+
+class Session(Transmitter, ABC):
+
+    @property
+    def database(self) -> SessionDBI:
+        """ Session Database """
+        raise NotImplemented
+
+    @property
+    def remote_address(self) -> Tuple[str, int]:
+        """ Remote (host, port) """
+        raise NotImplemented
+
+    @property
+    def key(self) -> Optional[str]:
+        """ Session Key """
+        raise NotImplemented
+
+    @property
+    def identifier(self) -> Optional[ID]:
+        """ Login User ID """
+        raise NotImplemented
+
+    def set_identifier(self, identifier: ID) -> bool:
+        """ Update ID and return True on changed """
+        raise NotImplemented
+
+    @property
+    def active(self) -> bool:
+        """ Session active """
+        raise NotImplemented
+
+    @abstractmethod
+    def set_active(self, active: bool, when: float = None):
+        """ Update active flag and return True on changed """
+        raise NotImplemented
+
+    def __str__(self) -> str:
+        clazz = self.__class__.__name__
+        return '<%s:%s %s|%s active=%s />' % (clazz, self.key, self.remote_address, self.identifier, self.active)
+
+    def __repr__(self) -> str:
+        clazz = self.__class__.__name__
+        return '<%s:%s %s|%s active=%s />' % (clazz, self.key, self.remote_address, self.identifier, self.active)
+
+    def queue_message_package(self, msg: ReliableMessage, data: bytes, priority: int = 0) -> bool:
+        """
+        Pack message into a waiting queue
+
+        :param msg:      network message
+        :param data:     serialized message
+        :param priority: smaller is faster
+        :return: False on error
+        """
+        raise NotImplemented
```

### Comparing `dimples-0.1.4/dimples/config.py` & `dimples-0.1.5/dimples/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,41 +29,43 @@
 from mkm.types import Dictionary
 from mkm import ID
 
 
 class Node(Dictionary):
     """ DIM Network Node """
 
-    def __init__(self, name: str = None, host: str = None, port: int = 0, identifier: ID = None):
+    def __init__(self, name: str = None, host: str = None, port: int = 0):
         super().__init__()
         if name is not None:
             self['name'] = name
         if host is not None:
             self['host'] = host
         if port > 0:
             self['port'] = port
-        if identifier is not None:
-            self['ID'] = str(identifier)
+
+    def __str__(self) -> str:
+        clazz = self.__class__.__name__
+        return '<%s host="%s" port=%d name="%s" />' % (clazz, self.host, self.port, self.name)
+
+    def __repr__(self) -> str:
+        clazz = self.__class__.__name__
+        return '<%s host="%s" port=%d name="%s" />' % (clazz, self.host, self.port, self.name)
 
     @property
     def name(self) -> str:
         return self.get('name')
 
     @property
     def host(self) -> str:
         return self.get('host')
 
     @property
     def port(self) -> int:
         return self.get('port')
 
-    @property
-    def identifier(self) -> ID:
-        return ID.parse(identifier=self.get('ID'))
-
 
 def get_socket_address(value: str) -> Tuple[str, int]:
     pair = value.split(':')
     if len(pair) == 2:
         return pair[0].strip(), int(pair[1])
     else:
         return pair[0].strip(), 9394
@@ -72,16 +74,16 @@
 def parse_nodes(nodes: Dict[str, str]) -> List[Node]:
     """ parse lines with 'name = host:port, ID' format """
     stations = []
     for name in nodes:
         value = nodes[name]
         pair = value.split(',')
         host, port = get_socket_address(value=pair[0])
-        sid = ID.parse(identifier=pair[1].strip())
-        stations.append(Node(name=name, host=host, port=port, identifier=sid))
+        node = Node(name=name, host=host, port=port)
+        stations.append(node)
     return stations
 
 
 def str_to_bool(value: Optional[str]) -> bool:
     if value is None or len(value) == 0:
         return False
     lower = value.lower()
```

### Comparing `dimples-0.1.4/dimples/conn/__init__.py` & `dimples-0.1.5/dimples/conn/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/conn/gate.py` & `dimples-0.1.5/dimples/conn/gate.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 from .mars import MarsStreamArrival, MarsStreamDocker, MarsHelper
 from .ws import WSDocker
 
 
 H = TypeVar('H')
 
 
+# noinspection PyAbstractClass
 class BaseGate(StarGate, Generic[H], ABC):
 
     def __init__(self, delegate: DockerDelegate):
         super().__init__(delegate=delegate)
         self.__hub: H = None
 
     @property
@@ -106,14 +107,15 @@
 
     # Override
     def _clear_advance_party(self, connection: Connection):
         # TODO: remove advance party for this connection
         pass
 
 
+# noinspection PyAbstractClass
 class CommonGate(BaseGate, Logging, Generic[H], ABC):
     """ Gate with Hub for connections """
 
     def __init__(self, delegate: DockerDelegate):
         super().__init__(delegate=delegate)
         self.__running = False
 
@@ -139,28 +141,28 @@
     # def _idle(self):
     #     time.sleep(0.25)
 
     # Override
     def connection_state_changed(self, previous: ConnectionState, current: ConnectionState, connection: Connection):
         # debug info
         if current is None or current == ConnectionState.ERROR:
-            self.error(msg='connection lost: %s -> %s, %s' % (previous, current, connection))
+            self.error(msg='connection lost: %s -> %s, %s' % (previous, current, connection.remote_address))
         elif current != ConnectionState.EXPIRED and current != ConnectionState.MAINTAINING:
-            self.debug(msg='connection state changed: %s -> %s, %s' % (previous, current, connection))
+            self.debug(msg='connection state changed: %s -> %s, %s' % (previous, current, connection.remote_address))
         super().connection_state_changed(previous=previous, current=current, connection=connection)
 
     # Override
     def connection_received(self, data: bytes, connection: Connection):
+        self.debug(msg='received %d byte(s): %s' % (len(data), connection.remote_address))
         super().connection_received(data=data, connection=connection)
-        self.debug(msg='received %d byte(s): %s' % (len(data), connection))
 
     # Override
     def connection_sent(self, sent: int, data: bytes, connection: Connection):
         super().connection_sent(sent=sent, data=data, connection=connection)
-        self.debug(msg='sent %d byte(s): %s' % (len(data), connection))
+        self.debug(msg='sent %d byte(s): %s' % (len(data), connection.remote_address))
 
     # Override
     def connection_failed(self, error: Union[IOError, socket.error], data: bytes, connection: Connection):
         super().connection_failed(error=error, data=data, connection=connection)
         self.error(msg='failed to send %d byte(s): %s, remote=%s' % (len(data), error, connection.remote_address))
 
     # Override
```

### Comparing `dimples-0.1.4/dimples/conn/gatekeeper.py` & `dimples-0.1.5/dimples/conn/gatekeeper.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/conn/mars.py` & `dimples-0.1.5/dimples/conn/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/conn/mtp.py` & `dimples-0.1.5/dimples/conn/mtp.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/conn/protocol/__init__.py` & `dimples-0.1.5/dimples/conn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/conn/protocol/mars.py` & `dimples-0.1.5/dimples/conn/protocol/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/conn/protocol/ws.py` & `dimples-0.1.5/dimples/conn/protocol/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/conn/queue.py` & `dimples-0.1.5/dimples/conn/queue.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/conn/seeker.py` & `dimples-0.1.5/dimples/conn/seeker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/conn/session.py` & `dimples-0.1.5/dimples/conn/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,22 +65,22 @@
     # Override
     def set_identifier(self, identifier: ID) -> bool:
         if self.__identifier != identifier:
             self.__identifier = identifier
             return True
 
     @property
-    def messenger(self) -> CommonMessenger:
+    def messenger(self) -> Optional[CommonMessenger]:
         ref = self.__messenger
-        assert ref is not None, 'messenger not set yet'
-        return ref()
+        if ref is not None:
+            return ref()
 
     @messenger.setter
     def messenger(self, transceiver: CommonMessenger):
-        self.__messenger = weakref.ref(transceiver)
+        self.__messenger = None if transceiver is None else weakref.ref(transceiver)
 
     # Override
     def queue_message_package(self, msg: ReliableMessage, data: bytes, priority: int = 0) -> bool:
         ship = self._docker_pack(payload=data, priority=priority)
         return self._queue_append(msg=msg, ship=ship)
 
     #
```

### Comparing `dimples-0.1.4/dimples/conn/ws.py` & `dimples-0.1.5/dimples/conn/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/database/__init__.py` & `dimples-0.1.5/dimples/database/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,34 +39,35 @@
 from .t_user import UserTable
 from .t_group import GroupTable
 
 from .t_message import ReliableMessageTable
 from .t_cipherkey import CipherKeyTable
 
 from .t_login import LoginTable
-from .t_provider import ProviderTable
+from .t_station import StationTable
 
 from .account import AccountDatabase
 from .message import MessageDatabase
 from .session import SessionDatabase
 
 
 __all__ = [
     #
     #   DBI
     #
     'PrivateKeyDBI', 'MetaDBI', 'DocumentDBI',
-    'UserDBI', 'GroupDBI',
+    'UserDBI', 'ContactDBI', 'GroupDBI',
     'AccountDBI',
 
     'ReliableMessageDBI', 'CipherKeyDBI',
     'MessageDBI',
 
-    'LoginDBI', 'ProviderDBI',
+    'LoginDBI', 'ProviderDBI', 'SessionDBI',
     'SessionDBI',
+    'StationInfo',
 
     #
     #   DOS
     #
     'Storage',
     'PrivateKeyStorage', 'MetaStorage', 'DocumentStorage',
     'UserStorage', 'GroupStorage',
@@ -74,15 +75,15 @@
 
     #
     #   Table
     #
     'PrivateKeyTable', 'MetaTable', 'DocumentTable',
     'UserTable', 'GroupTable',
     'ReliableMessageTable', 'CipherKeyTable',
-    'LoginTable', 'ProviderTable',
+    'LoginTable', 'StationTable',
 
     #
     #   Database
     #
     'AccountDatabase',
     'MessageDatabase',
     'SessionDatabase',
```

### Comparing `dimples-0.1.4/dimples/database/account.py` & `dimples-0.1.5/dimples/database/account.py`

 * *Files 22% similar despite different names*

```diff
@@ -59,28 +59,28 @@
         self.__group_table.show_info()
 
     #
     #   PrivateKey DBI
     #
 
     # Override
-    def save_private_key(self, key: PrivateKey, identifier: ID, key_type: str = 'M') -> bool:
-        return self.__private_table.save_private_key(key=key, identifier=identifier, key_type=key_type)
+    def save_private_key(self, key: PrivateKey, user: ID, key_type: str = 'M') -> bool:
+        return self.__private_table.save_private_key(key=key, user=user, key_type=key_type)
 
     # Override
-    def private_keys_for_decryption(self, identifier: ID) -> List[DecryptKey]:
-        return self.__private_table.private_keys_for_decryption(identifier=identifier)
+    def private_keys_for_decryption(self, user: ID) -> List[DecryptKey]:
+        return self.__private_table.private_keys_for_decryption(user=user)
 
     # Override
-    def private_key_for_signature(self, identifier: ID) -> Optional[SignKey]:
-        return self.__private_table.private_key_for_signature(identifier=identifier)
+    def private_key_for_signature(self, user: ID) -> Optional[SignKey]:
+        return self.__private_table.private_key_for_signature(user=user)
 
     # Override
-    def private_key_for_visa_signature(self, identifier: ID) -> Optional[SignKey]:
-        return self.__private_table.private_key_for_visa_signature(identifier=identifier)
+    def private_key_for_visa_signature(self, user: ID) -> Optional[SignKey]:
+        return self.__private_table.private_key_for_visa_signature(user=user)
 
     #
     #   Meta DBI
     #
 
     # Override
     def save_meta(self, meta: Meta, identifier: ID) -> bool:
@@ -120,41 +120,81 @@
         return self.__user_table.local_users()
 
     # Override
     def save_local_users(self, users: List[ID]) -> bool:
         return self.__user_table.save_local_users(users=users)
 
     # Override
-    def contacts(self, identifier: ID) -> List[ID]:
-        return self.__user_table.contacts(identifier=identifier)
+    def add_user(self, user: ID) -> bool:
+        return self.__user_table.add_user(user=user)
 
     # Override
-    def save_contacts(self, contacts: List[ID], identifier: ID) -> bool:
-        return self.__user_table.save_contacts(contacts=contacts, identifier=identifier)
+    def remove_user(self, user: ID) -> bool:
+        return self.__user_table.remove_user(user=user)
+
+    # Override
+    def current_user(self) -> Optional[ID]:
+        return self.__user_table.current_user()
+
+    # Override
+    def set_current_user(self, user: ID) -> bool:
+        return self.__user_table.set_current_user(user=user)
+
+    #
+    #   Contact DBI
+    #
+
+    # Override
+    def contacts(self, user: ID) -> List[ID]:
+        return self.__user_table.contacts(user=user)
+
+    # Override
+    def save_contacts(self, contacts: List[ID], user: ID) -> bool:
+        return self.__user_table.save_contacts(contacts=contacts, user=user)
+
+    # Override
+    def add_contact(self, contact: ID, user: ID) -> bool:
+        return self.__user_table.add_contact(contact=contact, user=user)
+
+    # Override
+    def remove_contact(self, contact: ID, user: ID) -> bool:
+        return self.__user_table.remove_contact(contact=contact, user=user)
 
     #
     #   Group DBI
     #
 
     # Override
-    def founder(self, identifier: ID) -> Optional[ID]:
-        return self.__group_table.founder(identifier=identifier)
+    def founder(self, group: ID) -> Optional[ID]:
+        return self.__group_table.founder(group=group)
+
+    # Override
+    def owner(self, group: ID) -> Optional[ID]:
+        return self.__group_table.owner(group=group)
+
+    # Override
+    def members(self, group: ID) -> List[ID]:
+        return self.__group_table.members(group=group)
+
+    # Override
+    def save_members(self, members: List[ID], group: ID) -> bool:
+        return self.__group_table.save_members(members=members, group=group)
 
     # Override
-    def owner(self, identifier: ID) -> Optional[ID]:
-        return self.__group_table.owner(identifier=identifier)
+    def add_member(self, member: ID, group: ID) -> bool:
+        return self.__group_table.add_member(member=member, group=group)
 
     # Override
-    def members(self, identifier: ID) -> List[ID]:
-        return self.__group_table.members(identifier=identifier)
+    def remove_member(self, member: ID, group: ID) -> bool:
+        return self.__group_table.remove_member(member=member, group=group)
 
     # Override
-    def assistants(self, identifier: ID) -> List[ID]:
-        return self.__group_table.assistants(identifier=identifier)
+    def remove_group(self, group: ID) -> bool:
+        return self.__group_table.remove_group(group=group)
 
     # Override
-    def save_members(self, members: List[ID], identifier: ID) -> bool:
-        return self.__group_table.save_members(members=members, identifier=identifier)
+    def assistants(self, group: ID) -> List[ID]:
+        return self.__group_table.assistants(group=group)
 
     # Override
-    def save_assistants(self, assistants: List[ID], identifier: ID) -> bool:
-        return self.__group_table.save_assistants(assistants=assistants, identifier=identifier)
+    def save_assistants(self, assistants: List[ID], group: ID) -> bool:
+        return self.__group_table.save_assistants(assistants=assistants, group=group)
```

### Comparing `dimples-0.1.4/dimples/database/dos/__init__.py` & `dimples-0.1.5/dimples/database/dos/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,20 +36,24 @@
 from .document import DocumentStorage
 
 from .user import UserStorage
 from .group import GroupStorage
 
 from .login import LoginStorage
 
+from .station import StationStorage
+
 __all__ = [
 
     'Storage',
 
     'PrivateKeyStorage',
     'MetaStorage',
     'DocumentStorage',
 
     'UserStorage',
     'GroupStorage',
 
     'LoginStorage',
+
+    'StationStorage',
 ]
```

### Comparing `dimples-0.1.4/dimples/database/dos/base.py` & `dimples-0.1.5/dimples/database/dos/base.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/database/dos/document.py` & `dimples-0.1.5/dimples/database/dos/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/database/dos/group.py` & `dimples-0.1.5/dimples/database/dos/meta.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,76 +19,53 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-from typing import List, Optional
+from typing import Optional
 
-from dimsdk import ID
+from dimsdk import ID, Meta
 
-from ...common import GroupDBI
+from ...common import MetaDBI
 
 from .base import Storage
 from .base import template_replace
 
 
-class GroupStorage(Storage, GroupDBI):
+class MetaStorage(Storage, MetaDBI):
     """
-        Group Storage
-        ~~~~~~~~~~~~~
-        file path: '.dim/private/{ADDRESS}/members.js'
+        Meta for Entities (User/Group)
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        file path: '.dim/public/{ADDRESS}/meta.js'
     """
-    members_path = '{PRIVATE}/{ADDRESS}/members.js'
+    meta_path = '{PUBLIC}/{ADDRESS}/meta.js'
 
     def show_info(self):
-        path = template_replace(self.members_path, 'PRIVATE', self._private)
-        print('!!!   members path: %s' % path)
+        path = template_replace(self.meta_path, 'PUBLIC', self._public)
+        print('!!!      meta path: %s' % path)
 
-    def __members_path(self, identifier: ID) -> str:
-        path = self.members_path
-        path = template_replace(path, 'PRIVATE', self._private)
+    def __meta_path(self, identifier: ID) -> str:
+        path = self.meta_path
+        path = template_replace(path, 'PUBLIC', self._public)
         return template_replace(path, 'ADDRESS', str(identifier.address))
 
     #
-    #   User DBI
+    #   Meta DBI
     #
 
     # Override
-    def founder(self, identifier: ID) -> Optional[ID]:
-        # TODO: load group founder
-        pass
+    def save_meta(self, meta: Meta, identifier: ID) -> bool:
+        """ save meta into file """
+        path = self.__meta_path(identifier=identifier)
+        self.info(msg='Saving meta into: %s' % path)
+        return self.write_json(container=meta.dictionary, path=path)
 
     # Override
-    def owner(self, identifier: ID) -> Optional[ID]:
-        # TODO: load group owner
-        pass
-
-    # Override
-    def members(self, identifier: ID) -> List[ID]:
-        """ load members from file """
-        path = self.__members_path(identifier=identifier)
-        self.info(msg='Loading members from: %s' % path)
-        contacts = self.read_json(path=path)
-        if contacts is None:
-            # members not found
-            return []
-        return ID.convert(array=contacts)
-
-    # Override
-    def assistants(self, identifier: ID) -> List[ID]:
-        # TODO: load group assistants
-        pass
-
-    # Override
-    def save_members(self, members: List[ID], identifier: ID) -> bool:
-        """ save members into file """
-        path = self.__members_path(identifier=identifier)
-        self.info(msg='Saving members into: %s' % path)
-        return self.write_json(container=ID.revert(array=members), path=path)
-
-    # Override
-    def save_assistants(self, assistants: List[ID], identifier: ID) -> bool:
-        # TODO: save assistants
-        self.info(msg='TODO: Saving assistants: %s -> %s' % (identifier, assistants))
-        return True
+    def meta(self, identifier: ID) -> Optional[Meta]:
+        """ load meta from file """
+        path = self.__meta_path(identifier=identifier)
+        self.info(msg='Loading meta from: %s' % path)
+        info = self.read_json(path=path)
+        if info is not None:
+            return Meta.parse(meta=info)
```

### Comparing `dimples-0.1.4/dimples/database/dos/login.py` & `dimples-0.1.5/dimples/database/dos/login.py`

 * *Files 18% similar despite different names*

```diff
@@ -53,31 +53,31 @@
         return template_replace(path, 'ADDRESS', str(identifier.address))
 
     #
     #   Login DBI
     #
 
     # Override
-    def login_command_message(self, identifier: ID) -> Tuple[Optional[LoginCommand], Optional[ReliableMessage]]:
+    def login_command_message(self, user: ID) -> Tuple[Optional[LoginCommand], Optional[ReliableMessage]]:
         """ load login command from file """
-        path = self.__login_path(identifier=identifier)
+        path = self.__login_path(identifier=user)
         self.info(msg='Loading login command from: %s' % path)
         info = self.read_json(path=path)
         if info is None:
             # login command not found
             return None, None
         cmd = info.get('cmd')
         msg = info.get('msg')
         if cmd is not None:
             cmd = LoginCommand(content=cmd)
         return cmd, ReliableMessage.parse(msg=msg)
 
     # Override
-    def save_login_command_message(self, identifier: ID, content: LoginCommand, msg: ReliableMessage) -> bool:
+    def save_login_command_message(self, user: ID, content: LoginCommand, msg: ReliableMessage) -> bool:
         """ save login command into file """
         info = {
             'cmd': content.dictionary,
             'msg': msg.dictionary
         }
-        path = self.__login_path(identifier=identifier)
+        path = self.__login_path(identifier=user)
         self.info(msg='Saving login command into: %s' % path)
         return self.write_json(container=info, path=path)
```

### Comparing `dimples-0.1.4/dimples/database/dos/private.py` & `dimples-0.1.5/dimples/database/dos/private.py`

 * *Files 12% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.info(msg='Loading identity private key from: %s' % path)
         info = self.read_json(path=path)
         if info is not None:
             return PrivateKey.parse(key=info)
 
     def _save_msg_key(self, key: PrivateKey, identifier: ID) -> bool:
         private_keys = self._load_msg_keys(identifier=identifier)
-        private_keys = insert_key(key=key, private_keys=private_keys)
+        private_keys = PrivateKeyDBI.insert(item=key, array=private_keys)
         if private_keys is None:
             # nothing changed
             return False
         plain = [item.dictionary for item in private_keys]
         path = self.__msg_keys_path(identifier=identifier)
         self.info(msg='Saving message private keys into: %s' % path)
         return self.write_json(container=plain, path=path)
@@ -105,57 +105,33 @@
         return keys
 
     #
     #   PrivateKey DBI
     #
 
     # Override
-    def save_private_key(self, key: PrivateKey, identifier: ID, key_type: str = 'M') -> bool:
+    def save_private_key(self, key: PrivateKey, user: ID, key_type: str = 'M') -> bool:
         if key_type == self.ID_KEY_TAG:
             # save private key for meta
-            return self._save_id_key(key=key, identifier=identifier)
+            return self._save_id_key(key=key, identifier=user)
         else:
             # save private key for visa
-            return self._save_msg_key(key=key, identifier=identifier)
+            return self._save_msg_key(key=key, identifier=user)
 
     # Override
-    def private_keys_for_decryption(self, identifier: ID) -> List[DecryptKey]:
-        keys: list = self._load_msg_keys(identifier=identifier)
+    def private_keys_for_decryption(self, user: ID) -> List[DecryptKey]:
+        keys: list = self._load_msg_keys(identifier=user)
         # the 'ID key' could be used for encrypting message too (RSA),
         # so we append it to the decrypt keys here
-        id_key = self._load_id_key(identifier=identifier)
-        if isinstance(id_key, DecryptKey) and find_key(key=id_key, private_keys=keys) < 0:
+        id_key = self._load_id_key(identifier=user)
+        if isinstance(id_key, DecryptKey) and PrivateKeyDBI.find(item=id_key, array=keys) < 0:
             keys.append(id_key)
         return keys
 
     # Override
-    def private_key_for_signature(self, identifier: ID) -> Optional[SignKey]:
+    def private_key_for_signature(self, user: ID) -> Optional[SignKey]:
         # TODO: support multi private keys
-        return self.private_key_for_visa_signature(identifier=identifier)
+        return self.private_key_for_visa_signature(user=user)
 
     # Override
-    def private_key_for_visa_signature(self, identifier: ID) -> Optional[SignKey]:
-        return self._load_id_key(identifier=identifier)
-
-
-#   insert_key(key: PrivateKey, private_keys: List[PrivateKey]) -> Optional[List[PrivateKey]]:
-def insert_key(key: PrivateKey, private_keys: list) -> Optional[List[PrivateKey]]:
-    index = find_key(key=key, private_keys=private_keys)
-    if index == 0:
-        return None  # nothing changed
-    elif index > 0:
-        private_keys.pop(index)  # move to the front
-    elif len(private_keys) > 2:
-        private_keys.pop()  # keep only last three records
-    private_keys.insert(0, key)
-    return private_keys
-
-
-def find_key(key, private_keys: List[PrivateKey]) -> int:
-    index = 0
-    data = key.get('data')
-    for item in private_keys:
-        if item.get('data') == data:
-            return index
-        else:
-            index += 1
-    return -1
+    def private_key_for_visa_signature(self, user: ID) -> Optional[SignKey]:
+        return self._load_id_key(identifier=user)
```

### Comparing `dimples-0.1.4/dimples/database/message.py` & `dimples-0.1.5/dimples/database/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/database/t_document.py` & `dimples-0.1.5/dimples/database/t_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         doc_type = document.type
         # 0. check old record with time
         old = self.document(identifier=identifier, doc_type=doc_type)
         if old is not None and 0 < document.time < old.time:
             # document expired, drop it
             return False
         # 1. store into memory cache
-        self.__doc_cache.update(key=identifier, value=document, life_span=3600)
+        self.__doc_cache.update(key=identifier, value=document, life_span=600)
         # 2. store into local storage
         return self.__doc_storage.save_document(document=document)
 
     # Override
     def document(self, identifier: ID, doc_type: str = '*') -> Optional[Document]:
         """ get document for ID """
         now = time.time()
@@ -81,10 +81,10 @@
                     # document not exists
                     return None
                 # document expired, wait to reload
                 holder.renewal(duration=128, now=now)
             # 2. check local storage
             value = self.__doc_storage.document(identifier=identifier, doc_type=doc_type)
             # 3. update memory cache
-            self.__doc_cache.update(key=identifier, value=value, life_span=3600, now=now)
+            self.__doc_cache.update(key=identifier, value=value, life_span=600, now=now)
         # OK, return cached value
         return value
```

### Comparing `dimples-0.1.4/dimples/database/t_group.py` & `dimples-0.1.5/dimples/database/t_group.py`

 * *Files 21% similar despite different names*

```diff
@@ -50,115 +50,142 @@
         self.__group_storage.show_info()
 
     #
     #   Group DBI
     #
 
     # Override
-    def founder(self, identifier: ID) -> Optional[ID]:
+    def founder(self, group: ID) -> Optional[ID]:
         """ get founder of group """
         now = time.time()
         # 1. check memory cache
-        value, holder = self.__founder_cache.fetch(key=identifier, now=now)
+        value, holder = self.__founder_cache.fetch(key=group, now=now)
         if value is None:
             # cache empty
             if holder is None:
                 # founder not load yet, wait to load
-                self.__founder_cache.update(key=identifier, life_span=128, now=now)
+                self.__founder_cache.update(key=group, life_span=128, now=now)
             else:
                 if holder.is_alive(now=now):
                     # founder not exists
                     return None
                 # founder expired, wait to reload
                 holder.renewal(duration=128, now=now)
             # 2. check local storage
-            value = self.__group_storage.founder(identifier=identifier)
+            value = self.__group_storage.founder(group=group)
             # 3. update memory cache
-            self.__founder_cache.update(key=identifier, value=value, life_span=3600, now=now)
+            if value is None:
+                self.__founder_cache.update(key=group, value=value, life_span=600, now=now)
+            else:
+                self.__founder_cache.update(key=group, value=value, life_span=36000, now=now)
         # OK, return cached value
         return value
 
     # Override
-    def owner(self, identifier: ID) -> Optional[ID]:
+    def owner(self, group: ID) -> Optional[ID]:
         """ get owner of group """
         now = time.time()
         # 1. check memory cache
-        value, holder = self.__owner_cache.fetch(key=identifier, now=now)
+        value, holder = self.__owner_cache.fetch(key=group, now=now)
         if value is None:
             # cache empty
             if holder is None:
                 # owner not load yet, wait to load
-                self.__owner_cache.update(key=identifier, life_span=128, now=now)
+                self.__owner_cache.update(key=group, life_span=128, now=now)
             else:
                 if holder.is_alive(now=now):
                     # owner not exists
                     return None
                 # owner expired, wait to reload
                 holder.renewal(duration=128, now=now)
             # 2. check local storage
-            value = self.__group_storage.owner(identifier=identifier)
+            value = self.__group_storage.owner(group=group)
             # 3. update memory cache
-            self.__owner_cache.update(key=identifier, value=value, life_span=3600, now=now)
+            self.__owner_cache.update(key=group, value=value, life_span=600, now=now)
         # OK, return cached value
         return value
 
     # Override
-    def members(self, identifier: ID) -> List[ID]:
+    def members(self, group: ID) -> List[ID]:
         """ get members of group """
         now = time.time()
         # 1. check memory cache
-        value, holder = self.__members_cache.fetch(key=identifier, now=now)
+        value, holder = self.__members_cache.fetch(key=group, now=now)
         if value is None:
             # cache empty
             if holder is None:
                 # members not load yet, wait to load
-                self.__members_cache.update(key=identifier, life_span=128, now=now)
+                self.__members_cache.update(key=group, life_span=128, now=now)
             else:
                 if holder.is_alive(now=now):
                     # members not exists
                     return []
                 # members expired, wait to reload
                 holder.renewal(duration=128, now=now)
             # 2. check local storage
-            value = self.__group_storage.members(identifier=identifier)
+            value = self.__group_storage.members(group=group)
             # 3. update memory cache
-            self.__members_cache.update(key=identifier, value=value, life_span=3600, now=now)
+            self.__members_cache.update(key=group, value=value, life_span=600, now=now)
         # OK, return cached value
         return value
 
     # Override
-    def assistants(self, identifier: ID) -> List[ID]:
+    def save_members(self, members: List[ID], group: ID) -> bool:
+        # 1. store into memory cache
+        self.__members_cache.update(key=group, value=members, life_span=600)
+        # 2. store into local storage
+        return self.__group_storage.save_members(members=members, group=group)
+
+    # Override
+    def add_member(self, member: ID, group: ID) -> bool:
+        array = self.members(group=group)
+        if member in array:
+            # self.warning(msg='member exists: %s, group: %s' % (member, group))
+            return True
+        array.append(member)
+        return self.save_members(members=array, group=group)
+
+    # Override
+    def remove_member(self, member: ID, group: ID) -> bool:
+        array = self.members(group=group)
+        if member not in array:
+            # self.warning(msg='member not exists: %s, group: %s' % (member, group))
+            return True
+        array.remove(member)
+        return self.save_members(members=array, group=group)
+
+    # Override
+    def remove_group(self, group: ID) -> bool:
+        # TODO: remove group
+        # self.warning(msg='TODO: remove group: %s' % group)
+        return False
+
+    # Override
+    def assistants(self, group: ID) -> List[ID]:
         """ get assistants of group """
         now = time.time()
         # 1. check memory cache
-        value, holder = self.__assistants_cache.fetch(key=identifier, now=now)
+        value, holder = self.__assistants_cache.fetch(key=group, now=now)
         if value is None:
             # cache empty
             if holder is None:
                 # assistants not load yet, wait to load
-                self.__assistants_cache.update(key=identifier, life_span=128, now=now)
+                self.__assistants_cache.update(key=group, life_span=128, now=now)
             else:
                 if holder.is_alive(now=now):
                     # assistants not exists
                     return []
                 # assistants expired, wait to reload
                 holder.renewal(duration=128, now=now)
             # 2. check local storage
-            value = self.__group_storage.assistants(identifier=identifier)
+            value = self.__group_storage.assistants(group=group)
             # 3. update memory cache
-            self.__assistants_cache.update(key=identifier, value=value, life_span=3600, now=now)
+            self.__assistants_cache.update(key=group, value=value, life_span=600, now=now)
         # OK, return cached value
         return value
 
     # Override
-    def save_members(self, members: List[ID], identifier: ID) -> bool:
-        # 1. store into memory cache
-        self.__members_cache.update(key=identifier, value=members, life_span=3600)
-        # 2. store into local storage
-        return self.__group_storage.save_members(members=members, identifier=identifier)
-
-    # Override
-    def save_assistants(self, assistants: List[ID], identifier: ID) -> bool:
+    def save_assistants(self, assistants: List[ID], group: ID) -> bool:
         # 1. store into memory cache
-        self.__assistants_cache.update(key=identifier, value=assistants, life_span=3600)
+        self.__assistants_cache.update(key=group, value=assistants, life_span=600)
         # 2. store into local storage
-        return self.__group_storage.save_assistants(assistants=assistants, identifier=identifier)
+        return self.__group_storage.save_assistants(assistants=assistants, group=group)
```

### Comparing `dimples-0.1.4/dimples/database/t_login.py` & `dimples-0.1.5/dimples/database/t_login.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,42 +44,42 @@
         self.__login_cache = man.get_pool(name='login')  # ID => (LoginCommand, ReliableMessage)
         self.__login_storage = LoginStorage(root=root, public=public, private=private)
 
     def show_info(self):
         self.__login_storage.show_info()
 
     # Override
-    def login_command_message(self, identifier: ID) -> Tuple[Optional[LoginCommand], Optional[ReliableMessage]]:
+    def login_command_message(self, user: ID) -> Tuple[Optional[LoginCommand], Optional[ReliableMessage]]:
         """ get login command message for user """
         now = time.time()
         # 1. check memory cache
-        value, holder = self.__login_cache.fetch(key=identifier, now=now)
+        value, holder = self.__login_cache.fetch(key=user, now=now)
         if value is None:
             # cache empty
             if holder is None:
                 # login command not load yet, wait to load
-                self.__login_cache.update(key=identifier, life_span=128, now=now)
+                self.__login_cache.update(key=user, life_span=128, now=now)
             else:
                 if holder.is_alive(now=now):
                     # login command not exists
                     return None, None
                 # login command expired, wait to reload
                 holder.renewal(duration=128, now=now)
             # 2. check local storage
-            cmd, msg = self.__login_storage.login_command_message(identifier=identifier)
+            cmd, msg = self.__login_storage.login_command_message(user=user)
             value = (cmd, msg)
             # 3. update memory cache
-            self.__login_cache.update(key=identifier, value=value, life_span=36000, now=now)
+            self.__login_cache.update(key=user, value=value, life_span=600, now=now)
         # OK, return cached value
         return value
 
     # Override
-    def save_login_command_message(self, identifier: ID, content: LoginCommand, msg: ReliableMessage) -> bool:
+    def save_login_command_message(self, user: ID, content: LoginCommand, msg: ReliableMessage) -> bool:
         # 1. check old record
-        old, _ = self.login_command_message(identifier=identifier)
+        old, _ = self.login_command_message(user=user)
         if isinstance(old, LoginCommand) and old.time >= content.time > 0:
             # command expired
             return False
         # 2. store into memory cache
-        self.__login_cache.update(key=identifier, value=(content, msg), life_span=36000)
+        self.__login_cache.update(key=user, value=(content, msg), life_span=600)
         # 3. store into local storage
-        return self.__login_storage.save_login_command_message(identifier=identifier, content=content, msg=msg)
+        return self.__login_storage.save_login_command_message(user=user, content=content, msg=msg)
```

### Comparing `dimples-0.1.4/dimples/database/t_message.py` & `dimples-0.1.5/dimples/database/t_message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/database/t_meta.py` & `dimples-0.1.5/dimples/database/t_meta.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,10 +78,13 @@
                     # meta not exists
                     return None
                 # meta expired, wait to reload
                 holder.renewal(duration=128, now=now)
             # 2. check local storage
             value = self.__meta_storage.meta(identifier=identifier)
             # 3. update memory cache
-            self.__meta_cache.update(key=identifier, value=value, life_span=36000, now=now)
+            if value is None:
+                self.__meta_cache.update(key=identifier, value=value, life_span=600, now=now)
+            else:
+                self.__meta_cache.update(key=identifier, value=value, life_span=36000, now=now)
         # OK, return cached value
         return value
```

### Comparing `dimples-0.1.4/dimples/database/t_private.py` & `dimples-0.1.5/dimples/database/t_private.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from dimsdk import PrivateKey, DecryptKey, SignKey
 from dimsdk import ID
 
 from ..utils import CacheManager
 from ..common import PrivateKeyDBI
 
 from .dos import PrivateKeyStorage
-from .dos.private import insert_key
 
 
 class PrivateKeyTable(PrivateKeyDBI):
     """ Implementations of PrivateKeyDBI """
 
     def __init__(self, root: str = None, public: str = None, private: str = None):
         super().__init__()
@@ -50,77 +49,84 @@
         self.__key_storage.show_info()
 
     #
     #   PrivateKey DBI
     #
 
     # Override
-    def save_private_key(self, key: PrivateKey, identifier: ID, key_type: str = 'M') -> bool:
+    def save_private_key(self, key: PrivateKey, user: ID, key_type: str = 'M') -> bool:
         now = time.time()
         # 1. update memory cache
         if key_type == PrivateKeyStorage.ID_KEY_TAG:
             # update 'id_key'
-            self.__id_key_cache.update(key=identifier, value=key, life_span=36000, now=now)
+            self.__id_key_cache.update(key=user, value=key, life_span=36000, now=now)
         else:
             # add to old keys
-            private_keys = self.private_keys_for_decryption(identifier=identifier)
-            private_keys = insert_key(key=key, private_keys=private_keys)
+            private_keys = self.private_keys_for_decryption(user=user)
+            private_keys = PrivateKeyDBI.convert_private_keys(keys=private_keys)
+            private_keys = PrivateKeyDBI.insert(item=key, array=private_keys)
             if private_keys is None:
                 # key already exists, nothing changed
                 return False
             # update 'msg_keys'
-            self.__msg_keys_cache.update(key=identifier, value=private_keys, life_span=36000, now=now)
+            self.__msg_keys_cache.update(key=user, value=private_keys, life_span=36000, now=now)
         # 2. update local storage
-        return self.__key_storage.save_private_key(key=key, identifier=identifier, key_type=key_type)
+        return self.__key_storage.save_private_key(key=key, user=user, key_type=key_type)
 
     # Override
-    def private_keys_for_decryption(self, identifier: ID) -> List[DecryptKey]:
+    def private_keys_for_decryption(self, user: ID) -> List[DecryptKey]:
         """ get sign key for ID """
         now = time.time()
         # 1. check memory cache
-        value, holder = self.__msg_keys_cache.fetch(key=identifier, now=now)
+        value, holder = self.__msg_keys_cache.fetch(key=user, now=now)
         if value is None:
             # cache empty
             if holder is None:
                 # msg keys not load yet, wait to load
-                self.__msg_keys_cache.update(key=identifier, life_span=128, now=now)
+                self.__msg_keys_cache.update(key=user, life_span=128, now=now)
             else:
                 if holder.is_alive(now=now):
                     # msg keys not exists
                     return []
                 # msg keys expired, wait to reload
                 holder.renewal(duration=128, now=now)
             # 2. check local storage
-            value = self.__key_storage.private_keys_for_decryption(identifier=identifier)
+            value = self.__key_storage.private_keys_for_decryption(user=user)
             # 3. update memory cache
-            self.__msg_keys_cache.update(key=identifier, value=value, life_span=36000, now=now)
+            if value is None:
+                self.__msg_keys_cache.update(key=user, value=value, life_span=600, now=now)
+            else:
+                self.__msg_keys_cache.update(key=user, value=value, life_span=36000, now=now)
         # OK, return cached value
         return value
 
     # Override
-    def private_key_for_signature(self, identifier: ID) -> Optional[SignKey]:
+    def private_key_for_signature(self, user: ID) -> Optional[SignKey]:
         # TODO: support multi private keys
-        return self.private_key_for_visa_signature(identifier=identifier)
+        return self.private_key_for_visa_signature(user=user)
 
     # Override
-    def private_key_for_visa_signature(self, identifier: ID) -> Optional[SignKey]:
+    def private_key_for_visa_signature(self, user: ID) -> Optional[SignKey]:
         """ get sign key for ID """
         now = time.time()
         # 1. check memory cache
-        value, holder = self.__id_key_cache.fetch(key=identifier, now=now)
+        value, holder = self.__id_key_cache.fetch(key=user, now=now)
         if value is None:
             # cache empty
             if holder is None:
                 # id key not load yet, wait to load
-                self.__id_key_cache.update(key=identifier, life_span=128, now=now)
+                self.__id_key_cache.update(key=user, life_span=128, now=now)
             else:
                 if holder.is_alive(now=now):
                     # id key not exists
                     return None
                 # id key expired, wait to reload
                 holder.renewal(duration=128, now=now)
             # 2. check local storage
-            value = self.__key_storage.private_key_for_visa_signature(identifier=identifier)
+            value = self.__key_storage.private_key_for_visa_signature(user=user)
             # 3. update memory cache
-            self.__id_key_cache.update(key=identifier, value=value, life_span=36000, now=now)
+            if value is None:
+                self.__id_key_cache.update(key=user, value=value, life_span=600, now=now)
+            else:
+                self.__id_key_cache.update(key=user, value=value, life_span=36000, now=now)
         # OK, return cached value
         return value
```

### Comparing `dimples-0.1.4/dimples/edge/__init__.py` & `dimples-0.1.5/dimples/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/edge/octopus.py` & `dimples-0.1.5/dimples/server/dispatcher.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # ==============================================================================
 # MIT License
 #
-# Copyright (c) 2019 Albert Moky
+# Copyright (c) 2022 Albert Moky
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -20,315 +20,349 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 """
-    Octopus
-    ~~~~~~~
+    Message Dispatcher
+    ~~~~~~~~~~~~~~~~~~
 
-    Edges for neighbor stations
+    A dispatcher to decide which way to deliver message.
 """
 
 import threading
-import time
-import weakref
 from abc import ABC, abstractmethod
-from typing import Optional, List, Set
+from typing import Optional, List
 
-from dimsdk import ContentType
 from dimsdk import EntityType, ID
+from dimsdk import Content
 from dimsdk import ReliableMessage
 
-from ..utils import Logging
-from ..utils import Runner
+from ..utils import Singleton, Logging, Runner
 from ..common import CommonFacebook
 from ..common import MessageDBI, SessionDBI
-from ..common import HandshakeCommand
-from ..conn.session import get_sig
+from ..common import LoginCommand, ReceiptCommand
 
-from ..client import ClientSession
-from ..client import ClientMessenger
-from ..client import ClientMessagePacker
-from ..client import ClientMessageProcessor
-from ..client import Terminal
+from .session_center import SessionCenter
+from .pusher import Pusher
 
-from .shared import GlobalVariable
-from .shared import create_session
 
+class MessageDeliver(ABC):
+    """ Delegate for deliver message """
+
+    @abstractmethod
+    def deliver_message(self, msg: ReliableMessage, receiver: ID) -> List[Content]:
+        """
+        Deliver message to destination
+
+        :param msg:      message delivering
+        :param receiver: message destination
+        :return: responses
+        """
+        raise NotImplemented
 
-class Octopus(Runner, Logging):
 
-    def __init__(self, shared: GlobalVariable, local_host: str = '127.0.0.1', local_port: int = 9394):
+@Singleton
+class Dispatcher(MessageDeliver):
+
+    def __init__(self):
         super().__init__()
-        self.__shared = shared
-        self.__inner = self.create_inner_terminal(host=local_host, port=local_port)
-        self.__outers: Set[Terminal] = set()
-        self.__outer_map = weakref.WeakValueDictionary()
-        self.__outer_lock = threading.Lock()
+        self.__facebook: Optional[CommonFacebook] = None
+        self.__mdb: Optional[MessageDBI] = None
+        self.__sdb: Optional[SessionDBI] = None
+        self.__pusher: Optional[Pusher] = None
+        # actually deliver worker
+        self.__worker: Optional[DeliverWorker] = None
+        # roaming user receptionist
+        self.__roamer: Optional[Roamer] = None
 
     @property
-    def shared(self) -> GlobalVariable:
-        return self.__shared
+    def facebook(self) -> CommonFacebook:
+        return self.__facebook
+
+    @facebook.setter
+    def facebook(self, barrack: CommonFacebook):
+        self.__facebook = barrack
+
+    #
+    #   Database
+    #
 
     @property
-    def database(self) -> SessionDBI:
-        return self.__shared.sdb
+    def mdb(self) -> MessageDBI:
+        return self.__mdb
+
+    @mdb.setter
+    def mdb(self, db: MessageDBI):
+        self.__mdb = db
 
     @property
-    def inner_messenger(self) -> ClientMessenger:
-        terminal = self.__inner
-        return terminal.messenger
-
-    def get_outer_messenger(self, identifier: ID) -> Optional[ClientMessenger]:
-        with self.__outer_lock:
-            terminal = self.__outer_map.get(identifier)
-        if terminal is not None:
-            return terminal.messenger
-
-    def create_inner_terminal(self, host: str, port: int) -> Terminal:
-        shared = self.shared
-        session = create_session(facebook=shared.facebook, database=shared.sdb, host=host, port=port)
-        messenger = create_messenger(facebook=shared.facebook, database=shared.mdb,
-                                     session=session, messenger_class=InnerMessenger)
-        messenger.octopus = self
-        return create_terminal(messenger=messenger)
-
-    def create_outer_terminal(self, host: str, port: int) -> Terminal:
-        shared = self.shared
-        session = create_session(facebook=shared.facebook, database=shared.sdb, host=host, port=port)
-        messenger = create_messenger(facebook=shared.facebook, database=shared.mdb,
-                                     session=session, messenger_class=OuterMessenger)
-        messenger.octopus = self
-        return create_terminal(messenger=messenger)
-
-    def add_index(self, identifier: ID, terminal: Terminal):
-        with self.__outer_lock:
-            # self.__outers.add(terminal)
-            self.__outer_map[identifier] = terminal
-
-    def connect(self, host: str, port: int = 9394):
-        terminal = self.create_outer_terminal(host=host, port=port)
-        with self.__outer_lock:
-            self.__outers.add(terminal)
+    def sdb(self) -> SessionDBI:
+        return self.__sdb
 
-    def start(self):
-        thread = threading.Thread(target=self.run)
-        thread.start()
+    @sdb.setter
+    def sdb(self, db: SessionDBI):
+        self.__sdb = db
+
+    #
+    #   Push Notification service
+    #
 
-    # Override
-    def stop(self):
-        super().stop()
-        inner = self.__inner
-        if inner is not None:
-            inner.stop()
-        with self.__outer_lock:
-            outers = set(self.__outers)
-        for out in outers:
-            out.stop()
+    @property
+    def pusher(self) -> Pusher:
+        return self.__pusher
 
-    # Override
-    def _idle(self):
-        time.sleep(60)
+    @pusher.setter
+    def pusher(self, service: Pusher):
+        self.__pusher = service
+
+    def start(self):
+        worker = DeliverWorker(database=self.__sdb, facebook=self.__facebook)
+        roamer = Roamer(database=self.__mdb)
+        self.__worker = worker
+        self.__roamer = roamer
+        roamer.start()
+
+    #
+    #   Roamer
+    #
+
+    def add_roaming(self, user: ID, station: ID) -> bool:
+        """ Add roaming user with station """
+        roamer = self.__roamer
+        if roamer is not None:
+            return roamer.add_roaming(user=user, station=station)
+
+    #
+    #   Deliver
+    #
 
     # Override
-    def process(self) -> bool:
-        # get all neighbor stations
-        db = self.database
-        neighbors = db.all_neighbors()
-        # get all outer terminals
-        with self.__outer_lock:
-            outers = set(self.__outers)
-        for out in outers:
-            # check station
-            station = out.session.station
-            host = station.host
-            port = station.port
-            for item in neighbors:
-                if item[0] == host and item[1] == port:
-                    # got
-                    neighbors.discard(item)
-                    break
-            if out.is_alive:
-                # outer terminal alive, ignore it
-                continue
-            # remove dead terminal
-            sid = station.identifier
-            with self.__outer_lock:
-                self.__outers.discard(out)
-                if sid is not None:
-                    self.__outer_map.pop(sid, None)
-        # check new neighbors
-        for item in neighbors:
-            host = item[0]
-            port = item[1]
-            sid = item[2]
-            self.info(msg='connecting neighbor station "%s" (%s:%d)' % (sid, host, port))
-            self.connect(host=host, port=port)
-        return False
-
-    def income_message(self, msg: ReliableMessage, priority: int = 0) -> List[ReliableMessage]:
-        """ redirect message from remote station """
-        messenger = self.inner_messenger
-        if messenger.send_reliable_message(msg=msg, priority=priority):
-            sig = get_sig(msg=msg)
-            self.info(msg='redirected msg (%s) for receiver (%s)' % (sig, msg.receiver))
-            # no need to respond receipt for station
-            return []
-        sig = get_sig(msg=msg)
-        self.error(msg='failed to redirect msg (%s) for receiver (%s)' % (sig, msg.receiver))
-        return []
+    def deliver_message(self, msg: ReliableMessage, receiver: ID) -> List[Content]:
+        """ Deliver message to destination """
+        worker = self.__worker
+        if receiver.type == EntityType.STATION:
+            # message to other stations
+            # station won't roam to other station, so just push for it directly
+            responses = worker.redirect_message(msg=msg, neighbor=receiver)
+        elif receiver.type == EntityType.BOT:
+            # message to a bot
+            # save message before trying to push
+            self.__save_reliable_message(msg=msg, receiver=receiver)
+            responses = worker.push_message(msg=msg, receiver=receiver)
+        else:
+            # message to user
+            # save message before trying to push
+            self.__save_reliable_message(msg=msg, receiver=receiver)
+            responses = worker.push_message(msg=msg, receiver=receiver)
+            if responses is None:
+                # failed to push message, user not online and not roamed to other station,
+                # push notification for the receiver
+                pusher = self.__pusher
+                if pusher is None:
+                    self.warning(msg='pusher not set yet, drop notification for: %s' % receiver)
+                else:
+                    pusher.push_notification(msg=msg)
+        # OK
+        return [] if responses is None else responses
+
+    def __save_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
+        if receiver.type == EntityType.STATION or msg.sender.type == EntityType.STATION:
+            # no need to save station message
+            return False
+        db = self.__mdb
+        return db.cache_reliable_message(msg=msg, receiver=receiver)
 
-    def outgo_message(self, msg: ReliableMessage, priority: int = 0) -> List[ReliableMessage]:
-        """ redirect message to remote station """
-        target = ID.parse(identifier=msg.get('neighbor'))
-        if target is None:
-            # target station not found
-            self.info(msg='cannot get target station for receiver (%s)' % msg.receiver)
-            return []
-        messenger = self.get_outer_messenger(identifier=target)
-        if messenger is None:
-            # target station not my neighbor
-            self.info(msg='receiver (%s) is targeted to (%s), but not my neighbor' % (msg.receiver, target))
-            return []
-        msg.pop('neighbor', None)
-        if messenger.send_reliable_message(msg=msg, priority=priority):
-            sig = get_sig(msg=msg)
-            self.info(msg='redirected msg (%s) to target (%s) for receiver (%s)' % (sig, target, msg.receiver))
-            # no need to respond receipt for station
-            return []
-        sig = get_sig(msg=msg)
-        self.error(msg='failed to redirect msg (%s) to target (%s) for receiver (%s)' % (sig, target, msg.receiver))
-        return []
 
+class RoamingInfo:
 
-class OctopusMessenger(ClientMessenger, ABC):
-    """ Messenger for processing message from remote station """
+    def __init__(self, user: ID, station: ID):
+        super().__init__()
+        self.user = user
+        self.station = station
+        self.start_pos = 0
 
-    def __init__(self, session: ClientSession, facebook: CommonFacebook, database: MessageDBI):
-        super().__init__(session=session, facebook=facebook, database=database)
-        self.__terminal: Optional[weakref.ReferenceType] = None
-        self.__octopus: Optional[weakref.ReferenceType] = None
 
-    @property
-    def terminal(self) -> Terminal:
-        return self.__terminal()
+class Roamer(Runner, Logging):
+    """ Delegate for redirect cached messages to roamed station """
 
-    @terminal.setter
-    def terminal(self, client: Terminal):
-        self.__terminal = weakref.ref(client)
+    def __init__(self, database: MessageDBI):
+        super().__init__()
+        self.__database = database
+        # roaming (user id => station id)
+        self.__queue: List[RoamingInfo] = []
+        self.__lock = threading.Lock()
 
     @property
-    def octopus(self):
-        bot = self.__octopus()
-        assert isinstance(bot, Octopus), 'octopus error: %s' % bot
-        return bot
-
-    @octopus.setter
-    def octopus(self, bot):
-        self.__octopus = weakref.ref(bot)
+    def database(self) -> Optional[MessageDBI]:
+        return self.__database
 
-    @property
-    def local_station(self) -> ID:
-        facebook = self.facebook
-        current = facebook.current_user
-        return current.identifier
-
-    def __is_handshaking(self, msg: ReliableMessage) -> bool:
-        """ check HandshakeCommand sent to this station """
-        receiver = msg.receiver
-        if receiver.type != EntityType.STATION or receiver != self.local_station:
-            # not for this station
-            return False
-        if msg.type != ContentType.COMMAND:
-            # not a command
-            return False
-        i_msg = self.decrypt_message(msg=msg)
-        if i_msg is not None:
-            return isinstance(i_msg.content, HandshakeCommand)
+    def __append(self, info: RoamingInfo):
+        with self.__lock:
+            self.__queue.append(info)
+
+    def __next(self) -> Optional[RoamingInfo]:
+        with self.__lock:
+            if len(self.__queue) > 0:
+                return self.__queue.pop(0)
+
+    def add_roaming(self, user: ID, station: ID) -> bool:
+        """
+        Add roaming user with station
+
+        :param user:    roaming user
+        :param station: station roamed to
+        :return: False on error
+        """
+        info = RoamingInfo(user=user, station=station)
+        self.__append(info=info)
+        return True
 
     # Override
-    def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
-        # check for HandshakeCommand
-        if self.__is_handshaking(msg=msg):
-            self.info(msg='receive handshaking: %s' % msg.sender)
-            return super().process_reliable_message(msg=msg)
-        # check for cycled message
-        if msg.receiver == msg.sender:
-            self.error(msg='drop cycled msg(type=%d): %s -> %s | from %s, traces: %s'
-                       % (msg.type, msg.sender, msg.receiver, get_remote_station(messenger=self), msg.get('traces')))
-            return []
-        # handshake accepted, redirecting message
-        self.info(msg='redirect msg(type=%d): %s -> %s | from %s, traces: %s'
-                  % (msg.type, msg.sender, msg.receiver, get_remote_station(messenger=self), msg.get('traces')))
-        return self.deliver_message(msg=msg)
-
-    @abstractmethod
-    def deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
-        """ call octopus to redirect message """
-        pass
-
+    def process(self) -> bool:
+        info = self.__next()
+        if info is None:
+            # nothing to do
+            return False
+        receiver = info.user
+        roaming = info.station
+        start = info.start_pos
+        limit = 1024
+        try:
+            db = self.database
+            cached_messages, remaining = db.reliable_messages(receiver=receiver, start=start, limit=limit)
+            if remaining > 0:
+                # there are remaining messages, push the roaming user back for next try
+                info.start_pos = start + limit
+                self.__append(info=info)
+            elif cached_messages is None or len(cached_messages) == 0:
+                self.debug(msg='no cached message for this user: %s' % receiver)
+                return True
+            # get deliver delegate for receiver
+            dispatcher = Dispatcher()
+            # deliver cached messages one by one
+            for msg in cached_messages:
+                dispatcher.deliver_message(msg=msg, receiver=receiver)
+        except Exception as e:
+            self.error(msg='process roaming user (%s => %s) error: %s' % (receiver, roaming, e))
+        # return True to process next immediately
+        return True
 
-def get_remote_station(messenger: ClientMessenger) -> ID:
-    session = messenger.session
-    station = session.station
-    return station.identifier
+    def start(self):
+        thread = threading.Thread(target=self.run, daemon=True)
+        thread.start()
 
 
-class InnerMessenger(OctopusMessenger):
-    """ Messenger for local station """
+class DeliverWorker(Logging):
+    """ Actual deliver worker """
 
-    # Override
-    def deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
-        priority = 0  # NORMAL
-        if msg.receiver.is_broadcast:
-            priority = 1  # SLOWER
-        octopus = self.octopus
-        return octopus.outgo_message(msg=msg, priority=priority)
+    def __init__(self, database: SessionDBI, facebook: CommonFacebook):
+        super().__init__()
+        self.__database = database
+        self.__facebook = facebook
 
+    @property
+    def database(self) -> Optional[SessionDBI]:
+        return self.__database
 
-class OuterMessenger(OctopusMessenger):
-    """ Messenger for remote station """
+    @property
+    def facebook(self) -> Optional[CommonFacebook]:
+        return self.__facebook
 
-    # Override
-    def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
-        if msg.sender == self.local_station:
-            self.debug(msg='cycled message from this station: %s => %s' % (msg.sender, msg.receiver))
-            return []
-        return super().process_reliable_message(msg=msg)
+    def push_message(self, msg: ReliableMessage, receiver: ID) -> Optional[List[Content]]:
+        """
+        Push message for receiver
+
+        :param msg:      network message
+        :param receiver: actual receiver
+        :return: responses
+        """
+        assert receiver.is_user, 'receiver ID error: %s' % receiver
+        assert receiver.type != EntityType.STATION, 'should not push message for station: %s' % receiver
+        # 1. try to push message directly
+        if session_push(msg=msg, receiver=receiver) > 0:
+            text = 'Message pushed'
+            cmd = ReceiptCommand.create(text=text, msg=msg)
+            return [cmd]
+        # 2. get roaming station
+        roaming = get_roaming_station(receiver=receiver, database=self.database)
+        if roaming is None:
+            # login command not found
+            # return None to tell the pusher to push notification for it.
+            return None
+        # 3. redirect message to roaming station
+        return self.redirect_message(msg=msg, neighbor=roaming)
+
+    def redirect_message(self, msg: ReliableMessage, neighbor: ID) -> Optional[List[Content]]:
+        """
+        Redirect message to neighbor station
+
+        :param msg:      network message
+        :param neighbor: neighbor station
+        :return: responses
+        """
+        """ Redirect message to neighbor station """
+        assert neighbor.type == EntityType.STATION, 'neighbor station ID error: %s' % neighbor
+        self.info(msg='redirect message %s => %s to neighbor station: %s' % (msg.sender, msg.receiver, neighbor))
+        # 0. check current station
+        current = self.facebook.current_user.identifier
+        assert current.type == EntityType.STATION, 'current station ID error: %s' % current
+        if neighbor == current:
+            self.debug(msg='same destination: %s, msg %s => %s' % (neighbor, msg.sender, msg.receiver))
+            # the user is roaming to current station, but it's not online now
+            # return None to tell the pusher to push notification for it.
+            return None
+        # 1. try to push message to neighbor station directly
+        if session_push(msg=msg, receiver=neighbor) > 0:
+            text = 'Message redirected to neighbor station'
+            cmd = ReceiptCommand.create(text=text, msg=msg)
+            cmd['neighbor'] = str(neighbor)
+            return [cmd]
+        # 2. push message to bridge
+        return bridge_message(msg=msg, neighbor=neighbor, bridge=current)
+
+
+def bridge_message(msg: ReliableMessage, neighbor: ID, bridge: ID) -> Optional[List[Content]]:
+    """
+    Redirect message to neighbor station via the station bridge
+
+    :param msg:      network message
+    :param neighbor: roaming station
+    :param bridge:   current station
+    :return: responses
+    """
+    # NOTE: the messenger will serialize this message immediately, so
+    #       we don't need to clone this dictionary to avoid 'neighbor'
+    #       be changed to another value before pushing to the bridge.
+    # clone = msg.copy_dictionary()
+    # msg = ReliableMessage.parse(msg=clone)
+    msg['neighbor'] = str(neighbor)
+    if session_push(msg=msg, receiver=bridge) > 0:
+        text = 'Message pushing to neighbor station via the bridge'
+        cmd = ReceiptCommand.create(text=text, msg=msg)
+        cmd['neighbor'] = str(neighbor)
+        return [cmd]
+    else:
+        # station bridge not found
+        # return an empty array to avoid calling pusher
+        return []
 
-    # Override
-    def deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
-        priority = 0  # NORMAL
-        if msg.receiver.is_broadcast:
-            priority = 1  # SLOWER
-        octopus = self.octopus
-        return octopus.income_message(msg=msg, priority=priority)
 
-    # Override
-    def handshake_success(self):
-        super().handshake_success()
-        station = self.session.station
-        octopus = self.octopus
-        octopus.add_index(identifier=station.identifier, terminal=self.terminal)
-
-
-def create_messenger(facebook: CommonFacebook, database: MessageDBI,
-                     session: ClientSession, messenger_class) -> OctopusMessenger:
-    assert issubclass(messenger_class, OctopusMessenger), 'messenger class error: %s' % messenger_class
-    # 1. create messenger with session and MessageDB
-    messenger = messenger_class(session=session, facebook=facebook, database=database)
-    # 2. create packer, processor for messenger
-    #    they have weak references to facebook & messenger
-    messenger.packer = ClientMessagePacker(facebook=facebook, messenger=messenger)
-    messenger.processor = ClientMessageProcessor(facebook=facebook, messenger=messenger)
-    # 3. set weak reference to messenger
-    session.messenger = messenger
-    return messenger
-
-
-def create_terminal(messenger: OctopusMessenger) -> Terminal:
-    terminal = Terminal(messenger=messenger)
-    messenger.terminal = terminal
-    terminal.start()
-    return terminal
+def session_push(msg: ReliableMessage, receiver: ID) -> int:
+    """ push message via active session(s) of receiver """
+    success = 0
+    center = SessionCenter()
+    active_sessions = center.active_sessions(identifier=receiver)
+    for session in active_sessions:
+        if session.send_reliable_message(msg=msg):
+            success += 1
+    return success
+
+
+def get_roaming_station(receiver: ID, database: SessionDBI) -> Optional[ID]:
+    """ get login command for roaming station """
+    cmd, msg = database.login_command_message(user=receiver)
+    if isinstance(cmd, LoginCommand):
+        station = cmd.station
+        assert isinstance(station, dict), 'login command error: %s' % cmd
+        return ID.parse(identifier=station.get('ID'))
```

### Comparing `dimples-0.1.4/dimples/edge/shared.py` & `dimples-0.1.5/dimples/edge/shared.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from typing import Optional, Tuple
 
 from dimsdk import ID, Station
 
 from ..utils import Singleton
 from ..common import CommonFacebook
 from ..common import AccountDBI, MessageDBI, SessionDBI
+from ..common import ProviderInfo
 from ..database import AccountDatabase, MessageDatabase, SessionDatabase
 from ..database import Storage
 from ..client import ClientSession
 
 from ..config import Config
 
 
@@ -107,19 +108,21 @@
     # create database
     adb = AccountDatabase(root=root, public=public, private=private)
     mdb = MessageDatabase(root=root, public=public, private=private)
     sdb = SessionDatabase(root=root, public=public, private=private)
     adb.show_info()
     mdb.show_info()
     sdb.show_info()
+    # default provider
+    provider = ProviderInfo.GSP
     # add neighbors
     neighbors = config.neighbors
     for node in neighbors:
-        print('adding neighbor node: (%s:%d), ID=%s' % (node.host, node.port, node.identifier))
-        sdb.add_neighbor(host=node.host, port=node.port)
+        print('adding neighbor node: %s' % node)
+        sdb.add_station(identifier=None, host=node.host, port=node.port, provider=provider)
     return adb, mdb, sdb
 
 
 def create_facebook(database: AccountDBI, current_user: ID) -> CommonFacebook:
     """ Step 3: create facebook """
     facebook = CommonFacebook(database=database)
     # make sure private keys exists
```

### Comparing `dimples-0.1.4/dimples/edge/start.py` & `dimples-0.1.5/dimples/edge/start.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from dimples.edge.shared import GlobalVariable
 from dimples.edge.octopus import Octopus
 
 
 #
 # show logs
 #
-Log.LEVEL = Log.DEVELOP
+Log.LEVEL = Log.DEBUG
 
 
 DEFAULT_CONFIG = '/etc/dim/edge.ini'
 
 
 def main():
     # create global variable
```

### Comparing `dimples-0.1.4/dimples/register/__init__.py` & `dimples-0.1.5/dimples/register/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/register/generate.py` & `dimples-0.1.5/dimples/register/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 from typing import List
 
 from mkm.crypto import PrivateKey, SignKey
-from mkm.protocol import entity_is_group, meta_has_seed
 from mkm import EntityType, ID
 from mkm import MetaType, Meta
 from mkm import Document, Visa, Bulletin
 
 from dimplugins.network import NetworkType, network_to_type
 
 from ..common import AccountDBI
@@ -66,18 +65,18 @@
             print('!!! private key: %s, msg keys: %s' % (private_key.algorithm, array))
 
     def save(self, db: AccountDBI) -> bool:
         identifier = self.identifier
         # save keys
         private_key = self.private_key
         if private_key is not None:
-            db.save_private_key(key=private_key, identifier=identifier, key_type=PrivateKeyStorage.ID_KEY_TAG)
+            db.save_private_key(key=private_key, user=identifier, key_type=PrivateKeyStorage.ID_KEY_TAG)
         msg_keys = self.msg_keys
         for key in msg_keys:
-            db.save_private_key(key=key, identifier=identifier, key_type=PrivateKeyStorage.MSG_KEY_TAG)
+            db.save_private_key(key=key, user=identifier, key_type=PrivateKeyStorage.MSG_KEY_TAG)
         # save meta & document
         db.save_meta(meta=self.meta, identifier=identifier)
         return db.save_document(document=self.document)
 
 
 id_types = [
     (EntityType.USER,       'User'),
@@ -203,17 +202,17 @@
     #
     # Step 3: get meta seed (ID.name)
     #
     if network in [EntityType.STATION, NetworkType.STATION]:
         default_seed = 'station'
     elif network in [EntityType.BOT, NetworkType.BOT]:
         default_seed = 'bot'
-    elif entity_is_group(network=network_to_type(network=network)):
+    elif EntityType.is_group(network=network_to_type(network=network)):
         default_seed = 'group'
-    elif meta_has_seed(version=version):
+    elif MetaType.has_seed(version=version):
         default_seed = 'user'
     else:
         # BTC/ETH address as ID without seed
         default_seed = None
     if default_seed is None:
         seed = None
     else:
@@ -223,19 +222,19 @@
             seed = default_seed
         print('!!! meta seed: %s' % seed)
     #
     # Step 4: generate account info
     #
     if network in [EntityType.STATION, NetworkType.STATION]:
         info = gen_station(network=network, seed=seed)
-    elif entity_is_group(network=network_to_type(network=network)):
+    elif EntityType.is_group(network=network_to_type(network=network)):
         fid = input('>>> please input founder ID: ')
         founder = ID.parse(identifier=fid)
         assert founder is not None and founder.is_user, 'group founder error: %s' % fid
-        sign_key = db.private_key_for_visa_signature(identifier=founder)
+        sign_key = db.private_key_for_visa_signature(user=founder)
         assert sign_key is not None, 'founder private key not found: %s' % founder
         info = gen_group(network=network, seed=seed, founder=founder, sign_key=sign_key)
     else:
         info = gen_user(network=network, version=version, seed=seed)
     #
     # Step 5: save account info
     #
```

### Comparing `dimples-0.1.4/dimples/register/modify.py` & `dimples-0.1.5/dimples/register/modify.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 from typing import List
 
 from mkm.crypto import PrivateKey, SignKey, DecryptKey
-from mkm.protocol import entity_is_group
 from mkm import EntityType, ID
 from mkm import Document, Visa
 
 from ..common import AccountDBI
 from ..database import PrivateKeyStorage
 
 
@@ -57,15 +56,15 @@
 
     def save(self, db: AccountDBI) -> bool:
         doc = self.document
         identifier = doc.identifier
         # save keys
         msg_keys = self.msg_keys
         for key in msg_keys:
-            db.save_private_key(key=key, identifier=identifier, key_type=PrivateKeyStorage.MSG_KEY_TAG)
+            db.save_private_key(key=key, user=identifier, key_type=PrivateKeyStorage.MSG_KEY_TAG)
         # save document
         return db.save_document(document=self.document)
 
 
 def show_document(document: Document):
     name = document.name
     identifier = document.identifier
@@ -144,42 +143,42 @@
     # Step 1: check meta & private keys
     #
     meta = db.meta(identifier=identifier)
     if meta is None:
         print('!!! meta not exists: %s' % identifier)
         return False
     network = identifier.type
-    if entity_is_group(network=network):
+    if EntityType.is_group(network=network):
         # TODO: get group founder(owner) and its id key
         print('!!! TODO: modify bulletin document for group: %s' % identifier)
         return False
-    id_key = db.private_key_for_visa_signature(identifier=identifier)
+    id_key = db.private_key_for_visa_signature(user=identifier)
     if id_key is None:
         print('!!! private key not exists: %s' % identifier)
         return False
-    msg_keys = db.private_keys_for_decryption(identifier=identifier)
+    msg_keys = db.private_keys_for_decryption(user=identifier)
     print('!!! old msg keys found: %d, id key: %s' % (len(msg_keys), id_key.algorithm))
     #
     # Step 2: create document
     #
     doc = db.document(identifier=identifier)
     if doc is not None:
         print('!!! old document found: %s' % identifier)
         show_document(document=doc)
         doc = Document.parse(document=doc.copy_dictionary())
-    elif entity_is_group(network=network):
+    elif EntityType.is_group(network=network):
         doc = Document.create(doc_type=Document.BULLETIN, identifier=identifier)
     else:
         doc = Document.create(doc_type=Document.VISA, identifier=identifier)
     #
     # Step 3: modify document
     #
     if network == EntityType.STATION:
         info = modify_station(document=doc, sign_key=id_key, msg_keys=msg_keys)
-    elif entity_is_group(network=network):
+    elif EntityType.is_group(network=network):
         info = modify_group(document=doc, sign_key=id_key)
     else:
         info = modify_user(document=doc, sign_key=id_key, msg_keys=msg_keys)
     #
     # Step 3: save account info
     #
     info.show_info()
```

### Comparing `dimples-0.1.4/dimples/register/run.py` & `dimples-0.1.5/dimples/register/run.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/register/shared.py` & `dimples-0.1.5/dimples/register/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/server/__init__.py` & `dimples-0.1.5/dimples/server/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,24 +34,22 @@
 from .session import ServerSession
 from .session_center import SessionCenter  # SessionPool
 
 from .push_info import PushAlert, PushInfo
 from .push_service import PushService, PushCenter
 from .pusher import Pusher, DefaultPusher
 
-from .dispatcher import Roamer, Deliver, Worker
+# from .dispatcher import Roamer, MessageDeliver, DeliverWorker
 from .dispatcher import Dispatcher
-from .deliver import UserDeliver, BotDeliver, StationDeliver
-from .delivers import GroupDeliver, BroadcastDeliver
-from .delivering import DeliverWorker, DefaultRoamer
-from .filter import Filter, DefaultFilter
 
-from .messenger import ServerMessenger
+from .packer import BlockFilter, MuteFilter, FilterManager
+
 from .packer import ServerMessagePacker
 from .processor import ServerMessageProcessor, ServerContentProcessorCreator
+from .messenger import ServerMessenger
 
 
 __all__ = [
 
     #
     #   CPU
     #
@@ -61,20 +59,18 @@
     # Session
     'ServerSession', 'SessionCenter',  # 'SessionPool',
 
     # Push Notification
     'PushAlert', 'PushInfo', 'PushService', 'PushCenter',
     'Pusher', 'DefaultPusher',
 
-    # Deliver
-    'Roamer', 'Deliver', 'Worker',
+    # Dispatcher
+    # 'Roamer', 'MessageDeliver', 'DeliverWorker',
     'Dispatcher',
-    'UserDeliver', 'BotDeliver', 'StationDeliver',
-    'GroupDeliver', 'BroadcastDeliver',
-    'DeliverWorker', 'DefaultRoamer',
-    'Filter', 'DefaultFilter',
 
-    'ServerMessenger',
+    # Filter
+    'BlockFilter', 'MuteFilter', 'FilterManager',
+
     'ServerMessagePacker',
-    'ServerMessageProcessor',
-    'ServerContentProcessorCreator',
+    'ServerMessageProcessor', 'ServerContentProcessorCreator',
+    'ServerMessenger',
 ]
```

### Comparing `dimples-0.1.4/dimples/server/cpu/__init__.py` & `dimples-0.1.5/dimples/server/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/server/cpu/ans.py` & `dimples-0.1.5/dimples/server/cpu/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/server/cpu/document.py` & `dimples-0.1.5/dimples/server/cpu/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     if sender == node:
         # the station is querying itself, ignore it
         return None
     elif sender.type == EntityType.BOT:
         # no need to respond LoginCommand message to a bot,
         # just ignore it
         return None
-    cmd, msg = database.login_command_message(identifier=doc_id)
+    cmd, msg = database.login_command_message(user=doc_id)
     if cmd is not None:
         if sender.type == EntityType.STATION:
             # this is a request from another station.
             # if the user is not roaming to this station, just ignore it,
             # let the target station to respond.
             roaming = cmd.station
             assert isinstance(roaming, dict), 'login command error: %s' % cmd
```

### Comparing `dimples-0.1.4/dimples/server/cpu/handshake.py` & `dimples-0.1.5/dimples/server/cpu/handshake.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
 from dimp import ID
 from dimp import ReliableMessage
 from dimp import Content
 
 from dimsdk.cpu import BaseCommandProcessor
 
+from ...utils import Log
 from ...common import HandshakeCommand
 from ...common import CommonMessenger, Session
 
 
 class HandshakeCommandProcessor(BaseCommandProcessor):
 
     @property
@@ -60,14 +61,15 @@
             return self._respond_text(text=text)
         # C -> S: Hello world!
         assert 'Hello world!' == title, 'Handshake command error: %s' % content
         # set/update session in session server with new session key
         session = self.session
         if session.key == content.session:
             # session key match
+            Log.info(msg='handshake accepted: %s, session: %s' % (msg.sender, session.key))
             # verified success
             handshake_accepted(identifier=msg.sender, session=session)
             res = HandshakeCommand.success(session=session.key)
         else:
             # session key not match
             # ask client to sign it with the new session key
             res = HandshakeCommand.again(session=session.key)
```

### Comparing `dimples-0.1.4/dimples/server/cpu/login.py` & `dimples-0.1.5/dimples/server/cpu/login.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, LoginCommand), 'command error: %s' % content
         sender = content.identifier
         # 1. store login command
         session = self.messenger.session
         db = session.database
-        if not db.save_login_command_message(identifier=sender, content=content, msg=msg):
+        if not db.save_login_command_message(user=sender, content=content, msg=msg):
             self.error(msg='login command error/expired: %s' % content)
             return []
         # 2. check roaming station
         current = self.facebook.current_user
         station = content.station
         roaming = ID.parse(identifier=station.get('ID'))
         assert isinstance(roaming, ID), 'login command error: %s' % content
```

### Comparing `dimples-0.1.4/dimples/server/cpu/receipt.py` & `dimples-0.1.5/dimples/server/cpu/receipt.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/server/cpu/report.py` & `dimples-0.1.5/dimples/server/cpu/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/server/deliver.py` & `dimples-0.1.5/dimples/server/packer.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,180 +20,188 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 """
-    Message Deliver
-    ~~~~~~~~~~~~~~~
-
-    A deliver to decide which way to redirect message.
+    Common extensions for MessagePacker
+    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 
-import threading
-from abc import ABC, abstractmethod
-from typing import Optional, List, Tuple
+from typing import Optional, Dict
 
 from dimsdk import EntityType, ID
-from dimsdk import Content
-from dimsdk import ReliableMessage
-
-from ..utils import Logging
-from ..utils import Runner
-from ..common import MessageDBI
-
-from .pusher import Pusher
-from .dispatcher import Deliver
-from .dispatcher import Dispatcher
-
-
-class DeliverTask:
-
-    def __init__(self, msg: ReliableMessage, receiver: ID):
-        super().__init__()
-        self.msg = msg
-        self.receiver = receiver
-
-
-class DeliverQueue:
-
-    def __init__(self):
-        super().__init__()
-        # locked queue
-        self.__tasks: List[DeliverTask] = []
-        self.__lock = threading.Lock()
-
-    def append(self, task: DeliverTask):
-        with self.__lock:
-            self.__tasks.append(task)
-
-    def next(self) -> Optional[DeliverTask]:
-        with self.__lock:
-            if len(self.__tasks) > 0:
-                return self.__tasks.pop(0)
-
-
-class BaseDeliver(Runner, Deliver, Logging, ABC):
-
-    def __init__(self):
-        super().__init__()
-        self.__queue = DeliverQueue()  # locked queue
+from dimsdk import SecureMessage, ReliableMessage
 
-    def __append(self, msg: ReliableMessage, receiver: ID):
-        task = DeliverTask(msg=msg, receiver=receiver)
-        self.__queue.append(task=task)
-
-    def __next(self) -> Tuple[Optional[ReliableMessage], Optional[ID]]:
-        task = self.__queue.next()
-        if task is None:
-            return None, None
+from ..utils import Singleton, Logging
+from ..common import CommonFacebook
+from ..common import CommonMessagePacker
+
+
+class ServerMessagePacker(CommonMessagePacker):
+
+    def __current(self) -> ID:
+        """ current station ID """
+        facebook = get_facebook(packer=self)
+        current = facebook.current_user
+        sid = current.identifier
+        assert sid is not None, 'current station error: %s' % current
+        return sid
+
+    def __is_traced(self, msg: ReliableMessage) -> bool:
+        is_traced = False
+        node = self.__current()
+        # check current node in msg['traces']
+        traces = msg.get('traces')
+        if traces is None:
+            # start from here
+            msg['traces'] = [str(node)]
         else:
-            return task.msg, task.receiver
+            for item in traces:
+                if isinstance(item, Dict):
+                    sid = item.get('ID')
+                else:
+                    # assert isinstance(item, str), 'MTA error: %s' % item
+                    sid = item
+                if node == sid:
+                    is_traced = True
+                    break
+            # append current node to msg['traces']
+            traces.append(str(node))
+        return is_traced
+
+    def __is_trusted(self, sender: ID) -> bool:
+        messenger = get_messenger(packer=self)
+        session = messenger.session
+        user = session.identifier
+        if user is None:
+            # current user not login yet
+            return False
+        # handshake accepted, check current user with sender
+        if user == sender:
+            # no need to verify signature of this message
+            # which sender is equal to current id in session
+            return True
+        if user.type == EntityType.STATION:
+            # if it's a roaming message delivered from another neighbor station,
+            # shall we trust that neighbor totally and skip verifying too ???
+            # TODO: trusted station list
+            return True
 
     # Override
-    def deliver_message(self, msg: ReliableMessage, receiver: ID) -> List[Content]:
-        assert receiver.is_user and not receiver.is_broadcast, 'receiver error: %s' % receiver
-        self.__append(msg=msg, receiver=receiver)
-        return []
+    def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
+        sender = msg.sender
+        receiver = msg.receiver
+        # check duplicated
+        if self.__is_traced(msg=msg):
+            # cycled message
+            if sender.type == EntityType.STATION or receiver.type == EntityType.STATION:
+                # ignore cycled station message
+                return None
+            elif receiver.is_broadcast:
+                # ignore cycled broadcast message
+                return None
+            self.warning(msg='cycled message: %s -> %s' % (sender, receiver))
+        if not self.__check_reliable_message_receiver(msg=msg):
+            # receiver (group) not ready
+            self.warning(msg='receiver not ready: %s' % msg.receiver)
+            return None
+        # check session
+        if self.__is_trusted(sender=msg.sender):
+            # no need to verify message from this sender
+            self.debug(msg='trusted sender: %s' % msg.sender)
+            return msg
+        # verify after sender is OK
+        return super().verify_message(msg=msg)
 
     # Override
-    def process(self) -> bool:
-        msg, receiver = self.__next()
-        if msg is None:  # or recipients is None:
-            # nothing to do
-            return False
-        try:
-            responses = self._dispatch(msg=msg, receiver=receiver)
-            self._respond(responses=responses, msg=msg)
-        except Exception as e:
-            self.error(msg='process delivering (%s => %s) error: %s' % (msg.sender, receiver, e))
-        # return True to process next immediately
+    def _check_reliable_message_receiver(self, msg: ReliableMessage) -> bool:
+        # skip for "super().verify_message(msg=msg)"
         return True
 
-    def _respond(self, responses: Optional[List[Content]], msg: ReliableMessage):
-        # TODO: send responses to msg.receiver
-        pass
+    def __check_reliable_message_receiver(self, msg: ReliableMessage) -> bool:
+        node = self.__current()
+        receiver = msg.receiver
+        if receiver.is_broadcast:
+            if receiver.is_group:
+                # broadcast to neighbor stations
+                messenger = get_messenger(packer=self)
+                messenger.broadcast_reliable_message(msg=msg, station=node)
+            # elif receiver == 'archivist@anywhere':
+            #     # forward to search bot
+            #     pass
+            else:
+                # broadcast message to single destination
+                # if receiver == 'station@anywhere',
+                #     it must be the first handshake without station ID;
+                # if receiver == 'anyone@anywhere',
+                #     it should be other plain message without encryption.
+                pass
+            # OK
+            return True
+        # elif receiver.is_group:
+        #     sender = msg.sender
+        #     self.error(msg='Should not send group message to a station!! %s -> %s' % (sender, receiver))
+        #     return False
+        return super()._check_reliable_message_receiver(msg=msg)
+
+
+def get_facebook(packer: CommonMessagePacker) -> CommonFacebook:
+    barrack = packer.facebook
+    assert isinstance(barrack, CommonFacebook), 'facebook error: %s' % barrack
+    return barrack
+
+
+def get_messenger(packer: CommonMessagePacker):
+    transceiver = packer.messenger
+    from .messenger import ServerMessenger
+    assert isinstance(transceiver, ServerMessenger), 'messenger error: %s' % transceiver
+    return transceiver
 
-    @abstractmethod
-    def _dispatch(self, msg: ReliableMessage, receiver: ID) -> Optional[List[Content]]:
-        """ deliver message by dispatcher """
-        raise NotImplemented
-
-    def start(self):
-        thread = threading.Thread(target=self.run, daemon=True)
-        thread.start()
 
+"""
+    Filter
+    ~~~~~~
 
-class StationDeliver(BaseDeliver):
+    Filters for delivering message
+"""
 
-    # Override
-    def _dispatch(self, msg: ReliableMessage, receiver: ID) -> Optional[List[Content]]:
-        assert receiver.type == EntityType.STATION, 'station ID error: %s' % receiver
-        dispatcher = Dispatcher()
-        worker = dispatcher.deliver_worker
-        return worker.redirect_message(msg=msg, neighbor=receiver)
 
+class BlockFilter(Logging):
 
-class BotDeliver(BaseDeliver):
+    def is_blocked(self, msg: ReliableMessage) -> bool:
+        sender = msg.sender
+        receiver = msg.receiver
+        group = msg.group
+        self.debug(msg='checking block-list for: %s -> %s (group: %s)' % (sender, receiver, group))
+        # TODO: check block-list
+        return False
 
-    def __init__(self, database: MessageDBI):
-        super().__init__()
-        self.__database = database
 
-    @property
-    def database(self) -> MessageDBI:
-        return self.__database
+class MuteFilter(Logging):
+    """ Filter for Push Notification service """
 
-    # Override
-    def _dispatch(self, msg: ReliableMessage, receiver: ID) -> Optional[List[Content]]:
-        assert receiver.type == EntityType.BOT, 'bot ID error: %s' % receiver
-        # 1. save message for group assistant
-        save_reliable_message(msg=msg, receiver=receiver, database=self.database)
-        # 2. push message
-        dispatcher = Dispatcher()
-        worker = dispatcher.deliver_worker
-        return worker.push_message(msg=msg, receiver=receiver)
+    def is_muted(self, msg: ReliableMessage) -> bool:
+        sender = msg.sender
+        receiver = msg.receiver
+        group = msg.group
+        self.debug(msg='checking mute-list for: %s -> %s (group: %s)' % (sender, receiver, group))
+        if sender.type == EntityType.STATION or receiver.type == EntityType.STATION:
+            # mute all messages for stations
+            return True
+        elif sender.type == EntityType.BOT:
+            # mute group message from bot
+            return group is not None or receiver.is_group
+        elif receiver.type == EntityType.BOT:
+            # mute all messages to bots
+            return True
+        # TODO: check mute-list
 
 
-class UserDeliver(BaseDeliver):
+@Singleton
+class FilterManager:
 
-    def __init__(self, database: MessageDBI, pusher: Pusher = None):
+    def __init__(self):
         super().__init__()
-        self.__database = database
-        self.__pusher = pusher
-
-    @property
-    def database(self) -> MessageDBI:
-        return self.__database
-
-    @property
-    def pusher(self) -> Optional[Pusher]:
-        return self.__pusher
-
-    # Override
-    def _dispatch(self, msg: ReliableMessage, receiver: ID) -> Optional[List[Content]]:
-        assert receiver.is_user, 'user ID error: %s' % receiver
-        assert receiver.type != EntityType.STATION, 'user ID error: %s' % receiver
-        assert receiver.type != EntityType.BOT, 'user ID error: %s' % receiver
-        # 1. save message for receiver
-        save_reliable_message(msg=msg, receiver=receiver, database=self.database)
-        # 2. push message
-        dispatcher = Dispatcher()
-        worker = dispatcher.deliver_worker
-        responses = worker.push_message(msg=msg, receiver=receiver)
-        if responses is not None:
-            # pushed to active session, or redirect to neighbor station
-            return responses
-        # 3. push notification
-        pusher = self.pusher
-        if pusher is None:
-            self.warning(msg='pusher not set yet, drop notification for: %s' % receiver)
-        else:
-            pusher.push_notification(msg=msg)
-
-
-def save_reliable_message(msg: ReliableMessage, receiver: ID, database: MessageDBI) -> bool:
-    if receiver.type == EntityType.STATION or msg.sender.type == EntityType.STATION:
-        # no need to save station message
-        return False
-    return database.cache_reliable_message(msg=msg, receiver=receiver)
+        self.block_filter = BlockFilter()
+        self.mute_filter = MuteFilter()
```

### Comparing `dimples-0.1.4/dimples/server/processor.py` & `dimples-0.1.5/dimples/server/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/server/push_info.py` & `dimples-0.1.5/dimples/server/push_info.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/server/push_service.py` & `dimples-0.1.5/dimples/server/push_service.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/server/pusher.py` & `dimples-0.1.5/dimples/server/pusher.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from dimsdk import ID
 from dimsdk import ContentType
 from dimsdk import Envelope, ReliableMessage
 
 from ..utils import Logging
 from ..common import CommonFacebook
 
+from .packer import FilterManager
 from .push_service import PushCenter
 
 
 class Pusher(ABC):
     """ Notification Pusher for Message """
 
     @abstractmethod
@@ -67,21 +68,22 @@
         # 1. check original sender, group & msg type
         env = self._origin_envelope(msg=msg)
         receiver = msg.receiver
         sender = env.sender
         group = env.group
         msg_type = env.type
         # 2. check mute-list
-        if self._is_mute(sender=sender, receiver=receiver, group=group, msg_type=msg_type):
-            # muted by receiver
+        mute_filter = FilterManager().mute_filter
+        if mute_filter.is_muted(msg=msg):
+            self.info(msg='muted sender: %s -> %s (group: %s) type: %d' % (sender, receiver, group, msg_type))
             return
         # 3. build title & content text
         title, text = self._build_message(sender=sender, receiver=receiver, group=group, msg_type=msg_type)
         if text is None:
-            # ignore msg type
+            self.info(msg='ignore msg type: %s -> %s (group: %s) type: %d' % (sender, receiver, group, msg_type))
             return
         # 4. add notification to a waiting queue in PushCenter
         center = PushCenter()
         center.add_notification(sender=sender, receiver=receiver, title=title, content=text)
 
     # noinspection PyMethodMayBeStatic
     def _origin_envelope(self, msg: ReliableMessage) -> Envelope:
```

### Comparing `dimples-0.1.4/dimples/server/session.py` & `dimples-0.1.5/dimples/server/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/server/session_center.py` & `dimples-0.1.5/dimples/server/session_center.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/station/__init__.py` & `dimples-0.1.5/dimples/station/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/station/handler.py` & `dimples-0.1.5/dimples/station/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,28 +37,26 @@
 from ..common import MessageDBI
 from ..common import CommonFacebook
 
 from ..server import ServerSession, SessionCenter
 from ..server import ServerMessenger
 from ..server import ServerMessagePacker
 from ..server import ServerMessageProcessor
-from ..server import DefaultFilter
 
 from .shared import GlobalVariable
 
 
 def create_messenger(facebook: CommonFacebook, database: MessageDBI,
                      session: ServerSession) -> ServerMessenger:
     # 1. create messenger with session and MessageDB
     messenger = ServerMessenger(session=session, facebook=facebook, database=database)
     # 2. create packer, processor, filter for messenger
     #    they have weak references to session, facebook & messenger
     messenger.packer = ServerMessagePacker(facebook=facebook, messenger=messenger)
     messenger.processor = ServerMessageProcessor(facebook=facebook, messenger=messenger)
-    messenger.filter = DefaultFilter(session=session, facebook=facebook)
     # 3. set weak reference messenger in session
     session.messenger = messenger
     return messenger
 
 
 class RequestHandler(StreamRequestHandler, Logging):
```

### Comparing `dimples-0.1.4/dimples/station/shared.py` & `dimples-0.1.5/dimples/station/shared.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,21 +28,19 @@
 from typing import Optional, Tuple
 
 from dimsdk import Address, ID, IDFactory
 
 from ..utils import Singleton
 from ..common import AddressNameServer, CommonFacebook
 from ..common import AccountDBI, MessageDBI, SessionDBI
+from ..common import ProviderInfo
 from ..database import AccountDatabase, MessageDatabase, SessionDatabase
 from ..database import Storage
 from ..server import Pusher, DefaultPusher, PushCenter
 from ..server import Dispatcher
-from ..server import UserDeliver, BotDeliver, StationDeliver
-from ..server import GroupDeliver, BroadcastDeliver
-from ..server import DeliverWorker, DefaultRoamer
 
 from ..config import Config
 
 
 class ANSFactory(IDFactory):
 
     def __init__(self, factory: IDFactory, ans: AddressNameServer):
@@ -136,19 +134,21 @@
     # create database
     adb = AccountDatabase(root=root, public=public, private=private)
     mdb = MessageDatabase(root=root, public=public, private=private)
     sdb = SessionDatabase(root=root, public=public, private=private)
     adb.show_info()
     mdb.show_info()
     sdb.show_info()
+    # default provider
+    provider = ProviderInfo.GSP
     # add neighbors
     neighbors = config.neighbors
     for node in neighbors:
-        print('adding neighbor node: (%s:%d), ID="%s"' % (node.host, node.port, node.identifier))
-        sdb.add_neighbor(host=node.host, port=node.port, identifier=node.identifier)
+        print('adding neighbor node: %s' % node)
+        sdb.add_station(identifier=None, host=node.host, port=node.port, provider=provider)
     return adb, mdb, sdb
 
 
 def create_facebook(database: AccountDBI, current_user: ID) -> CommonFacebook:
     """ Step 3: create facebook """
     facebook = CommonFacebook(database=database)
     # make sure private keys exists
@@ -183,32 +183,13 @@
     center.start()
     return pusher
 
 
 def create_dispatcher(shared: GlobalVariable) -> Dispatcher:
     """ Step 6: create dispatcher """
     dispatcher = Dispatcher()
-    dispatcher.database = shared.mdb
+    dispatcher.mdb = shared.mdb
+    dispatcher.sdb = shared.sdb
     dispatcher.facebook = shared.facebook
-    # set base deliver delegates
-    user_deliver = UserDeliver(database=shared.mdb, pusher=shared.pusher)
-    bot_deliver = BotDeliver(database=shared.mdb)
-    station_deliver = StationDeliver()
-    dispatcher.set_user_deliver(deliver=user_deliver)
-    dispatcher.set_bot_deliver(deliver=bot_deliver)
-    dispatcher.set_station_deliver(deliver=station_deliver)
-    # set special deliver delegates
-    group_deliver = GroupDeliver(facebook=shared.facebook)
-    broadcast_deliver = BroadcastDeliver(database=shared.sdb)
-    dispatcher.set_group_deliver(deliver=group_deliver)
-    dispatcher.set_broadcast_deliver(deliver=broadcast_deliver)
-    # set roamer & worker
-    roamer = DefaultRoamer(database=shared.mdb)
-    worker = DeliverWorker(database=shared.sdb, facebook=shared.facebook)
-    dispatcher.set_roamer(roamer=roamer)
-    dispatcher.set_deliver_worker(worker=worker)
-    # start all delegates
-    user_deliver.start()
-    bot_deliver.start()
-    station_deliver.start()
-    roamer.start()
+    dispatcher.pusher = shared.pusher
+    dispatcher.start()
     return dispatcher
```

### Comparing `dimples-0.1.4/dimples/station/start.py` & `dimples-0.1.5/dimples/station/start.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 from dimples.station.shared import create_dispatcher
 from dimples.station.handler import RequestHandler
 
 
 #
 # show logs
 #
-Log.LEVEL = Log.DEVELOP
+Log.LEVEL = Log.DEBUG
 
 
 DEFAULT_CONFIG = '/etc/dim/station.ini'
 
 
 def main():
     # create global variable
```

### Comparing `dimples-0.1.4/dimples/utils/__init__.py` & `dimples-0.1.5/dimples/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/utils/cache.py` & `dimples-0.1.5/dimples/utils/cache.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/utils/checker.py` & `dimples-0.1.5/dimples/utils/checker.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,23 +44,30 @@
 
 class FrequencyChecker(Generic[K]):
     """ Frequency checker for duplicated queries """
 
     def __init__(self, expires: float = 3600):
         super().__init__()
         self.__expires = expires
-        self.__map: Dict[K, float] = {}
+        self.__records: Dict[K, float] = {}
 
-    def expired(self, key: K, expires: float = None) -> bool:
-        if expires is None:
-            expires = self.__expires
-        now = time.time()
-        if now > self.__map.get(key, 0):
-            self.__map[key] = now + expires
-            return True
+    def expired(self, key: K, now: float = None, force: bool = False) -> bool:
+        if now is None:
+            now = time.time()
+        if force:
+            # ignore last updated time, force to update now
+            pass
+        else:
+            # check last update time
+            expired = self.__records.get(key)
+            if expired is not None and expired > now:
+                # record exists and not expired yet
+                return False
+        self.__records[key] = now + self.__expires
+        return True
 
 
 @Singleton
 class QueryFrequencyChecker:
     """ Synchronizer for Facebook """
 
     # each query will be expired after 10 minutes
@@ -73,19 +80,25 @@
         self.__meta_lock = threading.Lock()
         # query for document
         self.__document_queries: FrequencyChecker[ID] = FrequencyChecker(expires=self.QUERY_EXPIRES)
         self.__document_lock = threading.Lock()
         # query for group members
         self.__members_queries: FrequencyChecker[ID] = FrequencyChecker(expires=self.QUERY_EXPIRES)
         self.__members_lock = threading.Lock()
+        # response for document
+        self.__document_responses: FrequencyChecker[ID] = FrequencyChecker(expires=self.QUERY_EXPIRES)
 
-    def meta_query_expired(self, identifier: ID) -> bool:
+    def meta_query_expired(self, identifier: ID, now: float = None) -> bool:
         with self.__meta_lock:
-            return self.__meta_queries.expired(key=identifier)
+            return self.__meta_queries.expired(key=identifier, now=now)
 
-    def document_query_expired(self, identifier: ID) -> bool:
+    def document_query_expired(self, identifier: ID, now: float = None) -> bool:
         with self.__document_lock:
-            return self.__document_queries.expired(key=identifier)
+            return self.__document_queries.expired(key=identifier, now=now)
 
-    def members_query_expired(self, identifier: ID) -> bool:
+    def members_query_expired(self, identifier: ID, now: float = None) -> bool:
         with self.__members_lock:
-            return self.__members_queries.expired(key=identifier)
+            return self.__members_queries.expired(key=identifier, now=now)
+
+    def document_response_expired(self, identifier: ID, now: float = None, force: bool = False) -> bool:
+        with self.__document_lock:
+            return self.__document_responses.expired(key=identifier, now=now, force=force)
```

### Comparing `dimples-0.1.4/dimples/utils/dos.py` & `dimples-0.1.5/dimples/utils/dos.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/utils/log.py` & `dimples-0.1.5/dimples/utils/log.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples/utils/singleton.py` & `dimples-0.1.5/dimples/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.4/dimples.egg-info/PKG-INFO` & `dimples-0.1.5/dimples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.1.4
+Version: 0.1.5
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.1.4/dimples.egg-info/SOURCES.txt` & `dimples-0.1.5/dimples.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 dimples.egg-info/PKG-INFO
 dimples.egg-info/SOURCES.txt
 dimples.egg-info/dependency_links.txt
 dimples.egg-info/entry_points.txt
 dimples.egg-info/requires.txt
 dimples.egg-info/top_level.txt
 dimples/client/__init__.py
+dimples/client/group.py
 dimples/client/messenger.py
 dimples/client/packer.py
 dimples/client/processor.py
 dimples/client/terminal.py
 dimples/client/cpu/__init__.py
 dimples/client/cpu/grp_expel.py
 dimples/client/cpu/grp_invite.py
@@ -27,16 +28,16 @@
 dimples/client/network/session.py
 dimples/client/network/state.py
 dimples/client/network/transition.py
 dimples/common/__init__.py
 dimples/common/ans.py
 dimples/common/facebook.py
 dimples/common/messenger.py
+dimples/common/packer.py
 dimples/common/session.py
-dimples/common/transmitter.py
 dimples/common/dbi/__init__.py
 dimples/common/dbi/account.py
 dimples/common/dbi/message.py
 dimples/common/dbi/session.py
 dimples/common/protocol/__init__.py
 dimples/common/protocol/ans.py
 dimples/common/protocol/handshake.py
@@ -62,39 +63,36 @@
 dimples/database/t_cipherkey.py
 dimples/database/t_document.py
 dimples/database/t_group.py
 dimples/database/t_login.py
 dimples/database/t_message.py
 dimples/database/t_meta.py
 dimples/database/t_private.py
-dimples/database/t_provider.py
+dimples/database/t_station.py
 dimples/database/t_user.py
 dimples/database/dos/__init__.py
 dimples/database/dos/base.py
 dimples/database/dos/document.py
 dimples/database/dos/group.py
 dimples/database/dos/login.py
 dimples/database/dos/meta.py
 dimples/database/dos/private.py
+dimples/database/dos/station.py
 dimples/database/dos/user.py
 dimples/edge/__init__.py
 dimples/edge/octopus.py
 dimples/edge/shared.py
 dimples/edge/start.py
 dimples/register/__init__.py
 dimples/register/generate.py
 dimples/register/modify.py
 dimples/register/run.py
 dimples/register/shared.py
 dimples/server/__init__.py
-dimples/server/deliver.py
-dimples/server/delivering.py
-dimples/server/delivers.py
 dimples/server/dispatcher.py
-dimples/server/filter.py
 dimples/server/messenger.py
 dimples/server/packer.py
 dimples/server/processor.py
 dimples/server/push_info.py
 dimples/server/push_service.py
 dimples/server/pusher.py
 dimples/server/session.py
```

### Comparing `dimples-0.1.4/setup.py` & `dimples-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
@@ -47,19 +47,19 @@
             'dime=dimples.edge.start:main'
         ]
     },
     install_requires=[
         # 'pycryptodome',  # 3.14.1
         # 'base58',  # 1.0.3
         # 'ecdsa',   # 0.16.1
-        'dimplugins>=0.1.3',
+        'dimplugins>=0.1.4',
 
-        'dimsdk>=0.8.4',
-        'dimp>=0.12.6',
-        'dkd>=0.12.6',
-        'mkm>=0.12.6',
+        'dimsdk>=0.8.5',
+        'dimp>=0.12.8',
+        'dkd>=0.12.7',
+        'mkm>=0.12.7',
 
         'startrek>=0.4.1',
         'tcp>=0.4.1',
         'udp>=0.5.10',
     ]
 )
```

