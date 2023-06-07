# Comparing `tmp/pyevr-0.5.3.dev1.tar.gz` & `tmp/pyevr-0.6.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyevr-0.5.3.dev1.tar", last modified: Wed Jun  7 07:57:00 2023, max compression
+gzip compressed data, was "pyevr-0.6.0.dev1.tar", last modified: Tue Sep 20 08:37:35 2022, max compression
```

## Comparing `pyevr-0.5.3.dev1.tar` & `pyevr-0.6.0.dev1.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-07 07:57:00.488195 pyevr-0.5.3.dev1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      152 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/AUTHORS.rst
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2128 2023-06-07 06:51:17.000000 pyevr-0.5.3.dev1/CHANGELOG.rst
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3683 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/CONTRIBUTING.rst
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1067 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      264 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3930 2023-06-07 07:57:00.488195 pyevr-0.5.3.dev1/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1132 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/README.rst
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-07 07:57:00.478195 pyevr-0.5.3.dev1/docs/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      606 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/docs/Makefile
--rw-r--r--   0 sergey    (1000) sergey    (1000)       28 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/docs/authors.rst
--rw-r--r--   0 sergey    (1000) sergey    (1000)       30 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/docs/changelog.rst
--rwxr-xr-x   0 sergey    (1000) sergey    (1000)     4778 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/docs/conf.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)       33 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/docs/contributing.rst
--rw-r--r--   0 sergey    (1000) sergey    (1000)      279 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/docs/index.rst
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1098 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/docs/installation.rst
--rw-r--r--   0 sergey    (1000) sergey    (1000)      767 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/docs/make.bat
--rw-r--r--   0 sergey    (1000) sergey    (1000)       52 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/docs/modules.rst
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1787 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/docs/pyevr.openapi_client.api.rst
--rw-r--r--   0 sergey    (1000) sergey    (1000)    13031 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/docs/pyevr.openapi_client.models.rst
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1054 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/docs/pyevr.openapi_client.rst
--rw-r--r--   0 sergey    (1000) sergey    (1000)      605 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/docs/pyevr.rst
--rw-r--r--   0 sergey    (1000) sergey    (1000)       27 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/docs/readme.rst
--rw-r--r--   0 sergey    (1000) sergey    (1000)      935 2023-05-25 09:13:11.000000 pyevr-0.5.3.dev1/docs/usage.rst
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-07 07:57:00.478195 pyevr-0.5.3.dev1/pyevr/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      198 2023-06-07 06:50:13.000000 pyevr-0.5.3.dev1/pyevr/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2617 2023-05-25 09:13:08.000000 pyevr-0.5.3.dev1/pyevr/apis.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2272 2023-05-25 09:13:08.000000 pyevr-0.5.3.dev1/pyevr/client.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      418 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/pyevr/main.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-07 07:57:00.481528 pyevr-0.5.3.dev1/pyevr/openapi_client/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5966 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-07 07:57:00.481528 pyevr-0.5.3.dev1/pyevr/openapi_client/api/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      590 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/api/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7593 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/api/assortments_api.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7616 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/api/certificates_api.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7686 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/api/measurement_units_api.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    14525 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/api/measurements_api.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    13352 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/api/organizations_api.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    22586 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/api/place_of_deliveries_api.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    60341 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/api/waybills_api.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    25639 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/api_client.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    13304 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/configuration.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3838 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/exceptions.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-07 07:57:00.488195 pyevr-0.5.3.dev1/pyevr/openapi_client/models/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4985 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5779 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/add_measurement_act_request.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3825 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/add_shipments_to_waybill_request.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3755 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/add_waybill_note_request.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8049 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/address.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5952 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/assortment.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2928 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/authorization_type.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4126 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/cancel_waybill_request.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4046 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/certificate.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5081 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/certificate_claim.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8787 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/consolidated_act.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8907 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/consolidated_act_all_of.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5329 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/contact_person.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    10301 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/contract_for_transfer_of_cutting_rights.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4214 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/coordinates.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5228 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/entity.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8643 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/forest_act.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7415 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/forest_notice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7515 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/forest_notice_all_of.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4159 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/holding_base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9014 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/inventory_act.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9134 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/inventory_act_all_of.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7642 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/measurement_act.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4094 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/measurement_unit.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8049 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/organization.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8318 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/owner.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    10458 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/pack.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2872 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/pack_location.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6165 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/paged_result_of_assortment.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6188 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/paged_result_of_certificate.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6257 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/paged_result_of_measurement_act.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6280 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/paged_result_of_measurement_unit.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6211 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/paged_result_of_organization.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6280 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/paged_result_of_place_of_delivery.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6096 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/paged_result_of_waybill.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    14444 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/place_of_delivery.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6665 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/previous_owner.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6424 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/problem_details.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    14872 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/put_place_of_delivery_request.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6832 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/receiver.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9133 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/representer.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9713 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/sales_contract.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9853 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/sales_contract_all_of.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8368 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/shipment.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7206 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/shipment_assortment.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7066 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/shipment_item.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12315 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/source.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15632 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/start_waybill_request.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    10914 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/transport.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6090 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/transporter.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5528 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/unload_waybill_request.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3438 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/validation_result.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3966 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/viewer.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    25695 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/waybill.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4883 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/waybill_authorization.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4938 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/waybill_note.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2762 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/waybill_note_creator.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9596 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/waybill_place_of_delivery.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3116 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/waybill_sort_field.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2969 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/waybill_status.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6581 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/without_forest_notice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6661 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/models/without_forest_notice_all_of.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12553 2023-05-25 09:21:48.000000 pyevr-0.5.3.dev1/pyevr/openapi_client/rest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-07 07:57:00.478195 pyevr-0.5.3.dev1/pyevr.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3930 2023-06-07 07:57:00.000000 pyevr-0.5.3.dev1/pyevr.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4314 2023-06-07 07:57:00.000000 pyevr-0.5.3.dev1/pyevr.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-06-07 07:57:00.000000 pyevr-0.5.3.dev1/pyevr.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       41 2023-06-07 07:57:00.000000 pyevr-0.5.3.dev1/pyevr.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-06-07 07:57:00.000000 pyevr-0.5.3.dev1/pyevr.egg-info/not-zip-safe
--rw-r--r--   0 sergey    (1000) sergey    (1000)       34 2023-06-07 07:57:00.000000 pyevr-0.5.3.dev1/pyevr.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        6 2023-06-07 07:57:00.000000 pyevr-0.5.3.dev1/pyevr.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      417 2023-06-07 07:57:00.488195 pyevr-0.5.3.dev1/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1510 2023-05-25 09:13:08.000000 pyevr-0.5.3.dev1/setup.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-07 07:57:00.488195 pyevr-0.5.3.dev1/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       60 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2342 2023-05-25 09:13:08.000000 pyevr-0.5.3.dev1/tests/test_apis.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3269 2023-05-25 09:13:11.000000 pyevr-0.5.3.dev1/tests/test_client.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      964 2021-11-18 10:13:29.000000 pyevr-0.5.3.dev1/tests/test_main.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-09-20 08:37:35.693079 pyevr-0.6.0.dev1/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      152 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/AUTHORS.rst
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2561 2022-09-20 08:32:23.000000 pyevr-0.6.0.dev1/CHANGELOG.rst
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3683 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/CONTRIBUTING.rst
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1067 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      264 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4363 2022-09-20 08:37:35.693079 pyevr-0.6.0.dev1/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1132 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/README.rst
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-09-20 08:37:35.686412 pyevr-0.6.0.dev1/docs/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      606 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/docs/Makefile
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       28 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/docs/authors.rst
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       30 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/docs/changelog.rst
+-rwxr-xr-x   0 sergey    (1000) sergey    (1000)     4778 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/docs/conf.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       33 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/docs/contributing.rst
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      279 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/docs/index.rst
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1098 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/docs/installation.rst
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      767 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/docs/make.bat
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       52 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/docs/modules.rst
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1787 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/docs/pyevr.openapi_client.api.rst
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    13031 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/docs/pyevr.openapi_client.models.rst
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1054 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/docs/pyevr.openapi_client.rst
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      605 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/docs/pyevr.rst
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       27 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/docs/readme.rst
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      935 2021-11-18 10:18:43.000000 pyevr-0.6.0.dev1/docs/usage.rst
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-09-20 08:37:35.686412 pyevr-0.6.0.dev1/pyevr/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      110 2022-07-11 09:21:22.000000 pyevr-0.6.0.dev1/pyevr/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2707 2022-07-11 11:39:07.000000 pyevr-0.6.0.dev1/pyevr/apis.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3853 2022-07-11 12:05:57.000000 pyevr-0.6.0.dev1/pyevr/client.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      418 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/pyevr/main.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-09-20 08:37:35.689745 pyevr-0.6.0.dev1/pyevr/openapi_client/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5966 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-09-20 08:37:35.689745 pyevr-0.6.0.dev1/pyevr/openapi_client/api/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      590 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/api/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7593 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/api/assortments_api.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7616 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/api/certificates_api.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7686 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/api/measurement_units_api.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    14525 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/api/measurements_api.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    13352 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/api/organizations_api.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    22586 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/api/place_of_deliveries_api.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    60341 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/api/waybills_api.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    25621 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/api_client.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    13304 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/configuration.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3838 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/exceptions.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-09-20 08:37:35.693079 pyevr-0.6.0.dev1/pyevr/openapi_client/models/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4985 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5779 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/add_measurement_act_request.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3825 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/add_shipments_to_waybill_request.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3755 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/add_waybill_note_request.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8049 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/address.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5952 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/assortment.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2928 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/authorization_type.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4126 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/cancel_waybill_request.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4046 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/certificate.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5081 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/certificate_claim.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8787 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/consolidated_act.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8907 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/consolidated_act_all_of.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5329 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/contact_person.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    10301 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/contract_for_transfer_of_cutting_rights.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4214 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/coordinates.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5228 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/entity.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8643 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/forest_act.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7415 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/forest_notice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7515 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/forest_notice_all_of.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4159 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/holding_base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9014 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/inventory_act.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9134 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/inventory_act_all_of.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7642 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/measurement_act.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4094 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/measurement_unit.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8049 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/organization.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8318 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/owner.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    10458 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/pack.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2872 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/pack_location.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5821 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/paged_result_of_assortment.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5844 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/paged_result_of_certificate.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5913 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/paged_result_of_measurement_act.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5936 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/paged_result_of_measurement_unit.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5867 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/paged_result_of_organization.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5936 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/paged_result_of_place_of_delivery.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5752 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/paged_result_of_waybill.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    14444 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/place_of_delivery.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6665 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/previous_owner.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6563 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/problem_details.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    14872 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/put_place_of_delivery_request.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6832 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/receiver.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9133 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/representer.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9713 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/sales_contract.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9853 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/sales_contract_all_of.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8368 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/shipment.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7206 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/shipment_assortment.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7066 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/shipment_item.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12315 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/source.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15632 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/start_waybill_request.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    10914 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/transport.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6090 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/transporter.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5528 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/unload_waybill_request.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3438 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/validation_result.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3966 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/viewer.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    25695 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/waybill.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4883 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/waybill_authorization.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4938 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/waybill_note.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2762 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/waybill_note_creator.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9596 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/waybill_place_of_delivery.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3116 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/waybill_sort_field.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2969 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/waybill_status.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6581 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/without_forest_notice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6661 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/models/without_forest_notice_all_of.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12553 2022-09-20 08:23:56.000000 pyevr-0.6.0.dev1/pyevr/openapi_client/rest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-09-20 08:37:35.686412 pyevr-0.6.0.dev1/pyevr.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4363 2022-09-20 08:37:35.000000 pyevr-0.6.0.dev1/pyevr.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4314 2022-09-20 08:37:35.000000 pyevr-0.6.0.dev1/pyevr.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2022-09-20 08:37:35.000000 pyevr-0.6.0.dev1/pyevr.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       41 2022-09-20 08:37:35.000000 pyevr-0.6.0.dev1/pyevr.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2022-09-20 08:37:35.000000 pyevr-0.6.0.dev1/pyevr.egg-info/not-zip-safe
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       34 2022-09-20 08:37:35.000000 pyevr-0.6.0.dev1/pyevr.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        6 2022-09-20 08:37:35.000000 pyevr-0.6.0.dev1/pyevr.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      417 2022-09-20 08:37:35.693079 pyevr-0.6.0.dev1/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1488 2022-09-20 08:32:48.000000 pyevr-0.6.0.dev1/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-09-20 08:37:35.693079 pyevr-0.6.0.dev1/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       60 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2354 2022-07-11 11:39:52.000000 pyevr-0.6.0.dev1/tests/test_apis.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4750 2022-07-11 12:06:10.000000 pyevr-0.6.0.dev1/tests/test_client.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      964 2021-11-18 10:13:29.000000 pyevr-0.6.0.dev1/tests/test_main.py
```

### Comparing `pyevr-0.5.3.dev1/CHANGELOG.rst` & `pyevr-0.6.0.dev1/CHANGELOG.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,38 @@
 =========
 Changelog
 =========
 
