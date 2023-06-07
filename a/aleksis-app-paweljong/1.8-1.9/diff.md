# Comparing `tmp/AlekSIS-App-Paweljong-1.8.tar.gz` & `tmp/AlekSIS-App-Paweljong-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlekSIS-App-Paweljong-1.8.tar", max compression
+gzip compressed data, was "AlekSIS-App-Paweljong-1.9.tar", max compression
```

## Comparing `AlekSIS-App-Paweljong-1.8.tar` & `AlekSIS-App-Paweljong-1.9.tar`

### file list

```diff
@@ -1,99 +1,103 @@
--rw-r--r--   0        0        0     3437 2022-05-04 17:07:49.804504 AlekSIS-App-Paweljong-1.8/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2021-11-30 15:14:06.498459 AlekSIS-App-Paweljong-1.8/LICENCE.rst
--rw-r--r--   0        0        0     1173 2022-02-21 18:12:43.394342 AlekSIS-App-Paweljong-1.8/README.rst
--rw-r--r--   0        0        0      155 2021-11-30 15:50:47.629248 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/__init__.py
--rw-r--r--   0        0        0      530 2022-02-21 18:12:43.394342 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/apps.py
--rw-r--r--   0        0        0     1254 2022-06-19 20:01:59.822897 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/data_checks.py
--rw-r--r--   0        0        0     1726 2022-06-24 14:54:41.596452 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/filters.py
--rw-r--r--   0        0        0    14952 2022-06-19 19:58:48.687395 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/forms.py
--rw-r--r--   0        0        0        0 2021-11-30 15:14:06.498459 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/.keepdir
--rw-r--r--   0        0        0      463 2022-06-24 15:05:36.614903 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43064 2022-06-24 14:54:51.116429 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    28604 2022-06-24 15:05:36.614903 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    58890 2022-06-24 15:05:14.006959 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2022-06-24 15:05:36.614903 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    42980 2022-06-24 14:54:51.100430 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2022-06-24 15:05:36.618903 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    42934 2022-06-24 14:54:51.088430 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2022-06-24 15:05:36.614903 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    42934 2022-06-24 14:54:51.044430 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2022-06-24 15:05:36.614903 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    42934 2022-06-24 14:54:51.056430 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3256 2022-06-19 19:58:48.687395 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/menus.py
--rw-r--r--   0        0        0     8646 2022-02-21 09:18:10.132166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0001_initial.py
--rw-r--r--   0        0        0      457 2021-11-30 15:50:20.745263 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0002_event_website.py
--rw-r--r--   0        0        0      493 2022-02-21 09:18:10.132166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0003_alter_event_feedback_aspects.py
--rw-r--r--   0        0        0      911 2022-02-21 09:18:10.132166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0004_richtext_field_information.py
--rw-r--r--   0        0        0      479 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0005_eventregistration_medical_information.py
--rw-r--r--   0        0        0      860 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0006_unique_constraints.py
--rw-r--r--   0        0        0     2493 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0007_terms.py
--rw-r--r--   0        0        0      582 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0008_remove_terms_from_event.py
--rw-r--r--   0        0        0      609 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0009_remove_feedback.py
--rw-r--r--   0        0        0      461 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0010_term_confirmation_text.py
--rw-r--r--   0        0        0      484 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0011_registration_accepted_terms.py
--rw-r--r--   0        0        0      463 2022-02-21 20:54:12.455591 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0012_event_slug.py
--rw-r--r--   0        0        0     2429 2022-03-01 20:42:19.678476 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0013_info_mailings.py
--rw-r--r--   0        0        0     2855 2022-03-03 20:52:23.956034 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0014_move_sent_to_to_through.py
--rw-r--r--   0        0        0     1268 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0015_registrationstate.py
--rw-r--r--   0        0        0      475 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0016_eventregistration_states.py
--rw-r--r--   0        0        0      419 2022-03-13 13:23:46.984225 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0017_fix_voucher_max_length.py
--rw-r--r--   0        0        0     1781 2022-03-13 13:23:46.984225 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0018_payment_with_tezor.py
--rw-r--r--   0        0        0      637 2022-06-19 20:01:59.822897 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0019_retractions.py
--rw-r--r--   0        0        0      638 2022-06-24 14:54:41.596452 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0020_check_in.py
--rw-r--r--   0        0        0        0 2021-11-30 15:14:06.498459 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/__init__.py
--rw-r--r--   0        0        0    14443 2022-06-24 14:54:41.596452 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/models.py
--rw-r--r--   0        0        0     1333 2022-06-19 21:06:49.061623 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/predicates.py
--rw-r--r--   0        0        0      732 2022-03-06 19:51:43.057119 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/preferences.py
--rw-r--r--   0        0        0     8532 2022-06-24 14:54:41.596452 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/rules.py
--rw-r--r--   0        0        0       51 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/settings.py
--rw-r--r--   0        0        0      990 2022-06-19 19:58:48.687395 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/static/css/paweljong.css
--rw-r--r--   0        0        0     4446 2022-06-24 14:54:41.596452 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/tables.py
--rw-r--r--   0        0        0      266 2022-03-01 20:03:12.342378 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/tasks.py
--rw-r--r--   0        0        0     1316 2022-02-22 22:51:08.579836 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/account_wizard.html
--rw-r--r--   0        0        0      592 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/create.html
--rw-r--r--   0        0        0     3217 2022-06-24 14:54:41.596452 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/detail.html
--rw-r--r--   0        0        0      585 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/edit.html
--rw-r--r--   0        0        0     2475 2022-02-21 22:05:46.538591 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/full.html
--rw-r--r--   0        0        0      568 2021-11-30 15:38:18.987000 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/list.html
--rw-r--r--   0        0        0      915 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/manage.html
--rw-r--r--   0        0        0      518 2022-06-19 19:58:48.687395 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/persons_group.html
--rw-r--r--   0        0        0     4488 2022-02-21 20:54:12.455591 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/register_start.html
--rw-r--r--   0        0        0     1640 2022-02-21 20:56:23.799158 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html
--rw-r--r--   0        0        0     1876 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html
--rw-r--r--   0        0        0      312 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/registered.html
--rw-r--r--   0        0        0      535 2022-06-19 21:06:49.061623 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/terms.html
--rw-r--r--   0        0        0      599 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html
--rw-r--r--   0        0        0    12811 2022-06-24 14:54:41.600452 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event_registration/full.html
--rw-r--r--   0        0        0      514 2022-03-06 19:55:13.296748 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html
--rw-r--r--   0        0        0      513 2022-03-01 20:03:12.342378 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/info_mailing/create.html
--rw-r--r--   0        0        0      508 2022-03-01 20:03:12.342378 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/info_mailing/edit.html
--rw-r--r--   0        0        0      483 2022-03-01 20:03:12.342378 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html
--rw-r--r--   0        0        0     6730 2022-03-13 13:23:46.984225 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html
--rw-r--r--   0        0        0     1461 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/print/corona.html
--rw-r--r--   0        0        0     3192 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html
--rw-r--r--   0        0        0     1947 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/print/list_participants.html
--rw-r--r--   0        0        0     1081 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/print/list_sign.html
--rw-r--r--   0        0        0      494 2021-11-30 15:38:18.987000 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/print/manage.html
--rw-r--r--   0        0        0     1025 2022-06-21 19:40:35.903740 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/print/voucher.html
--rw-r--r--   0        0        0      505 2021-11-30 15:38:18.987000 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/register.html
--rw-r--r--   0        0        0     2434 2022-02-22 22:51:08.583835 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/register_start.html
--rw-r--r--   0        0        0      506 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/registration_state/chip.html
--rw-r--r--   0        0        0      525 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/registration_state/create.html
--rw-r--r--   0        0        0      520 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html
--rw-r--r--   0        0        0      507 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/registration_state/list.html
--rw-r--r--   0        0        0      497 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/term/create.html
--rw-r--r--   0        0        0      492 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/term/edit.html
--rw-r--r--   0        0        0      451 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/term/list.html
--rw-r--r--   0        0        0      594 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/voucher/create.html
--rw-r--r--   0        0        0      590 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/voucher/edit.html
--rw-r--r--   0        0        0      939 2022-06-21 19:41:29.939654 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/voucher/list.html
--rw-r--r--   0        0        0     2365 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/templated_email/event_created.email
--rw-r--r--   0        0        0       94 2022-03-06 19:55:13.296748 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/templated_email/event_notification.email
--rw-r--r--   0        0        0     3879 2022-03-13 13:23:46.984225 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/templated_email/event_registered.email
--rw-r--r--   0        0        0       94 2022-03-01 20:03:12.342378 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/templated_email/info_mailing.email
--rw-r--r--   0        0        0      235 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templatetags/coerce.py
--rw-r--r--   0        0        0     5270 2022-06-24 14:54:41.600452 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/urls.py
--rw-r--r--   0        0        0    36468 2022-06-24 14:54:41.600452 AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/views.py
--rw-r--r--   0        0        0     1452 2022-06-24 15:05:47.798876 AlekSIS-App-Paweljong-1.8/pyproject.toml
--rw-r--r--   0        0        0    15941 2022-06-24 15:05:55.279505 AlekSIS-App-Paweljong-1.8/setup.py
--rw-r--r--   0        0        0     2208 2022-06-24 15:05:55.280131 AlekSIS-App-Paweljong-1.8/PKG-INFO
+-rw-r--r--   0        0        0     3437 2022-05-04 17:07:49.804504 AlekSIS-App-Paweljong-1.9/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2021-11-30 15:14:06.498459 AlekSIS-App-Paweljong-1.9/LICENCE.rst
+-rw-r--r--   0        0        0     1173 2022-02-21 18:12:43.394342 AlekSIS-App-Paweljong-1.9/README.rst
+-rw-r--r--   0        0        0      155 2021-11-30 15:50:47.629248 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/__init__.py
+-rw-r--r--   0        0        0      530 2022-02-21 18:12:43.394342 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/apps.py
+-rw-r--r--   0        0        0     1254 2022-06-19 20:01:59.822897 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/data_checks.py
+-rw-r--r--   0        0        0     1726 2022-06-24 14:54:41.596452 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/filters.py
+-rw-r--r--   0        0        0    16143 2022-06-27 11:04:58.585278 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/forms.py
+-rw-r--r--   0        0        0        0 2021-11-30 15:14:06.498459 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/.keepdir
+-rw-r--r--   0        0        0      463 2022-06-28 15:45:03.630316 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    44339 2022-06-28 15:44:36.897766 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    28604 2022-06-28 15:45:03.634316 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    60401 2022-06-28 15:44:36.941766 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2022-06-28 15:45:03.630316 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    44255 2022-06-28 15:44:36.909766 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2022-06-28 15:45:03.634316 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    44209 2022-06-28 15:44:36.921766 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2022-06-28 15:45:03.630316 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    44209 2022-06-28 15:44:36.965767 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2022-06-28 15:45:03.634316 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    44209 2022-06-28 15:44:36.953766 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3256 2022-06-27 10:59:49.965700 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/menus.py
+-rw-r--r--   0        0        0     8646 2022-02-21 09:18:10.132166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0001_initial.py
+-rw-r--r--   0        0        0      457 2021-11-30 15:50:20.745263 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0002_event_website.py
+-rw-r--r--   0        0        0      493 2022-02-21 09:18:10.132166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0003_alter_event_feedback_aspects.py
+-rw-r--r--   0        0        0      911 2022-02-21 09:18:10.132166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0004_richtext_field_information.py
+-rw-r--r--   0        0        0      479 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0005_eventregistration_medical_information.py
+-rw-r--r--   0        0        0      860 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0006_unique_constraints.py
+-rw-r--r--   0        0        0     2493 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0007_terms.py
+-rw-r--r--   0        0        0      582 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0008_remove_terms_from_event.py
+-rw-r--r--   0        0        0      609 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0009_remove_feedback.py
+-rw-r--r--   0        0        0      461 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0010_term_confirmation_text.py
+-rw-r--r--   0        0        0      484 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0011_registration_accepted_terms.py
+-rw-r--r--   0        0        0      463 2022-02-21 20:54:12.455591 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0012_event_slug.py
+-rw-r--r--   0        0        0     2429 2022-03-01 20:42:19.678476 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0013_info_mailings.py
+-rw-r--r--   0        0        0     2855 2022-03-03 20:52:23.956034 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0014_move_sent_to_to_through.py
+-rw-r--r--   0        0        0     1268 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0015_registrationstate.py
+-rw-r--r--   0        0        0      475 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0016_eventregistration_states.py
+-rw-r--r--   0        0        0      419 2022-03-13 13:23:46.984225 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0017_fix_voucher_max_length.py
+-rw-r--r--   0        0        0     1781 2022-03-13 13:23:46.984225 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0018_payment_with_tezor.py
+-rw-r--r--   0        0        0      637 2022-06-19 20:01:59.822897 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0019_retractions.py
+-rw-r--r--   0        0        0      638 2022-06-24 14:54:41.596452 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0020_check_in.py
+-rw-r--r--   0        0        0     2217 2022-06-27 10:59:54.101694 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0021_checkpoint.py
+-rw-r--r--   0        0        0        0 2021-11-30 15:14:06.498459 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/__init__.py
+-rw-r--r--   0        0        0    15306 2022-06-28 15:42:20.693243 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/models.py
+-rw-r--r--   0        0        0     1333 2022-06-19 21:06:49.061623 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/predicates.py
+-rw-r--r--   0        0        0      732 2022-03-06 19:51:43.057119 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/preferences.py
+-rw-r--r--   0        0        0     8923 2022-06-27 10:59:54.101694 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/rules.py
+-rw-r--r--   0        0        0       51 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/settings.py
+-rw-r--r--   0        0        0      990 2022-06-19 19:58:48.687395 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/static/css/paweljong.css
+-rw-r--r--   0        0        0      481 2022-06-27 10:59:54.101694 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/static/js/paweljong/checkpoint.js
+-rw-r--r--   0        0        0      597 2022-06-27 10:59:54.101694 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/static/js/paweljong/qrscanner.js
+-rw-r--r--   0        0        0     4446 2022-06-24 14:54:41.596452 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/tables.py
+-rw-r--r--   0        0        0      266 2022-03-01 20:03:12.342378 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/tasks.py
+-rw-r--r--   0        0        0     1316 2022-02-22 22:51:08.579836 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/account_wizard.html
+-rw-r--r--   0        0        0      560 2022-06-27 10:59:54.101694 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html
+-rw-r--r--   0        0        0      592 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/create.html
+-rw-r--r--   0        0        0     3547 2022-06-28 15:43:45.196693 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/detail.html
+-rw-r--r--   0        0        0      585 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/edit.html
+-rw-r--r--   0        0        0     2475 2022-02-21 22:05:46.538591 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/full.html
+-rw-r--r--   0        0        0      568 2021-11-30 15:38:18.987000 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/list.html
+-rw-r--r--   0        0        0      915 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/manage.html
+-rw-r--r--   0        0        0      576 2022-06-27 10:59:54.101694 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/persons_group.html
+-rw-r--r--   0        0        0     4488 2022-02-21 20:54:12.455591 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/register_start.html
+-rw-r--r--   0        0        0     1640 2022-02-21 20:56:23.799158 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html
+-rw-r--r--   0        0        0     1876 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html
+-rw-r--r--   0        0        0      312 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/registered.html
+-rw-r--r--   0        0        0      535 2022-06-19 21:06:49.061623 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/terms.html
+-rw-r--r--   0        0        0      599 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html
+-rw-r--r--   0        0        0    12811 2022-06-28 08:40:58.099898 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event_registration/full.html
+-rw-r--r--   0        0        0      514 2022-03-06 19:55:13.296748 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html
+-rw-r--r--   0        0        0      513 2022-03-01 20:03:12.342378 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/info_mailing/create.html
+-rw-r--r--   0        0        0      508 2022-03-01 20:03:12.342378 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/info_mailing/edit.html
+-rw-r--r--   0        0        0      483 2022-03-01 20:03:12.342378 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html
+-rw-r--r--   0        0        0     6730 2022-03-13 13:23:46.984225 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html
+-rw-r--r--   0        0        0     1461 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/corona.html
+-rw-r--r--   0        0        0     3192 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html
+-rw-r--r--   0        0        0     1947 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/list_participants.html
+-rw-r--r--   0        0        0     1081 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/list_sign.html
+-rw-r--r--   0        0        0      494 2021-11-30 15:38:18.987000 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/manage.html
+-rw-r--r--   0        0        0     1025 2022-06-21 19:40:35.903740 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/voucher.html
+-rw-r--r--   0        0        0      505 2021-11-30 15:38:18.987000 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/register.html
+-rw-r--r--   0        0        0     2434 2022-02-22 22:51:08.583835 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/register_start.html
+-rw-r--r--   0        0        0      506 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/registration_state/chip.html
+-rw-r--r--   0        0        0      525 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/registration_state/create.html
+-rw-r--r--   0        0        0      520 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html
+-rw-r--r--   0        0        0      507 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/registration_state/list.html
+-rw-r--r--   0        0        0      497 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/term/create.html
+-rw-r--r--   0        0        0      492 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/term/edit.html
+-rw-r--r--   0        0        0      451 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/term/list.html
+-rw-r--r--   0        0        0      594 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/voucher/create.html
+-rw-r--r--   0        0        0      590 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/voucher/edit.html
+-rw-r--r--   0        0        0      939 2022-06-21 19:41:29.939654 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/voucher/list.html
+-rw-r--r--   0        0        0     2365 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/templated_email/event_created.email
+-rw-r--r--   0        0        0       94 2022-03-06 19:55:13.296748 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/templated_email/event_notification.email
+-rw-r--r--   0        0        0     3879 2022-03-13 13:23:46.984225 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/templated_email/event_registered.email
+-rw-r--r--   0        0        0       94 2022-03-01 20:03:12.342378 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/templated_email/info_mailing.email
+-rw-r--r--   0        0        0      235 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templatetags/coerce.py
+-rw-r--r--   0        0        0     5382 2022-06-28 08:40:58.099898 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/urls.py
+-rw-r--r--   0        0        0    38228 2022-06-28 08:40:58.099898 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/views.py
+-rw-r--r--   0        0        0     1452 2022-06-28 15:44:26.977692 AlekSIS-App-Paweljong-1.9/pyproject.toml
+-rw-r--r--   0        0        0    17809 2022-06-28 15:45:06.274288 AlekSIS-App-Paweljong-1.9/setup.py
+-rw-r--r--   0        0        0     2208 2022-06-28 15:45:06.274820 AlekSIS-App-Paweljong-1.9/PKG-INFO
```

### Comparing `AlekSIS-App-Paweljong-1.8/CHANGELOG.rst` & `AlekSIS-App-Paweljong-1.9/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/LICENCE.rst` & `AlekSIS-App-Paweljong-1.9/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/README.rst` & `AlekSIS-App-Paweljong-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/apps.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/apps.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/data_checks.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/data_checks.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/filters.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/filters.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/forms.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -488,16 +488,63 @@
 class RegistrationStatesForm(forms.ModelForm):
     class Meta:
         model = RegistrationState
         exclude = []
 
 
 class PersonGroupFormPerson(forms.Form):
