# Comparing `tmp/oncall-2.0.0.tar.gz` & `tmp/oncall-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oncall-2.0.0.tar", last modified: Wed Jun  7 18:25:41 2023, max compression
+gzip compressed data, was "oncall-2.0.1.tar", last modified: Wed Jun  7 18:29:31 2023, max compression
```

## Comparing `oncall-2.0.0.tar` & `oncall-2.0.1.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.644373 oncall-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-07 18:25:31.000000 oncall-2.0.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-07 18:25:31.000000 oncall-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-07 18:25:31.000000 oncall-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-07 18:25:31.000000 oncall-2.0.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-07 18:25:41.644373 oncall-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-07 18:25:31.000000 oncall-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:25:41.644373 oncall-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-07 18:25:31.000000 oncall-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.624373 oncall-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.624373 oncall-2.0.0/src/oncall/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.628373 oncall-2.0.0/src/oncall/api/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.636373 oncall-2.0.0/src/oncall/api/v0/
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/bonus_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/event_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/event_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/event_swap.py
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/events_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/ical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/ical_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/ical_key_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/ical_key_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/ical_key_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/ical_key_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/iris_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/modes.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/notification_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/populate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/public_ical.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/roster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/roster_suggest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/roster_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/roster_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/rosters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    17229 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/service_oncall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/service_teams.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2853 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    10456 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/team_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/team_admins.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/team_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/team_ical.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/team_iris_escalate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/team_oncall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/team_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/team_services.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/team_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/team_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/team_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/team_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/team_users.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8493 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/timezones.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/upcoming_shifts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/user_ical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/user_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/user_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/user_pinned_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/user_pinned_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/user_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/api/v0/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.636373 oncall-2.0.0/src/oncall/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/auth/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/auth/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.636373 oncall-2.0.0/src/oncall/auth/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/auth/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/auth/modules/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/auth/modules/ldap_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/auth/modules/ldap_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.636373 oncall-2.0.0/src/oncall/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/bin/build_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/bin/notifier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2120 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/bin/run_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/bin/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/bin/user_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/doc_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/iris.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.636373 oncall-2.0.0/src/oncall/messengers/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/messengers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/messengers/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/messengers/iris_messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/messengers/rocketchat_messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/messengers/teams_messenger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.636373 oncall-2.0.0/src/oncall/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/metrics/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/metrics/influx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/metrics/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.636373 oncall-2.0.0/src/oncall/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/notifier/reminder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/notifier/user_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.636373 oncall-2.0.0/src/oncall/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/scheduler/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/scheduler/no-skip-matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/scheduler/round-robin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/sphinx_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.636373 oncall-2.0.0/src/oncall/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.624373 oncall-2.0.0/src/oncall/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.640373 oncall-2.0.0/src/oncall/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   122540 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/css/incalendar.css
--rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/css/jquery.dataTables.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/css/loginsplash.css
--rw-r--r--   0 runner    (1001) docker     (123)    43949 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/css/oncall.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.640373 oncall-2.0.0/src/oncall/ui/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   476120 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/fonts/Source-Sans-Pro.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.640373 oncall-2.0.0/src/oncall/ui/static/images/
--rwxr-xr-x   0 runner    (1001) docker     (123)      177 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/images/chevron-bottom.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/images/headshot-blank.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/images/inbug.png
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/images/oncall_logo_blue.png
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/images/oncall_logo_white.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.640373 oncall-2.0.0/src/oncall/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    36816 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    64520 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/js/handlebars-4.0.12.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    82802 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/js/incalendar.js
--rw-r--r--   0 runner    (1001) docker     (123)    86926 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/js/jquery-3.3.1.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    79882 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/js/jquery.dataTables.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/js/loginsplash.js
--rw-r--r--   0 runner    (1001) docker     (123)    17095 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/js/moment-timezone.js
--rw-r--r--   0 runner    (1001) docker     (123)   178745 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/js/moment-tz-data-full.js
--rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/js/moment-tz-data.js
--rw-r--r--   0 runner    (1001) docker     (123)   123548 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/js/moment.js
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/js/navigo.js
--rw-r--r--   0 runner    (1001) docker     (123)   136156 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/js/oncall.js
--rw-r--r--   0 runner    (1001) docker     (123)    96224 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/static/js/typeahead.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.644373 oncall-2.0.0/src/oncall/ui/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    22629 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    87781 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/ui/templates/loginsplash.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.644373 oncall-2.0.0/src/oncall/user_sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/user_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18447 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/user_sync/ldap_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/user_sync/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-07 18:25:31.000000 oncall-2.0.0/src/oncall/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.628373 oncall-2.0.0/src/oncall.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-07 18:25:41.000000 oncall-2.0.0/src/oncall.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-06-07 18:25:41.000000 oncall-2.0.0/src/oncall.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:25:41.000000 oncall-2.0.0/src/oncall.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-07 18:25:41.000000 oncall-2.0.0/src/oncall.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-07 18:25:41.000000 oncall-2.0.0/src/oncall.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 18:25:41.000000 oncall-2.0.0/src/oncall.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:41.644373 oncall-2.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-07 18:25:31.000000 oncall-2.0.0/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-07 18:25:31.000000 oncall-2.0.0/test/test_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-06-07 18:25:31.000000 oncall-2.0.0/test/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.086718 oncall-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-07 18:29:09.000000 oncall-2.0.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-07 18:29:09.000000 oncall-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-07 18:29:09.000000 oncall-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-07 18:29:09.000000 oncall-2.0.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-07 18:29:31.086718 oncall-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-07 18:29:09.000000 oncall-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:29:31.086718 oncall-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-07 18:29:09.000000 oncall-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.066718 oncall-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.070718 oncall-2.0.1/src/oncall/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.070718 oncall-2.0.1/src/oncall/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.078718 oncall-2.0.1/src/oncall/api/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/bonus_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/event_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/event_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/event_swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/events_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/ical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/ical_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/ical_key_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/ical_key_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/ical_key_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/ical_key_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/iris_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/notification_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/populate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/public_ical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/roster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/roster_suggest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/roster_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/roster_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/rosters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17229 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/service_oncall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/service_teams.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2853 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10456 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/team_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/team_admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/team_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/team_ical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/team_iris_escalate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/team_oncall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/team_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/team_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/team_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/team_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/team_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/team_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/team_users.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8493 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/timezones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/upcoming_shifts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/user_ical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/user_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/user_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/user_pinned_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/user_pinned_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/user_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/api/v0/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.078718 oncall-2.0.1/src/oncall/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/auth/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/auth/logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.078718 oncall-2.0.1/src/oncall/auth/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/auth/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/auth/modules/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/auth/modules/ldap_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/auth/modules/ldap_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.078718 oncall-2.0.1/src/oncall/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/bin/build_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/bin/notifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2120 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/bin/run_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/bin/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/bin/user_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/doc_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/iris.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.078718 oncall-2.0.1/src/oncall/messengers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/messengers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/messengers/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/messengers/iris_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/messengers/rocketchat_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/messengers/teams_messenger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.078718 oncall-2.0.1/src/oncall/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/metrics/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/metrics/influx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/metrics/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.078718 oncall-2.0.1/src/oncall/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/notifier/reminder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/notifier/user_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.078718 oncall-2.0.1/src/oncall/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/scheduler/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/scheduler/no-skip-matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/scheduler/round-robin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/sphinx_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.078718 oncall-2.0.1/src/oncall/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.070718 oncall-2.0.1/src/oncall/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.082718 oncall-2.0.1/src/oncall/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   122540 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/css/incalendar.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/css/jquery.dataTables.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/css/loginsplash.css
+-rw-r--r--   0 runner    (1001) docker     (123)    43949 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/css/oncall.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.082718 oncall-2.0.1/src/oncall/ui/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   476120 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/fonts/Source-Sans-Pro.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.082718 oncall-2.0.1/src/oncall/ui/static/images/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      177 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/images/chevron-bottom.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/images/headshot-blank.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/images/inbug.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/images/oncall_logo_blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/images/oncall_logo_white.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.082718 oncall-2.0.1/src/oncall/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    36816 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    64520 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/js/handlebars-4.0.12.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    82802 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/js/incalendar.js
+-rw-r--r--   0 runner    (1001) docker     (123)    86926 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/js/jquery-3.3.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    79882 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/js/jquery.dataTables.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/js/loginsplash.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17095 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/js/moment-timezone.js
+-rw-r--r--   0 runner    (1001) docker     (123)   178745 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/js/moment-tz-data-full.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/js/moment-tz-data.js
+-rw-r--r--   0 runner    (1001) docker     (123)   123548 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/js/moment.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/js/navigo.js
+-rw-r--r--   0 runner    (1001) docker     (123)   136156 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/js/oncall.js
+-rw-r--r--   0 runner    (1001) docker     (123)    96224 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/static/js/typeahead.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.082718 oncall-2.0.1/src/oncall/ui/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    22629 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    87781 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/ui/templates/loginsplash.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.082718 oncall-2.0.1/src/oncall/user_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/user_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18447 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/user_sync/ldap_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/user_sync/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-07 18:29:09.000000 oncall-2.0.1/src/oncall/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.070718 oncall-2.0.1/src/oncall.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-07 18:29:30.000000 oncall-2.0.1/src/oncall.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-06-07 18:29:31.000000 oncall-2.0.1/src/oncall.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:29:30.000000 oncall-2.0.1/src/oncall.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-07 18:29:30.000000 oncall-2.0.1/src/oncall.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-07 18:29:30.000000 oncall-2.0.1/src/oncall.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 18:29:30.000000 oncall-2.0.1/src/oncall.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:29:31.086718 oncall-2.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-07 18:29:09.000000 oncall-2.0.1/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-07 18:29:09.000000 oncall-2.0.1/test/test_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-06-07 18:29:09.000000 oncall-2.0.1/test/test_scheduler.py
```

### Comparing `oncall-2.0.0/LICENSE` & `oncall-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/NOTICE` & `oncall-2.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/PKG-INFO` & `oncall-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oncall
-Version: 2.0.0
+Version: 2.0.1
 Summary: Oncall is a calendar tool designed for scheduling and managing on-call shifts
 Home-page: https://github.com/linkedin/oncall
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `oncall-2.0.0/README.md` & `oncall-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/setup.py` & `oncall-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/__init__.py` & `oncall-2.0.1/src/oncall/api/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/audit.py` & `oncall-2.0.1/src/oncall/api/v0/audit.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/bonus_events.py` & `oncall-2.0.1/src/oncall/api/v0/bonus_events.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/event.py` & `oncall-2.0.1/src/oncall/api/v0/event.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/event_link.py` & `oncall-2.0.1/src/oncall/api/v0/event_link.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/event_override.py` & `oncall-2.0.1/src/oncall/api/v0/event_override.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/event_swap.py` & `oncall-2.0.1/src/oncall/api/v0/event_swap.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/events.py` & `oncall-2.0.1/src/oncall/api/v0/events.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/events_link.py` & `oncall-2.0.1/src/oncall/api/v0/events_link.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/ical.py` & `oncall-2.0.1/src/oncall/api/v0/ical.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/ical_key.py` & `oncall-2.0.1/src/oncall/api/v0/ical_key.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/ical_key_detail.py` & `oncall-2.0.1/src/oncall/api/v0/ical_key_detail.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/ical_key_requester.py` & `oncall-2.0.1/src/oncall/api/v0/ical_key_requester.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/ical_key_team.py` & `oncall-2.0.1/src/oncall/api/v0/ical_key_team.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/ical_key_user.py` & `oncall-2.0.1/src/oncall/api/v0/ical_key_user.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/modes.py` & `oncall-2.0.1/src/oncall/api/v0/modes.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/notification_types.py` & `oncall-2.0.1/src/oncall/api/v0/notification_types.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/notifications.py` & `oncall-2.0.1/src/oncall/api/v0/notifications.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/populate.py` & `oncall-2.0.1/src/oncall/api/v0/populate.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/preview.py` & `oncall-2.0.1/src/oncall/api/v0/preview.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/public_ical.py` & `oncall-2.0.1/src/oncall/api/v0/public_ical.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/role.py` & `oncall-2.0.1/src/oncall/api/v0/role.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/roles.py` & `oncall-2.0.1/src/oncall/api/v0/roles.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/roster.py` & `oncall-2.0.1/src/oncall/api/v0/roster.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/roster_suggest.py` & `oncall-2.0.1/src/oncall/api/v0/roster_suggest.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/roster_user.py` & `oncall-2.0.1/src/oncall/api/v0/roster_user.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/roster_users.py` & `oncall-2.0.1/src/oncall/api/v0/roster_users.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/rosters.py` & `oncall-2.0.1/src/oncall/api/v0/rosters.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/schedule.py` & `oncall-2.0.1/src/oncall/api/v0/schedule.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/schedules.py` & `oncall-2.0.1/src/oncall/api/v0/schedules.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/search.py` & `oncall-2.0.1/src/oncall/api/v0/search.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/service.py` & `oncall-2.0.1/src/oncall/api/v0/service.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/service_oncall.py` & `oncall-2.0.1/src/oncall/api/v0/service_oncall.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/service_teams.py` & `oncall-2.0.1/src/oncall/api/v0/service_teams.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/services.py` & `oncall-2.0.1/src/oncall/api/v0/services.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/team.py` & `oncall-2.0.1/src/oncall/api/v0/team.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/team_admin.py` & `oncall-2.0.1/src/oncall/api/v0/team_admin.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/team_admins.py` & `oncall-2.0.1/src/oncall/api/v0/team_admins.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/team_changes.py` & `oncall-2.0.1/src/oncall/api/v0/team_changes.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/team_ical.py` & `oncall-2.0.1/src/oncall/api/v0/team_ical.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/team_iris_escalate.py` & `oncall-2.0.1/src/oncall/api/v0/team_iris_escalate.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/team_oncall.py` & `oncall-2.0.1/src/oncall/api/v0/team_oncall.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/team_service.py` & `oncall-2.0.1/src/oncall/api/v0/team_service.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/team_services.py` & `oncall-2.0.1/src/oncall/api/v0/team_services.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/team_subscription.py` & `oncall-2.0.1/src/oncall/api/v0/team_subscription.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/team_subscriptions.py` & `oncall-2.0.1/src/oncall/api/v0/team_subscriptions.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/team_summary.py` & `oncall-2.0.1/src/oncall/api/v0/team_summary.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/team_user.py` & `oncall-2.0.1/src/oncall/api/v0/team_user.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/team_users.py` & `oncall-2.0.1/src/oncall/api/v0/team_users.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/teams.py` & `oncall-2.0.1/src/oncall/api/v0/teams.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/upcoming_shifts.py` & `oncall-2.0.1/src/oncall/api/v0/upcoming_shifts.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/user.py` & `oncall-2.0.1/src/oncall/api/v0/user.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/user_ical.py` & `oncall-2.0.1/src/oncall/api/v0/user_ical.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/user_notification.py` & `oncall-2.0.1/src/oncall/api/v0/user_notification.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/user_notifications.py` & `oncall-2.0.1/src/oncall/api/v0/user_notifications.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/user_pinned_team.py` & `oncall-2.0.1/src/oncall/api/v0/user_pinned_team.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/user_pinned_teams.py` & `oncall-2.0.1/src/oncall/api/v0/user_pinned_teams.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/user_teams.py` & `oncall-2.0.1/src/oncall/api/v0/user_teams.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/api/v0/users.py` & `oncall-2.0.1/src/oncall/api/v0/users.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/app.py` & `oncall-2.0.1/src/oncall/app.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/auth/__init__.py` & `oncall-2.0.1/src/oncall/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/auth/login.py` & `oncall-2.0.1/src/oncall/auth/login.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/auth/modules/ldap_example.py` & `oncall-2.0.1/src/oncall/auth/modules/ldap_example.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/auth/modules/ldap_import.py` & `oncall-2.0.1/src/oncall/auth/modules/ldap_import.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/bin/notifier.py` & `oncall-2.0.1/src/oncall/bin/notifier.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/bin/run_server.py` & `oncall-2.0.1/src/oncall/bin/run_server.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/bin/scheduler.py` & `oncall-2.0.1/src/oncall/bin/scheduler.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/bin/user_sync.py` & `oncall-2.0.1/src/oncall/bin/user_sync.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/constants.py` & `oncall-2.0.1/src/oncall/constants.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/db.py` & `oncall-2.0.1/src/oncall/db.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/doc_helper.py` & `oncall-2.0.1/src/oncall/doc_helper.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/healthcheck.py` & `oncall-2.0.1/src/oncall/healthcheck.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/messengers/__init__.py` & `oncall-2.0.1/src/oncall/messengers/__init__.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/messengers/iris_messenger.py` & `oncall-2.0.1/src/oncall/messengers/iris_messenger.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/messengers/rocketchat_messenger.py` & `oncall-2.0.1/src/oncall/messengers/rocketchat_messenger.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/messengers/teams_messenger.py` & `oncall-2.0.1/src/oncall/messengers/teams_messenger.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/metrics/__init__.py` & `oncall-2.0.1/src/oncall/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/metrics/dummy.py` & `oncall-2.0.1/src/oncall/metrics/dummy.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/metrics/influx.py` & `oncall-2.0.1/src/oncall/metrics/influx.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/metrics/prometheus.py` & `oncall-2.0.1/src/oncall/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/notifier/reminder.py` & `oncall-2.0.1/src/oncall/notifier/reminder.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/notifier/user_validator.py` & `oncall-2.0.1/src/oncall/notifier/user_validator.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/scheduler/default.py` & `oncall-2.0.1/src/oncall/scheduler/default.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/scheduler/round-robin.py` & `oncall-2.0.1/src/oncall/scheduler/round-robin.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/sphinx_extension.py` & `oncall-2.0.1/src/oncall/sphinx_extension.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/__init__.py` & `oncall-2.0.1/src/oncall/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/css/bootstrap.min.css` & `oncall-2.0.1/src/oncall/ui/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/css/incalendar.css` & `oncall-2.0.1/src/oncall/ui/static/css/incalendar.css`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/css/jquery.dataTables.min.css` & `oncall-2.0.1/src/oncall/ui/static/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/css/loginsplash.css` & `oncall-2.0.1/src/oncall/ui/static/css/loginsplash.css`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/css/oncall.css` & `oncall-2.0.1/src/oncall/ui/static/css/oncall.css`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/fonts/Source-Sans-Pro.css` & `oncall-2.0.1/src/oncall/ui/static/fonts/Source-Sans-Pro.css`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/images/favicon.png` & `oncall-2.0.1/src/oncall/ui/static/images/favicon.png`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/images/headshot-blank.jpg` & `oncall-2.0.1/src/oncall/ui/static/images/headshot-blank.jpg`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/images/oncall_logo_blue.png` & `oncall-2.0.1/src/oncall/ui/static/images/oncall_logo_blue.png`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/images/oncall_logo_white.png` & `oncall-2.0.1/src/oncall/ui/static/images/oncall_logo_white.png`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/js/bootstrap.min.js` & `oncall-2.0.1/src/oncall/ui/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/js/handlebars-4.0.12.min.js` & `oncall-2.0.1/src/oncall/ui/static/js/handlebars-4.0.12.min.js`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/js/incalendar.js` & `oncall-2.0.1/src/oncall/ui/static/js/incalendar.js`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/js/jquery-3.3.1.min.js` & `oncall-2.0.1/src/oncall/ui/static/js/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/js/jquery.dataTables.min.js` & `oncall-2.0.1/src/oncall/ui/static/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/js/loginsplash.js` & `oncall-2.0.1/src/oncall/ui/static/js/loginsplash.js`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/js/moment-timezone.js` & `oncall-2.0.1/src/oncall/ui/static/js/moment-timezone.js`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/js/moment-tz-data-full.js` & `oncall-2.0.1/src/oncall/ui/static/js/moment-tz-data-full.js`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/js/moment-tz-data.js` & `oncall-2.0.1/src/oncall/ui/static/js/moment-tz-data.js`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/js/moment.js` & `oncall-2.0.1/src/oncall/ui/static/js/moment.js`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/js/navigo.js` & `oncall-2.0.1/src/oncall/ui/static/js/navigo.js`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/js/oncall.js` & `oncall-2.0.1/src/oncall/ui/static/js/oncall.js`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/static/js/typeahead.js` & `oncall-2.0.1/src/oncall/ui/static/js/typeahead.js`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/templates/base.html` & `oncall-2.0.1/src/oncall/ui/templates/base.html`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/templates/index.html` & `oncall-2.0.1/src/oncall/ui/templates/index.html`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/ui/templates/loginsplash.html` & `oncall-2.0.1/src/oncall/ui/templates/loginsplash.html`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/user_sync/ldap_sync.py` & `oncall-2.0.1/src/oncall/user_sync/ldap_sync.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/user_sync/slack.py` & `oncall-2.0.1/src/oncall/user_sync/slack.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall/utils.py` & `oncall-2.0.1/src/oncall/utils.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/src/oncall.egg-info/PKG-INFO` & `oncall-2.0.1/src/oncall.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oncall
-Version: 2.0.0
+Version: 2.0.1
 Summary: Oncall is a calendar tool designed for scheduling and managing on-call shifts
 Home-page: https://github.com/linkedin/oncall
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `oncall-2.0.0/src/oncall.egg-info/SOURCES.txt` & `oncall-2.0.1/src/oncall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/test/test_auth.py` & `oncall-2.0.1/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/test/test_notifier.py` & `oncall-2.0.1/test/test_notifier.py`

 * *Files identical despite different names*

### Comparing `oncall-2.0.0/test/test_scheduler.py` & `oncall-2.0.1/test/test_scheduler.py`

 * *Files identical despite different names*