-0.5.3 (2023-06-07)
------------------------
+0.6.0.dev1
+----------
 
-**Compatibility**
+**Generic**
+
+* Change `all` method to be a generator instead of returning a list, to
+  allow data consumer to start consumption faster and avoid loading the
+  unnecessary pages if error happens early on
+* Add `deserialize_data` method that allows to rehydrate the model from
+  result of `sanitize_for_serialization` (allowing to store models as
+  json and similar use-cases)
+
+**Updates**
+
+Use EVR schema 1.9.0 from staging server
+
+* Support `WithoutForestNotice` holding base
+
+* Support `page_size` parameter for list endpoints
+
+* Support `last_modified_after` and `last_modified_before` for waybill list
 
-* Update to newest EVR schema
-* Remove workarounds that are no longer compatible with the schema
-* Fix issue with dockerized openapi generator causing out of memory error on arch linux
+* Support `waybill_latest_measurements` in waybill model
 
 
 0.5.2 (2022-04-06)
------------------------
+------------------
 
 **Generic**
 
 * Improve documentation
 
 **Compatibility**
```

### Comparing `pyevr-0.5.3.dev1/CONTRIBUTING.rst` & `pyevr-0.6.0.dev1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/LICENSE` & `pyevr-0.6.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/PKG-INFO` & `pyevr-0.6.0.dev1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyevr
-Version: 0.5.3.dev1
+Version: 0.6.0.dev1
 Summary: Python client for EVR
 Home-page: https://github.com/thorgate/pyevr
 Author: Thorgate
 Author-email: code@thorgate.eu
 License: MIT license
 Keywords: pyevr
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -59,26 +59,41 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =========
 Changelog
 =========
 