+    class Media:
+        js = ("https://unpkg.com/html5-qrcode", "js/paweljong/qrscanner.js")
 
     layout = Layout("username")
 
     username = forms.CharField(
         required=True,
         label=_("Person"),
         widget=forms.TextInput(attrs={"autofocus": "", "autocomplete": "off"}),
         help_text=_("Please enter a username."),
     )
+
+
+class EventCheckpointForm(forms.Form):
+    class Media:
+        js = ("https://unpkg.com/html5-qrcode", "js/paweljong/qrscanner.js", "js/paweljong/checkpoint.js")
+
+    layout = Layout(
+        "comment", "use_latlon",
+    )
+
+    comment = forms.CharField(
+        required=True,
+        label=_("Comment"),
+        help_text=_("Please enter a comment describing the checkpoint (e.g. Dinner)."),
+    )
+
+    username = forms.CharField(
+        required=True,
+        label=_("Person"),
+        help_text=_("Please enter a username."),
+        widget=forms.HiddenInput(),
+    )
+
+    use_latlon = forms.BooleanField(
+        required=False,
+        label=_("Submit geolocation"),
+        initial=True,
+    )
+
+    lat = forms.DecimalField(
+        required=False,
+        min_value=-90.0,
+        max_value=90.0,
+        max_digits=10,
+        decimal_places=8,
+        widget=forms.HiddenInput(),
+    )
+    lon = forms.DecimalField(
+        required=False,
+        min_value=-180.0,
+        max_value=180.0,
+        max_digits=11,
+        decimal_places=8,
+        widget=forms.HiddenInput(),
+    )
```

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.po` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-24 14:54+0000\n"
+"POT-Creation-Date: 2022-06-28 15:44+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: aleksis/apps/paweljong/data_checks.py:8
 msgid "Sync members"
 msgstr ""
 
 #: aleksis/apps/paweljong/data_checks.py:19
 msgid "Ensure that all registered persons are member of the linked group"
@@ -344,25 +344,38 @@
 msgid "Account data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:455
 msgid "The username must only contain lower case letters and numbers, and must begin with a letter."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:500 aleksis/apps/paweljong/models.py:228
-#: aleksis/apps/paweljong/models.py:257 aleksis/apps/paweljong/tables.py:46
+#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:524
+#: aleksis/apps/paweljong/models.py:228 aleksis/apps/paweljong/models.py:257
+#: aleksis/apps/paweljong/tables.py:46
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:61
 msgid "Person"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:502
+#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:525
 msgid "Please enter a username."
 msgstr ""
 
+#: aleksis/apps/paweljong/forms.py:518 aleksis/apps/paweljong/models.py:417
+msgid "Comment"
+msgstr ""
+
+#: aleksis/apps/paweljong/forms.py:519
+msgid "Please enter a comment describing the checkpoint (e.g. Dinner)."
+msgstr ""
+
+#: aleksis/apps/paweljong/forms.py:531
+msgid "Submit geolocation"
+msgstr ""
+
 #: aleksis/apps/paweljong/menus.py:6
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
 msgid "Register"
 msgstr ""
 
 #: aleksis/apps/paweljong/menus.py:14
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
@@ -385,15 +398,15 @@
 
 #: aleksis/apps/paweljong/menus.py:70
 msgid "Generate participant list"
 msgstr ""
 
 #: aleksis/apps/paweljong/menus.py:81
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
-#: aleksis/apps/paweljong/views.py:746
+#: aleksis/apps/paweljong/views.py:748
 msgid "Upcoming events"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:28
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:25
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:63
@@ -557,15 +570,15 @@
 msgid "Checked in"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:290
 msgid "Checked in at"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:989
+#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:1034
 msgid "Person is already checked in!"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:334
 msgid "Participation of {} in event {}"
 msgstr ""
 
@@ -573,22 +586,46 @@
 msgid "Social Sponsoring / Extra Donation"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:374
 msgid "Voucher / Granted discount"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:390
+#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:392
 msgid "Event registration"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:403
 msgid "Event registrations"
 msgstr ""
 
+#: aleksis/apps/paweljong/models.py:412
+msgid "Related event"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:413
+msgid "Checked person"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:414
+msgid "Checked by person"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:419
+msgid "Date and time of check"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:420
+msgid "Latitude of check"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:421
+msgid "Longitude of check"
+msgstr ""
+
 #: aleksis/apps/paweljong/preferences.py:10
 msgid "Paweljong"
 msgstr ""
 
 #: aleksis/apps/paweljong/preferences.py:20
 msgid "Mail recipient for event notifications"
 msgstr ""
@@ -684,60 +721,66 @@
 
 #: aleksis/apps/paweljong/templates/paweljong/account_wizard.html:32
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html:44
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html:58
 msgid "Next"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html:4
+#: aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html:5
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:30
+msgid "Checkpoint"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/event/create.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/create.html:5
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:20
 msgid "Create event"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:43
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:47
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:31
 msgid "Registration open until"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:48
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:52
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:36
 msgid "Participation fee (all inclusive)"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:54
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:58
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:42
 msgid "of"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:58
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:62
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:17
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:45
 msgid "Owners"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:76
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:80
 msgid "Additional fields"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:80
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:84
 msgid "Child groups"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:85
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:89
 msgid "Registrations"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:88
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:92
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:14
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:14
 msgid "Search"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:92
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:96
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:18
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:18
 msgid "Clear"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:5
@@ -945,15 +988,15 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:246
 msgid "Billing information"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:278
-#: aleksis/apps/paweljong/views.py:419
+#: aleksis/apps/paweljong/views.py:421
 msgid "Payment"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:316
 msgid "Guardians / Parents "
 msgstr ""
 
@@ -1184,144 +1227,152 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:54
 #, python-format
 msgid "New registration: %(registration)s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:66 aleksis/apps/paweljong/views.py:78
+#: aleksis/apps/paweljong/views.py:68 aleksis/apps/paweljong/views.py:80
 msgid "The event has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:150
+#: aleksis/apps/paweljong/views.py:152
 msgid "The event registration has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:162
+#: aleksis/apps/paweljong/views.py:164
 msgid "The event registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:183
+#: aleksis/apps/paweljong/views.py:185
 msgid "The registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:228
+#: aleksis/apps/paweljong/views.py:230
 msgid "The registration has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:240
+#: aleksis/apps/paweljong/views.py:242
 msgid "The voucher has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:252
+#: aleksis/apps/paweljong/views.py:254
 msgid "The voucher has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:262
+#: aleksis/apps/paweljong/views.py:264
 msgid "The voucher has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:381
+#: aleksis/apps/paweljong/views.py:383
 msgid "Create e-mail address"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:383
+#: aleksis/apps/paweljong/views.py:385
 msgid "All participants need a personal e-mail address, which they check and read temselves. We offer the possibility to register an e-mail address on our secure servers, made for young users. For information about receiving mails, see: <a href='https://leopard.institute/pages/services.html'>https://leopard.institute/pages/services.html</a>."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:392
+#: aleksis/apps/paweljong/views.py:394
 msgid "First, please enter some basic information about yourself, and check whether all information is correct."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:396
+#: aleksis/apps/paweljong/views.py:398
 msgid "Contact information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:398
+#: aleksis/apps/paweljong/views.py:400
 msgid "Tell us how we can contact you. You will receive information about the event by e-mail. Please use your personal e-mail address where you will read mails yourself, not an address of your parents. We will always send all important information to your parents as well, and you will enter their e-mail address on the next page."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:405
+#: aleksis/apps/paweljong/views.py:407
 msgid "Legal guardians / parents"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:407
+#: aleksis/apps/paweljong/views.py:409
 msgid "Tell us how we can reach your parents or other legal guardians. This should be the person who was present when you registered for the event (which is now). If you want to add another parent, please tell us later as a comment."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:413
+#: aleksis/apps/paweljong/views.py:415
 msgid "Additional registration information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:415