-0.5.3 (2023-06-07)
------------------------
+0.6.0.dev1
+----------
 
-**Compatibility**
+**Generic**
+
+* Change `all` method to be a generator instead of returning a list, to
+  allow data consumer to start consumption faster and avoid loading the
+  unnecessary pages if error happens early on
+* Add `deserialize_data` method that allows to rehydrate the model from
+  result of `sanitize_for_serialization` (allowing to store models as
+  json and similar use-cases)
+
+**Updates**
+
+Use EVR schema 1.9.0 from staging server
+
+* Support `WithoutForestNotice` holding base
+
+* Support `page_size` parameter for list endpoints
+
+* Support `last_modified_after` and `last_modified_before` for waybill list
 
-* Update to newest EVR schema
-* Remove workarounds that are no longer compatible with the schema
-* Fix issue with dockerized openapi generator causing out of memory error on arch linux
+* Support `waybill_latest_measurements` in waybill model
 
 
 0.5.2 (2022-04-06)
------------------------
+------------------
 
 **Generic**
 
 * Improve documentation
 
 **Compatibility**
```

### Comparing `pyevr-0.5.3.dev1/README.rst` & `pyevr-0.6.0.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/docs/Makefile` & `pyevr-0.6.0.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/docs/conf.py` & `pyevr-0.6.0.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/docs/installation.rst` & `pyevr-0.6.0.dev1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/docs/make.bat` & `pyevr-0.6.0.dev1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/docs/pyevr.openapi_client.api.rst` & `pyevr-0.6.0.dev1/docs/pyevr.openapi_client.api.rst`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/docs/pyevr.openapi_client.models.rst` & `pyevr-0.6.0.dev1/docs/pyevr.openapi_client.models.rst`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/docs/pyevr.openapi_client.rst` & `pyevr-0.6.0.dev1/docs/pyevr.openapi_client.rst`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/docs/pyevr.rst` & `pyevr-0.6.0.dev1/docs/pyevr.rst`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/docs/usage.rst` & `pyevr-0.6.0.dev1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/apis.py` & `pyevr-0.6.0.dev1/pyevr/apis.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from math import ceil
 from typing import Callable
 
 from pyevr.openapi_client import api
 
 
 class AllMixin:
     """Mixin for API endpoint classes to have an all() method for returning objects from all pages.
@@ -29,30 +28,33 @@
 
     def all(self, **kwargs):
         """Method for going through all the pages of a list view that is responsible for returning paged results"""
         if self.evr_page_param in kwargs:
             del kwargs[self.evr_page_param]
         endpoint = self.get_list_endpoint()
 
-        kwargs[self.evr_page_param] = 1
-        first_page_response = endpoint(**kwargs)
-        results = first_page_response.page_result
-        page_size = first_page_response.page_size
-        total_count = first_page_response.total_count
-
-        if total_count <= page_size:
-            return results
-
-        total_pages = ceil(total_count / page_size)
-        for page in range(2, total_pages + 1):
-            kwargs[self.evr_page_param] = page
+        current_page = 1
+        current_count = 0
+        total_count = None
+
+        while total_count is None or current_count < total_count:
+            kwargs[self.evr_page_param] = current_page
             page_response = endpoint(**kwargs)
-            results.extend(page_response.page_result)
+            if total_count is None:
+                total_count = page_response.total_count
+
+            if page_response.page_result:
+                for item in page_response.page_result:
+                    current_count += 1
+                    yield item
+            else:
+                # Possibly number of items changed while iterating, in this case assume no more items are coming
+                return
 
-        return results
+            current_page += 1
 
 
 class AssortmentsAPI(AllMixin, api.AssortmentsApi):
     list_endpoint_attr = 'assortments_list'
 
 
 class CertificatesAPI(AllMixin, api.CertificatesApi):
```

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/__init__.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/api/__init__.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/api/assortments_api.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/api/assortments_api.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/api/certificates_api.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/api/certificates_api.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/api/measurement_units_api.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/api/measurement_units_api.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/api/measurements_api.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/api/measurements_api.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/api/organizations_api.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/api/organizations_api.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/api/place_of_deliveries_api.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/api/place_of_deliveries_api.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/api/waybills_api.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/api/waybills_api.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/api_client.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,62 +249,62 @@
             deserialized object, or string of class name.
 
         :return: deserialized object.
         """
         # handle file downloading
         # save response body into a tmp file and return the instance
         if response_type == "file":
-            return self.__deserialize_file(response)
+            return self._deserialize_file(response)
 
         # fetch data from response object
         try:
             data = json.loads(response.data)
         except ValueError:
             data = response.data
 
-        return self.__deserialize(data, response_type)
+        return self._deserialize(data, response_type)
 
-    def __deserialize(self, data, klass):
+    def _deserialize(self, data, klass):
         """Deserializes dict, list, str into an object.
 
         :param data: dict, list or str.
         :param klass: class literal, or string of class name.
 
         :return: object.
         """
         if data is None:
             return None
 
         if type(klass) == str:
             if klass.startswith('list['):
                 sub_kls = re.match(r'list\[(.*)\]', klass).group(1)
-                return [self.__deserialize(sub_data, sub_kls)
+                return [self._deserialize(sub_data, sub_kls)
                         for sub_data in data]
 
             if klass.startswith('dict('):
                 sub_kls = re.match(r'dict\(([^,]*), (.*)\)', klass).group(2)
-                return {k: self.__deserialize(v, sub_kls)
+                return {k: self._deserialize(v, sub_kls)
                         for k, v in six.iteritems(data)}
 
             # convert str to class
             if klass in self.NATIVE_TYPES_MAPPING:
                 klass = self.NATIVE_TYPES_MAPPING[klass]
             else:
                 klass = getattr(pyevr.openapi_client.models, klass)
 
         if klass in self.PRIMITIVE_TYPES:
-            return self.__deserialize_primitive(data, klass)
+            return self._deserialize_primitive(data, klass)
         elif klass == object:
-            return self.__deserialize_object(data)
+            return self._deserialize_object(data)
         elif klass == datetime.date:
-            return self.__deserialize_date(data)
+            return self._deserialize_date(data)
         elif klass == datetime.datetime:
-            return self.__deserialize_datetime(data)
+            return self._deserialize_datetime(data)
         else:
-            return self.__deserialize_model(data, klass)
+            return self._deserialize_model(data, klass)
 
     def call_api(self, resource_path, method,
                  path_params=None, query_params=None, header_params=None,
                  body=None, post_params=None, files=None,
                  response_type=None, auth_settings=None, async_req=None,
                  _return_http_data_only=None, collection_formats=None,
                  _preload_content=True, _request_timeout=None, _host=None):
@@ -530,15 +530,15 @@
                 elif auth_setting['in'] == 'query':
                     querys.append((auth_setting['key'], auth_setting['value']))
                 else:
                     raise ApiValueError(
                         'Authentication token must be in `query` or `header`'
                     )
 
-    def __deserialize_file(self, response):
+    def _deserialize_file(self, response):
         """Deserializes body to file
 
         Saves response body into a file in a temporary folder,
         using the filename from the `Content-Disposition` header if provided.
 
         :param response:  RESTResponse.
         :return: file path.
@@ -554,37 +554,37 @@
             path = os.path.join(os.path.dirname(path), filename)
 
         with open(path, "wb") as f:
             f.write(response.data)
 
         return path
 
-    def __deserialize_primitive(self, data, klass):
+    def _deserialize_primitive(self, data, klass):
         """Deserializes string to primitive type.
 
         :param data: str.
         :param klass: class literal.
 
         :return: int, long, float, str, bool.
         """
         try:
             return klass(data)
         except UnicodeEncodeError:
             return six.text_type(data)
         except TypeError:
             return data
 
-    def __deserialize_object(self, value):
+    def _deserialize_object(self, value):
         """Return an original value.
 
         :return: object.
         """
         return value
 
-    def __deserialize_date(self, string):
+    def _deserialize_date(self, string):
         """Deserializes string to date.
 
         :param string: str.
         :return: date.
         """
         try:
             return parse(string).date()
@@ -592,15 +592,15 @@
             return string
         except ValueError:
             raise rest.ApiException(
                 status=0,
                 reason="Failed to parse `{0}` as date object".format(string)
             )
 
-    def __deserialize_datetime(self, string):
+    def _deserialize_datetime(self, string):
         """Deserializes string to datetime.
 
         The string should be in iso8601 datetime format.
 
         :param string: str.
         :return: datetime.
         """
@@ -613,15 +613,15 @@
                 status=0,
                 reason=(
                     "Failed to parse `{0}` as datetime object"
                     .format(string)
                 )
             )
 
-    def __deserialize_model(self, data, klass):
+    def _deserialize_model(self, data, klass):
         """Deserializes list or dict to model.
 
         :param data: dict, list.
         :param klass: class literal.
         :return: model object.
         """
 
@@ -632,16 +632,16 @@
         kwargs = {}
         if (data is not None and
                 klass.openapi_types is not None and
                 isinstance(data, (list, dict))):
             for attr, attr_type in six.iteritems(klass.openapi_types):
                 if klass.attribute_map[attr] in data:
                     value = data[klass.attribute_map[attr]]
-                    kwargs[attr] = self.__deserialize(value, attr_type)
+                    kwargs[attr] = self._deserialize(value, attr_type)
 
         instance = klass(**kwargs)
 
         if hasattr(instance, 'get_real_child_model'):
             klass_name = instance.get_real_child_model(data)
             if klass_name:
-                instance = self.__deserialize(data, klass_name)
+                instance = self._deserialize(data, klass_name)
         return instance
```

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/configuration.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/exceptions.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/__init__.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/add_measurement_act_request.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/add_measurement_act_request.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/add_shipments_to_waybill_request.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/add_shipments_to_waybill_request.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/add_waybill_note_request.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/add_waybill_note_request.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/address.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/address.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/assortment.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/assortment.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/authorization_type.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/authorization_type.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/cancel_waybill_request.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/cancel_waybill_request.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/certificate.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/certificate.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/certificate_claim.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/certificate_claim.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/consolidated_act.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/consolidated_act.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/consolidated_act_all_of.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/consolidated_act_all_of.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/contact_person.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/contact_person.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/contract_for_transfer_of_cutting_rights.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/contract_for_transfer_of_cutting_rights.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/coordinates.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/coordinates.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/entity.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,16 +77,16 @@
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 name is not None and len(name) > 200):
             raise ValueError("Invalid value for `name`, length must be less than or equal to `200`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) < 1):
-            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
+                name is not None and len(name) < 0):
+            raise ValueError("Invalid value for `name`, length must be greater than or equal to `0`")  # noqa: E501
 
         self._name = name
 
     @property
     def code(self):
         """Gets the code of this Entity.  # noqa: E501
 
@@ -108,16 +108,16 @@
         """
         if self.local_vars_configuration.client_side_validation and code is None:  # noqa: E501
             raise ValueError("Invalid value for `code`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 code is not None and len(code) > 20):
             raise ValueError("Invalid value for `code`, length must be less than or equal to `20`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                code is not None and len(code) < 1):
-            raise ValueError("Invalid value for `code`, length must be greater than or equal to `1`")  # noqa: E501
+                code is not None and len(code) < 0):
+            raise ValueError("Invalid value for `code`, length must be greater than or equal to `0`")  # noqa: E501
 
         self._code = code
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/forest_act.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/forest_act.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/forest_notice.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/forest_notice.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/forest_notice_all_of.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/forest_notice_all_of.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/holding_base.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/holding_base.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/inventory_act.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/inventory_act.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/inventory_act_all_of.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/inventory_act_all_of.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/measurement_act.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/measurement_act.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/measurement_unit.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/measurement_unit.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/organization.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/organization.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/owner.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/owner.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/pack.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/pack.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/pack_location.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/pack_location.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/paged_result_of_assortment.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/paged_result_of_assortment.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,95 +67,87 @@
         if total_count is not None:
             self.total_count = total_count
 
     @property
     def page_number(self):
         """Gets the page_number of this PagedResultOfAssortment.  # noqa: E501
 
-        Lehekülje number  # noqa: E501
 
         :return: The page_number of this PagedResultOfAssortment.  # noqa: E501
         :rtype: int
         """
         return self._page_number
 
     @page_number.setter
     def page_number(self, page_number):
         """Sets the page_number of this PagedResultOfAssortment.
 
-        Lehekülje number  # noqa: E501
 
         :param page_number: The page_number of this PagedResultOfAssortment.  # noqa: E501
         :type: int
         """
 
         self._page_number = page_number
 
     @property
     def page_size(self):
         """Gets the page_size of this PagedResultOfAssortment.  # noqa: E501
 
-        Lehekülje suurus  # noqa: E501
 
         :return: The page_size of this PagedResultOfAssortment.  # noqa: E501
         :rtype: int
         """
         return self._page_size
 
     @page_size.setter
     def page_size(self, page_size):
         """Sets the page_size of this PagedResultOfAssortment.
 
-        Lehekülje suurus  # noqa: E501
 
         :param page_size: The page_size of this PagedResultOfAssortment.  # noqa: E501
         :type: int
         """
 
         self._page_size = page_size
 
     @property
     def page_result(self):
         """Gets the page_result of this PagedResultOfAssortment.  # noqa: E501
 
-        Lehekülje tulemused  # noqa: E501
 
         :return: The page_result of this PagedResultOfAssortment.  # noqa: E501
         :rtype: list[Assortment]
         """
         return self._page_result
 
     @page_result.setter
     def page_result(self, page_result):
         """Sets the page_result of this PagedResultOfAssortment.
 
-        Lehekülje tulemused  # noqa: E501
 
         :param page_result: The page_result of this PagedResultOfAssortment.  # noqa: E501
         :type: list[Assortment]
         """
 
         self._page_result = page_result
 
     @property
     def total_count(self):
         """Gets the total_count of this PagedResultOfAssortment.  # noqa: E501
 
-        Päringu vastete arv kokku  # noqa: E501
 
         :return: The total_count of this PagedResultOfAssortment.  # noqa: E501
         :rtype: int
         """
         return self._total_count
 
     @total_count.setter
     def total_count(self, total_count):
         """Sets the total_count of this PagedResultOfAssortment.
 
-        Päringu vastete arv kokku  # noqa: E501
 
         :param total_count: The total_count of this PagedResultOfAssortment.  # noqa: E501
         :type: int
         """
 
         self._total_count = total_count
```

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/paged_result_of_certificate.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/paged_result_of_certificate.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,95 +67,87 @@
         if total_count is not None:
             self.total_count = total_count
 
     @property
     def page_number(self):
         """Gets the page_number of this PagedResultOfCertificate.  # noqa: E501
 
-        Lehekülje number  # noqa: E501
 
         :return: The page_number of this PagedResultOfCertificate.  # noqa: E501
         :rtype: int
         """
         return self._page_number
 
     @page_number.setter
     def page_number(self, page_number):
         """Sets the page_number of this PagedResultOfCertificate.
 
-        Lehekülje number  # noqa: E501
 
         :param page_number: The page_number of this PagedResultOfCertificate.  # noqa: E501
         :type: int
         """
 
         self._page_number = page_number
 
     @property
     def page_size(self):
         """Gets the page_size of this PagedResultOfCertificate.  # noqa: E501
 
-        Lehekülje suurus  # noqa: E501
 
         :return: The page_size of this PagedResultOfCertificate.  # noqa: E501
         :rtype: int
         """
         return self._page_size
 
     @page_size.setter
     def page_size(self, page_size):
         """Sets the page_size of this PagedResultOfCertificate.
 
-        Lehekülje suurus  # noqa: E501
 
         :param page_size: The page_size of this PagedResultOfCertificate.  # noqa: E501
         :type: int
         """
 
         self._page_size = page_size
 
     @property
     def page_result(self):
         """Gets the page_result of this PagedResultOfCertificate.  # noqa: E501
 
-        Lehekülje tulemused  # noqa: E501
 
         :return: The page_result of this PagedResultOfCertificate.  # noqa: E501
         :rtype: list[Certificate]
         """
         return self._page_result
 
     @page_result.setter
     def page_result(self, page_result):
         """Sets the page_result of this PagedResultOfCertificate.
 
-        Lehekülje tulemused  # noqa: E501
 
         :param page_result: The page_result of this PagedResultOfCertificate.  # noqa: E501
         :type: list[Certificate]
         """
 
         self._page_result = page_result
 
     @property
     def total_count(self):
         """Gets the total_count of this PagedResultOfCertificate.  # noqa: E501
 
-        Päringu vastete arv kokku  # noqa: E501
 
         :return: The total_count of this PagedResultOfCertificate.  # noqa: E501
         :rtype: int
         """
         return self._total_count
 
     @total_count.setter
     def total_count(self, total_count):
         """Sets the total_count of this PagedResultOfCertificate.
 
-        Päringu vastete arv kokku  # noqa: E501
 
         :param total_count: The total_count of this PagedResultOfCertificate.  # noqa: E501
         :type: int
         """
 
         self._total_count = total_count
```

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/paged_result_of_measurement_act.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/paged_result_of_organization.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from pyevr.openapi_client.configuration import Configuration
 
 
-class PagedResultOfMeasurementAct(object):
+class PagedResultOfOrganization(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -31,27 +31,27 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'page_number': 'int',
         'page_size': 'int',
-        'page_result': 'list[MeasurementAct]',
+        'page_result': 'list[Organization]',
         'total_count': 'int'
     }
 
     attribute_map = {
         'page_number': 'pageNumber',
         'page_size': 'pageSize',
         'page_result': 'pageResult',
         'total_count': 'totalCount'
     }
 
     def __init__(self, page_number=None, page_size=None, page_result=None, total_count=None, local_vars_configuration=None):  # noqa: E501
-        """PagedResultOfMeasurementAct - a model defined in OpenAPI"""  # noqa: E501
+        """PagedResultOfOrganization - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._page_number = None
         self._page_size = None
         self._page_result = None
@@ -65,99 +65,91 @@
         if page_result is not None:
             self.page_result = page_result
         if total_count is not None:
             self.total_count = total_count
 
     @property
     def page_number(self):
-        """Gets the page_number of this PagedResultOfMeasurementAct.  # noqa: E501
+        """Gets the page_number of this PagedResultOfOrganization.  # noqa: E501
 
-        Lehekülje number  # noqa: E501
 
-        :return: The page_number of this PagedResultOfMeasurementAct.  # noqa: E501
+        :return: The page_number of this PagedResultOfOrganization.  # noqa: E501
         :rtype: int
         """
         return self._page_number
 
     @page_number.setter
     def page_number(self, page_number):
-        """Sets the page_number of this PagedResultOfMeasurementAct.
+        """Sets the page_number of this PagedResultOfOrganization.
 
-        Lehekülje number  # noqa: E501
 
-        :param page_number: The page_number of this PagedResultOfMeasurementAct.  # noqa: E501
+        :param page_number: The page_number of this PagedResultOfOrganization.  # noqa: E501
         :type: int
         """
 
         self._page_number = page_number
 
     @property
     def page_size(self):
-        """Gets the page_size of this PagedResultOfMeasurementAct.  # noqa: E501
+        """Gets the page_size of this PagedResultOfOrganization.  # noqa: E501
 
-        Lehekülje suurus  # noqa: E501
 
-        :return: The page_size of this PagedResultOfMeasurementAct.  # noqa: E501
+        :return: The page_size of this PagedResultOfOrganization.  # noqa: E501
         :rtype: int
         """
         return self._page_size
 
     @page_size.setter
     def page_size(self, page_size):
-        """Sets the page_size of this PagedResultOfMeasurementAct.
+        """Sets the page_size of this PagedResultOfOrganization.
 
-        Lehekülje suurus  # noqa: E501
 
-        :param page_size: The page_size of this PagedResultOfMeasurementAct.  # noqa: E501
+        :param page_size: The page_size of this PagedResultOfOrganization.  # noqa: E501
         :type: int
         """
 
         self._page_size = page_size
 
     @property
     def page_result(self):
-        """Gets the page_result of this PagedResultOfMeasurementAct.  # noqa: E501
+        """Gets the page_result of this PagedResultOfOrganization.  # noqa: E501
 
-        Lehekülje tulemused  # noqa: E501
 
-        :return: The page_result of this PagedResultOfMeasurementAct.  # noqa: E501
-        :rtype: list[MeasurementAct]
+        :return: The page_result of this PagedResultOfOrganization.  # noqa: E501
+        :rtype: list[Organization]
         """
         return self._page_result
 
     @page_result.setter
     def page_result(self, page_result):
-        """Sets the page_result of this PagedResultOfMeasurementAct.
+        """Sets the page_result of this PagedResultOfOrganization.
 
-        Lehekülje tulemused  # noqa: E501
 
-        :param page_result: The page_result of this PagedResultOfMeasurementAct.  # noqa: E501
-        :type: list[MeasurementAct]
+        :param page_result: The page_result of this PagedResultOfOrganization.  # noqa: E501
+        :type: list[Organization]
         """
 
         self._page_result = page_result
 
     @property
     def total_count(self):
-        """Gets the total_count of this PagedResultOfMeasurementAct.  # noqa: E501
+        """Gets the total_count of this PagedResultOfOrganization.  # noqa: E501
 
-        Päringu vastete arv kokku  # noqa: E501
 
-        :return: The total_count of this PagedResultOfMeasurementAct.  # noqa: E501
+        :return: The total_count of this PagedResultOfOrganization.  # noqa: E501
         :rtype: int
         """
         return self._total_count
 
     @total_count.setter
     def total_count(self, total_count):
-        """Sets the total_count of this PagedResultOfMeasurementAct.
+        """Sets the total_count of this PagedResultOfOrganization.
 
-        Päringu vastete arv kokku  # noqa: E501
 
-        :param total_count: The total_count of this PagedResultOfMeasurementAct.  # noqa: E501
+        :param total_count: The total_count of this PagedResultOfOrganization.  # noqa: E501
         :type: int
         """
 
         self._total_count = total_count
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -189,18 +181,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, PagedResultOfMeasurementAct):
+        if not isinstance(other, PagedResultOfOrganization):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, PagedResultOfMeasurementAct):
+        if not isinstance(other, PagedResultOfOrganization):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/paged_result_of_measurement_unit.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/paged_result_of_measurement_unit.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,95 +67,87 @@
         if total_count is not None:
             self.total_count = total_count
 
     @property
     def page_number(self):
         """Gets the page_number of this PagedResultOfMeasurementUnit.  # noqa: E501
 
-        Lehekülje number  # noqa: E501
 
         :return: The page_number of this PagedResultOfMeasurementUnit.  # noqa: E501
         :rtype: int
         """
         return self._page_number
 
     @page_number.setter
     def page_number(self, page_number):
         """Sets the page_number of this PagedResultOfMeasurementUnit.
 
-        Lehekülje number  # noqa: E501
 
         :param page_number: The page_number of this PagedResultOfMeasurementUnit.  # noqa: E501
         :type: int
         """
 
         self._page_number = page_number
 
     @property
     def page_size(self):
         """Gets the page_size of this PagedResultOfMeasurementUnit.  # noqa: E501
 
-        Lehekülje suurus  # noqa: E501
 
         :return: The page_size of this PagedResultOfMeasurementUnit.  # noqa: E501
         :rtype: int
         """
         return self._page_size
 
     @page_size.setter
     def page_size(self, page_size):
         """Sets the page_size of this PagedResultOfMeasurementUnit.
 
-        Lehekülje suurus  # noqa: E501
 
         :param page_size: The page_size of this PagedResultOfMeasurementUnit.  # noqa: E501
         :type: int
         """
 
         self._page_size = page_size
 
     @property
     def page_result(self):
         """Gets the page_result of this PagedResultOfMeasurementUnit.  # noqa: E501
 
-        Lehekülje tulemused  # noqa: E501
 
         :return: The page_result of this PagedResultOfMeasurementUnit.  # noqa: E501
         :rtype: list[MeasurementUnit]
         """
         return self._page_result
 
     @page_result.setter
     def page_result(self, page_result):
         """Sets the page_result of this PagedResultOfMeasurementUnit.
 
-        Lehekülje tulemused  # noqa: E501
 
         :param page_result: The page_result of this PagedResultOfMeasurementUnit.  # noqa: E501
         :type: list[MeasurementUnit]
         """
 
         self._page_result = page_result
 
     @property
     def total_count(self):
         """Gets the total_count of this PagedResultOfMeasurementUnit.  # noqa: E501
 
-        Päringu vastete arv kokku  # noqa: E501
 
         :return: The total_count of this PagedResultOfMeasurementUnit.  # noqa: E501
         :rtype: int
         """
         return self._total_count
 
     @total_count.setter
     def total_count(self, total_count):
         """Sets the total_count of this PagedResultOfMeasurementUnit.
 
-        Päringu vastete arv kokku  # noqa: E501
 
         :param total_count: The total_count of this PagedResultOfMeasurementUnit.  # noqa: E501
         :type: int
         """
 
         self._total_count = total_count