+#: aleksis/apps/paweljong/views.py:417
 msgid "Please answer the following questions as precisely as you can, so we can make sure your event attendance will be organised as wel las possible."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:421
+#: aleksis/apps/paweljong/views.py:423
 msgid "Please decide with your parents how you want to pay. In this step, you only select a payment method. The real payment will be done in a separate step, after the registration is complete."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:426
+#: aleksis/apps/paweljong/views.py:428
 msgid "Consent"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:428
+#: aleksis/apps/paweljong/views.py:430
 msgid "Lastly, please read the terms and conditions carefully, together with your parents. After that, you will need to confirm that you agree with everything yourself, and that your parents also agree."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:526 aleksis/apps/paweljong/views.py:636
+#: aleksis/apps/paweljong/views.py:528 aleksis/apps/paweljong/views.py:638
 msgid "You entered an invalid voucher code!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:662
+#: aleksis/apps/paweljong/views.py:664
 msgid "You have successfully registered for the event. Please give us up to two days to process your registration. You will then receive an email from us."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:669
+#: aleksis/apps/paweljong/views.py:671
 msgid "You registered for an event"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:670
+#: aleksis/apps/paweljong/views.py:672
 #, python-format
 msgid "You registered for the event %s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:727 aleksis/apps/paweljong/views.py:878
+#: aleksis/apps/paweljong/views.py:729 aleksis/apps/paweljong/views.py:880
 msgid "The term has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:739 aleksis/apps/paweljong/views.py:890
+#: aleksis/apps/paweljong/views.py:741 aleksis/apps/paweljong/views.py:892
 msgid "The term has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:755
+#: aleksis/apps/paweljong/views.py:757
 msgid "Announcement feed of all upcoming events"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:796
+#: aleksis/apps/paweljong/views.py:798
 msgid "The info mailing has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:808
+#: aleksis/apps/paweljong/views.py:810
 msgid "The info mailing has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:818
+#: aleksis/apps/paweljong/views.py:820
 msgid "The info mailing has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:901
+#: aleksis/apps/paweljong/views.py:906
 msgid "Registration successfully retracted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:959
+#: aleksis/apps/paweljong/views.py:964
 #, python-brace-format
 msgid "Person {person} added successfully!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:961
+#: aleksis/apps/paweljong/views.py:966
 msgid "Person does not exist!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:987
+#: aleksis/apps/paweljong/views.py:993
+msgid "The provided username is not linked to a person."
+msgstr ""
+
+#: aleksis/apps/paweljong/views.py:1003
+msgid "{} successfully checked for {}."
+msgstr ""
+
+#: aleksis/apps/paweljong/views.py:1032
 msgid "Successfully checked in."
 msgstr ""
```

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.mo` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.po` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,35 +3,32 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-24 14:54+0000\n"
+"POT-Creation-Date: 2022-06-28 15:44+0000\n"
 "PO-Revision-Date: 2022-06-24 15:05+0000\n"
 "Last-Translator: Tom Teichler <tom.teichler@teckids.org>\n"
-"Language-Team: German <https://translate.edugit.org/projects/hacknfun/"
-"aleksis-app-paweljong/de/>\n"
+"Language-Team: German <https://translate.edugit.org/projects/hacknfun/aleksis-app-paweljong/de/>\n"
 "Language: de_DE\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.12.1\n"
 
 #: aleksis/apps/paweljong/data_checks.py:8
 msgid "Sync members"
 msgstr "Teilnehmer syncronisieren"
 
 #: aleksis/apps/paweljong/data_checks.py:19
 msgid "Ensure that all registered persons are member of the linked group"
-msgstr ""
-"Stelle sicher, dass alle registrierten Personen auch Mitglied der verlinkten "
-"Gruppe sind"
+msgstr "Stelle sicher, dass alle registrierten Personen auch Mitglied der verlinkten Gruppe sind"
 
 #: aleksis/apps/paweljong/data_checks.py:20
 msgid "Event members are out of sync with registrations!"
 msgstr "Veranstaltungsteilnehmer sind asyncron mit den Anmeldungen!"
 
 #: aleksis/apps/paweljong/filters.py:17 aleksis/apps/paweljong/filters.py:45
 msgid "Search by name"
@@ -67,17 +64,15 @@
 
 #: aleksis/apps/paweljong/forms.py:30
 msgid "Creative Commons with attribution, 4.0 or later"
 msgstr "Creative Commons mit Namensnennung 4.0 International (CC BY 4.0) oder neuer"
 
 #: aleksis/apps/paweljong/forms.py:34
 msgid "Creative Commons with attribution and distribution only under the same conditions, 4.0 or later"
-msgstr ""
-"Creative Commons mit Namensnennung und Weitergabe unter gleichen "
-"Bedingungen, 4.0 oder später"
+msgstr "Creative Commons mit Namensnennung und Weitergabe unter gleichen Bedingungen, 4.0 oder später"
 
 #: aleksis/apps/paweljong/forms.py:46 aleksis/apps/paweljong/forms.py:436
 msgid "Base data"
 msgstr "Basisdaten"
 
 #: aleksis/apps/paweljong/forms.py:50
 msgid "Date data"
@@ -349,25 +344,38 @@
 msgid "Account data"
 msgstr "Kontodaten"
 
 #: aleksis/apps/paweljong/forms.py:455
 msgid "The username must only contain lower case letters and numbers, and must begin with a letter."
 msgstr "Der Benutzername darf nur Kleinbuchstaben und Zahlen beinhalten, und muss mit einem Buchstaben beginnen."
 
-#: aleksis/apps/paweljong/forms.py:500 aleksis/apps/paweljong/models.py:228
-#: aleksis/apps/paweljong/models.py:257 aleksis/apps/paweljong/tables.py:46
+#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:524
+#: aleksis/apps/paweljong/models.py:228 aleksis/apps/paweljong/models.py:257
+#: aleksis/apps/paweljong/tables.py:46
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:61
 msgid "Person"
 msgstr "Person"
 
-#: aleksis/apps/paweljong/forms.py:502
+#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:525
 msgid "Please enter a username."
 msgstr "Bitte wähle einen Benutzernamen."
 
+#: aleksis/apps/paweljong/forms.py:518 aleksis/apps/paweljong/models.py:417
+msgid "Comment"
+msgstr ""
+
+#: aleksis/apps/paweljong/forms.py:519
+msgid "Please enter a comment describing the checkpoint (e.g. Dinner)."
+msgstr ""
+
+#: aleksis/apps/paweljong/forms.py:531
+msgid "Submit geolocation"
+msgstr ""
+
 #: aleksis/apps/paweljong/menus.py:6
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
 msgid "Register"
 msgstr "Registrieren"
 
 #: aleksis/apps/paweljong/menus.py:14
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
@@ -390,15 +398,15 @@
 
 #: aleksis/apps/paweljong/menus.py:70
 msgid "Generate participant list"
 msgstr "Teilnehmerlisten generieren"
 
 #: aleksis/apps/paweljong/menus.py:81
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
-#: aleksis/apps/paweljong/views.py:746
+#: aleksis/apps/paweljong/views.py:748
 msgid "Upcoming events"
 msgstr "Anstehende Veranstaltungen"
 
 #: aleksis/apps/paweljong/models.py:28
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:25
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:63
@@ -562,15 +570,15 @@
 msgid "Checked in"
 msgstr "Eingechecked"
 
 #: aleksis/apps/paweljong/models.py:290
 msgid "Checked in at"
 msgstr "Eingechecked am"
 
-#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:989
+#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:1034
 msgid "Person is already checked in!"
 msgstr "Person ist bereits eingechecked!"
 
 #: aleksis/apps/paweljong/models.py:334
 msgid "Participation of {} in event {}"
 msgstr "Teilnahme von {} bei Veranstaltung {}"
 
@@ -578,22 +586,52 @@
 msgid "Social Sponsoring / Extra Donation"
 msgstr "Social-Sponsoring / Spende"
 
 #: aleksis/apps/paweljong/models.py:374
 msgid "Voucher / Granted discount"
 msgstr "Rabatt"
 
-#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:390
+#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:392
 msgid "Event registration"
 msgstr "Veranstaltungsanmeldung"
 
 #: aleksis/apps/paweljong/models.py:403
 msgid "Event registrations"
 msgstr "Veranstaltungsanmeldungen"
 
+#: aleksis/apps/paweljong/models.py:412
+#, fuzzy
+#| msgid "Create event"
+msgid "Related event"
+msgstr "Veranstaltung erstellen"
+
+#: aleksis/apps/paweljong/models.py:413
+#, fuzzy
+#| msgid "Checked in"
+msgid "Checked person"
+msgstr "Eingechecked"
+
+#: aleksis/apps/paweljong/models.py:414
+#, fuzzy
+#| msgid "Checked in"
+msgid "Checked by person"
+msgstr "Eingechecked"
+
+#: aleksis/apps/paweljong/models.py:419
+msgid "Date and time of check"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:420
+msgid "Latitude of check"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:421
+msgid "Longitude of check"
+msgstr ""
+
 #: aleksis/apps/paweljong/preferences.py:10
 msgid "Paweljong"
 msgstr "Paweljong"
 
 #: aleksis/apps/paweljong/preferences.py:20
 msgid "Mail recipient for event notifications"
 msgstr "Mail-Empfänger für Veranstaltungsbenachrichtigungen"
@@ -689,60 +727,68 @@
 
 #: aleksis/apps/paweljong/templates/paweljong/account_wizard.html:32
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html:44
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html:58
 msgid "Next"
 msgstr "Weiter"
 
+#: aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html:4
+#: aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html:5
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:30
+#, fuzzy
+#| msgid "Check in"
+msgid "Checkpoint"
+msgstr "Einchecken"
+
 #: aleksis/apps/paweljong/templates/paweljong/event/create.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/create.html:5
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:20
 msgid "Create event"
 msgstr "Veranstaltung erstellen"
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:43
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:47
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:31
 msgid "Registration open until"
 msgstr "Anmeldung möglich bis"
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:48
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:52
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:36
 msgid "Participation fee (all inclusive)"
 msgstr "Teilnahmegebühr (alles inklusive)"
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:54
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:58
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:42
 msgid "of"
 msgstr "von"
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:58
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:62
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:17
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:45
 msgid "Owners"
 msgstr "Besitzer"
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:76
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:80
 msgid "Additional fields"
 msgstr "Zusätzliche Felder"
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:80
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:84
 msgid "Child groups"
 msgstr "Kind-Gruppen"
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:85
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:89
 msgid "Registrations"
 msgstr "Anmeldungen"
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:88
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:92
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:14
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:14
 msgid "Search"
 msgstr "Suche"
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:92
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:96
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:18
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:18
 msgid "Clear"
 msgstr "Leeren"
 
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:5
@@ -993,15 +1039,15 @@
 msgstr "Rechnungsinformationen"
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:246
 msgid "Billing information"
 msgstr "Zahlungsinformationen"
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:278
-#: aleksis/apps/paweljong/views.py:419
+#: aleksis/apps/paweljong/views.py:421
 msgid "Payment"
 msgstr "Bezahlung"
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:316
 msgid "Guardians / Parents "
 msgstr "Erziehungsberechtigte / Eltern "
 
@@ -1250,149 +1296,159 @@
 msgstr "Zusätzliches"
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:54
 #, python-format
 msgid "New registration: %(registration)s"
 msgstr "Neue Anmeldung: %(registration)s"
 
-#: aleksis/apps/paweljong/views.py:66 aleksis/apps/paweljong/views.py:78
+#: aleksis/apps/paweljong/views.py:68 aleksis/apps/paweljong/views.py:80
 msgid "The event has been saved."
 msgstr "Die Veranstaltung wurde gespeichert."
 
-#: aleksis/apps/paweljong/views.py:150
+#: aleksis/apps/paweljong/views.py:152
 msgid "The event registration has been created."
 msgstr "Die Veranstaltungsanmeldung wurde erstellt."
 
-#: aleksis/apps/paweljong/views.py:162
+#: aleksis/apps/paweljong/views.py:164
 msgid "The event registration has been saved."
 msgstr "Die Veranstaltungsanmeldung wurde gespeichert."
 
-#: aleksis/apps/paweljong/views.py:183
+#: aleksis/apps/paweljong/views.py:185
 msgid "The registration has been saved."
 msgstr "Die Anmeldung wurde gespeichert."
 
-#: aleksis/apps/paweljong/views.py:228
+#: aleksis/apps/paweljong/views.py:230
 msgid "The registration has been deleted."
 msgstr "Die Veranstaltung wurde gelöscht."
 
-#: aleksis/apps/paweljong/views.py:240
+#: aleksis/apps/paweljong/views.py:242
 msgid "The voucher has been created."
 msgstr "Der Gutschein wurde erstellt."
 
-#: aleksis/apps/paweljong/views.py:252
+#: aleksis/apps/paweljong/views.py:254
 msgid "The voucher has been saved."
 msgstr "Der Gutschein wurde gespeichert."
 
-#: aleksis/apps/paweljong/views.py:262
+#: aleksis/apps/paweljong/views.py:264
 msgid "The voucher has been deleted."
 msgstr "Der Gutschein wurde gelöscht."
 
-#: aleksis/apps/paweljong/views.py:381
+#: aleksis/apps/paweljong/views.py:383
 msgid "Create e-mail address"
 msgstr "E-Mail-Adresse erstellen"
 
-#: aleksis/apps/paweljong/views.py:383
+#: aleksis/apps/paweljong/views.py:385
 msgid "All participants need a personal e-mail address, which they check and read temselves. We offer the possibility to register an e-mail address on our secure servers, made for young users. For information about receiving mails, see: <a href='https://leopard.institute/pages/services.html'>https://leopard.institute/pages/services.html</a>."
 msgstr "Alle Teilnehmenden brauchen eine persönliche Adresse, die sie selbst abrufen und lesen. Wir bieten die Möglichkeit an, E-Mail-Adressen auf unseren sicheren Servern zu registrieren. Informationen, wie Du deine Mails abrufen kannst, findest Du unter <a href='https://leopard.institute/pages/services.html'>https://leopard.institute/pages/services.html</a>."
 
-#: aleksis/apps/paweljong/views.py:392
+#: aleksis/apps/paweljong/views.py:394
 msgid "First, please enter some basic information about yourself, and check whether all information is correct."
 msgstr "Zuerst, gib bitte einige Informationen über dich an und prüfe, dass alle Informationen korrekt sind."
 
-#: aleksis/apps/paweljong/views.py:396
+#: aleksis/apps/paweljong/views.py:398
 msgid "Contact information"
 msgstr "Kontaktinformationen"
 
-#: aleksis/apps/paweljong/views.py:398
+#: aleksis/apps/paweljong/views.py:400
 msgid "Tell us how we can contact you. You will receive information about the event by e-mail. Please use your personal e-mail address where you will read mails yourself, not an address of your parents. We will always send all important information to your parents as well, and you will enter their e-mail address on the next page."
 msgstr "Teile uns mit, wie wir dich erreichen können. Du wirst Informationen zu der Veranstaltung per E-Mail erhalten. Bitte nutze deine persönliche E-Mail-Adresse, die selbst liest, nicht die E-Mail-Adresse deiner Eltern. Wir senden wichtige Informationen immer zusätzlich an deine Eltern. Ihre E-Mail-Adresse wirst du im nächsten Schritt eingeben."
 
-#: aleksis/apps/paweljong/views.py:405
+#: aleksis/apps/paweljong/views.py:407
 msgid "Legal guardians / parents"
 msgstr "Erziehungsberechtigte / Eltern"
 
-#: aleksis/apps/paweljong/views.py:407
+#: aleksis/apps/paweljong/views.py:409
 msgid "Tell us how we can reach your parents or other legal guardians. This should be the person who was present when you registered for the event (which is now). If you want to add another parent, please tell us later as a comment."
 msgstr "Teile uns mit, wie wir deine Eltern oder Erziehungsberechtigten während der Veranstaltung erreichen können. Das sollte eine Person sein, die während der Anmeldung (also jetzt gerade), bei Dir ist. Wenn du einen weiteren Erziehungsberechtigten angeben möchtest, kannst du uns das später als Kommentar mitteilen."
 
-#: aleksis/apps/paweljong/views.py:413
+#: aleksis/apps/paweljong/views.py:415
 msgid "Additional registration information"
 msgstr "Zusätzliche Anmeldungsinformationen"
 
-#: aleksis/apps/paweljong/views.py:415
+#: aleksis/apps/paweljong/views.py:417
 msgid "Please answer the following questions as precisely as you can, so we can make sure your event attendance will be organised as wel las possible."
 msgstr "Bitte beantworte die folgenden Fragen so genau wie möglich, sodass wir sicher gehen können, dass deine Teilnahme bei der Veranstaltung so gut wie möglich organisiert ist."
 
-#: aleksis/apps/paweljong/views.py:421
+#: aleksis/apps/paweljong/views.py:423
 msgid "Please decide with your parents how you want to pay. In this step, you only select a payment method. The real payment will be done in a separate step, after the registration is complete."
 msgstr "Bitte wählen mit Deinen Eltern, wie Du bezahlen möchtest. In diesem Schritt wird nur die Zahlungsmethode ausgewählt. Die eigentliche Zahlung wird in einem separaten Schritt nach der Anmeldung durchgeführt."
 
-#: aleksis/apps/paweljong/views.py:426
+#: aleksis/apps/paweljong/views.py:428
 msgid "Consent"
 msgstr "Einverständnis"
 
-#: aleksis/apps/paweljong/views.py:428
+#: aleksis/apps/paweljong/views.py:430
 msgid "Lastly, please read the terms and conditions carefully, together with your parents. After that, you will need to confirm that you agree with everything yourself, and that your parents also agree."
 msgstr "Zuletzt lies bitte alle Bedingungen sorgfältig zusammen mit deinen Eltern durch. Danach musst du bestätigen, dass du und deine Eltern alles gelesen habt und akzeptiert."
 
-#: aleksis/apps/paweljong/views.py:526 aleksis/apps/paweljong/views.py:636
+#: aleksis/apps/paweljong/views.py:528 aleksis/apps/paweljong/views.py:638
 msgid "You entered an invalid voucher code!"
 msgstr "Du hast einen ungütigen Gutscheincode eingegeben!"
 
-#: aleksis/apps/paweljong/views.py:662
+#: aleksis/apps/paweljong/views.py:664
 msgid "You have successfully registered for the event. Please give us up to two days to process your registration. You will then receive an email from us."
 msgstr "Du hast dich erfolgreich zu der Veranstaltung angemeldet. Bitte gib uns ein paar Tage, um deine Anmeldung zu bearbeiten. Du wirst dann eine E-Mail von uns bekommen."
 
-#: aleksis/apps/paweljong/views.py:669
+#: aleksis/apps/paweljong/views.py:671
 msgid "You registered for an event"
 msgstr "Du hast dich zu einer Veranstaltung angemeldet"
 
-#: aleksis/apps/paweljong/views.py:670
+#: aleksis/apps/paweljong/views.py:672
 #, python-format
 msgid "You registered for the event %s"
 msgstr "Du hast dich zur Veranstaltung %s angemeldet"
 
-#: aleksis/apps/paweljong/views.py:727 aleksis/apps/paweljong/views.py:878
+#: aleksis/apps/paweljong/views.py:729 aleksis/apps/paweljong/views.py:880
 msgid "The term has been created."
 msgstr "Die Bedingung wurde erfolgreich erstellt."
 
-#: aleksis/apps/paweljong/views.py:739 aleksis/apps/paweljong/views.py:890
+#: aleksis/apps/paweljong/views.py:741 aleksis/apps/paweljong/views.py:892
 msgid "The term has been saved."
 msgstr "Die Bedingung wurde gespeichert."
 
-#: aleksis/apps/paweljong/views.py:755
+#: aleksis/apps/paweljong/views.py:757
 msgid "Announcement feed of all upcoming events"
 msgstr "Ankündigungs-Feed aller bevorstehenden Veranstaltungen"
 
-#: aleksis/apps/paweljong/views.py:796
+#: aleksis/apps/paweljong/views.py:798
 msgid "The info mailing has been created."
 msgstr "Das Info-Mailing wurde erstellt."
 
-#: aleksis/apps/paweljong/views.py:808
+#: aleksis/apps/paweljong/views.py:810
 msgid "The info mailing has been saved."
 msgstr "Das Info-Mailing wurde gespeichert."
 
-#: aleksis/apps/paweljong/views.py:818
+#: aleksis/apps/paweljong/views.py:820
 msgid "The info mailing has been deleted."
 msgstr "Das Info-Mailing wurde gelöscht."
 
-#: aleksis/apps/paweljong/views.py:901
+#: aleksis/apps/paweljong/views.py:906
 msgid "Registration successfully retracted."
 msgstr "Anmeldung erfolgreich storniert."
 
-#: aleksis/apps/paweljong/views.py:959
+#: aleksis/apps/paweljong/views.py:964
 #, python-brace-format
 msgid "Person {person} added successfully!"
 msgstr "Person {person} erfolgreich hinzugefügt!"
 
-#: aleksis/apps/paweljong/views.py:961
+#: aleksis/apps/paweljong/views.py:966
 msgid "Person does not exist!"
 msgstr "Person existiert nicht!"
 
-#: aleksis/apps/paweljong/views.py:987
+#: aleksis/apps/paweljong/views.py:993
+msgid "The provided username is not linked to a person."
+msgstr ""
+
+#: aleksis/apps/paweljong/views.py:1003
+#, fuzzy
+#| msgid "Successfully checked in."
+msgid "{} successfully checked for {}."
+msgstr "Erfolgreich eingechecked."
+
+#: aleksis/apps/paweljong/views.py:1032
 msgid "Successfully checked in."
 msgstr "Erfolgreich eingechecked."
 
 #~ msgid "Filter registrations"
 #~ msgstr "Anmeldungen filtern"
 
 #~ msgid "Selected registrations"
```

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.po` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-24 14:54+0000\n"
+"POT-Creation-Date: 2022-06-28 15:44+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: aleksis/apps/paweljong/data_checks.py:8
 msgid "Sync members"
 msgstr ""
 
 #: aleksis/apps/paweljong/data_checks.py:19
 msgid "Ensure that all registered persons are member of the linked group"
@@ -344,25 +343,38 @@
 msgid "Account data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:455
 msgid "The username must only contain lower case letters and numbers, and must begin with a letter."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:500 aleksis/apps/paweljong/models.py:228
-#: aleksis/apps/paweljong/models.py:257 aleksis/apps/paweljong/tables.py:46
+#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:524
+#: aleksis/apps/paweljong/models.py:228 aleksis/apps/paweljong/models.py:257
+#: aleksis/apps/paweljong/tables.py:46
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:61
 msgid "Person"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:502
+#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:525
 msgid "Please enter a username."
 msgstr ""
 
+#: aleksis/apps/paweljong/forms.py:518 aleksis/apps/paweljong/models.py:417
+msgid "Comment"
+msgstr ""
+
+#: aleksis/apps/paweljong/forms.py:519
+msgid "Please enter a comment describing the checkpoint (e.g. Dinner)."
+msgstr ""
+
+#: aleksis/apps/paweljong/forms.py:531
+msgid "Submit geolocation"
+msgstr ""
+
 #: aleksis/apps/paweljong/menus.py:6
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
 msgid "Register"
 msgstr ""
 
 #: aleksis/apps/paweljong/menus.py:14
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
@@ -385,15 +397,15 @@
 
 #: aleksis/apps/paweljong/menus.py:70
 msgid "Generate participant list"
 msgstr ""
 
 #: aleksis/apps/paweljong/menus.py:81
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
-#: aleksis/apps/paweljong/views.py:746
+#: aleksis/apps/paweljong/views.py:748
 msgid "Upcoming events"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:28
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:25
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:63
@@ -557,15 +569,15 @@
 msgid "Checked in"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:290
 msgid "Checked in at"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:989
+#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:1034
 msgid "Person is already checked in!"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:334
 msgid "Participation of {} in event {}"
 msgstr ""
 
@@ -573,22 +585,46 @@
 msgid "Social Sponsoring / Extra Donation"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:374
 msgid "Voucher / Granted discount"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:390
+#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:392
 msgid "Event registration"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:403
 msgid "Event registrations"
 msgstr ""
 
+#: aleksis/apps/paweljong/models.py:412
+msgid "Related event"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:413
+msgid "Checked person"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:414
+msgid "Checked by person"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:419
+msgid "Date and time of check"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:420
+msgid "Latitude of check"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:421
+msgid "Longitude of check"
+msgstr ""
+
 #: aleksis/apps/paweljong/preferences.py:10
 msgid "Paweljong"
 msgstr ""
 
 #: aleksis/apps/paweljong/preferences.py:20
 msgid "Mail recipient for event notifications"
 msgstr ""
@@ -684,60 +720,66 @@
 
 #: aleksis/apps/paweljong/templates/paweljong/account_wizard.html:32
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html:44
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html:58
 msgid "Next"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html:4
+#: aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html:5
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:30
+msgid "Checkpoint"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/event/create.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/create.html:5
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:20
 msgid "Create event"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:43
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:47
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:31
 msgid "Registration open until"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:48
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:52
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:36
 msgid "Participation fee (all inclusive)"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:54
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:58
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:42
 msgid "of"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:58
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:62
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:17
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:45
 msgid "Owners"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:76
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:80
 msgid "Additional fields"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:80
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:84
 msgid "Child groups"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:85
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:89
 msgid "Registrations"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:88
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:92
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:14
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:14
 msgid "Search"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:92
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:96
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:18
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:18
 msgid "Clear"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:5
@@ -945,15 +987,15 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:246
 msgid "Billing information"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:278
-#: aleksis/apps/paweljong/views.py:419
+#: aleksis/apps/paweljong/views.py:421
 msgid "Payment"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:316
 msgid "Guardians / Parents "
 msgstr ""
 
@@ -1184,144 +1226,152 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:54
 #, python-format
 msgid "New registration: %(registration)s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:66 aleksis/apps/paweljong/views.py:78
+#: aleksis/apps/paweljong/views.py:68 aleksis/apps/paweljong/views.py:80
 msgid "The event has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:150
+#: aleksis/apps/paweljong/views.py:152
 msgid "The event registration has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:162
+#: aleksis/apps/paweljong/views.py:164
 msgid "The event registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:183
+#: aleksis/apps/paweljong/views.py:185
 msgid "The registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:228
+#: aleksis/apps/paweljong/views.py:230
 msgid "The registration has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:240
+#: aleksis/apps/paweljong/views.py:242
 msgid "The voucher has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:252
+#: aleksis/apps/paweljong/views.py:254
 msgid "The voucher has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:262
+#: aleksis/apps/paweljong/views.py:264
 msgid "The voucher has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:381
+#: aleksis/apps/paweljong/views.py:383
 msgid "Create e-mail address"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:383
+#: aleksis/apps/paweljong/views.py:385
 msgid "All participants need a personal e-mail address, which they check and read temselves. We offer the possibility to register an e-mail address on our secure servers, made for young users. For information about receiving mails, see: <a href='https://leopard.institute/pages/services.html'>https://leopard.institute/pages/services.html</a>."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:392
+#: aleksis/apps/paweljong/views.py:394
 msgid "First, please enter some basic information about yourself, and check whether all information is correct."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:396
+#: aleksis/apps/paweljong/views.py:398
 msgid "Contact information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:398
+#: aleksis/apps/paweljong/views.py:400
 msgid "Tell us how we can contact you. You will receive information about the event by e-mail. Please use your personal e-mail address where you will read mails yourself, not an address of your parents. We will always send all important information to your parents as well, and you will enter their e-mail address on the next page."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:405
+#: aleksis/apps/paweljong/views.py:407
 msgid "Legal guardians / parents"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:407
+#: aleksis/apps/paweljong/views.py:409
 msgid "Tell us how we can reach your parents or other legal guardians. This should be the person who was present when you registered for the event (which is now). If you want to add another parent, please tell us later as a comment."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:413
+#: aleksis/apps/paweljong/views.py:415
 msgid "Additional registration information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:415
+#: aleksis/apps/paweljong/views.py:417
 msgid "Please answer the following questions as precisely as you can, so we can make sure your event attendance will be organised as wel las possible."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:421
+#: aleksis/apps/paweljong/views.py:423
 msgid "Please decide with your parents how you want to pay. In this step, you only select a payment method. The real payment will be done in a separate step, after the registration is complete."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:426
+#: aleksis/apps/paweljong/views.py:428
 msgid "Consent"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:428
+#: aleksis/apps/paweljong/views.py:430
 msgid "Lastly, please read the terms and conditions carefully, together with your parents. After that, you will need to confirm that you agree with everything yourself, and that your parents also agree."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:526 aleksis/apps/paweljong/views.py:636
+#: aleksis/apps/paweljong/views.py:528 aleksis/apps/paweljong/views.py:638
 msgid "You entered an invalid voucher code!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:662
+#: aleksis/apps/paweljong/views.py:664
 msgid "You have successfully registered for the event. Please give us up to two days to process your registration. You will then receive an email from us."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:669
+#: aleksis/apps/paweljong/views.py:671
 msgid "You registered for an event"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:670
+#: aleksis/apps/paweljong/views.py:672
 #, python-format
 msgid "You registered for the event %s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:727 aleksis/apps/paweljong/views.py:878
+#: aleksis/apps/paweljong/views.py:729 aleksis/apps/paweljong/views.py:880
 msgid "The term has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:739 aleksis/apps/paweljong/views.py:890
+#: aleksis/apps/paweljong/views.py:741 aleksis/apps/paweljong/views.py:892
 msgid "The term has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:755
+#: aleksis/apps/paweljong/views.py:757
 msgid "Announcement feed of all upcoming events"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:796
+#: aleksis/apps/paweljong/views.py:798
 msgid "The info mailing has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:808
+#: aleksis/apps/paweljong/views.py:810
 msgid "The info mailing has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:818
+#: aleksis/apps/paweljong/views.py:820
 msgid "The info mailing has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:901
+#: aleksis/apps/paweljong/views.py:906
 msgid "Registration successfully retracted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:959
+#: aleksis/apps/paweljong/views.py:964
 #, python-brace-format
 msgid "Person {person} added successfully!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:961
+#: aleksis/apps/paweljong/views.py:966
 msgid "Person does not exist!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:987
+#: aleksis/apps/paweljong/views.py:993
+msgid "The provided username is not linked to a person."
+msgstr ""
+
+#: aleksis/apps/paweljong/views.py:1003
+msgid "{} successfully checked for {}."
+msgstr ""
+
+#: aleksis/apps/paweljong/views.py:1032
 msgid "Successfully checked in."
 msgstr ""
```

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.po` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-24 14:54+0000\n"
+"POT-Creation-Date: 2022-06-28 15:44+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -343,25 +343,38 @@
 msgid "Account data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:455
 msgid "The username must only contain lower case letters and numbers, and must begin with a letter."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:500 aleksis/apps/paweljong/models.py:228
-#: aleksis/apps/paweljong/models.py:257 aleksis/apps/paweljong/tables.py:46
+#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:524
+#: aleksis/apps/paweljong/models.py:228 aleksis/apps/paweljong/models.py:257
+#: aleksis/apps/paweljong/tables.py:46
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:61
 msgid "Person"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:502
+#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:525
 msgid "Please enter a username."
 msgstr ""
 
+#: aleksis/apps/paweljong/forms.py:518 aleksis/apps/paweljong/models.py:417
+msgid "Comment"
+msgstr ""
+
+#: aleksis/apps/paweljong/forms.py:519
+msgid "Please enter a comment describing the checkpoint (e.g. Dinner)."
+msgstr ""
+
+#: aleksis/apps/paweljong/forms.py:531
+msgid "Submit geolocation"
+msgstr ""
+
 #: aleksis/apps/paweljong/menus.py:6
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
 msgid "Register"
 msgstr ""
 
 #: aleksis/apps/paweljong/menus.py:14
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
@@ -384,15 +397,15 @@
 
 #: aleksis/apps/paweljong/menus.py:70
 msgid "Generate participant list"
 msgstr ""
 
 #: aleksis/apps/paweljong/menus.py:81
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
-#: aleksis/apps/paweljong/views.py:746
+#: aleksis/apps/paweljong/views.py:748
 msgid "Upcoming events"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:28
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:25
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:63
@@ -556,15 +569,15 @@
 msgid "Checked in"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:290
 msgid "Checked in at"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:989
+#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:1034
 msgid "Person is already checked in!"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:334
 msgid "Participation of {} in event {}"
 msgstr ""
 
@@ -572,22 +585,46 @@
 msgid "Social Sponsoring / Extra Donation"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:374
 msgid "Voucher / Granted discount"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:390
+#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:392
 msgid "Event registration"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:403
 msgid "Event registrations"
 msgstr ""
 
+#: aleksis/apps/paweljong/models.py:412
+msgid "Related event"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:413
+msgid "Checked person"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:414
+msgid "Checked by person"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:419
+msgid "Date and time of check"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:420
+msgid "Latitude of check"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:421
+msgid "Longitude of check"
+msgstr ""
+
 #: aleksis/apps/paweljong/preferences.py:10
 msgid "Paweljong"
 msgstr ""
 
 #: aleksis/apps/paweljong/preferences.py:20
 msgid "Mail recipient for event notifications"
 msgstr ""
@@ -683,60 +720,66 @@
 
 #: aleksis/apps/paweljong/templates/paweljong/account_wizard.html:32
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html:44
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html:58
 msgid "Next"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html:4
+#: aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html:5
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:30
+msgid "Checkpoint"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/event/create.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/create.html:5
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:20
 msgid "Create event"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:43
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:47
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:31
 msgid "Registration open until"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:48
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:52
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:36
 msgid "Participation fee (all inclusive)"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:54
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:58
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:42
 msgid "of"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:58
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:62
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:17
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:45
 msgid "Owners"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:76
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:80
 msgid "Additional fields"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:80
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:84
 msgid "Child groups"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:85
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:89
 msgid "Registrations"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:88
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:92
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:14
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:14
 msgid "Search"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:92
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:96
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:18
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:18
 msgid "Clear"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:5
@@ -944,15 +987,15 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:246
 msgid "Billing information"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:278
-#: aleksis/apps/paweljong/views.py:419
+#: aleksis/apps/paweljong/views.py:421
 msgid "Payment"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:316
 msgid "Guardians / Parents "
 msgstr ""
 
@@ -1183,144 +1226,152 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:54
 #, python-format
 msgid "New registration: %(registration)s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:66 aleksis/apps/paweljong/views.py:78
+#: aleksis/apps/paweljong/views.py:68 aleksis/apps/paweljong/views.py:80
 msgid "The event has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:150
+#: aleksis/apps/paweljong/views.py:152
 msgid "The event registration has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:162
+#: aleksis/apps/paweljong/views.py:164
 msgid "The event registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:183
+#: aleksis/apps/paweljong/views.py:185
 msgid "The registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:228
+#: aleksis/apps/paweljong/views.py:230
 msgid "The registration has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:240
+#: aleksis/apps/paweljong/views.py:242
 msgid "The voucher has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:252
+#: aleksis/apps/paweljong/views.py:254
 msgid "The voucher has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:262
+#: aleksis/apps/paweljong/views.py:264
 msgid "The voucher has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:381
+#: aleksis/apps/paweljong/views.py:383
 msgid "Create e-mail address"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:383
+#: aleksis/apps/paweljong/views.py:385
 msgid "All participants need a personal e-mail address, which they check and read temselves. We offer the possibility to register an e-mail address on our secure servers, made for young users. For information about receiving mails, see: <a href='https://leopard.institute/pages/services.html'>https://leopard.institute/pages/services.html</a>."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:392
+#: aleksis/apps/paweljong/views.py:394
 msgid "First, please enter some basic information about yourself, and check whether all information is correct."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:396
+#: aleksis/apps/paweljong/views.py:398
 msgid "Contact information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:398
+#: aleksis/apps/paweljong/views.py:400
 msgid "Tell us how we can contact you. You will receive information about the event by e-mail. Please use your personal e-mail address where you will read mails yourself, not an address of your parents. We will always send all important information to your parents as well, and you will enter their e-mail address on the next page."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:405
+#: aleksis/apps/paweljong/views.py:407
 msgid "Legal guardians / parents"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:407
+#: aleksis/apps/paweljong/views.py:409
 msgid "Tell us how we can reach your parents or other legal guardians. This should be the person who was present when you registered for the event (which is now). If you want to add another parent, please tell us later as a comment."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:413
+#: aleksis/apps/paweljong/views.py:415
 msgid "Additional registration information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:415
+#: aleksis/apps/paweljong/views.py:417
 msgid "Please answer the following questions as precisely as you can, so we can make sure your event attendance will be organised as wel las possible."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:421
+#: aleksis/apps/paweljong/views.py:423
 msgid "Please decide with your parents how you want to pay. In this step, you only select a payment method. The real payment will be done in a separate step, after the registration is complete."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:426
+#: aleksis/apps/paweljong/views.py:428
 msgid "Consent"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:428
+#: aleksis/apps/paweljong/views.py:430
 msgid "Lastly, please read the terms and conditions carefully, together with your parents. After that, you will need to confirm that you agree with everything yourself, and that your parents also agree."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:526 aleksis/apps/paweljong/views.py:636
+#: aleksis/apps/paweljong/views.py:528 aleksis/apps/paweljong/views.py:638
 msgid "You entered an invalid voucher code!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:662
+#: aleksis/apps/paweljong/views.py:664
 msgid "You have successfully registered for the event. Please give us up to two days to process your registration. You will then receive an email from us."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:669
+#: aleksis/apps/paweljong/views.py:671
 msgid "You registered for an event"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:670
+#: aleksis/apps/paweljong/views.py:672
 #, python-format
 msgid "You registered for the event %s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:727 aleksis/apps/paweljong/views.py:878
+#: aleksis/apps/paweljong/views.py:729 aleksis/apps/paweljong/views.py:880
 msgid "The term has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:739 aleksis/apps/paweljong/views.py:890
+#: aleksis/apps/paweljong/views.py:741 aleksis/apps/paweljong/views.py:892
 msgid "The term has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:755
+#: aleksis/apps/paweljong/views.py:757
 msgid "Announcement feed of all upcoming events"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:796
+#: aleksis/apps/paweljong/views.py:798
 msgid "The info mailing has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:808
+#: aleksis/apps/paweljong/views.py:810
 msgid "The info mailing has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:818
+#: aleksis/apps/paweljong/views.py:820
 msgid "The info mailing has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:901
+#: aleksis/apps/paweljong/views.py:906
 msgid "Registration successfully retracted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:959
+#: aleksis/apps/paweljong/views.py:964
 #, python-brace-format
 msgid "Person {person} added successfully!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:961
+#: aleksis/apps/paweljong/views.py:966
 msgid "Person does not exist!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:987
+#: aleksis/apps/paweljong/views.py:993
+msgid "The provided username is not linked to a person."
+msgstr ""
+
+#: aleksis/apps/paweljong/views.py:1003
+msgid "{} successfully checked for {}."
+msgstr ""
+
+#: aleksis/apps/paweljong/views.py:1032
 msgid "Successfully checked in."
 msgstr ""
```

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.po` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-24 14:54+0000\n"
+"POT-Creation-Date: 2022-06-28 15:44+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -343,25 +343,38 @@
 msgid "Account data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:455
 msgid "The username must only contain lower case letters and numbers, and must begin with a letter."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:500 aleksis/apps/paweljong/models.py:228
-#: aleksis/apps/paweljong/models.py:257 aleksis/apps/paweljong/tables.py:46
+#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:524
+#: aleksis/apps/paweljong/models.py:228 aleksis/apps/paweljong/models.py:257
+#: aleksis/apps/paweljong/tables.py:46
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:61
 msgid "Person"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:502
+#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:525
 msgid "Please enter a username."
 msgstr ""
 
+#: aleksis/apps/paweljong/forms.py:518 aleksis/apps/paweljong/models.py:417
+msgid "Comment"
+msgstr ""
+
+#: aleksis/apps/paweljong/forms.py:519
+msgid "Please enter a comment describing the checkpoint (e.g. Dinner)."
+msgstr ""
+
+#: aleksis/apps/paweljong/forms.py:531
+msgid "Submit geolocation"
+msgstr ""
+
 #: aleksis/apps/paweljong/menus.py:6
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
 msgid "Register"
 msgstr ""
 
 #: aleksis/apps/paweljong/menus.py:14
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
@@ -384,15 +397,15 @@
 
 #: aleksis/apps/paweljong/menus.py:70
 msgid "Generate participant list"
 msgstr ""
 
 #: aleksis/apps/paweljong/menus.py:81
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
-#: aleksis/apps/paweljong/views.py:746
+#: aleksis/apps/paweljong/views.py:748
 msgid "Upcoming events"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:28
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:25
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:63
@@ -556,15 +569,15 @@
 msgid "Checked in"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:290
 msgid "Checked in at"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:989
+#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:1034
 msgid "Person is already checked in!"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:334
 msgid "Participation of {} in event {}"
 msgstr ""
 
@@ -572,22 +585,46 @@
 msgid "Social Sponsoring / Extra Donation"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:374
 msgid "Voucher / Granted discount"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:390
+#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:392
 msgid "Event registration"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:403
 msgid "Event registrations"
 msgstr ""
 
+#: aleksis/apps/paweljong/models.py:412
+msgid "Related event"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:413
+msgid "Checked person"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:414
+msgid "Checked by person"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:419
+msgid "Date and time of check"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:420
+msgid "Latitude of check"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:421
+msgid "Longitude of check"
+msgstr ""
+
 #: aleksis/apps/paweljong/preferences.py:10
 msgid "Paweljong"
 msgstr ""
 
 #: aleksis/apps/paweljong/preferences.py:20
 msgid "Mail recipient for event notifications"
 msgstr ""
@@ -683,60 +720,66 @@
 
 #: aleksis/apps/paweljong/templates/paweljong/account_wizard.html:32
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html:44
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html:58
 msgid "Next"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html:4
+#: aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html:5
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:30
+msgid "Checkpoint"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/event/create.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/create.html:5
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:20
 msgid "Create event"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:43
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:47
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:31
 msgid "Registration open until"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:48
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:52
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:36
 msgid "Participation fee (all inclusive)"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:54
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:58
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:42
 msgid "of"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:58
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:62
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:17
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:45
 msgid "Owners"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:76
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:80
 msgid "Additional fields"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:80
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:84
 msgid "Child groups"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:85
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:89
 msgid "Registrations"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:88
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:92
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:14
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:14
 msgid "Search"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:92
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:96
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:18
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:18
 msgid "Clear"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:5
@@ -944,15 +987,15 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:246
 msgid "Billing information"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:278
-#: aleksis/apps/paweljong/views.py:419
+#: aleksis/apps/paweljong/views.py:421
 msgid "Payment"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:316
 msgid "Guardians / Parents "
 msgstr ""
 
@@ -1183,144 +1226,152 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:54
 #, python-format
 msgid "New registration: %(registration)s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:66 aleksis/apps/paweljong/views.py:78
+#: aleksis/apps/paweljong/views.py:68 aleksis/apps/paweljong/views.py:80
 msgid "The event has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:150
+#: aleksis/apps/paweljong/views.py:152
 msgid "The event registration has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:162
+#: aleksis/apps/paweljong/views.py:164
 msgid "The event registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:183
+#: aleksis/apps/paweljong/views.py:185
 msgid "The registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:228
+#: aleksis/apps/paweljong/views.py:230
 msgid "The registration has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:240
+#: aleksis/apps/paweljong/views.py:242
 msgid "The voucher has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:252
+#: aleksis/apps/paweljong/views.py:254
 msgid "The voucher has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:262
+#: aleksis/apps/paweljong/views.py:264
 msgid "The voucher has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:381
+#: aleksis/apps/paweljong/views.py:383
 msgid "Create e-mail address"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:383
+#: aleksis/apps/paweljong/views.py:385
 msgid "All participants need a personal e-mail address, which they check and read temselves. We offer the possibility to register an e-mail address on our secure servers, made for young users. For information about receiving mails, see: <a href='https://leopard.institute/pages/services.html'>https://leopard.institute/pages/services.html</a>."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:392
+#: aleksis/apps/paweljong/views.py:394
 msgid "First, please enter some basic information about yourself, and check whether all information is correct."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:396
+#: aleksis/apps/paweljong/views.py:398
 msgid "Contact information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:398
+#: aleksis/apps/paweljong/views.py:400
 msgid "Tell us how we can contact you. You will receive information about the event by e-mail. Please use your personal e-mail address where you will read mails yourself, not an address of your parents. We will always send all important information to your parents as well, and you will enter their e-mail address on the next page."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:405
+#: aleksis/apps/paweljong/views.py:407
 msgid "Legal guardians / parents"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:407
+#: aleksis/apps/paweljong/views.py:409
 msgid "Tell us how we can reach your parents or other legal guardians. This should be the person who was present when you registered for the event (which is now). If you want to add another parent, please tell us later as a comment."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:413
+#: aleksis/apps/paweljong/views.py:415
 msgid "Additional registration information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:415
+#: aleksis/apps/paweljong/views.py:417
 msgid "Please answer the following questions as precisely as you can, so we can make sure your event attendance will be organised as wel las possible."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:421
+#: aleksis/apps/paweljong/views.py:423
 msgid "Please decide with your parents how you want to pay. In this step, you only select a payment method. The real payment will be done in a separate step, after the registration is complete."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:426
+#: aleksis/apps/paweljong/views.py:428
 msgid "Consent"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:428
+#: aleksis/apps/paweljong/views.py:430
 msgid "Lastly, please read the terms and conditions carefully, together with your parents. After that, you will need to confirm that you agree with everything yourself, and that your parents also agree."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:526 aleksis/apps/paweljong/views.py:636
+#: aleksis/apps/paweljong/views.py:528 aleksis/apps/paweljong/views.py:638
 msgid "You entered an invalid voucher code!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:662
+#: aleksis/apps/paweljong/views.py:664
 msgid "You have successfully registered for the event. Please give us up to two days to process your registration. You will then receive an email from us."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:669
+#: aleksis/apps/paweljong/views.py:671
 msgid "You registered for an event"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:670
+#: aleksis/apps/paweljong/views.py:672
 #, python-format
 msgid "You registered for the event %s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:727 aleksis/apps/paweljong/views.py:878
+#: aleksis/apps/paweljong/views.py:729 aleksis/apps/paweljong/views.py:880
 msgid "The term has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:739 aleksis/apps/paweljong/views.py:890
+#: aleksis/apps/paweljong/views.py:741 aleksis/apps/paweljong/views.py:892
 msgid "The term has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:755
+#: aleksis/apps/paweljong/views.py:757
 msgid "Announcement feed of all upcoming events"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:796
+#: aleksis/apps/paweljong/views.py:798
 msgid "The info mailing has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:808
+#: aleksis/apps/paweljong/views.py:810
 msgid "The info mailing has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:818
+#: aleksis/apps/paweljong/views.py:820
 msgid "The info mailing has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:901
+#: aleksis/apps/paweljong/views.py:906
 msgid "Registration successfully retracted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:959
+#: aleksis/apps/paweljong/views.py:964
 #, python-brace-format
 msgid "Person {person} added successfully!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:961
+#: aleksis/apps/paweljong/views.py:966
 msgid "Person does not exist!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:987
+#: aleksis/apps/paweljong/views.py:993
+msgid "The provided username is not linked to a person."
+msgstr ""
+
+#: aleksis/apps/paweljong/views.py:1003
+msgid "{} successfully checked for {}."
+msgstr ""
+
+#: aleksis/apps/paweljong/views.py:1032
 msgid "Successfully checked in."
 msgstr ""
```

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.po` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-24 14:54+0000\n"
+"POT-Creation-Date: 2022-06-28 15:44+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
 #: aleksis/apps/paweljong/data_checks.py:8
 msgid "Sync members"
 msgstr ""
 
 #: aleksis/apps/paweljong/data_checks.py:19
 msgid "Ensure that all registered persons are member of the linked group"
@@ -343,25 +344,38 @@
 msgid "Account data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:455
 msgid "The username must only contain lower case letters and numbers, and must begin with a letter."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:500 aleksis/apps/paweljong/models.py:228
-#: aleksis/apps/paweljong/models.py:257 aleksis/apps/paweljong/tables.py:46
+#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:524
+#: aleksis/apps/paweljong/models.py:228 aleksis/apps/paweljong/models.py:257
+#: aleksis/apps/paweljong/tables.py:46
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:61
 msgid "Person"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:502
+#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:525
 msgid "Please enter a username."
 msgstr ""
 
+#: aleksis/apps/paweljong/forms.py:518 aleksis/apps/paweljong/models.py:417
+msgid "Comment"
+msgstr ""
+
+#: aleksis/apps/paweljong/forms.py:519
+msgid "Please enter a comment describing the checkpoint (e.g. Dinner)."
+msgstr ""
+
+#: aleksis/apps/paweljong/forms.py:531
+msgid "Submit geolocation"
+msgstr ""
+
 #: aleksis/apps/paweljong/menus.py:6
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
 msgid "Register"
 msgstr ""
 
 #: aleksis/apps/paweljong/menus.py:14
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
@@ -384,15 +398,15 @@
 
 #: aleksis/apps/paweljong/menus.py:70
 msgid "Generate participant list"
 msgstr ""
 
 #: aleksis/apps/paweljong/menus.py:81
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
-#: aleksis/apps/paweljong/views.py:746
+#: aleksis/apps/paweljong/views.py:748
 msgid "Upcoming events"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:28
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:25
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:63
@@ -556,15 +570,15 @@
 msgid "Checked in"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:290
 msgid "Checked in at"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:989
+#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:1034
 msgid "Person is already checked in!"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:334
 msgid "Participation of {} in event {}"
 msgstr ""
 
@@ -572,22 +586,46 @@
 msgid "Social Sponsoring / Extra Donation"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:374
 msgid "Voucher / Granted discount"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:390
+#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:392
 msgid "Event registration"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:403
 msgid "Event registrations"
 msgstr ""
 
+#: aleksis/apps/paweljong/models.py:412
+msgid "Related event"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:413
+msgid "Checked person"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:414
+msgid "Checked by person"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:419
+msgid "Date and time of check"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:420
+msgid "Latitude of check"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:421
+msgid "Longitude of check"
+msgstr ""
+
 #: aleksis/apps/paweljong/preferences.py:10
 msgid "Paweljong"
 msgstr ""
 
 #: aleksis/apps/paweljong/preferences.py:20
 msgid "Mail recipient for event notifications"
 msgstr ""
@@ -683,60 +721,66 @@
 
 #: aleksis/apps/paweljong/templates/paweljong/account_wizard.html:32
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html:44
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html:58
 msgid "Next"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html:4
+#: aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html:5
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:30
+msgid "Checkpoint"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/event/create.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/create.html:5
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:20
 msgid "Create event"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:43
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:47
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:31
 msgid "Registration open until"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:48
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:52
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:36
 msgid "Participation fee (all inclusive)"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:54
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:58
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:42
 msgid "of"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:58
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:62
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:17
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:45
 msgid "Owners"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:76
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:80
 msgid "Additional fields"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:80
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:84
 msgid "Child groups"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:85
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:89
 msgid "Registrations"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:88
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:92
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:14
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:14
 msgid "Search"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:92
+#: aleksis/apps/paweljong/templates/paweljong/event/detail.html:96
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:18
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:18
 msgid "Clear"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:5
@@ -944,15 +988,15 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:246
 msgid "Billing information"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:278
-#: aleksis/apps/paweljong/views.py:419
+#: aleksis/apps/paweljong/views.py:421
 msgid "Payment"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:316
 msgid "Guardians / Parents "
 msgstr ""
 
@@ -1183,144 +1227,152 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:54
 #, python-format
 msgid "New registration: %(registration)s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:66 aleksis/apps/paweljong/views.py:78
+#: aleksis/apps/paweljong/views.py:68 aleksis/apps/paweljong/views.py:80
 msgid "The event has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:150
+#: aleksis/apps/paweljong/views.py:152
 msgid "The event registration has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:162
+#: aleksis/apps/paweljong/views.py:164
 msgid "The event registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:183
+#: aleksis/apps/paweljong/views.py:185
 msgid "The registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:228
+#: aleksis/apps/paweljong/views.py:230
 msgid "The registration has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:240
+#: aleksis/apps/paweljong/views.py:242
 msgid "The voucher has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:252
+#: aleksis/apps/paweljong/views.py:254
 msgid "The voucher has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:262
+#: aleksis/apps/paweljong/views.py:264
 msgid "The voucher has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:381
+#: aleksis/apps/paweljong/views.py:383
 msgid "Create e-mail address"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:383
+#: aleksis/apps/paweljong/views.py:385
 msgid "All participants need a personal e-mail address, which they check and read temselves. We offer the possibility to register an e-mail address on our secure servers, made for young users. For information about receiving mails, see: <a href='https://leopard.institute/pages/services.html'>https://leopard.institute/pages/services.html</a>."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:392
+#: aleksis/apps/paweljong/views.py:394
 msgid "First, please enter some basic information about yourself, and check whether all information is correct."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:396
+#: aleksis/apps/paweljong/views.py:398
 msgid "Contact information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:398
+#: aleksis/apps/paweljong/views.py:400
 msgid "Tell us how we can contact you. You will receive information about the event by e-mail. Please use your personal e-mail address where you will read mails yourself, not an address of your parents. We will always send all important information to your parents as well, and you will enter their e-mail address on the next page."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:405
+#: aleksis/apps/paweljong/views.py:407
 msgid "Legal guardians / parents"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:407
+#: aleksis/apps/paweljong/views.py:409
 msgid "Tell us how we can reach your parents or other legal guardians. This should be the person who was present when you registered for the event (which is now). If you want to add another parent, please tell us later as a comment."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:413
+#: aleksis/apps/paweljong/views.py:415
 msgid "Additional registration information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:415
+#: aleksis/apps/paweljong/views.py:417
 msgid "Please answer the following questions as precisely as you can, so we can make sure your event attendance will be organised as wel las possible."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:421
+#: aleksis/apps/paweljong/views.py:423
 msgid "Please decide with your parents how you want to pay. In this step, you only select a payment method. The real payment will be done in a separate step, after the registration is complete."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:426
+#: aleksis/apps/paweljong/views.py:428
 msgid "Consent"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:428
+#: aleksis/apps/paweljong/views.py:430
 msgid "Lastly, please read the terms and conditions carefully, together with your parents. After that, you will need to confirm that you agree with everything yourself, and that your parents also agree."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:526 aleksis/apps/paweljong/views.py:636
+#: aleksis/apps/paweljong/views.py:528 aleksis/apps/paweljong/views.py:638
 msgid "You entered an invalid voucher code!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:662
+#: aleksis/apps/paweljong/views.py:664
 msgid "You have successfully registered for the event. Please give us up to two days to process your registration. You will then receive an email from us."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:669
+#: aleksis/apps/paweljong/views.py:671
 msgid "You registered for an event"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:670
+#: aleksis/apps/paweljong/views.py:672
 #, python-format
 msgid "You registered for the event %s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:727 aleksis/apps/paweljong/views.py:878
+#: aleksis/apps/paweljong/views.py:729 aleksis/apps/paweljong/views.py:880
 msgid "The term has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:739 aleksis/apps/paweljong/views.py:890
+#: aleksis/apps/paweljong/views.py:741 aleksis/apps/paweljong/views.py:892
 msgid "The term has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:755
+#: aleksis/apps/paweljong/views.py:757
 msgid "Announcement feed of all upcoming events"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:796
+#: aleksis/apps/paweljong/views.py:798
 msgid "The info mailing has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:808
+#: aleksis/apps/paweljong/views.py:810
 msgid "The info mailing has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:818
+#: aleksis/apps/paweljong/views.py:820
 msgid "The info mailing has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:901
+#: aleksis/apps/paweljong/views.py:906
 msgid "Registration successfully retracted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:959
+#: aleksis/apps/paweljong/views.py:964
 #, python-brace-format
 msgid "Person {person} added successfully!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:961
+#: aleksis/apps/paweljong/views.py:966
 msgid "Person does not exist!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:987
+#: aleksis/apps/paweljong/views.py:993
+msgid "The provided username is not linked to a person."
+msgstr ""
+
+#: aleksis/apps/paweljong/views.py:1003
+msgid "{} successfully checked for {}."
+msgstr ""
+
+#: aleksis/apps/paweljong/views.py:1032
 msgid "Successfully checked in."
 msgstr ""
```

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/menus.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/menus.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0001_initial.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0004_richtext_field_information.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0004_richtext_field_information.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0006_unique_constraints.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0006_unique_constraints.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0007_terms.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0007_terms.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0008_remove_terms_from_event.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0008_remove_terms_from_event.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0009_remove_feedback.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0009_remove_feedback.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0013_info_mailings.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0013_info_mailings.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0014_move_sent_to_to_through.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0014_move_sent_to_to_through.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0015_registrationstate.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0015_registrationstate.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0018_payment_with_tezor.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0018_payment_with_tezor.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0019_retractions.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0019_retractions.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/migrations/0020_check_in.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0020_check_in.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/models.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -402,7 +402,20 @@
         verbose_name = _("Event registration")
         verbose_name_plural = _("Event registrations")
         constraints = [
             models.UniqueConstraint(
                 fields=["person", "event"], name="unique_person_registration_per_event"
             )
         ]