```

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/paged_result_of_organization.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/paged_result_of_measurement_act.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from pyevr.openapi_client.configuration import Configuration
 
 
-class PagedResultOfOrganization(object):
+class PagedResultOfMeasurementAct(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -31,27 +31,27 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'page_number': 'int',
         'page_size': 'int',
-        'page_result': 'list[Organization]',
+        'page_result': 'list[MeasurementAct]',
         'total_count': 'int'
     }
 
     attribute_map = {
         'page_number': 'pageNumber',
         'page_size': 'pageSize',
         'page_result': 'pageResult',
         'total_count': 'totalCount'
     }
 
     def __init__(self, page_number=None, page_size=None, page_result=None, total_count=None, local_vars_configuration=None):  # noqa: E501
-        """PagedResultOfOrganization - a model defined in OpenAPI"""  # noqa: E501
+        """PagedResultOfMeasurementAct - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._page_number = None
         self._page_size = None
         self._page_result = None
@@ -65,99 +65,91 @@
         if page_result is not None:
             self.page_result = page_result
         if total_count is not None:
             self.total_count = total_count
 
     @property
     def page_number(self):
-        """Gets the page_number of this PagedResultOfOrganization.  # noqa: E501
+        """Gets the page_number of this PagedResultOfMeasurementAct.  # noqa: E501
 
-        Lehekülje number  # noqa: E501
 
-        :return: The page_number of this PagedResultOfOrganization.  # noqa: E501
+        :return: The page_number of this PagedResultOfMeasurementAct.  # noqa: E501
         :rtype: int
         """
         return self._page_number
 
     @page_number.setter
     def page_number(self, page_number):
-        """Sets the page_number of this PagedResultOfOrganization.
+        """Sets the page_number of this PagedResultOfMeasurementAct.
 
-        Lehekülje number  # noqa: E501
 
-        :param page_number: The page_number of this PagedResultOfOrganization.  # noqa: E501
+        :param page_number: The page_number of this PagedResultOfMeasurementAct.  # noqa: E501
         :type: int
         """
 
         self._page_number = page_number
 
     @property
     def page_size(self):
-        """Gets the page_size of this PagedResultOfOrganization.  # noqa: E501
+        """Gets the page_size of this PagedResultOfMeasurementAct.  # noqa: E501
 
-        Lehekülje suurus  # noqa: E501
 
-        :return: The page_size of this PagedResultOfOrganization.  # noqa: E501
+        :return: The page_size of this PagedResultOfMeasurementAct.  # noqa: E501
         :rtype: int
         """
         return self._page_size
 
     @page_size.setter
     def page_size(self, page_size):
-        """Sets the page_size of this PagedResultOfOrganization.
+        """Sets the page_size of this PagedResultOfMeasurementAct.
 
-        Lehekülje suurus  # noqa: E501
 
-        :param page_size: The page_size of this PagedResultOfOrganization.  # noqa: E501
+        :param page_size: The page_size of this PagedResultOfMeasurementAct.  # noqa: E501
         :type: int
         """
 
         self._page_size = page_size
 
     @property
     def page_result(self):
-        """Gets the page_result of this PagedResultOfOrganization.  # noqa: E501
+        """Gets the page_result of this PagedResultOfMeasurementAct.  # noqa: E501
 
-        Lehekülje tulemused  # noqa: E501
 
-        :return: The page_result of this PagedResultOfOrganization.  # noqa: E501
-        :rtype: list[Organization]
+        :return: The page_result of this PagedResultOfMeasurementAct.  # noqa: E501
+        :rtype: list[MeasurementAct]
         """
         return self._page_result
 
     @page_result.setter
     def page_result(self, page_result):
-        """Sets the page_result of this PagedResultOfOrganization.
+        """Sets the page_result of this PagedResultOfMeasurementAct.
 
-        Lehekülje tulemused  # noqa: E501
 
-        :param page_result: The page_result of this PagedResultOfOrganization.  # noqa: E501
-        :type: list[Organization]
+        :param page_result: The page_result of this PagedResultOfMeasurementAct.  # noqa: E501
+        :type: list[MeasurementAct]
         """
 
         self._page_result = page_result
 
     @property
     def total_count(self):
-        """Gets the total_count of this PagedResultOfOrganization.  # noqa: E501
+        """Gets the total_count of this PagedResultOfMeasurementAct.  # noqa: E501
 
-        Päringu vastete arv kokku  # noqa: E501
 
-        :return: The total_count of this PagedResultOfOrganization.  # noqa: E501
+        :return: The total_count of this PagedResultOfMeasurementAct.  # noqa: E501
         :rtype: int
         """
         return self._total_count
 
     @total_count.setter
     def total_count(self, total_count):
-        """Sets the total_count of this PagedResultOfOrganization.
+        """Sets the total_count of this PagedResultOfMeasurementAct.
 
-        Päringu vastete arv kokku  # noqa: E501
 
-        :param total_count: The total_count of this PagedResultOfOrganization.  # noqa: E501
+        :param total_count: The total_count of this PagedResultOfMeasurementAct.  # noqa: E501
         :type: int
         """
 
         self._total_count = total_count
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -189,18 +181,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, PagedResultOfOrganization):
+        if not isinstance(other, PagedResultOfMeasurementAct):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, PagedResultOfOrganization):
+        if not isinstance(other, PagedResultOfMeasurementAct):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/paged_result_of_place_of_delivery.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/paged_result_of_place_of_delivery.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,95 +67,87 @@
         if total_count is not None:
             self.total_count = total_count
 
     @property
     def page_number(self):
         """Gets the page_number of this PagedResultOfPlaceOfDelivery.  # noqa: E501
 
-        Lehekülje number  # noqa: E501
 
         :return: The page_number of this PagedResultOfPlaceOfDelivery.  # noqa: E501
         :rtype: int
         """
         return self._page_number
 
     @page_number.setter
     def page_number(self, page_number):
         """Sets the page_number of this PagedResultOfPlaceOfDelivery.
 
-        Lehekülje number  # noqa: E501
 
         :param page_number: The page_number of this PagedResultOfPlaceOfDelivery.  # noqa: E501
         :type: int
         """
 
         self._page_number = page_number
 
     @property
     def page_size(self):
         """Gets the page_size of this PagedResultOfPlaceOfDelivery.  # noqa: E501
 
-        Lehekülje suurus  # noqa: E501
 
         :return: The page_size of this PagedResultOfPlaceOfDelivery.  # noqa: E501
         :rtype: int
         """
         return self._page_size
 
     @page_size.setter
     def page_size(self, page_size):
         """Sets the page_size of this PagedResultOfPlaceOfDelivery.
 
-        Lehekülje suurus  # noqa: E501
 
         :param page_size: The page_size of this PagedResultOfPlaceOfDelivery.  # noqa: E501
         :type: int
         """
 
         self._page_size = page_size
 
     @property
     def page_result(self):
         """Gets the page_result of this PagedResultOfPlaceOfDelivery.  # noqa: E501
 
-        Lehekülje tulemused  # noqa: E501
 
         :return: The page_result of this PagedResultOfPlaceOfDelivery.  # noqa: E501
         :rtype: list[PlaceOfDelivery]
         """
         return self._page_result
 
     @page_result.setter
     def page_result(self, page_result):
         """Sets the page_result of this PagedResultOfPlaceOfDelivery.
 
-        Lehekülje tulemused  # noqa: E501
 
         :param page_result: The page_result of this PagedResultOfPlaceOfDelivery.  # noqa: E501
         :type: list[PlaceOfDelivery]
         """
 
         self._page_result = page_result
 
     @property
     def total_count(self):
         """Gets the total_count of this PagedResultOfPlaceOfDelivery.  # noqa: E501
 
-        Päringu vastete arv kokku  # noqa: E501
 
         :return: The total_count of this PagedResultOfPlaceOfDelivery.  # noqa: E501
         :rtype: int
         """
         return self._total_count
 
     @total_count.setter
     def total_count(self, total_count):
         """Sets the total_count of this PagedResultOfPlaceOfDelivery.
 
-        Päringu vastete arv kokku  # noqa: E501
 
         :param total_count: The total_count of this PagedResultOfPlaceOfDelivery.  # noqa: E501
         :type: int
         """
 
         self._total_count = total_count
```

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/paged_result_of_waybill.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/paged_result_of_waybill.py`

 * *Files 16% similar despite different names*

```diff
@@ -67,95 +67,87 @@
         if total_count is not None:
             self.total_count = total_count
 
     @property
     def page_number(self):
         """Gets the page_number of this PagedResultOfWaybill.  # noqa: E501
 
-        Lehekülje number  # noqa: E501
 
         :return: The page_number of this PagedResultOfWaybill.  # noqa: E501
         :rtype: int
         """
         return self._page_number
 
     @page_number.setter
     def page_number(self, page_number):
         """Sets the page_number of this PagedResultOfWaybill.
 
-        Lehekülje number  # noqa: E501
 
         :param page_number: The page_number of this PagedResultOfWaybill.  # noqa: E501
         :type: int
         """
 
         self._page_number = page_number
 
     @property
     def page_size(self):
         """Gets the page_size of this PagedResultOfWaybill.  # noqa: E501
 
-        Lehekülje suurus  # noqa: E501
 
         :return: The page_size of this PagedResultOfWaybill.  # noqa: E501
         :rtype: int
         """
         return self._page_size
 
     @page_size.setter
     def page_size(self, page_size):
         """Sets the page_size of this PagedResultOfWaybill.
 
-        Lehekülje suurus  # noqa: E501
 
         :param page_size: The page_size of this PagedResultOfWaybill.  # noqa: E501
         :type: int
         """
 
         self._page_size = page_size
 
     @property
     def page_result(self):
         """Gets the page_result of this PagedResultOfWaybill.  # noqa: E501
 
-        Lehekülje tulemused  # noqa: E501
 
         :return: The page_result of this PagedResultOfWaybill.  # noqa: E501
         :rtype: list[Waybill]
         """
         return self._page_result
 
     @page_result.setter
     def page_result(self, page_result):
         """Sets the page_result of this PagedResultOfWaybill.
 
-        Lehekülje tulemused  # noqa: E501
 
         :param page_result: The page_result of this PagedResultOfWaybill.  # noqa: E501
         :type: list[Waybill]
         """
 
         self._page_result = page_result
 
     @property
     def total_count(self):
         """Gets the total_count of this PagedResultOfWaybill.  # noqa: E501
 
-        Päringu vastete arv kokku  # noqa: E501
 
         :return: The total_count of this PagedResultOfWaybill.  # noqa: E501
         :rtype: int
         """
         return self._total_count
 
     @total_count.setter
     def total_count(self, total_count):
         """Sets the total_count of this PagedResultOfWaybill.
 
-        Päringu vastete arv kokku  # noqa: E501
 
         :param total_count: The total_count of this PagedResultOfWaybill.  # noqa: E501
         :type: int
         """
 
         self._total_count = total_count