+
+
+class Checkpoint(ExtensibleModel):
+    event = models.ForeignKey(Event, verbose_name=_("Related event"), related_name="checkpoints", on_delete=models.CASCADE)
+    person = models.ForeignKey(Person, verbose_name=_("Checked person"), related_name="event_checkpoints", on_delete=models.CASCADE)
+    checked_by = models.ForeignKey(Person, verbose_name=_("Checked by person"), related_name="event_checkpoints_created", on_delete=models.CASCADE)
+
+
+    comment = models.CharField(max_length=60, verbose_name=_("Comment"))
+
+    timestamp = models.DateTimeField(verbose_name=_("Date and time of check"), auto_now_add=True)
+    lat = models.DecimalField(max_digits=10, decimal_places=8, verbose_name=_("Latitude of check"), blank=True, null=True)
+    lon = models.DecimalField(max_digits=11, decimal_places=8, verbose_name=_("Longitude of check"), blank=True, null=True)
```

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/predicates.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/predicates.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/preferences.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/preferences.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/rules.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,24 +51,36 @@
 )
 rules.add_perm("paweljong.create_vouchers_rule", create_vouchers_predicate)
 
 ## Events
 
 # View events
 view_events_predicate = has_person & (
-    has_global_perm("paweljong.view_event") | has_any_object("paweljong.view_event", Event)
+    has_global_perm("paweljong.view_event") | has_any_object("paweljong.view_event_rule", Event)
 )
 rules.add_perm("paweljong.view_events_rule", view_events_predicate)
 
+# Edit events
+change_events_predicate = has_person & (
+    has_global_perm("paweljong.change_event") | has_any_object("paweljong.change_event_rule", Event)
+)
+rules.add_perm("paweljong.change_events_rule", change_events_predicate)
+
 # Edit event
 change_event_predicate = has_person & (
-    has_global_perm("paweljong.change_event") | has_object_perm("paweljong.change_event")
+    has_global_perm("paweljong.change_event")
+    | has_object_perm("paweljong.change_event")
+    | is_organiser
 )
 rules.add_perm("paweljong.change_event_rule", change_event_predicate)
 
+# Checkpoint
+checkpoint_predicate = change_event_predicate
+rules.add_perm("paweljong.event_checkpoint_rule", checkpoint_predicate)
+
 # View event
 view_event_predicate = (
     is_event_published | (has_person & is_organiser) | has_object_perm("paweljong.view_event")
 )
 rules.add_perm("paweljong.view_event_rule", view_event_predicate)
 
 # Event organiser view
```

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/static/css/paweljong.css` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/static/css/paweljong.css`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/tables.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/tables.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/account_wizard.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/account_wizard.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/create.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/create.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/detail.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/detail.html`

 * *Files 15% similar despite different names*

```diff
@@ -10,27 +10,31 @@
 {% block extra_head %}
   <link rel="stylesheet" href="{% static 'css/paweljong.css' %}"/>
 {% endblock %}
 
 {% block content %}
   <h4>{{ event }}</h4>
 
-  {% has_perm 'paweljong.manage_event' user event as can_manage_event %}
+  {% has_perm 'paweljong.change_event_rule' user event as can_change_event_rule %}
+  {% has_perm 'paweljong.event_checkpoint_rule' user event as can_checkpoint_rule %}
 
-  {% if can_manage_event %}
     <p>
-      {% if can_manage_event %}
-        <a href="{% url 'edit_event_by_slug' event.slug %}" class="btn waves-effect waves-light">
-          <i class="material-icons left iconify" data-icon="mdi:edit"></i>
-          {% trans "Edit" %}
-        </a>
-      {% endif %}
-
+     {% if can_change_event_rule %}
+      <a href="{% url 'edit_event_by_slug' event.slug %}" class="btn waves-effect waves-light">
+        <i class="material-icons left iconify" data-icon="mdi:edit"></i>
+        {% trans "Edit" %}
+      </a>
+     {% endif %}
+     {% if can_checkpoint %}
+       <a href="{% url 'event_by_name_checkpoint' event.slug %}" class="btn waves-effect waves-light">
+         <i class="material-icons left iconify" data-icon="mdi:access-point-check"></i>
+         {% trans "Checkpoint" %}
+       </a>
+     {% endif %}
     </p>
-  {% endif %}
 
     <div class="card">
       <div class="card-content">
         <p>{{ event.description }}</p>
         <table id="event-detail-table">
           <tr>
             <td><i class="material-icons small">event</i></td>