```

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/place_of_delivery.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/place_of_delivery.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/previous_owner.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/previous_owner.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,16 +109,16 @@
 
         :param code: The code of this PreviousOwner.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and code is None:  # noqa: E501
             raise ValueError("Invalid value for `code`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                code is not None and len(code) > 32):
-            raise ValueError("Invalid value for `code`, length must be less than or equal to `32`")  # noqa: E501
+                code is not None and len(code) > 20):
+            raise ValueError("Invalid value for `code`, length must be less than or equal to `20`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 code is not None and len(code) < 0):
             raise ValueError("Invalid value for `code`, length must be greater than or equal to `0`")  # noqa: E501
 
         self._code = code
 
     @property
```

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/problem_details.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/problem_details.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,19 +60,23 @@
         self._title = None
         self._status = None
         self._detail = None
         self._instance = None
         self._extensions = None
         self.discriminator = None
 
-        self.type = type
-        self.title = title
+        if type is not None:
+            self.type = type
+        if title is not None:
+            self.title = title
         self.status = status
-        self.detail = detail
-        self.instance = instance
+        if detail is not None:
+            self.detail = detail
+        if instance is not None:
+            self.instance = instance
         if extensions is not None:
             self.extensions = extensions
 
     @property
     def type(self):
         """Gets the type of this ProblemDetails.  # noqa: E501
```

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/put_place_of_delivery_request.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/put_place_of_delivery_request.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/receiver.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/receiver.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/representer.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/representer.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/sales_contract.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/sales_contract.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/sales_contract_all_of.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/sales_contract_all_of.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/shipment.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/shipment.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/shipment_assortment.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/shipment_assortment.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/shipment_item.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/shipment_item.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/source.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/source.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/start_waybill_request.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/start_waybill_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,16 +315,16 @@
         :param pre_journey_mileage: The pre_journey_mileage of this StartWaybillRequest.  # noqa: E501
         :type: int
         """
         if (self.local_vars_configuration.client_side_validation and
                 pre_journey_mileage is not None and pre_journey_mileage > 100000):  # noqa: E501
             raise ValueError("Invalid value for `pre_journey_mileage`, must be a value less than or equal to `100000`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                pre_journey_mileage is not None and pre_journey_mileage < 1):  # noqa: E501
-            raise ValueError("Invalid value for `pre_journey_mileage`, must be a value greater than or equal to `1`")  # noqa: E501
+                pre_journey_mileage is not None and pre_journey_mileage < 0):  # noqa: E501
+            raise ValueError("Invalid value for `pre_journey_mileage`, must be a value greater than or equal to `0`")  # noqa: E501
 
         self._pre_journey_mileage = pre_journey_mileage
 
     @property
     def user_custom_data(self):
         """Gets the user_custom_data of this StartWaybillRequest.  # noqa: E501
```

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/transport.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/transport.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/transporter.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/transporter.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/unload_waybill_request.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/unload_waybill_request.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/validation_result.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/validation_result.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/viewer.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/viewer.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/waybill.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/waybill.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/waybill_authorization.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/waybill_authorization.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/waybill_note.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/waybill_note.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/waybill_note_creator.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/waybill_note_creator.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/waybill_place_of_delivery.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/waybill_place_of_delivery.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/waybill_sort_field.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/waybill_sort_field.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/waybill_status.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/waybill_status.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/without_forest_notice.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/without_forest_notice.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/models/without_forest_notice_all_of.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/models/without_forest_notice_all_of.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr/openapi_client/rest.py` & `pyevr-0.6.0.dev1/pyevr/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/pyevr.egg-info/PKG-INFO` & `pyevr-0.6.0.dev1/pyevr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyevr
-Version: 0.5.3.dev1
+Version: 0.6.0.dev1
 Summary: Python client for EVR
 Home-page: https://github.com/thorgate/pyevr
 Author: Thorgate
 Author-email: code@thorgate.eu
 License: MIT license
 Keywords: pyevr
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -59,26 +59,41 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =========
 Changelog
 =========
 
-0.5.3 (2023-06-07)
------------------------
+0.6.0.dev1
+----------
 
-**Compatibility**
+**Generic**
+
+* Change `all` method to be a generator instead of returning a list, to
+  allow data consumer to start consumption faster and avoid loading the
+  unnecessary pages if error happens early on
+* Add `deserialize_data` method that allows to rehydrate the model from
+  result of `sanitize_for_serialization` (allowing to store models as
+  json and similar use-cases)
+
+**Updates**
+
+Use EVR schema 1.9.0 from staging server
+
+* Support `WithoutForestNotice` holding base
+
+* Support `page_size` parameter for list endpoints
+
+* Support `last_modified_after` and `last_modified_before` for waybill list
 
-* Update to newest EVR schema
-* Remove workarounds that are no longer compatible with the schema
-* Fix issue with dockerized openapi generator causing out of memory error on arch linux
+* Support `waybill_latest_measurements` in waybill model
 
 
 0.5.2 (2022-04-06)
------------------------
+------------------
 
 **Generic**
 
 * Improve documentation
 
 **Compatibility**
```

### Comparing `pyevr-0.5.3.dev1/pyevr.egg-info/SOURCES.txt` & `pyevr-0.6.0.dev1/pyevr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyevr-0.5.3.dev1/setup.py` & `pyevr-0.6.0.dev1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-import pyevr
-
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('CHANGELOG.rst') as changelog_file:
     changelog = changelog_file.read()
 
 requirements = ['Click>=7.0', 'python-dateutil>=2.8.1', ]
 
 setup_requirements = ['pytest-runner', ]
 
 test_requirements = ['pytest>=5.3.0', ]
 
 setup(
-    author=pyevr.__author__,
-    author_email=pyevr.__email__,
+    author="Thorgate",
+    author_email="code@thorgate.eu",
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
@@ -46,10 +44,10 @@
     keywords='pyevr',
     name='pyevr',
     packages=find_packages(include=['pyevr', 'pyevr.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/thorgate/pyevr',
-    version=pyevr.__version__,
+    version="0.6.0.dev1",
     zip_safe=False,
 )
```

### Comparing `pyevr-0.5.3.dev1/tests/test_apis.py` & `pyevr-0.6.0.dev1/tests/test_apis.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,17 +47,17 @@
             index_increment = (page - 1) * 3
             return PagedResult(
                 page, 3, data[0 + index_increment:3 + index_increment], len(data),
             )
 
         api = AssortmentsAPI(self.client)
         api.assortments_list = Mock(side_effect=assortments_list)
-        self.assertListEqual(api.all(), data)
+        self.assertListEqual(list(api.all()), data)
         # Pass in a random page to make sure that it does not have any effect
-        self.assertListEqual(api.all(page=99), data)
+        self.assertListEqual(list(api.all(page=99)), data)
 
     def test_all_mixin(self):
         with self.assertRaises(ValueError):
             api = AssortmentsAPI(self.client)
             api.list_endpoint_attr = None
             api.get_list_endpoint()
```

### Comparing `pyevr-0.5.3.dev1/tests/test_main.py` & `pyevr-0.6.0.dev1/tests/test_main.py`

 * *Files identical despite different names*