```

#### html2text {}

```diff
@@ -1,19 +1,21 @@
 {# -*- engine:django -*- #} {% extends "core/base.html" %} {% load i18n static
 rules material_form coerce html_helpers %} {% load render_table from
 django_tables2 %} {% block browser_title %}{{ event }}{% endblock %} {% block
 extra_head %}
  {% endblock %} {% block content %}
 *** {{ event }} ***
-{% has_perm 'paweljong.manage_event' user event as can_manage_event %} {% if
-can_manage_event %}
-{% if can_manage_event %}
+{% has_perm 'paweljong.change_event_rule' user event as can_change_event_rule
+%} {% has_perm 'paweljong.event_checkpoint_rule' user event as
+can_checkpoint_rule %}
+{% if can_change_event_rule %}
  {%_trans_"Edit"_%}
+ {% endif %} {% if can_checkpoint %}
+ {%_trans_"Checkpoint"_%}
  {% endif %}
-{% endif %}
 {{ event.description }}
 event         {{ event.date_event location_on        {{ event.place }}
               }}
                                                      {
 edit_calendar {% trans "Registration open until" %}: {
                                                      event.date_registration
                                                      }}
```

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/edit.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/edit.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/full.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/full.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/list.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/list.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/manage.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/manage.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/persons_group.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/persons_group.html`

 * *Files 13% similar despite different names*

```diff
@@ -11,10 +11,11 @@
 {% block content %}
 
   <form method="post">
     {% csrf_token %}
     {% form form=form %}{% form %}
     {% include "core/partials/save_button.html" %}
   </form>
+  <div id="qr-reader" data-target-input="username"></div>
   {{ form.media.js }}
 
 {% endblock %}
```

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/register_start.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/register_start.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event/terms.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/terms.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event_registration/full.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event_registration/full.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/info_mailing/create.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/info_mailing/create.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/print/corona.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/corona.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/print/list_participants.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/list_participants.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/print/list_sign.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/list_sign.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/print/voucher.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/voucher.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/register_start.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/register_start.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/registration_state/create.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/registration_state/create.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/voucher/create.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/voucher/create.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/voucher/edit.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/voucher/edit.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/paweljong/voucher/list.html` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/voucher/list.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/templated_email/event_created.email` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/templated_email/event_created.email`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/templates/templated_email/event_registered.email` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/templated_email/event_registered.email`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/urls.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     path(
         "group_persons/<int:pk>/add",
         views.PersonGroupView.as_view(),
         name="add_persons_to_group",
     ),
     path("event/<slug:slug>", views.EventFullView.as_view(), name="event_by_name"),
     path("event/<slug:slug>/detail", views.EventDetailView.as_view(), name="event_detail_by_name"),
+    path("event/<slug:slug>/checkpoint", views.EventCheckpointView.as_view(), name="event_by_name_checkpoint"),
     path(
         "event/<slug:slug>/start",
         views.RegisterEventStart.as_view(),
         name="register_event_by_slug_start",
     ),
     path("misc/set_email_needed/<slug:slug>", views.set_email_needed, name="set_email_needed"),
     path("misc/set_email_needed/", views.set_email_needed, name="set_email_needed_no_slug"),
```

### Comparing `AlekSIS-App-Paweljong-1.8/aleksis/apps/paweljong/views.py` & `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Optional
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.contrib.syndication.views import Feed
 from django.core.exceptions import ValidationError
 from django.http import HttpRequest, HttpResponse
-from django.shortcuts import redirect, render
+from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse, reverse_lazy
 from django.utils import timezone
 from django.utils.decorators import method_decorator
+from django.utils.http import urlencode
 from django.utils.text import slugify
 from django.utils.translation import ugettext as _
 from django.views.decorators.cache import never_cache
 from django.views.generic import FormView, TemplateView, View
 from django.views.generic.detail import DetailView
 
 import reversion
@@ -32,20 +33,21 @@
 from .filters import EventFilter, EventRegistrationFilter, VoucherFilter
 from .forms import (
     EditEventForm,
     EditEventRegistrationForm,
     EditInfoMailingForm,
     EditTermForm,
     EditVoucherForm,
+    EventCheckpointForm,
     GenerateListForm,
     PersonGroupFormPerson,
     RegistrationNotificationForm,
     RegistrationStatesForm,
 )
-from .models import Event, EventRegistration, InfoMailing, RegistrationState, Terms, Voucher
+from .models import Checkpoint, Event, EventRegistration, InfoMailing, RegistrationState, Terms, Voucher
 from .tables import (
     AdditionalFieldsTable,
     ChildGroupsTable,
     EventRegistrationsTable,
     InfoMailingsTable,
     ManageEventsTable,
     RegistrationStatesTable,
@@ -140,34 +142,34 @@
 
 @method_decorator(never_cache, name="dispatch")
 class EventRegistrationCreateView(PermissionRequiredMixin, AdvancedCreateView):
     """Create view for event registrations."""
 
     model = EventRegistration
     form_class = EditEventRegistrationForm
-    permission_required = "paweljong.create_eventregistration_rule"
+    permission_required = "paweljong.create_registration_rule"
     template_name = "paweljong/event_registration/create.html"
     success_url = reverse_lazy("registrations")
     success_message = _("The event registration has been created.")
 
 
 @method_decorator(never_cache, name="dispatch")
 class EventRegistrationEditView(PermissionRequiredMixin, AdvancedEditView):
     """Edit view for event registrations."""
 
     model = EventRegistration
     form_class = EditEventRegistrationForm
-    permission_required = "paweljong.change_eventregistration_rule"
+    permission_required = "paweljong.change_registration_rule"
     template_name = "paweljong/event_registration/edit.html"
     success_url = reverse_lazy("registrations")
     success_message = _("The event registration has been saved.")
 
 
 @permission_required(
-    "paweljong.change_eventregistration_rule",
+    "paweljong.change_registration_rule",
     fn=objectgetter_optional(EventRegistration, None, False),
 )
 def edit_registration(request: HttpRequest, pk) -> HttpResponse:
     context = {}
 
     registration = objectgetter_optional(EventRegistration, None, False)(request, pk)
 
@@ -890,16 +892,19 @@
     success_message = _("The term has been saved.")
 
 
 class RetractRegistration(PermissionRequiredMixin, View):
 
     permission_required = "paweljong.can_retract_registration_rule"
 
+    def get_object(self, *args, **kwargs):
+        return EventRegistration.objects.get(id=self.kwargs["pk"])
+
     def get(self, *args, **kwargs):
-        registration = EventRegistration.objects.get(id=self.kwargs["pk"])
+        registration = self.get_object()
 
         registration.retract()
         messages.success(self.request, _("Registration successfully retracted."))
 
         return redirect("event_detail_by_name", slug=registration.event.slug)
 
 
@@ -962,29 +967,69 @@
 
         return super().form_valid(self)
 
     def get_success_url(self):
         return reverse("add_persons_to_group", kwargs={"pk": self.kwargs["pk"]})
 
 
+class EventCheckpointView(PermissionRequiredMixin, FormView):
+
+    template_name = "paweljong/event/checkpoint.html"
+    permission_required = "paweljong.can_checkpoint"
+    form_class = EventCheckpointForm
+
+    def get_initial(self):
+        initial = super().get_initial() or {}
+        if "comment" in self.request.GET:
+            initial["comment"] = self.request.GET.get("comment")
+        return initial
+
+    def form_valid(self, form):
+        checkpoint = Checkpoint()
+
+        checkpoint.event = get_object_or_404(Event, slug=self.kwargs["slug"])
+        try:
+            checkpoint.person = Person.objects.get(user__username=form.cleaned_data["username"])
+        except Person.DoesNotExist:
+            messages.error(self.request, _("The provided username is not linked to a person."))
+        checkpoint.checked_by = self.request.user.person
+
+        checkpoint.comment = form.cleaned_data["comment"]
+        checkpoint.timestamp = timezone.now()
+        if form.cleaned_data["use_latlon"]:
+            checkpoint.lat = form.cleaned_data["lat"]
+            checkpoint.lon = form.cleaned_data["lon"]
+
+        checkpoint.save()
+        messages.success(self.request, _("{} successfully checked for {}.").format(str(checkpoint.person), str(checkpoint.comment)))
+        self._comment = checkpoint.comment
+        return super().form_valid(self)
+
+    def get_success_url(self):
+        return reverse("event_by_name_checkpoint", kwargs={"slug": self.kwargs["slug"]}) + "?" + urlencode({"comment": self._comment})
+
+
 class ViewTerms(PermissionRequiredMixin, DetailView):
 
     context_object_name = "event"
     template_name = "paweljong/event/terms.html"
     permission_required = "paweljong.can_view_terms_rule"
     model = Event
     slug_field = "slug"
 
 
 class CheckInRegistration(PermissionRequiredMixin, View):
 
     permission_required = "paweljong.change_registration_rule"
 
+    def get_object(self, *args, **kwargs):
+        return EventRegistration.objects.get(id=self.kwargs["pk"])
+
     def get(self, *args, **kwargs):
-        registration = EventRegistration.objects.get(id=self.kwargs["pk"])
+        registration = self.get_object()
 
         try:
             registration.mark_checked_in()
             messages.success(self.request, _("Successfully checked in."))
         except ValidationError:
             messages.error(self.request, _("Person is already checked in!"))
```

### Comparing `AlekSIS-App-Paweljong-1.8/pyproject.toml` & `AlekSIS-App-Paweljong-1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Paweljong"
-version = "1.8"
+version = "1.9"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = ["CHANGELOG.rst", "LICENCE.rst", "aleksis/**/*.mo"]
 
 description = "AlekSIS (School Information System) — App Paweljong (Camp/Event management)"
```

### Comparing `AlekSIS-App-Paweljong-1.8/setup.py` & `AlekSIS-App-Paweljong-1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,30 +13,46 @@
                             'locale/ar/LC_MESSAGES/*',
                             'locale/de_DE/LC_MESSAGES/*',
                             'locale/fr/LC_MESSAGES/*',
                             'locale/la/LC_MESSAGES/*',
                             'locale/nb_NO/LC_MESSAGES/*',
                             'locale/tr_TR/LC_MESSAGES/*',
                             'static/css/*',
+                            'static/js/paweljong/*',
                             'templates/paweljong/account_wizard.html',
                             'templates/paweljong/account_wizard.html',
                             'templates/paweljong/account_wizard.html',
                             'templates/paweljong/account_wizard.html',
+                            'templates/paweljong/event/checkpoint.html',
+                            'templates/paweljong/event/checkpoint.html',
+                            'templates/paweljong/event/checkpoint.html',
+                            'templates/paweljong/event/checkpoint.html',
+                            'templates/paweljong/event/checkpoint.html',
+                            'templates/paweljong/event/checkpoint.html',
+                            'templates/paweljong/event/checkpoint.html',
+                            'templates/paweljong/event/checkpoint.html',
+                            'templates/paweljong/event/checkpoint.html',
+                            'templates/paweljong/event/checkpoint.html',
+                            'templates/paweljong/event/checkpoint.html',
+                            'templates/paweljong/event/checkpoint.html',
+                            'templates/paweljong/event/checkpoint.html',
                             'templates/paweljong/event/create.html',
                             'templates/paweljong/event/create.html',
                             'templates/paweljong/event/create.html',
                             'templates/paweljong/event/create.html',
                             'templates/paweljong/event/create.html',
                             'templates/paweljong/event/create.html',
                             'templates/paweljong/event/create.html',
                             'templates/paweljong/event/create.html',
                             'templates/paweljong/event/create.html',
                             'templates/paweljong/event/create.html',
                             'templates/paweljong/event/create.html',
                             'templates/paweljong/event/create.html',
+                            'templates/paweljong/event/create.html',
+                            'templates/paweljong/event/detail.html',
                             'templates/paweljong/event/detail.html',
                             'templates/paweljong/event/detail.html',
                             'templates/paweljong/event/detail.html',
                             'templates/paweljong/event/detail.html',
                             'templates/paweljong/event/detail.html',
                             'templates/paweljong/event/detail.html',
                             'templates/paweljong/event/detail.html',
@@ -53,26 +69,29 @@
                             'templates/paweljong/event/edit.html',
                             'templates/paweljong/event/edit.html',
                             'templates/paweljong/event/edit.html',
                             'templates/paweljong/event/edit.html',
                             'templates/paweljong/event/edit.html',
                             'templates/paweljong/event/edit.html',
                             'templates/paweljong/event/edit.html',
+                            'templates/paweljong/event/edit.html',
                             'templates/paweljong/event/full.html',
                             'templates/paweljong/event/full.html',
                             'templates/paweljong/event/full.html',
                             'templates/paweljong/event/full.html',
                             'templates/paweljong/event/full.html',
                             'templates/paweljong/event/full.html',
                             'templates/paweljong/event/full.html',
                             'templates/paweljong/event/full.html',
                             'templates/paweljong/event/full.html',
                             'templates/paweljong/event/full.html',
                             'templates/paweljong/event/full.html',
                             'templates/paweljong/event/full.html',
+                            'templates/paweljong/event/full.html',
+                            'templates/paweljong/event/list.html',
                             'templates/paweljong/event/list.html',
                             'templates/paweljong/event/list.html',
                             'templates/paweljong/event/list.html',
                             'templates/paweljong/event/list.html',
                             'templates/paweljong/event/list.html',
                             'templates/paweljong/event/list.html',
                             'templates/paweljong/event/list.html',
@@ -89,26 +108,29 @@
                             'templates/paweljong/event/manage.html',
                             'templates/paweljong/event/manage.html',
                             'templates/paweljong/event/manage.html',
                             'templates/paweljong/event/manage.html',
                             'templates/paweljong/event/manage.html',
                             'templates/paweljong/event/manage.html',
                             'templates/paweljong/event/manage.html',
+                            'templates/paweljong/event/manage.html',
                             'templates/paweljong/event/persons_group.html',
                             'templates/paweljong/event/persons_group.html',
                             'templates/paweljong/event/persons_group.html',
                             'templates/paweljong/event/persons_group.html',
                             'templates/paweljong/event/persons_group.html',
                             'templates/paweljong/event/persons_group.html',
                             'templates/paweljong/event/persons_group.html',
                             'templates/paweljong/event/persons_group.html',
                             'templates/paweljong/event/persons_group.html',
                             'templates/paweljong/event/persons_group.html',
                             'templates/paweljong/event/persons_group.html',
                             'templates/paweljong/event/persons_group.html',
+                            'templates/paweljong/event/persons_group.html',
+                            'templates/paweljong/event/register_start.html',
                             'templates/paweljong/event/register_start.html',
                             'templates/paweljong/event/register_start.html',
                             'templates/paweljong/event/register_start.html',
                             'templates/paweljong/event/register_start.html',
                             'templates/paweljong/event/register_start.html',
                             'templates/paweljong/event/register_start.html',
                             'templates/paweljong/event/register_start.html',
@@ -125,26 +147,29 @@
                             'templates/paweljong/event/register_wizard.html',
                             'templates/paweljong/event/register_wizard.html',
                             'templates/paweljong/event/register_wizard.html',
                             'templates/paweljong/event/register_wizard.html',
                             'templates/paweljong/event/register_wizard.html',
                             'templates/paweljong/event/register_wizard.html',
                             'templates/paweljong/event/register_wizard.html',
+                            'templates/paweljong/event/register_wizard.html',
                             'templates/paweljong/event/register_wizard_consent.html',
                             'templates/paweljong/event/register_wizard_consent.html',
                             'templates/paweljong/event/register_wizard_consent.html',
                             'templates/paweljong/event/register_wizard_consent.html',
                             'templates/paweljong/event/register_wizard_consent.html',
                             'templates/paweljong/event/register_wizard_consent.html',
                             'templates/paweljong/event/register_wizard_consent.html',
                             'templates/paweljong/event/register_wizard_consent.html',
                             'templates/paweljong/event/register_wizard_consent.html',
                             'templates/paweljong/event/register_wizard_consent.html',
                             'templates/paweljong/event/register_wizard_consent.html',
                             'templates/paweljong/event/register_wizard_consent.html',
+                            'templates/paweljong/event/register_wizard_consent.html',
+                            'templates/paweljong/event/registered.html',
                             'templates/paweljong/event/registered.html',
                             'templates/paweljong/event/registered.html',
                             'templates/paweljong/event/registered.html',
                             'templates/paweljong/event/registered.html',
                             'templates/paweljong/event/registered.html',
                             'templates/paweljong/event/registered.html',
                             'templates/paweljong/event/registered.html',
@@ -161,14 +186,15 @@
                             'templates/paweljong/event/terms.html',
                             'templates/paweljong/event/terms.html',
                             'templates/paweljong/event/terms.html',
                             'templates/paweljong/event/terms.html',
                             'templates/paweljong/event/terms.html',
                             'templates/paweljong/event/terms.html',
                             'templates/paweljong/event/terms.html',
+                            'templates/paweljong/event/terms.html',
                             'templates/paweljong/event_registration/edit.html',
                             'templates/paweljong/event_registration/edit.html',
                             'templates/paweljong/event_registration/edit.html',
                             'templates/paweljong/event_registration/full.html',
                             'templates/paweljong/event_registration/full.html',
                             'templates/paweljong/event_registration/full.html',
                             'templates/paweljong/event_registration/notification.html',
@@ -210,15 +236,15 @@
  'django-starfield>=1.0,<2.0']
 
 entry_points = \
 {'aleksis.app': ['paweljong = aleksis.apps.paweljong.apps:DefaultConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-paweljong',
-    'version': '1.8',
+    'version': '1.9',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp Paweljong (Camp/Event management)',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp Paweljong (Camp/Event management)\n==================================================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\nThe author of this app did not describe it yet.\n\nLicence\n-------\n\n::\n\n  Copyright © 2018, 2021, 2022 Dominik George <dominik.george@teckids.org>\n  Copyright © 2019, 2022 Tom Teichler <tom.teichler@teckids.org>\n\n  Licenced under the EUPL, version 1.2 or later\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://edugit.org/AlekSIS/AlekSIS\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Tom Teichler',
     'author_email': 'tom.teichler@teckids.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://hacknfun.camp',
```

### Comparing `AlekSIS-App-Paweljong-1.8/PKG-INFO` & `AlekSIS-App-Paweljong-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-app-paweljong
-Version: 1.8
+Version: 1.9
 Summary: AlekSIS (School Information System) — App Paweljong (Camp/Event management)
 Home-page: https://hacknfun.camp
 License: EUPL-1.2-or-later
 Author: Tom Teichler
 Author-email: tom.teichler@teckids.org
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Web Environment
```

