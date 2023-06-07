# Comparing `tmp/idem_gcp-0.9.0.tar.gz` & `tmp/idem_gcp-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem_gcp-0.9.0.tar", last modified: Mon Jan 30 20:38:26 2023, max compression
+gzip compressed data, was "idem_gcp-1.1.0.tar", last modified: Wed Jun  7 13:38:27 2023, max compression
```

## Comparing `idem_gcp-0.9.0.tar` & `idem_gcp-1.1.0.tar`

### file list

```diff
@@ -1,160 +1,201 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/
--rw-r--r--   0 root         (0) root         (0)    11342 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       43 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5598 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4481 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.506585 idem_gcp-0.9.0/idem_gcp/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/acct/gcp/
--rw-r--r--   0 root         (0) root         (0)      701 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/acct/gcp/basic_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/acct/gcp/contracts/
--rw-r--r--   0 root         (0) root         (0)      603 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/acct/gcp/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      230 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/acct/gcp/default_auth.py
--rw-r--r--   0 root         (0) root         (0)     1965 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/acct/gcp/init.py
--rw-r--r--   0 root         (0) root         (0)     2723 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/acct/gcp/service_account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/autogen/gcp/
--rw-r--r--   0 root         (0) root         (0)     9965 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/autogen/gcp/schema_parser.py
--rw-r--r--   0 root         (0) root         (0)       75 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/autogen/init.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/exec/gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/exec/gcp/None/
--rw-r--r--   0 root         (0) root         (0)       35 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/None/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/exec/gcp/None/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)      905 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/None/recursive_contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/
--rw-r--r--   0 root         (0) root         (0)     4317 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/crypto_key.py
--rw-r--r--   0 root         (0) root         (0)    10437 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/crypto_key_version.py
--rw-r--r--   0 root         (0) root         (0)     4307 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/import_job.py
--rw-r--r--   0 root         (0) root         (0)     3970 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/key_ring.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/location.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/
--rw-r--r--   0 root         (0) root         (0)     6938 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/accelerator_type.py
--rw-r--r--   0 root         (0) root         (0)    10875 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/disk.py
--rw-r--r--   0 root         (0) root         (0)     6779 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/disk_type.py
--rw-r--r--   0 root         (0) root         (0)     6909 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/firewall.py
--rw-r--r--   0 root         (0) root         (0)     5919 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/image.py
--rw-r--r--   0 root         (0) root         (0)    49348 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/instance.py
--rw-r--r--   0 root         (0) root         (0)     4937 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/machine_image.py
--rw-r--r--   0 root         (0) root         (0)     6812 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/machine_type.py
--rw-r--r--   0 root         (0) root         (0)    15643 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/network.py
--rw-r--r--   0 root         (0) root         (0)     6731 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/node_template.py
--rw-r--r--   0 root         (0) root         (0)     5997 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/reservation.py
--rw-r--r--   0 root         (0) root         (0)     6268 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/resource_policy.py
--rw-r--r--   0 root         (0) root         (0)     5130 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     3858 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/subnetwork.py
--rw-r--r--   0 root         (0) root         (0)     5612 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/zone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/exec/gcp/contracts/
--rw-r--r--   0 root         (0) root         (0)      501 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/exec/gcp/storage/
--rw-r--r--   0 root         (0) root         (0)     2644 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/storage/buckets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/exec/gcp_api/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp_api/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/helpers/
--rw-r--r--   0 root         (0) root         (0)      834 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/helpers/exc.py
--rw-r--r--   0 root         (0) root         (0)      785 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/helpers/log.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/helpers/returns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/metadata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/
--rw-r--r--   0 root         (0) root         (0)      187 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/
--rw-r--r--   0 root         (0) root         (0)      204 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/crypto_key_versions.py
--rw-r--r--   0 root         (0) root         (0)      244 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/import_jobs/
--rw-r--r--   0 root         (0) root         (0)      244 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/import_jobs/init.py
--rw-r--r--   0 root         (0) root         (0)      220 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/
--rw-r--r--   0 root         (0) root         (0)      183 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/accelerator_type.py
--rw-r--r--   0 root         (0) root         (0)      137 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/disk.py
--rw-r--r--   0 root         (0) root         (0)      155 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/disk_type.py
--rw-r--r--   0 root         (0) root         (0)      147 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/firewall.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/global_operation.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/image.py
--rw-r--r--   0 root         (0) root         (0)      153 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/instance.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/machine_image.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/machine_type.py
--rw-r--r--   0 root         (0) root         (0)      143 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/network.py
--rw-r--r--   0 root         (0) root         (0)      175 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/node_template.py
--rw-r--r--   0 root         (0) root         (0)      175 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/region_operation.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/reservation.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/resource_policy.py
--rw-r--r--   0 root         (0) root         (0)      100 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/snapshot.py
--rw-r--r--   0 root         (0) root         (0)      116 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/subnetwork.py
--rw-r--r--   0 root         (0) root         (0)      124 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/zone.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/zone_operation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/storage/
--rw-r--r--   0 root         (0) root         (0)      177 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/storage/buckets.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/storage/objectAccessControls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/resources/
--rw-r--r--   0 root         (0) root         (0)    12993 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/resources/properties.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/states/gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/
--rw-r--r--   0 root         (0) root         (0)    21701 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/crypto_key.py
--rw-r--r--   0 root         (0) root         (0)    30426 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/crypto_key_version.py
--rw-r--r--   0 root         (0) root         (0)    15172 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/import_job.py
--rw-r--r--   0 root         (0) root         (0)     6842 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/key_ring.py
--rw-r--r--   0 root         (0) root         (0)     2497 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/location.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/
--rw-r--r--   0 root         (0) root         (0)    36625 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/disk.py
--rw-r--r--   0 root         (0) root         (0)    22499 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/image.py
--rw-r--r--   0 root         (0) root         (0)    97834 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/instance.py
--rw-r--r--   0 root         (0) root         (0)    16492 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/machine_image.py
--rw-r--r--   0 root         (0) root         (0)    22046 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/network.py
--rw-r--r--   0 root         (0) root         (0)     9183 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/node_template.py
--rw-r--r--   0 root         (0) root         (0)     9207 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/reservation.py
--rw-r--r--   0 root         (0) root         (0)    17881 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/resource_policy.py
--rw-r--r--   0 root         (0) root         (0)    23692 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/snapshot.py
--rw-r--r--   0 root         (0) root         (0)    26026 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/subnetwork.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/states/gcp/storage/
--rw-r--r--   0 root         (0) root         (0)    11025 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/storage/buckets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/tool/gcp/
--rw-r--r--   0 root         (0) root         (0)     1132 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/case.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/tool/gcp/cloudkms/
--rw-r--r--   0 root         (0) root         (0)     5296 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/cloudkms/patch.py
--rw-r--r--   0 root         (0) root         (0)     2852 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/comment_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/tool/gcp/compute/
--rw-r--r--   0 root         (0) root         (0)     7282 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/compute/instance.py
--rw-r--r--   0 root         (0) root         (0)     4705 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/compute/network.py
--rw-r--r--   0 root         (0) root         (0)     3004 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/conversion_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/
--rw-r--r--   0 root         (0) root         (0)     1116 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/exec_context.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/exec_param.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/generic_exec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/post_exec/
--rw-r--r--   0 root         (0) root         (0)      677 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/post_exec/item_getter.py
--rw-r--r--   0 root         (0) root         (0)     2661 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/post_exec/operation_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/pre_exec/
--rw-r--r--   0 root         (0) root         (0)     1547 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/pre_exec/function_getter.py
--rw-r--r--   0 root         (0) root         (0)      908 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/pre_exec/resource_id_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)      244 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/recursive_contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      309 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/scope.py
--rw-r--r--   0 root         (0) root         (0)    21705 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/init.py
--rw-r--r--   0 root         (0) root         (0)     4762 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/operation_utils.py
--rw-r--r--   0 root         (0) root         (0)     1924 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/policy.py
--rw-r--r--   0 root         (0) root         (0)    11807 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/resolver.py
--rw-r--r--   0 root         (0) root         (0)    12626 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/resource_prop_utils.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/session.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/state_comparison_utils.py
--rw-r--r--   0 root         (0) root         (0)     8390 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-01-30 20:38:26.000000 idem_gcp-0.9.0/idem_gcp/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5598 2023-01-30 20:38:26.000000 idem_gcp-0.9.0/idem_gcp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4634 2023-01-30 20:38:26.000000 idem_gcp-0.9.0/idem_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-30 20:38:26.000000 idem_gcp-0.9.0/idem_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-01-30 20:38:26.000000 idem_gcp-0.9.0/idem_gcp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      236 2023-01-30 20:38:26.000000 idem_gcp-0.9.0/idem_gcp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-01-30 20:38:26.000000 idem_gcp-0.9.0/idem_gcp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3300 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)    11342 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7881 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6761 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/acct/gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/acct/gcp/contracts/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/acct/gcp/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/acct/gcp/service_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/autogen/gcp/
+-rw-r--r--   0 root         (0) root         (0)     9958 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/autogen/gcp/schema_parser.py
+-rw-r--r--   0 root         (0) root         (0)       75 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/autogen/init.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/exec/gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/
+-rw-r--r--   0 root         (0) root         (0)     4101 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/crypto_key.py
+-rw-r--r--   0 root         (0) root         (0)    10239 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/crypto_key_version.py
+-rw-r--r--   0 root         (0) root         (0)     4092 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/import_job.py
+-rw-r--r--   0 root         (0) root         (0)     3759 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/key_ring.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/location.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/
+-rw-r--r--   0 root         (0) root         (0)     6946 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/accelerator_type.py
+-rw-r--r--   0 root         (0) root         (0)     5866 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/backend_service.py
+-rw-r--r--   0 root         (0) root         (0)    16748 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/disk.py
+-rw-r--r--   0 root         (0) root         (0)     7479 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/disk_type.py
+-rw-r--r--   0 root         (0) root         (0)     6938 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/firewall.py
+-rw-r--r--   0 root         (0) root         (0)    10946 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/forwarding_rule.py
+-rw-r--r--   0 root         (0) root         (0)     5200 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/health_check.py
+-rw-r--r--   0 root         (0) root         (0)     5925 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/image.py
+-rw-r--r--   0 root         (0) root         (0)    49424 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/instance.py
+-rw-r--r--   0 root         (0) root         (0)    17133 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/instance_group.py
+-rw-r--r--   0 root         (0) root         (0)     4958 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/machine_image.py
+-rw-r--r--   0 root         (0) root         (0)     6819 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/machine_type.py
+-rw-r--r--   0 root         (0) root         (0)    15742 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/network.py
+-rw-r--r--   0 root         (0) root         (0)     7311 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/node_template.py
+-rw-r--r--   0 root         (0) root         (0)     5977 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/reservation.py
+-rw-r--r--   0 root         (0) root         (0)     6275 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/resource_policy.py
+-rw-r--r--   0 root         (0) root         (0)     7766 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     6381 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/subnetwork.py
+-rw-r--r--   0 root         (0) root         (0)     5810 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/target_pool.py
+-rw-r--r--   0 root         (0) root         (0)     5619 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/zone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/exec/gcp/contracts/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/exec/gcp/iam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/exec/gcp/iam/projects/
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/iam/projects/service_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/exec/gcp/iam/projects/service_accounts/
+-rw-r--r--   0 root         (0) root         (0)     7914 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/iam/projects/service_accounts/key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/exec/gcp/storage/
+-rw-r--r--   0 root         (0) root         (0)     4382 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/storage/bucket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/exec/gcp_api/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp_api/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/helpers/
+-rw-r--r--   0 root         (0) root         (0)      834 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/helpers/exc.py
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/helpers/log.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/helpers/returns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/metadata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/
+-rw-r--r--   0 root         (0) root         (0)      187 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/
+-rw-r--r--   0 root         (0) root         (0)      204 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/crypto_key_versions.py
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/import_jobs/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/import_jobs/init.py
+-rw-r--r--   0 root         (0) root         (0)      220 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/
+-rw-r--r--   0 root         (0) root         (0)      183 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/accelerator_type.py
+-rw-r--r--   0 root         (0) root         (0)      236 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/backend_service.py
+-rw-r--r--   0 root         (0) root         (0)      238 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/disk.py
+-rw-r--r--   0 root         (0) root         (0)      270 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/disk_type.py
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/firewall.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/forwarding_rule.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/global_operation.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/health_check.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/image.py
+-rw-r--r--   0 root         (0) root         (0)      153 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/instance.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/instance_group.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/machine_image.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/machine_type.py
+-rw-r--r--   0 root         (0) root         (0)      143 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/network.py
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/node_template.py
+-rw-r--r--   0 root         (0) root         (0)      204 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/region_backend_service.py
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/region_operation.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/reservation.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/resource_policy.py
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/subnetwork.py
+-rw-r--r--   0 root         (0) root         (0)      184 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/target_pool.py
+-rw-r--r--   0 root         (0) root         (0)      124 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/zone.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/zone_operation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/iam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/iam/projects/
+-rw-r--r--   0 root         (0) root         (0)      170 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/iam/projects/service_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/iam/projects/service_accounts/
+-rw-r--r--   0 root         (0) root         (0)      183 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/iam/projects/service_accounts/key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/storage/
+-rw-r--r--   0 root         (0) root         (0)      219 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/storage/bucket.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/storage/objectAccessControls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/resources/
+-rw-r--r--   0 root         (0) root         (0)    22734 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/resources/properties.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/states/gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/
+-rw-r--r--   0 root         (0) root         (0)    22050 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/crypto_key.py
+-rw-r--r--   0 root         (0) root         (0)    28486 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/crypto_key_version.py
+-rw-r--r--   0 root         (0) root         (0)    15728 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/import_job.py
+-rw-r--r--   0 root         (0) root         (0)     7639 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/key_ring.py
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/location.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/
+-rw-r--r--   0 root         (0) root         (0)    80631 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/backend_service.py
+-rw-r--r--   0 root         (0) root         (0)    26659 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/disk.py
+-rw-r--r--   0 root         (0) root         (0)    18532 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/firewall.py
+-rw-r--r--   0 root         (0) root         (0)    27433 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/forwarding_rule.py
+-rw-r--r--   0 root         (0) root         (0)    35690 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/health_check.py
+-rw-r--r--   0 root         (0) root         (0)    19067 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/image.py
+-rw-r--r--   0 root         (0) root         (0)    89687 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/instance.py
+-rw-r--r--   0 root         (0) root         (0)    13388 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/instance_group.py
+-rw-r--r--   0 root         (0) root         (0)    14687 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/machine_image.py
+-rw-r--r--   0 root         (0) root         (0)    22166 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/network.py
+-rw-r--r--   0 root         (0) root         (0)     6028 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/node_template.py
+-rw-r--r--   0 root         (0) root         (0)     6068 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/reservation.py
+-rw-r--r--   0 root         (0) root         (0)    14696 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/resource_policy.py
+-rw-r--r--   0 root         (0) root         (0)    17125 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    20411 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/subnetwork.py
+-rw-r--r--   0 root         (0) root         (0)     8550 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/target_pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/states/gcp/iam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/states/gcp/iam/projects/
+-rw-r--r--   0 root         (0) root         (0)    11923 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/iam/projects/service_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/states/gcp/iam/projects/service_accounts/
+-rw-r--r--   0 root         (0) root         (0)     9632 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/iam/projects/service_accounts/key.py
+-rw-r--r--   0 root         (0) root         (0)      144 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/states/gcp/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)    15853 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/recursive_contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/states/gcp/storage/
+-rw-r--r--   0 root         (0) root         (0)    40592 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/storage/bucket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/
+-rw-r--r--   0 root         (0) root         (0)     1800 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/case.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/cloudkms/
+-rw-r--r--   0 root         (0) root         (0)     5296 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/cloudkms/patch.py
+-rw-r--r--   0 root         (0) root         (0)     3953 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/comment_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/
+-rw-r--r--   0 root         (0) root         (0)     9834 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/disk.py
+-rw-r--r--   0 root         (0) root         (0)    11892 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/instance.py
+-rw-r--r--   0 root         (0) root         (0)      722 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/instance_group.py
+-rw-r--r--   0 root         (0) root         (0)     5276 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/network.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/subnetwork.py
+-rw-r--r--   0 root         (0) root         (0)     4000 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/conversion_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/exec_context.py
+-rw-r--r--   0 root         (0) root         (0)      533 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/exec_param.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/generic_exec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/post_exec/
+-rw-r--r--   0 root         (0) root         (0)      704 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/post_exec/item_getter.py
+-rw-r--r--   0 root         (0) root         (0)     2771 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/post_exec/operation_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/pre_exec/
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/pre_exec/function_getter.py
+-rw-r--r--   0 root         (0) root         (0)      522 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/pre_exec/parameter_sanitizer.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/pre_exec/resource_id_extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/recursive_contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      309 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/scope.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/hub_resolver.py
+-rw-r--r--   0 root         (0) root         (0)    21776 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/init.py
+-rw-r--r--   0 root         (0) root         (0)     5614 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/operation_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/policy.py
+-rw-r--r--   0 root         (0) root         (0)    18555 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/resolver.py
+-rw-r--r--   0 root         (0) root         (0)    18698 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/resource_prop_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/sanitizers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/schema/
+-rw-r--r--   0 root         (0) root         (0)      874 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/schema/finding.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/schema/results_collector.py
+-rw-r--r--   0 root         (0) root         (0)     2725 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/schema/schema_compatibility_checker.py
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/schema/schema_naming_checker.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/schema/scm_utils.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/session.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/state_comparison_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/state_operation_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/storage/
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/storage/bucket.py
+-rw-r--r--   0 root         (0) root         (0)    19738 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-07 13:38:26.000000 idem_gcp-1.1.0/idem_gcp/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7881 2023-06-07 13:38:27.000000 idem_gcp-1.1.0/idem_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6140 2023-06-07 13:38:27.000000 idem_gcp-1.1.0/idem_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 13:38:27.000000 idem_gcp-1.1.0/idem_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-07 13:38:27.000000 idem_gcp-1.1.0/idem_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-07 13:38:27.000000 idem_gcp-1.1.0/idem_gcp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-07 13:38:27.000000 idem_gcp-1.1.0/idem_gcp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3303 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/setup.py
```

### Comparing `idem_gcp-0.9.0/LICENSE` & `idem_gcp-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.9.0/PKG-INFO` & `idem_gcp-1.1.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,22 @@
-Metadata-Version: 2.1
-Name: idem_gcp
-Version: 0.9.0
-Summary: GCP Cloud Provider for Idem
-Home-page: https://gitlab.com/vmware/idem/idem-gcp
-Author: VMware, Inc.
-Author-email: idemproject@vmware.com
-License: Apache Software License 2.0
-Project-URL: Code, https://gitlab.com/vmware/idem/idem-gcp
-Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-gcp/issues
-Platform: UNKNOWN
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: full
-Provides-Extra: autogen
-License-File: LICENSE
-
 ========
 idem-gcp
 ========
 
 .. image:: https://img.shields.io/badge/made%20with-pop-teal
    :alt: Made with pop, a Python implementation of Plugin Oriented Programming
    :target: https://pop.readthedocs.io/
 
 .. image:: https://img.shields.io/badge/made%20with-idem-teal
    :alt: Made with idem, a Python implementation of Plugin Oriented Programming
    :target: https://www.idemproject.io/
 
 .. image:: https://img.shields.io/badge/docs%20on-docs.idemproject.io-blue
    :alt: Documentation is published with Sphinx on docs.idemproject.io
-   :target: https://docs.idemproject.io/idem-aws/en/latest/index.html
+   :target: https://docs.idemproject.io/idem-gcp/en/latest/index.html
 
 .. image:: https://img.shields.io/badge/made%20with-python-yellow
    :alt: Made with Python
    :target: https://www.python.org/
 
 GCP Cloud Provider for Idem.
 
@@ -82,22 +53,47 @@
 
 * `Idem Project Website <https://www.idemproject.io/>`__
 * `Idem Project docs portal <https://docs.idemproject.io/>`__
 
 Getting Started
 ===============
 
-DEVELOPMENT
-===========
+Prerequisites
+-------------
+
+* Python 3.8+
+* git *(if installing from source, or contributing to the project)*
+
+Installation
+------------
+
+.. note::
+
+   If wanting to contribute to the project, and setup your local development
+   environment, see the ``CONTRIBUTING.rst`` document in the source repository
+   for this project.
 
-Clone the `idem_gcp` repository and install with pip.
+If wanting to use ``idem-gcp``, you can do so by either
+installing from PyPI or from source.
+
+Install from PyPI
++++++++++++++++++
+
+.. code-block:: bash
+
+  pip install idem-gcp
+
+Install from source
++++++++++++++++++++
+
+Clone the `idem_gcp` repository.
 
 .. code:: bash
 
-    git clone git@gitlab.com:my-user/idem_gcp.git
+    git clone git@gitlab.com:vmware/idem/idem-gcp.git
     cd idem_gcp
 
 Create a virtual environment, and then activate it:
 
 .. code:: bash
 
     python3 -m venv venv
@@ -113,80 +109,102 @@
 
 Install the following packages in order to run the tests:
 
 .. code:: bash
 
     pip3 install -r requirements/py3.10/tests.txt
 
-**NOTE:**  Change py3.10 if needed with your  Python version. There is support for py3.7, py3.8, py3.9 and py3.10.
+**NOTE:**  Change py3.10 if needed with your  Python version. There is support for py3.8, py3.9, py3.10 and py3.11.
 
-ACCT
-====
+Setup
+=====
 
-After installation gcp Idem Provider execution and state modules will be accessible to the pop `hub`.
+After installation GCP Idem Provider execution and state modules will be accessible to the pop `hub`.
 In order to use them we need to set up our credentials.
 
-Create a new file called `credentials.yaml` and populate it with profiles.
-The `default` profile will be used automatically by `idem` unless you specify one with `--acct-profile=profile_name` on the cli.
+Create a new file called `credentials.yaml` and populate it with your credential profiles.
 
-`acct backends <https://gitlab.com/saltstack/pop/acct-backends>`_ provide alternate methods for storing profiles.
-
-The gcp provider uses the gcp acct plugin for authentication.
-A profile needs to specify the authentication parameters for gcp.
+To provide your GCP credentials in the file, use the "gcp" provider key.
+Under that key, add different profiles as needed.
+A profile specifies authentication parameters for GCP.
+The `default` profile will be automatically used by `idem`,
+but the other ones could be explicitly specified for each run or SLS file.
+This is done through the `--acct-profile` `idem` cli flag or the
+`acct_profile` SLS property.
+
+There is currently one GCP authentication mechanism supported by idem-gcp -
+providing service account keys.
+The following example gives the overall structure of the authentication
+parameters' expected format.
 
 credentials.yaml
 
 ..  code:: sls
 
     gcp:
       default:
-        username: my_user
-        password: my_good_password
-        endpoint_url: https://console.gcp.com/api
+        type: service_account
+        project_id: “<project>”
+        private_key_id: “<key_id>”
+        private_key: |
+          -----BEGIN PRIVATE KEY-----
+          <private_key>
+          ——END PRIVATE KEY-----
+        client_email: “<service_account_email>“
+        client_id: “<client_id>”
+        auth_uri: https://accounts.google.com/o/oauth2/auth
+        token_uri: https://oauth2.googleapis.com/token
+        auth_provider_x509_cert_url: https://www.googleapis.com/oauth2/v1/certs
+        client_x509_cert_url: “<certificate_url>“
+        universe_domain: googleapis.com
+      <other_profile_name>:
+        ...
+
+The values of these parameters can be obtained through the GCP console after creating a service account and generating a service account key in JSON format.
+Be sure to assign appropriate roles for the service account, such that it has the rights to access and manage the needed resources.
+For a better security posture, follow the principal of least privilege and do not use service accounts with excessive rights.
+For more information on the authentication parameters used, refer to the `Credentials <https://google-auth.readthedocs.io/en/master/reference/google.oauth2.service_account.html#google.oauth2.service_account.Credentials>`_ docs.
 
-Now encrypt the credentials file and add the encryption key and encrypted file path to the ENVIRONMENT.
+Encrypt the created credentials file:
 
-The `acct` command should be available as it is a requisite of `idem` and `idem_gcp`.
-Encrypt the the credential file.
 
 .. code:: bash
 
     acct encrypt credentials.yaml
 
-output::
 
-    -A9ZkiCSOjWYG_lbGmmkVh4jKLFDyOFH4e4S1HNtNwI=
+The output of this command is the ACCT_KEY which needs to be securely stored.
+A `credentials.yaml.fernet` encrypted file is also created in the working directory, whose path should be used as ACCT_FILE.
+These could be given to idem either through environment variables or directly as `idem` run parameters.
 
-Add these to your environment:
+Setting environment variables
+-----------------------------
 
 .. code:: bash
 
-    export ACCT_KEY="-A9ZkiCSOjWYG_lbGmmkVh4jKLFDyOFH4e4S1HNtNwI="
+    export ACCT_KEY="<ACCT_KEY>"
     export ACCT_FILE=$PWD/credentials.yaml.fernet
 
-
-USAGE
-=====
-A profile can be specified for use with a specific state.
-If no profile is specified, the profile called "default", if one exists, will be used:
-
-.. code:: sls
-
-    ensure_user_exists:
-      gcp.user.present:
-        - acct_profile: my-staging-env
-        - name: a_user_name
-        - kwarg1: val1
-
-It can also be specified from the command line when executing states.
+Providing acct parameters to the idem run
+-----------------------------------------
 
 .. code:: bash
 
-    idem state --acct-profile my-staging-env my_state.sls
+    idem <subcommand> --acct-key "<ACCT_KEY>" --acct-file "$PWD/credentials.yaml.fernet" --acct-profile "<profile_name>"
 
-It can also be specified from the command line when calling an exec module directly.
+Specifying account profile in SLS files
+---------------------------------------
 
-.. code:: bash
+.. code:: sls
+
+    ensure_resource:
+      gcp.<service>.<resource>.present:
+        - acct_profile: <profile_name>
+        - name: resource_name
+        - kwarg1: val1
 
-    idem exec --acct-profile my-staging-env gcp.user.list
 
+For more information on the Idem ACCT authentication management subsystem, refer to the following resources:
 
+* `Account credentials file doc <https://docs.idemproject.io/idem/en/latest/topics/tutorials/acct_file.html>`_
+* `Multiple Account Management <https://docs.idemproject.io/idem/en/latest/topics/tutorials/acct.html>`_
+* `ACCT advanced features <https://docs.idemproject.io/idem/en/latest/topics/sls_acct.html>`_
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `idem_gcp-0.9.0/idem_gcp/acct/gcp/contracts/init.py` & `idem_gcp-1.1.0/idem_gcp/acct/gcp/contracts/init.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.9.0/idem_gcp/acct/gcp/service_account.py` & `idem_gcp-1.1.0/idem_gcp/acct/gcp/service_account.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 # SPDX-License-Identifier: Apache-2.0
 from typing import Any
 from typing import Dict
 
 try:
     from google.oauth2.service_account import Credentials as Oauth2Credentials
 
-    import google.auth._service_account_info as service_account_info
-
     HAS_LIBS = (True,)
 except ImportError as e:
     HAS_LIBS = False, str(e)
 
 
 def __virtual__(hub):
     return HAS_LIBS
@@ -47,21 +45,12 @@
               client_id: "xxxxxxxxxxxxxxxxxxxxx"
               auth_uri: "https://accounts.google.com/o/oauth2/auth"
               token_uri: "https://oauth2.googleapis.com/token"
               auth_provider_x509_cert_url: "https://www.googleapis.com/oauth2/v1/certs"
               client_x509_cert_url: "https://www.googleapis.com/robot/v1/metadata/x509/idem-gcp%40example.com.iam.gserviceaccount.com"
     """
     sub_profiles = {}
-    credentials = {}
     for profile, creds in profiles.get("gcp", {}).items():
-        signer = service_account_info.from_dict(
-            creds, require=["client_email", "token_uri"]
-        )
-        credentials = Oauth2Credentials(
-            signer,
-            service_account_email=creds["client_email"],
-            token_uri=creds["token_uri"],
-            project_id=creds["project_id"],
-        )
+        credentials = Oauth2Credentials.from_service_account_info(creds)
         sub_profiles[profile] = {"credentials": credentials}
 
     return sub_profiles
```

### Comparing `idem_gcp-0.9.0/idem_gcp/autogen/gcp/schema_parser.py` & `idem_gcp-1.1.0/idem_gcp/autogen/gcp/schema_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,14 @@
 def parse_resource_prop(
     hub,
     resource_prop: ResourceProperty,
     schemas: Dict[str, ResourceSchema],
     parsed_schemas: Dict[str, CloudSpecParam],
     name: str = None,
 ) -> CloudSpecParam:
-
     if not name:
         name = "unknown"
     # name is known only in the wrapper context - enclosing type field name or top level parameter name
     result = CloudSpecParam(
         name=name, required=False, target="kwargs", target_type="mapping", doc=""
     )
 
@@ -289,12 +288,12 @@
         }
     if isinstance(schema, list):
         return [hub.autogen.gcp.schema_parser.sanitize_schema(item) for item in schema]
     return schema
 
 
 def sanitize_key(hub, key: str) -> str:
-    return hub.tool.format.keyword.unclash(hub.tool.gcp.case.snake(key))
+    return hub.tool.gcp.case.unclash(hub.tool.gcp.case.snake(key))
 
 
 def _generate_random_classname() -> str:
     return "Class" + str(uuid.uuid4()).replace("-", "")
```

### Comparing `idem_gcp-0.9.0/idem_gcp/conf.py` & `idem_gcp-1.1.0/idem_gcp/conf.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/crypto_key.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/crypto_key.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             ),
         )
 
     return result
 
 
 async def list_(
-    hub, ctx, key_ring: str, filter: str = None, order_by: str = None
+    hub, ctx, key_ring: str, filter_: (str, "alias=filter") = None, order_by: str = None
 ) -> Dict[str, Any]:
     r"""Retrieves the crypto keys in a key ring.
 
     Args:
         key_ring(str):
             key ring resource_id.
 
@@ -116,25 +116,17 @@
     result = {
         "comment": [],
         "ret": [],
         "result": True,
     }
 
     crypto_keys = await hub.exec.gcp_api.client.cloudkms.projects.locations.key_rings.crypto_keys.list(
-        ctx, parent=key_ring, filter=filter, orderBy=order_by
+        ctx, parent=key_ring, filter=filter_, orderBy=order_by
     )
     if not crypto_keys["result"]:
         result["comment"] += crypto_keys["comment"]
         result["result"] = False
         return result
 
-    if crypto_keys["ret"].get("items"):
-        result["ret"].extend(crypto_keys["ret"]["items"])
-
-    if not result["ret"]:
-        result["comment"] += (
-            hub.tool.gcp.comment_utils.list_empty_comment(
-                "gcp.cloudkms.crypto_key", key_ring
-            ),
-        )
+    result["ret"] = crypto_keys["ret"].get("items", [])
 
     return result
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/crypto_key_version.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/crypto_key_version.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,21 +59,25 @@
             ),
         )
 
     return result
 
 
 async def list_(
-    hub, ctx, crypto_key: str, filter: str = None, order_by: str = None
+    hub,
+    ctx,
+    crypto_key: str,
+    filter_: (str, "alias=filter") = None,
+    order_by: str = None,
 ) -> Dict[str, Any]:
     r"""Retrieves the crypto key versions in a crypto key.
 
     Args:
         crypto_key(str):
-            key ring resource_id.
+            crypto key resource_id.
 
         filter(str, Optional):
             Only include resources that match the filter in the response. For more information, see
             `Sorting and filtering list results`_.
 
         order_by(str, Optional):
             Specify how the results should be sorted. If not specified, the results will be sorted in the default order.
@@ -85,39 +89,31 @@
         .. code-block:: sls
 
             list-crypto-key_versions-filtered:
                 exec.run:
                    - path: gcp.cloudkms.crypto_key_version.list
                    - kwargs:
                          crypto_key: projects/project-name/locations/global/keyRings/kr-global-test
-                         filter: algorithm = GOOGLE_SYMMETRIC_ENCRYPTION
+                         filter_: algorithm = GOOGLE_SYMMETRIC_ENCRYPTION
     """
     result = {
         "comment": [],
         "ret": [],
         "result": True,
     }
 
     crypto_key_versions = await hub.exec.gcp_api.client.cloudkms.projects.locations.key_rings.crypto_keys.crypto_key_versions.list(
-        ctx, parent=crypto_key, filter=filter, orderBy=order_by
+        ctx, parent=crypto_key, filter=filter_, orderBy=order_by
     )
     if not crypto_key_versions["result"]:
         result["comment"] += crypto_key_versions["comment"]
         result["result"] = False
         return result
 
-    if crypto_key_versions["ret"].get("items"):
-        result["ret"].extend(crypto_key_versions["ret"]["items"])
-
-    if not result["ret"]:
-        result["comment"] += (
-            hub.tool.gcp.comment_utils.list_empty_comment(
-                "gcp.cloudkms.crypto_key_version", crypto_key
-            ),
-        )
+    result["ret"] = crypto_key_versions["ret"].get("items", [])
 
     return result
 
 
 async def import_(
     hub,
     ctx,
@@ -127,42 +123,45 @@
     algorithm: str,
     key_material: str,
     crypto_key_version: str = None,
 ) -> Dict[str, Any]:
     r"""Import key material in crypto key version.
 
     Args:
-        parent:
+        parent(str):
             Required. The Idem resource_id of the `CryptoKey`_ to be imported into.
             The create permission is only required on this key when creating a new `CryptoKeyVersion`_.
             Authorization requires the following `IAM`_ permission on the specified resource parent:
-                - cloudkms.cryptoKeyVersions.create
-        import_job:
+
+            - cloudkms.cryptoKeyVersions.create
+        import_job(str):
             Required. Idem resource_id of the import job to be used.
-        import_job_pub_key:
+        import_job_pub_key(str):
             Required. PEM encoded public key of the import job to be used to wrap this key material.
             Authorization requires the following `IAM`_ permission on the specified resource import_job:
-                - cloudkms.importjobs.useToImport
-        algorithm:
+
+            - cloudkms.importjobs.useToImport
+        algorithm(str):
             Required. The `algorithm`_ of the key being imported. This does not need to match the `versionTemplate`_ of the
             `CryptoKey`_ this version imports into.
-        key_material:
+        key_material(str):
             Base64 encoded key material. If importing symmetric key material, it is expected that the key contains
             plain bytes. If importing asymmetric key material, it is expected that the key is in
             PKCS#8-encoded DER format (the PrivateKeyInfo structure from RFC 5208).
         crypto_key_version(str, Optional):
             The optional Idem resource_id of an existing `CryptoKeyVersion`_ to target for an import operation. If this field is
             not present, a new `CryptoKeyVersion`_ containing the supplied key material is created.
             If this field is present, the supplied key material is imported into the existing `CryptoKeyVersion`_. To
             import into an existing `CryptoKeyVersion`_, the `CryptoKeyVersion`_ must be a child of
             `ImportCryptoKeyVersionRequest.parent`_, have been previously created via [cryptoKeyVersions.import][], and
             be in `DESTROYED`_ or `IMPORT_FAILED`_ state. The key material and algorithm must match the previous
             `CryptoKeyVersion`_ exactly if the `CryptoKeyVersion`_ has ever contained key material.
             Authorization requires the following `IAM`_ permission on the specified resource cryptoKeyVersion:
-                - cloudkms.cryptoKeyVersions.update
+
+            - cloudkms.cryptoKeyVersions.update
 
     .. _CryptoKeyVersion: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys.cryptoKeyVersions#CryptoKeyVersion
     .. _name: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys.cryptoKeyVersions#CryptoKeyVersion.FIELDS.name
     .. _ImportCryptoKeyVersionRequest.parent: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys.cryptoKeyVersions/import#body.PATH_PARAMETERS.parent
     .. _DESTROYED: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys.cryptoKeyVersions#CryptoKeyVersion.CryptoKeyVersionState.ENUM_VALUES.DESTROYED
     .. _IMPORT_FAILED: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys.cryptoKeyVersions#CryptoKeyVersion.CryptoKeyVersionState.ENUM_VALUES.IMPORT_FAILED
     .. _IAM: https://cloud.google.com/iam/docs/
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/import_job.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/import_job.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             ),
         )
 
     return result
 
 
 async def list_(
-    hub, ctx, key_ring: str, filter: str = None, order_by: str = None
+    hub, ctx, key_ring: str, filter_: (str, "alias=filter") = None, order_by: str = None
 ) -> Dict[str, Any]:
     r"""Retrieves import jobs in a key ring.
 
     Args:
         key_ring(str):
             key ring resource_id.
 
@@ -107,34 +107,26 @@
             #!END
 
             list-import-jobs-filtered:
                 exec.run:
                    - path: gcp.cloudkms.import_job.list
                    - kwargs:
                          key_ring: projects/project-name/locations/global/keyRings/kr-global-test
-                         filter: expireTime < 2023-10-02
+                         filter_: expireTime < 2023-10-02
     """
     result = {
         "comment": [],
         "ret": [],
         "result": True,
     }
 
     import_jobs = await hub.exec.gcp_api.client.cloudkms.projects.locations.key_rings.import_jobs.list(
-        ctx, parent=key_ring, filter=filter, orderBy=order_by
+        ctx, parent=key_ring, filter=filter_, orderBy=order_by
     )
     if not import_jobs["result"]:
         result["comment"] += import_jobs["comment"]
         result["result"] = False
         return result
 
-    if import_jobs["ret"].get("items"):
-        result["ret"].extend(import_jobs["ret"]["items"])
-
-    if not result["ret"]:
-        result["comment"] += (
-            hub.tool.gcp.comment_utils.list_empty_comment(
-                "gcp.cloudkms.crypto_key", key_ring
-            ),
-        )
+    result["ret"] = import_jobs["ret"].get("items", [])
 
     return result
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/key_ring.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/key_ring.py`

 * *Files 20% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             ),
         )
 
     return result
 
 
 async def list_(
-    hub, ctx, location: str, filter: str = None, order_by: str = None
+    hub, ctx, location: str, filter_: (str, "alias=filter") = None, order_by: str = None
 ) -> Dict[str, Any]:
     r"""Retrieves key rings under specific location.
 
     Args:
         location(str):
             Location ID to be searched for key rings.
 
@@ -99,37 +99,29 @@
             #!END
 
             list-global-key-rings:
                 exec.run:
                    - path: gcp.cloudkms.key_ring.list
                    - kwargs:
                          location: projects/project-name/locations/global
-                         filter: NOT name=projects/project-name/locations/global/keyRings/kr-global-test
+                         filter_: NOT name=projects/project-name/locations/global/keyRings/kr-global-test
     """
     result = {
         "comment": [],
         "ret": [],
         "result": True,
     }
 
     key_rings = (
         await hub.exec.gcp_api.client.cloudkms.projects.locations.key_rings.list(
-            ctx, parent=location, filter=filter, orderBy=order_by
+            ctx, parent=location, filter=filter_, orderBy=order_by
         )
     )
 
     if not key_rings["result"]:
         result["comment"] += key_rings["comment"]
         result["result"] = False
         return result
 
-    if key_rings["ret"].get("items"):
-        result["ret"].extend(key_rings["ret"]["items"])
-
-    if not result["ret"]:
-        result["comment"] += (
-            hub.tool.gcp.comment_utils.list_empty_comment(
-                "gcp.cloudkms.key_ring", location
-            ),
-        )
+    result["ret"] = key_rings["ret"].get("items", [])
 
     return result
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/location.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/location.py`

 * *Files 16% similar despite different names*

```diff
@@ -54,15 +54,17 @@
                 "gcp.cloudkms.location", resource_id
             ),
         )
 
     return result
 
 
-async def list_(hub, ctx, project: str = None, filter: str = None) -> Dict[str, Any]:
+async def list_(
+    hub, ctx, project: str = None, filter_: (str, "alias=filter") = None
+) -> Dict[str, Any]:
     r"""Retrieves the locations for a specific project.
 
     Args:
         project(str, Optional):
             Project ID for this request. If not provided will use the one configured in `ctx`
 
         filter(str, Optional):
@@ -88,26 +90,18 @@
 
     if project:
         name = f"projects/{project}"
     else:
         name = f"projects/{ctx.acct.project_id}"
 
     locations = await hub.exec.gcp_api.client.cloudkms.projects.locations.list(
-        ctx, _name=name, filter=filter
+        ctx, _name=name, filter=filter_
     )
 
     if not locations["result"]:
         result["comment"] += locations["comment"]
         result["result"] = False
         return result
 
-    if locations["ret"].get("items"):
-        result["ret"] = locations["ret"]["items"]
-
-    if not result["ret"]:
-        result["comment"] += (
-            hub.tool.gcp.comment_utils.list_empty_comment(
-                "gcp.cloudkms.location", name
-            ),
-        )
+    result["ret"] = locations["ret"].get("items", [])
 
     return result
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/accelerator_type.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/accelerator_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """Exec module for managing Accelerator Types."""
 from typing import Any
 from typing import Dict
 
-from idem_gcp.tool.gcp.utils import get_project_from_account
-
 __func_alias__ = {"list_": "list"}
 
 
 async def list_(
     hub,
     ctx,
     project: str = None,
     zone: str = None,
-    filter: str = None,
+    filter_: (str, "alias=filter") = None,
     order_by: str = None,
     include_all_scopes: bool = None,
 ) -> Dict[str, Any]:
     r"""Retrieves a list of accelerator types that are available to the specified project.
 
     Args:
         project(str, Optional):
@@ -31,51 +29,51 @@
         order_by(str, Optional):
             Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
 
         include_all_scopes(bool, Optional):
             Indicates whether every visible scope for each scope type (zone, region, global) should be included in the response. For new resource types added after this field, the flag has no effect as new resource types will always include every visible scope for each scope type in response. For resource types which predate this field, if this flag is omitted or false, only scopes of the scope types where the resource type is expected to be found will be included.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.accelerator_type.list
               - kwargs:
                   project: project-name
                   zone: zone-name
-                  filter: id=1
+                  filter_: id=1
     """
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     result = dict(comment=[], ret=[], result=True)
 
     if zone and not include_all_scopes:
         ret = await hub.exec.gcp_api.client.compute.accelerator_type.list(
             ctx,
             project=project,
             zone=zone,
-            filter=filter,
+            filter=filter_,
             orderBy=order_by,
         )
     else:
         ret = await hub.exec.gcp_api.client.compute.accelerator_type.aggregatedList(
             ctx,
             project=project,
-            filter=filter,
+            filter=filter_,
             orderBy=order_by,
             includeAllScopes=include_all_scopes,
         )
 
     if not ret["result"]:
         result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
-    result["ret"] = ret["ret"]["items"]
+    result["ret"] = ret["ret"].get("items", [])
     result["comment"] += ret["comment"]
     return result
 
 
 async def get(
     hub,
     ctx,
@@ -97,25 +95,25 @@
         project(str, Optional):
             Project ID for this request.
 
         zone(str, Optional):
             The name of the zone for this request.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.accelerator_type.get
               - kwargs:
                   name: accelerator-type-name
                   project: project-name
                   zone: zone-name
     """
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     result = dict(comment=[], ret=[], result=True)
 
     if resource_id:
         ret = await hub.exec.gcp_api.client.compute.accelerator_type.get(
             ctx,
             resource_id=resource_id,
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/disk.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/disk_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,248 +1,164 @@
-"""Exec module for managing Disks."""
-__func_alias__ = {"list_": "list"}
-
-from dataclasses import make_dataclass, field
-from typing import Dict, Any, List
+"""Exec module for managing Disk Types."""
+from typing import Any
+from typing import Dict
 
-from idem_gcp.tool.gcp.generate.exec_context import ExecutionContext
-from idem_gcp.tool.gcp.utils import get_project_from_account
+__func_alias__ = {"list_": "list"}
 
 
 async def list_(
     hub,
     ctx,
     project: str = None,
     zone: str = None,
-    filter: str = None,
+    region: str = None,
+    filter_: (str, "alias=filter") = None,
     order_by: str = None,
-):
-    r"""Retrieves a list of persistent disks contained within the specified zone.
+    include_all_scopes: bool = False,
+) -> Dict[str, Any]:
+    r"""Retrieves a list of disk types available to the specified project.
 
     Args:
         project(str, Optional):
             Project ID for this request.
 
         zone(str, Optional):
             The name of the zone for this request.
 
+        region(str, Optional):
+            The name of the region for this request.
+
         filter(str, Optional):
-            A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name "instance", you would use `name ne .*instance`.
+            A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name \"instance\", you would use `name ne .*instance`.
 
         order_by(str, Optional):
             Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
 
+        include_all_scopes(bool, Optional):
+            Indicates whether every visible scope for each scope type (zone, region, global) should be included in the response. For new resource types added after this field, the flag has no effect as new resource types will always include every visible scope for each scope type in response. For resource types which predate this field, if this flag is omitted or false, only scopes of the scope types where the resource type is expected to be found will be included.
+
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.disk.list
+              - path: gcp.compute.disk_type.list
               - kwargs:
                   project: project-name
-                  zone: zone-name
     """
-    result = {
-        "comment": [],
-        "ret": None,
-        "result": True,
-    }
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
+
+    result = dict(comment=[], ret=[], result=True)
 
-    if zone:
-        ret = await hub.exec.gcp_api.client.compute.disk.list(
+    if zone and not include_all_scopes:
+        ret = await hub.exec.gcp_api.client.compute.disk_type.list(
             ctx,
             project=project,
             zone=zone,
-            filter=filter,
+            filter=filter_,
+            orderBy=order_by,
+        )
+    elif region and not include_all_scopes:
+        ret = await hub.exec.gcp_api.client.compute.disk_type.list(
+            ctx,
+            project=project,
+            region=region,
+            filter=filter_,
             orderBy=order_by,
         )
     else:
-        ret = await hub.exec.gcp_api.client.compute.disk.aggregatedList(
+        ret = await hub.exec.gcp_api.client.compute.disk_type.aggregatedList(
             ctx,
             project=project,
-            filter=filter,
+            filter=filter_,
             orderBy=order_by,
+            includeAllScopes=include_all_scopes,
         )
 
     if not ret["result"]:
         result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
-    result["ret"] = ret["ret"]["items"]
+    result["ret"] = ret["ret"].get("items", [])
+    result["comment"] += ret["comment"]
     return result
 
 
 async def get(
     hub,
     ctx,
+    name: str = None,
     project: str = None,
     zone: str = None,
-    name: str = None,
+    region: str = None,
     resource_id: str = None,
 ):
-    r"""Returns a specified persistent disk.
-
-    Use an un-managed disk as a data-source. Supply one of the inputs as the filter.
-    Gets a list of available persistent disks by making a list() request.
+    r"""Returns the specified disk type.
 
     Args:
+        resource_id(str, Optional):
+            An identifier of the resource in the provider.
+            Defaults to None.
+
+        name(str, Optional):
+            Name of the machine type to return.
+
         project(str, Optional):
-            Project ID for this request. Defaults to None.
+            Project ID for this request.
 
         zone(str, Optional):
-            The name of the zone for this request. Defaults to None.
-
-        name(str, Optional):
-            Name of the persistent disk to return. Defaults to None.
+            The name of the zone for this request.
 
-        resource_id(str, Optional):
-            An identifier of the resource in the provider. Defaults to None.
+        region(str, Optional):
+            The name of the region for this request.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.disk.get
+              - path: gcp.compute.disk_type.get
               - kwargs:
-                  disk: disk-name
+                  name: disk-type-name
                   project: project-name
                   zone: zone-name
     """
-    result = {
-        "comment": [],
-        "ret": None,
-        "result": True,
-    }
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
+
+    result = dict(comment=[], ret=[], result=True)
 
     if resource_id:
-        ret = await hub.exec.gcp_api.client.compute.disk.get(
+        ret = await hub.exec.gcp_api.client.compute.disk_type.get(
             ctx,
             resource_id=resource_id,
         )
     elif project and zone and name:
-        ret = await hub.exec.gcp_api.client.compute.disk.get(
-            ctx, project=project, zone=zone, disk=name
+        ret = await hub.exec.gcp_api.client.compute.disk_type.get(
+            ctx,
+            project=project,
+            zone=zone,
+            diskType=name,
+        )
+    elif project and region and name:
+        ret = await hub.exec.gcp_api.client.compute.disk_type.get(
+            ctx,
+            project=project,
+            region=region,
+            diskType=name,
         )
     else:
         result["result"] = False
         result["comment"] = [
-            f"gcp.compute.disk#get(): {name} either resource_id or project, zone and name"
+            f"gcp.compute.disk_type {name} either resource_id or project, zone/region and name"
             f" should be specified."
         ]
         return result
 
-    result["comment"] += ret["comment"]
     if not ret["result"]:
+        result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
     result["ret"] = ret["ret"]
+    result["comment"] += ret["comment"]
     return result
-
-
-async def create_snapshot(
-    hub,
-    ctx,
-    name: str,
-    project: str = None,
-    zone: str = None,
-    disk: str = None,
-    resource_id: str = None,
-    storage_locations: List[str] = None,
-    location_hint: str = None,
-    label_fingerprint: str = None,
-    description: str = None,
-    labels: Dict[str, Any] = None,
-    source_disk_encryption_key: make_dataclass(
-        "CustomerEncryptionKey",
-        [
-            ("kms_key_service_account", str, field(default=None)),
-            ("sha256", str, field(default=None)),
-            ("rsa_encrypted_key", str, field(default=None)),
-            ("kms_key_name", str, field(default=None)),
-            ("raw_key", str, field(default=None)),
-        ],
-    ) = None,
-    source_disk: str = None,
-    chain_name: str = None,
-    snapshot_type: str = None,
-    snapshot_encryption_key: make_dataclass(
-        "CustomerEncryptionKey",
-        [
-            ("kms_key_service_account", str, field(default=None)),
-            ("sha256", str, field(default=None)),
-            ("rsa_encrypted_key", str, field(default=None)),
-            ("kms_key_name", str, field(default=None)),
-            ("raw_key", str, field(default=None)),
-        ],
-    ) = None,
-    request_id: str = None,
-):
-    r"""Creates a snapshot of a specified persistent disk. For regular snapshot creation, consider using snapshots.insert instead, as that method supports more features, such as creating snapshots in a project different from the source disk project.
-
-    Args:
-        name(str):
-            Name of the resource; provided by the client when the resource is created. The name must be 1-63 characters long, and comply with RFC1035. Specifically, the name must be 1-63 characters long and match the regular expression `[a-z]([-a-z0-9]*[a-z0-9])?` which means the first character must be a lowercase letter, and all following characters must be a dash, lowercase letter, or digit, except the last character, which cannot be a dash.",
-                                "pattern": "[a-z](?:[-a-z0-9]{0,61}[a-z0-9])?
-
-        project(str, Optional):
-            Project ID for this request. Defaults to None.
-
-        zone(str, Optional):
-            The name of the zone for this request. Defaults to None.
-
-        disk(str, Optional):
-            Name of the persistent disk to snapshot.
-
-        resource_id(str, Optional):
-            An identifier of the resource in the provider. Defaults to None.
-
-        request_id(str, Optional):
-            An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000).
-
-    Examples:
-        .. code-block: sls
-
-            random-name:
-              exec.run:
-              - path: gcp.compute.disk.create_snapshot
-              - kwargs:
-                  name: snapshot-name
-                  disk: disk-name
-                  project: project-name
-                  zone: zone-name
-    """
-
-    project = get_project_from_account(ctx, project)
-
-    request_body = {
-        "name": name,
-        "storage_locations": storage_locations,
-        "location_hint": location_hint,
-        "label_fingerprint": label_fingerprint,
-        "description": description,
-        "labels": labels,
-        "source_disk_encryption_key": source_disk_encryption_key,
-        "source_disk": source_disk,
-        "chain_name": chain_name,
-        "snapshot_type": snapshot_type,
-        "snapshot_encryption_key": snapshot_encryption_key,
-    }
-
-    execution_context = ExecutionContext(
-        resource_type="compute.disk",
-        method_name="createSnapshot",
-        method_params={
-            "ctx": ctx,
-            "resource_id": resource_id,
-            "body": request_body,
-            "requestId": request_id,
-            "project": project,
-            "zone": zone,
-            "disk": disk,
-        },
-    )
-    return await hub.tool.gcp.generate.generic_exec.execute(execution_context)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/disk_type.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/machine_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,92 +1,90 @@
-"""Exec module for managing Disk Types."""
+"""Exec module for managing Machine Types."""
 from typing import Any
 from typing import Dict
 
-from idem_gcp.tool.gcp.utils import get_project_from_account
-
 __func_alias__ = {"list_": "list"}
 
 
 async def list_(
     hub,
     ctx,
     project: str = None,
     zone: str = None,
-    filter: str = None,
+    filter_: (str, "alias=filter") = None,
     order_by: str = None,
-    include_all_scopes: bool = False,
+    include_all_scopes: bool = None,
 ) -> Dict[str, Any]:
-    r"""Retrieves a list of disk types available to the specified project.
+    r"""Retrieves a list of machine types available to the specified project.
 
     Args:
         project(str, Optional):
             Project ID for this request.
 
         zone(str, Optional):
             The name of the zone for this request.
 
         filter(str, Optional):
-            A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name \"instance\", you would use `name ne .*instance`.
+            A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name "instance", you would use `name ne .*instance`.
 
         order_by(str, Optional):
             Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
 
         include_all_scopes(bool, Optional):
             Indicates whether every visible scope for each scope type (zone, region, global) should be included in the response. For new resource types added after this field, the flag has no effect as new resource types will always include every visible scope for each scope type in response. For resource types which predate this field, if this flag is omitted or false, only scopes of the scope types where the resource type is expected to be found will be included.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.disk_type.list
+              - path: gcp.compute.machine_type.list
               - kwargs:
                   project: project-name
     """
-    project = get_project_from_account(ctx, project)
-
     result = dict(comment=[], ret=[], result=True)
 
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
+
     if zone and not include_all_scopes:
-        ret = await hub.exec.gcp_api.client.compute.disk_type.list(
+        ret = await hub.exec.gcp_api.client.compute.machine_type.list(
             ctx,
             project=project,
             zone=zone,
-            filter=filter,
+            filter=filter_,
             orderBy=order_by,
         )
     else:
-        ret = await hub.exec.gcp_api.client.compute.disk_type.aggregatedList(
+        ret = await hub.exec.gcp_api.client.compute.machine_type.aggregatedList(
             ctx,
             project=project,
-            filter=filter,
+            filter=filter_,
             orderBy=order_by,
             includeAllScopes=include_all_scopes,
         )
 
     if not ret["result"]:
         result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
-    result["ret"] = ret["ret"]["items"]
+    result["ret"] = ret["ret"].get("items", [])
     result["comment"] += ret["comment"]
     return result
 
 
 async def get(
     hub,
     ctx,
     name: str = None,
     project: str = None,
     zone: str = None,
     resource_id: str = None,
 ):
-    r"""Returns the specified disk type.
+    r"""Returns the specified machine type.
 
     Args:
         resource_id(str, Optional):
             An identifier of the resource in the provider.
             Defaults to None.
 
         name(str, Optional):
@@ -95,44 +93,44 @@
         project(str, Optional):
             Project ID for this request.
 
         zone(str, Optional):
             The name of the zone for this request.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.disk_type.get
+              - path: gcp.compute.machine_type.get
               - kwargs:
-                  name: disk-type-name
+                  name: machine-type-name
                   project: project-name
                   zone: zone-name
     """
-    project = get_project_from_account(ctx, project)
-
     result = dict(comment=[], ret=[], result=True)
 
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
+
     if resource_id:
-        ret = await hub.exec.gcp_api.client.compute.disk_type.get(
+        ret = await hub.exec.gcp_api.client.compute.machine_type.get(
             ctx,
             resource_id=resource_id,
         )
     elif project and zone and name:
-        ret = await hub.exec.gcp_api.client.compute.disk_type.get(
+        ret = await hub.exec.gcp_api.client.compute.machine_type.get(
             ctx,
             project=project,
             zone=zone,
-            diskType=name,
+            machineType=name,
         )
     else:
         result["result"] = False
         result["comment"] = [
-            f"gcp.compute.disk_type {name} either resource_id or project, zone and name"
+            f"gcp.compute.machine_type {name} either resource_id or project, zone and name"
             f" should be specified."
         ]
         return result
 
     if not ret["result"]:
         result["comment"] += ret["comment"]
         result["result"] = False
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/firewall.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/firewall.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Exec module for managing Firewalls."""
 __func_alias__ = {"list_": "list"}
 
-from idem_gcp.tool.gcp.utils import get_project_from_account
 from typing import Any
 from typing import Dict
 
 
 async def list_(
     hub,
     ctx,
     max_results: int = None,
     project: str = None,
-    filter: str = None,
+    filter_: (str, "alias=filter") = None,
     order_by: str = None,
     page_token: str = None,
     return_partial_success: bool = None,
 ) -> Dict[str, Any]:
     r"""Retrieves the list of firewall rules available to the specified project.
 
     Args:
@@ -65,87 +64,87 @@
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
-        list-firewalls:
-            exec.run:
-               - path: gcp.compute.firewall.list
-               - kwargs:
-                   project: project-name
+            list-firewalls:
+                exec.run:
+                   - path: gcp.compute.firewall.list
+                   - kwargs:
+                       project: project-name
     """
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
     result = {
         "comment": [],
         "ret": None,
         "result": True,
     }
 
     ret = await hub.exec.gcp_api.client.compute.firewall.list(
         ctx,
         project=project,
         max_results=max_results,
-        filter=filter,
+        filter=filter_,
         orderBy=order_by,
         page_token=page_token,
         return_partial_success=return_partial_success,
     )
     if not ret["result"]:
         result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
-    result["ret"] = ret["ret"]["items"]
+    result["ret"] = ret["ret"].get("items", [])
     return result
 
 
 async def get(
     hub,
     ctx,
     project: str = None,
-    firewall: str = None,
+    name: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     r"""Returns the specified firewall.
 
     Args:
         project: Project ID for this request.
-        firewall: Name of the firewall rule to return.
+        name: Name of the firewall rule to return.
         resource_id: Idem resource ID.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
-        get-firewall:
-            exec.run:
-               - path: gcp.compute.firewall.get
-               - kwargs:
-                   project: project-name
-                   firewall: firewall-name
+            get-firewall:
+                exec.run:
+                   - path: gcp.compute.firewall.get
+                   - kwargs:
+                       project: project-name
+                       name: firewall-name
     """
     result = {
         "comment": [],
         "ret": None,
         "result": True,
     }
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     if resource_id:
         ret = await hub.exec.gcp_api.client.compute.firewall.get(
             ctx,
             resource_id=resource_id,
         )
-    elif project and firewall:
+    elif project and name:
         ret = await hub.exec.gcp_api.client.compute.firewall.get(
-            ctx, project=project, firewall=firewall
+            ctx, project=project, firewall=name
         )
     else:
         result["result"] = False
         result["comment"] = [
             f"gcp.compute.firewall#get(): either resource_id or project and firewall"
             f" should be specified."
         ]
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/image.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Exec module for managing Images."""
 __func_alias__ = {"list_": "list"}
 
-from idem_gcp.tool.gcp.utils import get_project_from_account
-
 
 async def list_(
     hub,
     ctx,
     project: str = None,
-    filter: str = None,
+    filter_: (str, "alias=filter") = None,
     order_by: str = None,
 ):
     r"""Retrieves the list of custom images available to the specified project.
 
     Custom images are images you create that belong to your project.
     This method does not get any images that belong to other projects, including publicly-available images,
     like Debian 8. If you want to get a list of publicly-available images, use this method to make a request
@@ -25,42 +23,42 @@
         filter(str, Optional):
             A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name "instance", you would use `name ne .*instance`.
 
         order_by(str, Optional):
             Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.image.list
               - kwargs:
                   project: project-name
     """
     result = {
         "comment": [],
         "ret": None,
         "result": True,
     }
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     ret = await hub.exec.gcp_api.client.compute.image.list(
         ctx,
         project=project,
-        filter=filter,
+        filter=filter_,
         orderBy=order_by,
     )
 
     result["comment"] += ret["comment"]
     if not ret["result"]:
         result["result"] = False
         return result
 
-    result["ret"] = ret["ret"]["items"]
+    result["ret"] = ret["ret"].get("items", [])
     return result
 
 
 async def get(
     hub,
     ctx,
     project: str = None,
@@ -76,29 +74,29 @@
         name(str, Optional):
             Name of the image resource to return. Defaults to None.
 
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.image.get
               - kwargs:
                   project: project-name
                   name: image-name
     """
     result = {
         "comment": [],
         "ret": None,
         "result": True,
     }
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     if resource_id:
         ret = await hub.exec.gcp_api.client.compute.image.get(
             ctx,
             resource_id=resource_id,
         )
     elif project and name:
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/instance.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 
 from dataclasses import make_dataclass, field
 from typing import Any, Dict, List
 
 from idem_gcp.tool.gcp.generate.exec_context import ExecutionContext
 from idem_gcp.tool.gcp.generate.exec_param import ExecParam
 from idem_gcp.tool.gcp.generate.scope import Scope
-from idem_gcp.tool.gcp.utils import get_project_from_account
 
 
 async def list_(
     hub,
     ctx,
     project: str = None,
     zone: str = None,
-    filter: str = None,
+    filter_: (str, "alias=filter") = None,
     order_by: str = None,
 ):
     r"""Retrieves the list of instances contained within the specified zone.
 
     Args:
         project(str, Optional):
             Project ID for this request.
@@ -31,35 +30,35 @@
         filter(str, Optional):
             A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name "instance", you would use `name ne .*instance`.
 
         order_by(str, Optional):
             Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.instance.list
               - kwargs:
                   project: project-name
                   zone: zone-name
     """
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     # GCP method name is simply the name of this func or the one from __func_alias - we can pass it
     # also we can pass the resource name based on the file name
     execution_context = ExecutionContext(
         resource_type="compute.instance",
         method_name="list",
         method_params={
             "ctx": ctx,
             "project": project,
             "zone": zone,
-            "filter": filter,
+            "filter": filter_,
             "order_by": order_by,
         },
         exec_params={
             ExecParam.SCOPED_FUNCTIONS: {
                 Scope.ZONAL: "list",
                 Scope.GLOBAL: "aggregatedList",
             }
@@ -70,53 +69,53 @@
 
 async def get(
     hub,
     ctx,
     resource_id: str = None,
     project: str = None,
     zone: str = None,
-    instance: str = None,
+    name: str = None,
 ):
     r"""Returns the specified Instance resource. Gets a list of available instances by making a list() request.
 
     Args:
         resource_id(str, Optional):
             An identifier of the resource in the provider.
 
         project(str, Optional):
             Project ID for this request.
 
         zone(str, Optional):
             Name of the zone for this request.
 
-        instance(str, Optional):
+        name(str, Optional):
             Name of the instance resource to return.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.instance.get
               - kwargs:
                   project: project-name
                   zone: zone-name
-                  instance: instance-name
+                  name: instance-name
     """
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     execution_context = ExecutionContext(
         resource_type="compute.instance",
         method_name="get",
         method_params={
             "ctx": ctx,
             "resource_id": resource_id,
             "project": project,
             "zone": zone,
-            "instance": instance,
+            "instance": name,
         },
     )
     return await hub.tool.gcp.generate.generic_exec.execute(execution_context)
 
 
 async def set_disk_auto_delete(
     hub,
@@ -149,15 +148,15 @@
 
         resource_id(str, Optional):
             An identifier of the resource in the provider.
 
         request_id(str, Optional):
             An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000).
     """
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     execution_context = ExecutionContext(
         resource_type="compute.instance",
         method_name="setDiskAutoDelete",
         method_params={
             "ctx": ctx,
             "device_name": device_name,
@@ -180,15 +179,17 @@
     instance: str = None,
     resource_id: str = None,
     request_id: str = None,
     disk_size_gb: str = None,
     auto_delete: bool = None,
     boot: bool = None,
     guest_os_features: List[
-        make_dataclass("GuestOsFeature", [("type", str, field(default=None))])
+        make_dataclass(
+            "GuestOsFeature", [("type_", (str, "alias=type"), field(default=None))]
+        )
     ] = None,
     source: str = None,
     disk_encryption_key: make_dataclass(
         "CustomerEncryptionKey",
         [
             ("kms_key_service_account", str, field(default=None)),
             ("sha256", str, field(default=None)),
@@ -255,15 +256,15 @@
             ("disk_type", str, field(default=None)),
             ("disk_name", str, field(default=None)),
             ("resource_policies", List[str], field(default=None)),
         ],
     ) = None,
     interface: str = None,
     mode: str = None,
-    type: str = None,
+    type_: (str, "alias=type") = None,
 ):
     r"""Attaches an existing Disk resource to an instance. You must first create the disk before you can attach it. It is not possible to create and attach a disk at the same time. For more information, read Adding a persistent disk to your instance.
 
     Args:
         project(str, Optional):
             Project ID for this request.
 
@@ -289,112 +290,117 @@
             Specifies whether the disk will be auto-deleted when the instance is deleted (but not when the disk is detached from the instance).
 
         boot(bool, Optional):
             Indicates that this is a boot disk. The virtual machine will use the first partition of the disk for its root filesystem.
 
         guest_os_features(List[Dict[str, Any]], Optional):
             A list of features to enable on the guest operating system. Applicable only for bootable images. Read Enabling guest operating system features to see a list of available options.
-                    * type(str, Optional): The ID of a supported feature. To add multiple values, use commas to separate values. Set to one or more of the following values: - VIRTIO_SCSI_MULTIQUEUE - WINDOWS - MULTI_IP_SUBNET - UEFI_COMPATIBLE - GVNIC - SEV_CAPABLE - SUSPEND_RESUME_COMPATIBLE - SEV_SNP_CAPABLE For more information, see Enabling guest operating system features.
-            Enum type. Allowed values:
-                "FEATURE_TYPE_UNSPECIFIED"
-                "GVNIC"
-                "MULTI_IP_SUBNET"
-                "SECURE_BOOT"
-                "SEV_CAPABLE"
-                "UEFI_COMPATIBLE"
-                "VIRTIO_SCSI_MULTIQUEUE"
-                "WINDOWS"
+
+            * type(str, Optional):
+                The ID of a supported feature. To add multiple values, use commas to separate values. Set to one or more of the following values: - VIRTIO_SCSI_MULTIQUEUE - WINDOWS - MULTI_IP_SUBNET - UEFI_COMPATIBLE - GVNIC - SEV_CAPABLE - SUSPEND_RESUME_COMPATIBLE - SEV_SNP_CAPABLE For more information, see Enabling guest operating system features.
+                    Enum type. Allowed values:
+                        "FEATURE_TYPE_UNSPECIFIED"
+                        "GVNIC"
+                        "MULTI_IP_SUBNET"
+                        "SECURE_BOOT"
+                        "SEV_CAPABLE"
+                        "UEFI_COMPATIBLE"
+                        "VIRTIO_SCSI_MULTIQUEUE"
+                        "WINDOWS"
 
         source(str, Optional):
             Specifies a valid partial or full URL to an existing Persistent Disk resource. When creating a new instance, one of initializeParams.sourceImage or initializeParams.sourceSnapshot or disks.source is required except for local SSD. If desired, you can also attach existing non-root persistent disks using this property. This field is only applicable for persistent disks. Note that for InstanceTemplate, specify the disk name for zonal disk, and the URL for regional disk.
 
         disk_encryption_key(Dict[str, Any], Optional):
             Encrypts or decrypts a disk using a customer-supplied encryption key. If you are creating a new disk, this field encrypts the new disk using an encryption key that you provide. If you are attaching an existing disk that is already encrypted, this field decrypts the disk using the customer-supplied encryption key. If you encrypt a disk using a customer-supplied key, you must provide the same key again when you attempt to use this resource at a later time. For example, you must provide the key when you create a snapshot or an image from the disk or when you attach the disk to a virtual machine instance. If you do not provide an encryption key, then the disk will be encrypted using an automatically generated key and you do not need to provide a key to use the disk later. Instance templates do not store customer-supplied encryption keys, so you cannot use your own keys to encrypt disks in a managed instance group.
-                    * kms_key_service_account (str, Optional): The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/
-                    * sha256 (str, Optional): [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
-                    * rsa_encrypted_key (str, Optional): Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
-                    * kms_key_name (str, Optional): The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
-                    * raw_key (str, Optional): Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
+
+            * kms_key_service_account (str, Optional): The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/"
+            * sha256 (str, Optional): [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
+            * rsa_encrypted_key (str, Optional): Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+            * kms_key_name (str, Optional): The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+            * raw_key (str, Optional): Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
 
         force_attach(bool, Optional):
             [Input Only] Whether to force attach the regional disk even if it's currently attached to another instance. If you try to force attach a zonal disk to an instance, you will receive an error.
 
         device_name(str, Optional):
             Specifies a unique device name of your choice that is reflected into the /dev/disk/by-id/google-* tree of a Linux operating system running within the instance. This name can be used to reference the device for mounting, resizing, and so on, from within the instance. If not specified, the server chooses a default device name to apply to this disk, in the form persistent-disk-x, where x is a number assigned by Google Compute Engine. This field is only applicable for persistent disks.
 
         initialize_params(Dict[str, Any], Optional):
             [Input Only] Specifies the parameters for a new disk that will be created alongside the new instance. Use initialization parameters to create boot disks or local SSDs attached to the new instance. This property is mutually exclusive with the source property; you can only define one or the other, but not both.
             AttachedDiskInitializeParams: [Input Only] Specifies the parameters for a new disk that will be created alongside the new instance. Use initialization parameters to create boot disks or local SSDs attached to the new instance. This field is persisted and returned for instanceTemplate and not returned in the context of instance. This property is mutually exclusive with the source property; you can only define one or the other, but not both.
-                    * resource_manager_tags (Dict[str, Any], Optional): Resource manager tags to be bound to the disk. Tag keys and values have the same definition as resource manager tags. Keys must be in the format `tagKeys/{tag_key_id}`, and values are in the format `tagValues/456`. The field is ignored (both PUT & PATCH) when empty.
-                    * source_image (str, Optional): The source image to create this disk. When creating a new instance, one of initializeParams.sourceImage or initializeParams.sourceSnapshot or disks.source is required except for local SSD. To create a disk with one of the public operating system images, specify the image by its family name. For example, specify family/debian-9 to use the latest Debian 9 image: projects/debian-cloud/global/images/family/debian-9 Alternatively, use a specific version of a public operating system image: projects/debian-cloud/global/images/debian-9-stretch-vYYYYMMDD To create a disk with a custom image that you created, specify the image name in the following format: global/images/my-custom-image You can also specify a custom image by its image family, which returns the latest version of the image in that family. Replace the image name with family/family-name: global/images/family/my-image-family If the source image is deleted later, this field will not be set.
-                    * description (str, Optional): An Optional description. Provide this property when creating the disk.
-                    * disk_size_gb (str, Optional): Specifies the size of the disk in base-2 GB. The size must be at least 10 GB. If you specify a sourceImage, which is required for boot disks, the default size is the size of the sourceImage. If you do not specify a sourceImage, the default disk size is 500 GB.
-                    * source_snapshot (str, Optional): The source snapshot to create this disk. When creating a new instance, one of initializeParams.sourceSnapshot or initializeParams.sourceImage or disks.source is required except for local SSD. To create a disk with a snapshot that you created, specify the snapshot name in the following format: global/snapshots/my-backup If the source snapshot is deleted later, this field will not be set.
-                    * provisioned_iops (str, Optional): Indicates how many IOPS to provision for the disk. This sets the number of I/O operations per second that the disk can handle. Values must be between 10,000 and 120,000. For more details, see the Extreme persistent disk documentation.
-                    * source_image_encryption_key (Dict[str, Any], Optional): The customer-supplied encryption key of the source image. Required if the source image is protected by a customer-supplied encryption key. InstanceTemplate and InstancePropertiesPatch do not store customer-supplied encryption keys, so you cannot create disks for instances in a managed instance group if the source images are encrypted with your own keys.
-                        * kms_key_service_account (str, Optional): The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/
-                        * sha256 (str, Optional): [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
-                        * rsa_encrypted_key (str, Optional): Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
-                        * kms_key_name (str, Optional): The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
-                        * raw_key (str, Optional): Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
-                    * on_update_action (str, Optional): Specifies which action to take on instance update with this disk. Default is to use the existing disk.
-            Enum type. Allowed values:
-                "RECREATE_DISK" - Always recreate the disk.
-                "RECREATE_DISK_IF_SOURCE_CHANGED" - Recreate the disk if source (image, snapshot) of this disk is different from source of existing disk.
-                "USE_EXISTING_DISK" - Use the existing disk, this is the default behaviour.
-                    * source_snapshot_encryption_key (Dict[str, Any], Optional): The customer-supplied encryption key of the source snapshot.
-                        * kms_key_service_account (str, Optional): The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/
-                        * sha256 (str, Optional): [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
-                        * rsa_encrypted_key (str, Optional): Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
-                        * kms_key_name (str, Optional): The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
-                        * raw_key (str, Optional): Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
-                    * architecture (str, Optional): The architecture of the attached disk. Valid values are arm64 or x86_64.
-            Enum type. Allowed values:
-                "ARCHITECTURE_UNSPECIFIED" - Default value indicating Architecture is not set.
-                "ARM64" - Machines with architecture ARM64
-                "X86_64" - Machines with architecture X86_64
-                    * licenses (List[str], Optional): A list of publicly visible licenses. Reserved for Google's use.
-                    * labels (Dict[str, Any], Optional): Labels to apply to this disk. These can be later modified by the disks.setLabels method. This field is only applicable for persistent disks.
-                    * disk_type (str, Optional): Specifies the disk type to use to create the instance. If not specified, the default is pd-standard, specified using the full URL. For example: https://www.googleapis.com/compute/v1/projects/project/zones/zone /diskTypes/pd-standard For a full list of acceptable values, see Persistent disk types. If you specify this field when creating a VM, you can provide either the full or partial URL. For example, the following values are valid: - https://www.googleapis.com/compute/v1/projects/project/zones/zone /diskTypes/diskType - projects/project/zones/zone/diskTypes/diskType - zones/zone/diskTypes/diskType If you specify this field when creating or updating an instance template or all-instances configuration, specify the type of the disk, not the URL. For example: pd-standard.
-                    * disk_name (str, Optional): Specifies the disk name. If not specified, the default is to use the name of the instance. If a disk with the same name already exists in the given region, the existing disk is attached to the new instance and the new disk is not created.
-                    * resource_policies (List[str], Optional): Resource policies applied to this disk for automatic snapshot creations. Specified using the full or partial URL. For instance template, specify only the resource policy name.
+
+            * resource_manager_tags (Dict[str, Any], Optional): Resource manager tags to be bound to the disk. Tag keys and values have the same definition as resource manager tags. Keys must be in the format `tagKeys/{tag_key_id}`, and values are in the format `tagValues/456`. The field is ignored (both PUT & PATCH) when empty.
+            * source_image (str, Optional): The source image to create this disk. When creating a new instance, one of initializeParams.sourceImage or initializeParams.sourceSnapshot or disks.source is required except for local SSD. To create a disk with one of the public operating system images, specify the image by its family name. For example, specify family/debian-9 to use the latest Debian 9 image: projects/debian-cloud/global/images/family/debian-9 Alternatively, use a specific version of a public operating system image: projects/debian-cloud/global/images/debian-9-stretch-vYYYYMMDD To create a disk with a custom image that you created, specify the image name in the following format: global/images/my-custom-image You can also specify a custom image by its image family, which returns the latest version of the image in that family. Replace the image name with family/family-name: global/images/family/my-image-family If the source image is deleted later, this field will not be set.
+            * description (str, Optional): An Optional description. Provide this property when creating the disk.
+            * disk_size_gb (str, Optional): Specifies the size of the disk in base-2 GB. The size must be at least 10 GB. If you specify a sourceImage, which is required for boot disks, the default size is the size of the sourceImage. If you do not specify a sourceImage, the default disk size is 500 GB.
+            * source_snapshot (str, Optional): The source snapshot to create this disk. When creating a new instance, one of initializeParams.sourceSnapshot or initializeParams.sourceImage or disks.source is required except for local SSD. To create a disk with a snapshot that you created, specify the snapshot name in the following format: global/snapshots/my-backup If the source snapshot is deleted later, this field will not be set.
+            * provisioned_iops (str, Optional): Indicates how many IOPS to provision for the disk. This sets the number of I/O operations per second that the disk can handle. Values must be between 10,000 and 120,000. For more details, see the Extreme persistent disk documentation.
+            * source_image_encryption_key (Dict[str, Any], Optional): The customer-supplied encryption key of the source image. Required if the source image is protected by a customer-supplied encryption key. InstanceTemplate and InstancePropertiesPatch do not store customer-supplied encryption keys, so you cannot create disks for instances in a managed instance group if the source images are encrypted with your own keys.
+                * kms_key_service_account (str, Optional): The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/"
+                * sha256 (str, Optional): [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
+                * rsa_encrypted_key (str, Optional): Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+                * kms_key_name (str, Optional): The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+                * raw_key (str, Optional): Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
+            * on_update_action (str, Optional):
+                Specifies which action to take on instance update with this disk. Default is to use the existing disk.
+                    Enum type. Allowed values:
+                        "RECREATE_DISK" - Always recreate the disk.
+                        "RECREATE_DISK_IF_SOURCE_CHANGED" - Recreate the disk if source (image, snapshot) of this disk is different from source of existing disk.
+                        "USE_EXISTING_DISK" - Use the existing disk, this is the default behaviour.
+
+            * source_snapshot_encryption_key (Dict[str, Any], Optional): The customer-supplied encryption key of the source snapshot.
+                * kms_key_service_account (str, Optional): The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/"
+                * sha256 (str, Optional): [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
+                * rsa_encrypted_key (str, Optional): Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+                * kms_key_name (str, Optional): The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+                * raw_key (str, Optional): Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
+            * architecture (str, Optional):
+                The architecture of the attached disk. Valid values are arm64 or x86_64.
+                    Enum type. Allowed values:
+                        "ARCHITECTURE_UNSPECIFIED" - Default value indicating Architecture is not set.
+                        "ARM64" - Machines with architecture ARM64
+                        "X86_64" - Machines with architecture X86_64
+            * licenses (List[str], Optional): A list of publicly visible licenses. Reserved for Google's use.
+            * labels (Dict[str, Any], Optional): Labels to apply to this disk. These can be later modified by the disks.setLabels method. This field is only applicable for persistent disks.
+            * disk_type (str, Optional): Specifies the disk type to use to create the instance. If not specified, the default is pd-standard, specified using the full URL. For example: https://www.googleapis.com/compute/v1/projects/project/zones/zone /diskTypes/pd-standard For a full list of acceptable values, see Persistent disk types. If you specify this field when creating a VM, you can provide either the full or partial URL. For example, the following values are valid: - https://www.googleapis.com/compute/v1/projects/project/zones/zone /diskTypes/diskType - projects/project/zones/zone/diskTypes/diskType - zones/zone/diskTypes/diskType If you specify this field when creating or updating an instance template or all-instances configuration, specify the type of the disk, not the URL. For example: pd-standard.
+            * disk_name (str, Optional): Specifies the disk name. If not specified, the default is to use the name of the instance. If a disk with the same name already exists in the given region, the existing disk is attached to the new instance and the new disk is not created.
+            * resource_policies (List[str], Optional): Resource policies applied to this disk for automatic snapshot creations. Specified using the full or partial URL. For instance template, specify only the resource policy name.
 
         interface(str, Optional):
             Specifies the disk interface to use for attaching this disk, which is either SCSI or NVME. For most machine types, the default is SCSI. Local SSDs can use either NVME or SCSI. In certain configurations, persistent disks can use NVMe. For more information, see About persistent disks.
-            Enum type. Allowed values:
-                "NVME"
-                "SCSI"
+                Enum type. Allowed values:
+                    "NVME"
+                    "SCSI"
 
         mode(str, Optional):
             The mode in which to attach this disk, either READ_WRITE or READ_ONLY. If not specified, the default is to attach the disk in READ_WRITE mode.
-            Enum type. Allowed values:
-                "READ_ONLY" - Attaches this disk in read-only mode. Multiple virtual machines can use a disk in read-only mode at a time.
-                "READ_WRITE" - *[Default]* Attaches this disk in read-write mode. Only one virtual machine at a time can be attached to a disk in read-write mode.
+                Enum type. Allowed values:
+                    "READ_ONLY" - Attaches this disk in read-only mode. Multiple virtual machines can use a disk in read-only mode at a time.
+                    "READ_WRITE" - *[Default]* Attaches this disk in read-write mode. Only one virtual machine at a time can be attached to a disk in read-write mode.
 
         type(str, Optional):
             Specifies the type of the disk, either SCRATCH or PERSISTENT. If not specified, the default is PERSISTENT.
-            Enum type. Allowed values:
-                "PERSISTENT"
-                "SCRATCH"
-
+                Enum type. Allowed values:
+                    "PERSISTENT"
+                    "SCRATCH"
     """
-
     request_body = {
         "disk_size_gb": disk_size_gb,
         "auto_delete": auto_delete,
         "boot": boot,
         "guest_os_features": guest_os_features,
         "source": source,
         "disk_encryption_key": disk_encryption_key,
         "force_attach": force_attach,
         "device_name": device_name,
         "initialize_params": initialize_params,
         "interface": interface,
         "mode": mode,
-        "type": type,
+        "type": type_,
     }
 
     execution_context = ExecutionContext(
         resource_type="compute.instance",
         method_name="attachDisk",
         method_params={
             "ctx": ctx,
@@ -463,15 +469,15 @@
     project: str = None,
     zone: str = None,
     instance: str = None,
     resource_id: str = None,
     network_interface: str = None,
     request_id: str = None,
 ) -> Dict[str, Any]:
-    r"""Returns effective firewalls applied to an interface of the instance
+    r"""Returns effective firewalls applied to an interface of the instance.
 
     Args:
         network_interface(str):
             The name of the network interface to get the effective firewalls.
 
         project(str, Optional):
             Project ID for this request. Defaults to None.
@@ -485,23 +491,23 @@
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
         request_id(str, Optional):
             An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000).  Defaults to None.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.instance.get_effective_firewalls
               - kwargs:
                   project: project-name
                   zone: zone-name
-                  instance: instance-name
+                  name: instance-name
                   network_interface: network-interface-name
     """
     execution_context = ExecutionContext(
         resource_type="compute.instance",
         method_name="getEffectiveFirewalls",
         method_params={
             "ctx": ctx,
@@ -543,15 +549,15 @@
         resource_id(str, Optional):
             An identifier of the resource in the provider.
 
         request_id(str, Optional):
             An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000).
     """
     request_body = {"update_auto_learn_policy": update_auto_learn_policy}
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
     execution_context = ExecutionContext(
         resource_type="compute.instance",
         method_name="setShieldedInstanceIntegrityPolicy",
         method_params={
             "ctx": ctx,
             "resource_id": resource_id,
             "request_id": request_id,
@@ -604,15 +610,15 @@
             An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000).
     """
     request_body = {
         "enable_secure_boot": enable_secure_boot,
         "enable_vtpm": enable_vtpm,
         "enable_integrity_monitoring": enable_integrity_monitoring,
     }
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
     execution_context = ExecutionContext(
         resource_type="compute.instance",
         method_name="updateShieldedInstanceConfig",
         method_params={
             "ctx": ctx,
             "resource_id": resource_id,
             "request_id": request_id,
@@ -649,15 +655,15 @@
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
         request_id(str, Optional):
             An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000).  Defaults to None.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.instance.start
               - kwargs:
                   project: project-name
                   zone: zone-name
@@ -702,15 +708,15 @@
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
         request_id(str, Optional):
             An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000).  Defaults to None.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.instance.stop
               - kwargs:
                   project: project-name
                   zone: zone-name
@@ -755,15 +761,15 @@
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
         request_id(str, Optional):
             An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000).  Defaults to None.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.instance.resume
               - kwargs:
                   project: project-name
                   zone: zone-name
@@ -808,15 +814,15 @@
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
         request_id(str, Optional):
             An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000).  Defaults to None.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.instance.resume
               - kwargs:
                   project: project-name
                   zone: zone-name
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/machine_image.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/machine_image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,92 +1,88 @@
+"""Exec module for managing Machine Images."""
 from typing import Any
 from typing import Dict
 
-from idem_gcp.tool.gcp.utils import get_project_from_account
-
 __func_alias__ = {"list_": "list"}
 
 
 async def list_(
     hub,
     ctx,
     project: str = None,
-    filter: str = None,
+    filter_: (str, "alias=filter") = None,
     order_by: str = None,
 ) -> Dict[str, Any]:
     r"""Retrieves a list of machine images that are contained within the specified project.
 
     Args:
         project(str, Optional):
             Project ID for this request.
 
         filter(str, Optional):
             A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name "instance", you would use `name ne .*instance`.
 
         order_by(str, Optional):
             Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
     """
-
     result = {
         "comment": [],
         "ret": None,
         "result": True,
     }
 
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     ret = await hub.exec.gcp_api.client.compute.machine_image.list(
         ctx,
         project=project,
-        filter=filter,
+        filter=filter_,
         orderBy=order_by,
     )
 
     result["comment"] += ret["comment"]
 
     if not ret["result"]:
         result["result"] = False
         return result
 
-    result["ret"] = ret["ret"]["items"]
+    result["ret"] = ret["ret"].get("items", [])
     return result
 
 
 async def get(
-    hub, ctx, resource_id: str = None, project: str = None, machine_image: str = None
+    hub, ctx, resource_id: str = None, project: str = None, name: str = None
 ) -> Dict[str, Any]:
     r"""Returns the specified machine image. Gets a list of available machine images by making a list() request.
 
     Args:
-
-        machine_image(str):
+        name(str):
             The name of the machine image.
 
         project(str, Optional):
             Project ID for this request.
 
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
     """
-
     result = {
         "comment": [],
         "ret": None,
         "result": True,
     }
 
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     if resource_id:
         ret = await hub.exec.gcp_api.client.compute.machine_image.get(
             ctx, resource_id=resource_id
         )
     else:
         ret = await hub.exec.gcp_api.client.compute.machine_image.get(
-            ctx, project=project, machineImage=machine_image
+            ctx, project=project, machineImage=name
         )
 
     result["comment"] += ret["comment"]
 
     if not ret["result"]:
         result["result"] = False
         return result
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/machine_type.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/resource_policy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,143 +1,136 @@
-"""Exec module for managing Machine Types."""
-from typing import Any
-from typing import Dict
-
-from idem_gcp.tool.gcp.utils import get_project_from_account
-
+"""Exec module for managing Resource Policies."""
 __func_alias__ = {"list_": "list"}
 
 
 async def list_(
     hub,
     ctx,
     project: str = None,
-    zone: str = None,
-    filter: str = None,
+    region: str = None,
+    filter_: (str, "alias=filter") = None,
     order_by: str = None,
-    include_all_scopes: bool = None,
-) -> Dict[str, Any]:
-    r"""Retrieves a list of machine types available to the specified project.
+):
+    r"""A list all the resource policies that have been configured for the specified project in specified region.
 
     Args:
         project(str, Optional):
             Project ID for this request.
 
-        zone(str, Optional):
-            The name of the zone for this request.
+        region(str, Optional):
+            Name of the region for this request.
 
         filter(str, Optional):
             A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name "instance", you would use `name ne .*instance`.
 
         order_by(str, Optional):
             Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
 
-        include_all_scopes(bool, Optional):
-            Indicates whether every visible scope for each scope type (zone, region, global) should be included in the response. For new resource types added after this field, the flag has no effect as new resource types will always include every visible scope for each scope type in response. For resource types which predate this field, if this flag is omitted or false, only scopes of the scope types where the resource type is expected to be found will be included.
-
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.machine_type.list
+              - path: gcp.compute.resource_policy.list
               - kwargs:
                   project: project-name
+                  region: region-name
     """
-    result = dict(comment=[], ret=[], result=True)
+    result = {
+        "comment": [],
+        "ret": None,
+        "result": True,
+    }
 
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
-    if zone and not include_all_scopes:
-        ret = await hub.exec.gcp_api.client.compute.machine_type.list(
+    if region:
+        ret = await hub.exec.gcp_api.client.compute.resource_policy.list(
             ctx,
             project=project,
-            zone=zone,
-            filter=filter,
+            region=region,
+            filter=filter_,
             orderBy=order_by,
         )
     else:
-        ret = await hub.exec.gcp_api.client.compute.machine_type.aggregatedList(
+        ret = await hub.exec.gcp_api.client.compute.resource_policy.aggregatedList(
             ctx,
             project=project,
-            filter=filter,
+            filter=filter_,
             orderBy=order_by,
-            includeAllScopes=include_all_scopes,
         )
 
+    result["comment"] += ret["comment"]
     if not ret["result"]:
-        result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
-    result["ret"] = ret["ret"]["items"]
-    result["comment"] += ret["comment"]
+    result["ret"] = ret["ret"].get("items", [])
     return result
 
 
 async def get(
     hub,
     ctx,
-    name: str = None,
     project: str = None,
-    zone: str = None,
+    region: str = None,
+    name: str = None,
     resource_id: str = None,
 ):
-    r"""Returns the specified machine type.
+    r"""Retrieves all information of the specified resource policy.
 
     Args:
-        resource_id(str, Optional):
-            An identifier of the resource in the provider.
-            Defaults to None.
+        project(str, Optional):
+            Project ID for this request. Defaults to None.
 
-        name(str, Optional):
-            Name of the machine type to return.
+        region(str, Optional):
+            Name of the region for this request. Defaults to None.
 
-        project(str, Optional):
-            Project ID for this request.
+        name(str, Optional):
+            Name of the resource policy to retrieve. Defaults to None.
 
-        zone(str, Optional):
-            The name of the zone for this request.
+        resource_id(str, Optional):
+            An identifier of the resource in the provider. Defaults to None.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.machine_type.get
+              - path: gcp.compute.resource_policy.get
               - kwargs:
-                  name: machine-type-name
                   project: project-name
-                  zone: zone-name
+                  region: region-name
+                  name: resource-policy-name
     """
-    result = dict(comment=[], ret=[], result=True)
+    result = {
+        "comment": [],
+        "ret": None,
+        "result": True,
+    }
 
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     if resource_id:
-        ret = await hub.exec.gcp_api.client.compute.machine_type.get(
+        ret = await hub.exec.gcp_api.client.compute.resource_policy.get(
             ctx,
             resource_id=resource_id,
         )
-    elif project and zone and name:
-        ret = await hub.exec.gcp_api.client.compute.machine_type.get(
-            ctx,
-            project=project,
-            zone=zone,
-            machineType=name,
+    elif project and region and name:
+        ret = await hub.exec.gcp_api.client.compute.resource_policy.get(
+            ctx, project=project, region=region, resource_policy=name
         )
     else:
         result["result"] = False
         result["comment"] = [
-            f"gcp.compute.machine_type {name} either resource_id or project, zone and name"
+            f"gcp.compute.resource_policy {name} either resource_id or project, region and name"
             f" should be specified."
         ]
         return result
 
+    result["comment"] += ret["comment"]
     if not ret["result"]:
-        result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
     result["ret"] = ret["ret"]
-    result["comment"] += ret["comment"]
     return result
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/network.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/network.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Exec module for managing Networks."""
 from typing import Any
 from typing import Dict
 
 from idem_gcp.tool.gcp.generate.exec_context import ExecutionContext
-from idem_gcp.tool.gcp.utils import get_project_from_account
 
 __func_alias__ = {"list_": "list"}
 
 
 async def list_(
     hub,
     ctx,
     project: str = None,
-    filter: str = None,
+    filter_: (str, "alias=filter") = None,
     max_results: int = 500,
     order_by: str = None,
     page_token: str = None,
     return_partial_success: bool = False,
 ) -> Dict[str, Any]:
     r"""Retrieves the list of networks available to the specified project.
 
@@ -36,46 +35,46 @@
         page_token(str, Optional):
             Specifies a page token to use. Set `pageToken` to the `nextPageToken` returned by a previous list request to get the next page of results.
 
         return_partial_success(bool, Optional):
             Opt-in for partial success behavior which provides partial results in case of failure. The default value is false.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.network.list
               - kwargs:
                   project: project-name
     """
     result = {
         "comment": [],
         "ret": None,
         "result": True,
     }
 
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     ret = await hub.exec.gcp_api.client.compute.network.list(
         ctx,
         project=project,
-        filter=filter,
+        filter=filter_,
         maxResults=max_results,
         orderBy=order_by,
         pageToken=page_token,
         returnPartialSuccess=return_partial_success,
     )
 
     if not ret["result"]:
         result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
-    result["ret"] = ret["ret"]["items"]
+    result["ret"] = ret["ret"].get("items", [])
     return result
 
 
 async def get(
     hub, ctx, resource_id: str = None, project: str = None, name: str = None
 ) -> Dict[str, Any]:
     r"""Returns the specified network. Gets a list of available networks by making a list() request.
@@ -87,30 +86,30 @@
         project(str, Optional):
             Project ID for this request.
 
         name(str, Optional):
             Name of the network to return.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.network.get
               - kwargs:
                   project: project-name
                   name: network-name
     """
     result = {
         "comment": [],
         "ret": None,
         "result": True,
     }
 
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     if resource_id:
         ret = await hub.exec.gcp_api.client.compute.network.get(
             ctx, resource_id=resource_id
         )
     elif project and name:
         ret = await hub.exec.gcp_api.client.compute.network.get(
@@ -152,24 +151,24 @@
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
         request_id(str, Optional):
             An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000).  Defaults to None.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.network.get_effective_firewalls
               - kwargs:
                   project: project-name
                   network: network-name
     """
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     execution_context = ExecutionContext(
         resource_type="compute.network",
         method_name="getEffectiveFirewalls",
         method_params={
             "ctx": ctx,
             "resource_id": resource_id,
@@ -185,28 +184,28 @@
     ctx,
     peering_name: str,
     region: str,
     direction: str,
     network: str = None,
     resource_id: str = None,
     project: str = None,
-    filter: str = None,
+    filter_: (str, "alias=filter") = None,
     order_by: str = None,
 ) -> Dict[str, Any]:
     r"""Lists the peering routes exchanged over peering connection.
 
     Args:
         peering_name(str):
             The response will show routes exchanged over the given peering connection.
 
         direction(str):
             The direction of the exchanged routes.
-            Enum type. Allowed values:
-            "INCOMING" - For routes exported from peer network.
-            "OUTGOING" - For routes exported from local network.
+                Enum type. Allowed values:
+                "INCOMING" - For routes exported from peer network.
+                "OUTGOING" - For routes exported from local network.
 
         region(str):
             The region of the request. The response will include all subnet routes, static routes and dynamic routes in the region.
 
         project(str, Optional):
             Project ID for this request.
 
@@ -219,42 +218,42 @@
         filter(str, Optional):
             A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name "instance", you would use `name ne .*instance`.
 
         order_by(str, Optional):
             Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.network.list_peering_routes
               - kwargs:
                   project: project-name
                   region: region-name
                   network: network-name
                   direction: direction-name
                   peering_name: peering-name
     """
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     # GCP method name is simply the name of this func or the one from __func_alias - we can pass it
     # also we can pass the resource name based on the file name
     execution_context = ExecutionContext(
         resource_type="compute.network",
         method_name="listPeeringRoutes",
         method_params={
             "ctx": ctx,
             "network": network,
             "peering_name": peering_name,
             "region": region,
             "direction": direction,
             "resource_id": resource_id,
             "project": project,
-            "filter": filter,
+            "filter": filter_,
             "order_by": order_by,
         },
     )
     return await hub.tool.gcp.generate.generic_exec.execute(execution_context)
 
 
 async def switch_to_custom_mode(
@@ -277,24 +276,24 @@
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
         request_id(str, Optional):
             An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000).  Defaults to None.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.network.switch_to_custom_mode
               - kwargs:
                   project: project-name
                   network: network-name
     """
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     execution_context = ExecutionContext(
         resource_type="compute.network",
         method_name="switchToCustomMode",
         method_params={
             "ctx": ctx,
             "resource_id": resource_id,
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/node_template.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/node_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """Exec module for managing Node Templates."""
 from typing import Any
 from typing import Dict
 
-from idem_gcp.tool.gcp.utils import get_project_from_account
-
 __func_alias__ = {"list_": "list"}
 
 
 async def list_(
     hub,
     ctx,
     project: str = None,
     region: str = None,
-    filter: str = None,
+    filter_: (str, "alias=filter") = None,
     max_results: int = 500,
     order_by: str = None,
     page_token: str = None,
     return_partial_success: bool = False,
 ) -> Dict[str, Any]:
     r"""Retrieves a list of node templates available to the specified project.
 
@@ -39,99 +37,119 @@
         page_token(str, Optional):
             Specifies a page token to use. Set `pageToken` to the `nextPageToken` returned by a previous list request to get the next page of results.
 
         return_partial_success(bool, Optional):
             Opt-in for partial success behavior which provides partial results in case of failure. The default value is false.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.node_template.list
               - kwargs:
                   project: project-name
     """
     result = {
         "comment": [],
         "ret": None,
         "result": True,
     }
 
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     if region:
         ret = await hub.exec.gcp_api.client.compute.node_template.list(
             ctx,
             project=project,
             region=region,
-            filter=filter,
+            filter=filter_,
             maxResults=max_results,
             orderBy=order_by,
             pageToken=page_token,
             returnPartialSuccess=return_partial_success,
         )
     else:
         ret = await hub.exec.gcp_api.client.compute.node_template.aggregatedList(
             ctx,
             project=project,
-            filter=filter,
+            filter=filter_,
             maxResults=max_results,
             orderBy=order_by,
             pageToken=page_token,
             returnPartialSuccess=return_partial_success,
         )
 
     if not ret["result"]:
         result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
-    result["ret"] = ret["ret"]["items"]
+    result["ret"] = ret["ret"].get("items", [])
     return result
 
 
 async def get(
-    hub, ctx, region: str, node_template: str, project: str = None
+    hub,
+    ctx,
+    resource_id: str = None,
+    region: str = None,
+    name: str = None,
+    project: str = None,
 ) -> Dict[str, Any]:
     r"""Returns the specified node template. Gets a list of available node templates by making a list() request.
 
     Args:
 
-        region(str):
+        resource_id(str, Optional):
+            An identifier of the resource in the provider.
+
+        region(str, Optional):
             The name of the region for this request.
 
-        node_template(str):
+        name(str, Optional):
             Name of the node template to return.
 
         project(str, Optional):
             Project ID for this request.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.node_template.get
               - kwargs:
                   project: project-name
                   region: region
-                  node_template: node-template-name
+                  name: node-template-name
     """
     result = {
         "comment": [],
         "ret": None,
         "result": True,
     }
 
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
-    ret = await hub.exec.gcp_api.client.compute.node_template.get(
-        ctx, project=project, region=region, nodeTemplate=node_template
-    )
+    if resource_id:
+        ret = await hub.exec.gcp_api.client.compute.node_template.get(
+            ctx,
+            resource_id=resource_id,
+        )
+    elif project and region and name:
+        ret = await hub.exec.gcp_api.client.compute.node_template.get(
+            ctx, project=project, region=region, nodeTemplate=name
+        )
+    else:
+        result["result"] = False
+        result["comment"] = [
+            f"gcp.compute.node_template#get(): {name} either resource_id or project, region and name should be specified."
+        ]
+        return result
 
     if not ret["result"]:
         result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
     result["ret"] = ret["ret"]
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/reservation.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/reservation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Exec module for managing Reservations."""
 from typing import Any
 from typing import Dict
 
-from idem_gcp.tool.gcp.utils import get_project_from_account
 
 __func_alias__ = {"list_": "list"}
 
 
 async def list_(
     hub,
     ctx,
     project: str = None,
     zone: str = None,
-    filter: str = None,
+    filter_: (str, "alias=filter") = None,
     order_by: str = None,
 ) -> Dict[str, Any]:
     r"""A list of all the reservations that have been configured for the specified project in specified zone.
 
     Args:
         project(str, Optional):
             Project ID for this request.
@@ -27,105 +26,105 @@
         filter(str, Optional):
             A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name "instance", you would use `name ne .*instance`.
 
         order_by(str, Optional):
             Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.reservation.list
               - kwargs:
                   project: project-name
     """
     result = {
         "comment": [],
         "ret": None,
         "result": True,
     }
 
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     if zone:
         ret = await hub.exec.gcp_api.client.compute.reservation.list(
             ctx,
             project=project,
             zone=zone,
-            filter=filter,
+            filter=filter_,
             orderBy=order_by,
         )
     else:
         ret = await hub.exec.gcp_api.client.compute.reservation.aggregatedList(
             ctx,
             project=project,
-            filter=filter,
+            filter=filter_,
             orderBy=order_by,
         )
 
     if not ret["result"]:
         result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
     result["comment"] += ret["comment"]
-    result["ret"] = ret["ret"]["items"]
+    result["ret"] = ret["ret"].get("items", [])
     return result
 
 
 async def get(
     hub,
     ctx,
     resource_id: str = None,
     project: str = None,
     zone: str = None,
-    reservation: str = None,
+    name: str = None,
 ) -> Dict[str, Any]:
     r"""Retrieves information about the specified reservation.
 
     Args:
         resource_id(str, Optional):
             An identifier of the resource in the provider.
 
         project(str, Optional):
             Project ID for this request.
 
         zone(str, Optional):
             Name of the zone for this request.
 
-        reservation(str, Optional):
+        name(str, Optional):
             Name of the reservation to retrieve.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
               - path: gcp.compute.reservation.get
               - kwargs:
                   project: project-name
                   zone: zone
-                  reservation: reservation-name
+                  name: reservation-name
     """
     result = {
         "comment": [],
         "ret": None,
         "result": True,
     }
 
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     if resource_id:
         ret = await hub.exec.gcp_api.client.compute.reservation.get(
             ctx, resource_id=resource_id
         )
     else:
         ret = await hub.exec.gcp_api.client.compute.reservation.get(
-            ctx, project=project, zone=zone, reservation=reservation
+            ctx, project=project, zone=zone, reservation=name
         )
 
     if not ret["result"]:
         result["comment"] += ret["comment"]
         result["result"] = False
         return result
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/resource_policy.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/zone.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,138 +1,118 @@
-"""Exec module for managing Resource Policies."""
-__func_alias__ = {"list_": "list"}
+"""Exec module for managing Zones."""
+from typing import Any
+from typing import Dict
 
-from idem_gcp.tool.gcp.utils import get_project_from_account
+__func_alias__ = {"list_": "list"}
 
 
 async def list_(
     hub,
     ctx,
     project: str = None,
-    region: str = None,
-    filter: str = None,
+    filter_: (str, "alias=filter") = None,
     order_by: str = None,
-):
-    r"""A list all the resource policies that have been configured for the specified project in specified region.
+) -> Dict[str, Any]:
+    r"""Retrieves the list of Zone resources available to the specified project.
 
     Args:
         project(str, Optional):
             Project ID for this request.
 
-        region(str, Optional):
-            Name of the region for this request.
-
         filter(str, Optional):
             A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name "instance", you would use `name ne .*instance`.
 
         order_by(str, Optional):
             Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.resource_policy.list
+              - path: gcp.compute.zone.list
               - kwargs:
                   project: project-name
-                  region: region-name
+                  filter_: status=UP
     """
-    result = {
-        "comment": [],
-        "ret": None,
-        "result": True,
-    }
+    result = dict(comment=[], ret=[], result=True)
 
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
-    if region:
-        ret = await hub.exec.gcp_api.client.compute.resource_policy.list(
-            ctx,
-            project=project,
-            region=region,
-            filter=filter,
-            orderBy=order_by,
-        )
-    else:
-        ret = await hub.exec.gcp_api.client.compute.resource_policy.aggregatedList(
-            ctx,
-            project=project,
-            filter=filter,
-            orderBy=order_by,
-        )
+    ret = await hub.exec.gcp_api.client.compute.zone.list(
+        ctx,
+        project=project,
+        filter=filter_,
+        orderBy=order_by,
+    )
 
-    result["comment"] += ret["comment"]
     if not ret["result"]:
+        result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
-    result["ret"] = ret["ret"]["items"]
+    result["ret"] = ret["ret"].get("items", [])
+    result["comment"] += ret["comment"]
     return result
 
 
 async def get(
     hub,
     ctx,
-    project: str = None,
-    region: str = None,
     name: str = None,
+    project: str = None,
     resource_id: str = None,
 ):
-    r"""Retrieves all information of the specified resource policy.
+    r"""Returns the specified Zone resource.
 
     Args:
-        project(str, Optional):
-            Project ID for this request. Defaults to None.
-
-        region(str, Optional):
-            Name of the region for this request. Defaults to None.
+        resource_id(str, Optional):
+            An identifier of the resource in the provider.
+            Defaults to None.
 
         name(str, Optional):
-            Name of the resource policy to retrieve. Defaults to None.
+            Name of the zone resource to return.
 
-        resource_id(str, Optional):
-            An identifier of the resource in the provider. Defaults to None.
+        project(str, Optional):
+            Project ID for this request.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.resource_policy.get
+              - path: gcp.compute.zone.get
               - kwargs:
                   project: project-name
-                  region: region-name
-                  name: resource-policy-name
+                  name: zone-name
     """
-    result = {
-        "comment": [],
-        "ret": None,
-        "result": True,
-    }
+    result = dict(comment=[], ret=[], result=True)
 
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     if resource_id:
-        ret = await hub.exec.gcp_api.client.compute.resource_policy.get(
+        ret = await hub.exec.gcp_api.client.compute.zone.get(
             ctx,
             resource_id=resource_id,
         )
-    elif project and region and name:
-        ret = await hub.exec.gcp_api.client.compute.resource_policy.get(
-            ctx, project=project, region=region, resource_policy=name
+    elif project and name:
+        ret = await hub.exec.gcp_api.client.compute.zone.get(
+            ctx,
+            project=project,
+            zone=name,
         )
     else:
         result["result"] = False
         result["comment"] = [
-            f"gcp.compute.resource_policy {name} either resource_id or project, region and name"
+            f"gcp.compute.zone {name} either resource_id or project and name"
             f" should be specified."
         ]
         return result
 
-    result["comment"] += ret["comment"]
     if not ret["result"]:
+        result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
     result["ret"] = ret["ret"]
+    result["comment"] += ret["comment"]
     return result
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/snapshot.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/target_pool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,92 +1,116 @@
+"""Exec module for managing Target Pool."""
+
 __func_alias__ = {"list_": "list"}
 
+from typing import Any, Dict
+
 from idem_gcp.tool.gcp.generate.exec_context import ExecutionContext
-from idem_gcp.tool.gcp.utils import get_project_from_account
+from idem_gcp.tool.gcp.generate.exec_param import ExecParam
+from idem_gcp.tool.gcp.generate.scope import Scope
 
 
 async def list_(
     hub,
     ctx,
     project: str = None,
-    filter: str = None,
+    region: str = None,
+    filter_: (str, "alias=filter") = None,
     order_by: str = None,
 ):
-    r"""Retrieves the list of Snapshot resources contained within the specified project.
+    r"""Retrieves a list of target pools available to the specified project and region.
 
     Args:
         project(str, Optional):
             Project ID for this request.
 
+        region(str, Optional):
+            Name of the region scoping this request.
+
         filter(str, Optional):
             A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name "instance", you would use `name ne .*instance`.
 
         order_by(str, Optional):
             Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
-            random-name:
+            list-target_pool:
               exec.run:
-              - path: gcp.compute.snapshot.list
+              - path: gcp.compute.target_pool.list
               - kwargs:
                   project: project-name
     """
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     execution_context = ExecutionContext(
-        resource_type="compute.snapshot",
+        resource_type="compute.target_pool",
         method_name="list",
         method_params={
             "ctx": ctx,
             "project": project,
-            "filter": filter,
+            "region": region,
+            "filter": filter_,
             "order_by": order_by,
         },
+        exec_params={
+            ExecParam.SCOPED_FUNCTIONS: {
+                Scope.REGIONAL: "list",
+                Scope.GLOBAL: "aggregatedList",
+            }
+        },
     )
+
     return await hub.tool.gcp.generate.generic_exec.execute(execution_context)
 
 
 async def get(
     hub,
     ctx,
-    resource_id: str = None,
     project: str = None,
-    snapshot: str = None,
-):
-    r"""Returns the specified Snapshot resource. Gets a list of available snapshots by making a list() request.
+    region: str = None,
+    name: str = None,
+    resource_id: str = None,
+) -> Dict[str, Any]:
+    r"""Returns the specified target pool.
 
     Args:
-        resource_id(str, Optional):
-            An identifier of the resource in the provider.
-
-        project(str, Optional):
+        project (str, Optional):
             Project ID for this request.
+        region (str, Optional):
+            The region in which to search.
+        name (str, Optional):
+            Name of the TargetPool resource to return.
+        resource_id (str, Optional):
+            Idem resource ID.
 
-        snapshot(str, Optional):
-            Name of the snapshot resource to return.
+    Returns:
+        Dict[str, Any]
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
-            random-name:
-              exec.run:
-              - path: gcp.compute.instance.get
-              - kwargs:
-                  project: project-name
-                  zone: zone-name
-                  instance: instance-name
+            get-target-pool:
+                exec.run:
+                   - path: gcp.compute.target_pool.get
+                   - kwargs:
+                       project: project-name
+                       name: target-pool-name
+                       region: region-name
+                       resource_id: resource-id
     """
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     execution_context = ExecutionContext(
-        resource_type="compute.snapshot",
+        resource_type="compute.target_pool",
         method_name="get",
         method_params={
             "ctx": ctx,
             "resource_id": resource_id,
             "project": project,
-            "snapshot": snapshot,
+            "region": region,
+            "targetPool": name,
         },
     )
+
     return await hub.tool.gcp.generate.generic_exec.execute(execution_context)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/zone.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/health_check.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,120 +1,93 @@
-"""Exec module for managing Zones."""
-from typing import Any
-from typing import Dict
-
-from idem_gcp.tool.gcp.utils import get_project_from_account
+"""Exec module for managing HealthChecks."""
+from idem_gcp.tool.gcp.generate.exec_context import ExecutionContext
 
 __func_alias__ = {"list_": "list"}
 
 
 async def list_(
     hub,
     ctx,
     project: str = None,
-    filter: str = None,
+    filter_: (str, "alias=filter") = None,
     order_by: str = None,
-) -> Dict[str, Any]:
-    r"""Retrieves the list of Zone resources available to the specified project.
+):
+    r"""Retrieves the list of HealthCheck resources available to the specified project.
 
     Args:
         project(str, Optional):
             Project ID for this request.
 
         filter(str, Optional):
             A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name "instance", you would use `name ne .*instance`.
 
         order_by(str, Optional):
             Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.zone.list
+              - path: gcp.compute.health_check.list
               - kwargs:
                   project: project-name
-                  filter: status=UP
     """
-    result = dict(comment=[], ret=[], result=True)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
-    project = get_project_from_account(ctx, project)
-
-    ret = await hub.exec.gcp_api.client.compute.zone.list(
-        ctx,
-        project=project,
-        filter=filter,
-        orderBy=order_by,
+    execution_context = ExecutionContext(
+        resource_type="compute.health_check",
+        method_name="list",
+        method_params={
+            "ctx": ctx,
+            "project": project,
+            "filter": filter_,
+            "order_by": order_by,
+        },
     )
 
-    if not ret["result"]:
-        result["comment"] += ret["comment"]
-        result["result"] = False
-        return result
-
-    result["ret"] = ret["ret"]["items"]
-    result["comment"] += ret["comment"]
-    return result
+    return await hub.tool.gcp.generate.generic_exec.execute(execution_context)
 
 
 async def get(
     hub,
     ctx,
-    name: str = None,
-    project: str = None,
     resource_id: str = None,
+    project: str = None,
+    name: str = None,
 ):
-    r"""Returns the specified Zone resource.
+    r"""Returns the specified HealthCheck resource. Gets a list of available health checks by making a list() request.
 
     Args:
-        resource_id(str, Optional):
-            An identifier of the resource in the provider.
-            Defaults to None.
+        project(str, Optional):
+            Project ID for this request. Defaults to None.
 
         name(str, Optional):
-            Name of the zone resource to return.
+            Name of the resource to return. Defaults to None.
 
-        project(str, Optional):
-            Project ID for this request.
+        resource_id(str, Optional):
+            An identifier of the resource in the provider. Defaults to None.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.zone.get
+              - path: gcp.compute.health_check.get
               - kwargs:
                   project: project-name
-                  name: zone-name
+                  name: health-check-name
     """
-    result = dict(comment=[], ret=[], result=True)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
-    project = get_project_from_account(ctx, project)
+    execution_context = ExecutionContext(
+        resource_type="compute.health_check",
+        method_name="get",
+        method_params={
+            "ctx": ctx,
+            "resource_id": resource_id,
+            "project": project,
+            "healthCheck": name,
+        },
+    )
 
-    if resource_id:
-        ret = await hub.exec.gcp_api.client.compute.zone.get(
-            ctx,
-            resource_id=resource_id,
-        )
-    elif project and name:
-        ret = await hub.exec.gcp_api.client.compute.zone.get(
-            ctx,
-            project=project,
-            zone=name,
-        )
-    else:
-        result["result"] = False
-        result["comment"] = [
-            f"gcp.compute.zone {name} either resource_id or project and name"
-            f" should be specified."
-        ]
-        return result
-
-    if not ret["result"]:
-        result["comment"] += ret["comment"]
-        result["result"] = False
-        return result
-
-    result["ret"] = ret["ret"]
-    result["comment"] += ret["comment"]
-    return result
+    return await hub.tool.gcp.generate.generic_exec.execute(execution_context)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/exec/gcp_api/init.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp_api/init.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.9.0/idem_gcp/helpers/exc.py` & `idem_gcp-1.1.0/idem_gcp/helpers/exc.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.9.0/idem_gcp/helpers/log.py` & `idem_gcp-1.1.0/idem_gcp/helpers/log.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.9.0/idem_gcp/helpers/returns.py` & `idem_gcp-1.1.0/idem_gcp/helpers/returns.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.9.0/idem_gcp/resources/properties.yaml` & `idem_gcp-1.1.0/idem_gcp/resources/properties.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 # TODO: check for nested create-only properties
 
 # TODO: Make sure to check if these properties correspond correctly to the JSON schema
-# e.g. according to the GCP docs for storage.bucket.instert https://cloud.google.com/storage/docs/json_api/v1/buckets/insert
-# we have the properties
-#    - customPlacementConfig
-#    - dataLocations
-# but according to the schema, dataLocations is a nested object of customPlacementConfig
 
 # TODO: Don't add projection
 
 compute.zone_operation:
   get:
     - project
     - zone
@@ -23,14 +18,16 @@
 
 compute.global_operation:
   get:
     - project
     - operation
 
 compute.instance:
+  manual_mapping:
+    body.network_interfaces.network_ip: networkIP
   get:
     - project
     - zone
     - instance
     - status
   insert:
 #    path parameters
@@ -127,23 +124,27 @@
     - sourceInstanceTemplate
     - requestId
     - mostDisruptiveAllowedAction
     - minimalAction
     - fingerprint
     - labelFingerprint
     - networkInterfaces[].fingerprint
-    - networkInterfaces[].networkIp
-    - networkInterfaces[].accessConfigs[].natIp
     - tags.fingerprint
     - metadata.fingerprint
+  readonly_return_props:
+    - id
   exclude_properties_from_transformation:
+    - disks.initializeParams.labels
     - labels
     - tags
   nested_non_updatable_properties:
     - disks[].initializeParams
+  relevant_dict_items_removed:
+    # dictKeysPlaceholder is used to specify that the label keys are relevant if removed, not the labels property itself
+    - labels.dictKeysPlaceholder
 
 compute.accelerator_type:
   get:
     - project
     - zone
     - acceleratorType
   fields_enum_type:
@@ -196,14 +197,15 @@
     - availableCpuPlatforms
     - supportsPzs
 
 compute.disk_type:
   get:
     - project
     - zone
+    - region
     - diskType
   fields_enum_type:
     - creationTimestamp
     - defaultDiskSizeGb
     - deprecated
     - description
     - id
@@ -214,19 +216,21 @@
     - validDiskSize
     - zone
 
 compute.disk:
   get:
     - project
     - zone
+    - region
     - disk
   insert:
 #    path parameters
     - project
     - zone
+    - region
 #    query parameters
     - requestId
     - sourceImage
 #    body
     - name
     - description
     - sizeGb
@@ -247,27 +251,36 @@
     - physicalBlockSizeBytes
     - resourcePolicies
     - sourceDisk
     - provisionedIops
     - locationHint
     - architecture
     - params
+  update:
+    - labels
+    - resourcePolicies
+    - sizeGb
   delete:
 #   path parameters
     - project
     - zone
     - disk
 #   query parameters
     - requestId
   exclude_paths:
     - label_fingerprint
+  readonly_return_props:
+    - id
   exclude_properties_from_transformation:
     - labels
     - tags
     - resourceManagerTags
+  missing_property_assumed_value:
+    labels: {}
+    resourcePolicies: []
 
 compute.machine_image:
   get:
     - project
     - machineImage
   insert:
 #    path parameters
@@ -308,30 +321,31 @@
     - internalIpv6Range
     - IPv4Range
     - mtu
     - networkFirewallPolicyEnforcementOrder
     - routingConfig
     - peerings
   update:
-    - name
-    - autoCreateSubnetworks
-    - description
     - enableUlaInternalIpv6
     - internalIpv6Range
     - IPv4Range
     - mtu
     - networkFirewallPolicyEnforcementOrder
     - routingConfig
     - peerings
+  readonly_return_props:
+    - id
   delete:
 #   path parameters
     - project
     - network
 #   query parameters
     - requestId
+  exclude_paths:
+    - peerings
 
 compute.node_template:
   get:
     - project
     - region
     - nodeTemplate
   insert:
@@ -395,74 +409,134 @@
 #   path parameters
     - project
     - zone
     - reservation
 #   query parameters
     - requestId
 
-storage.buckets:
+storage.bucket:
   get:
     - bucket
-#    - ifMetagenerationMatch
-#    - ifMetagenerationNotMatch
+    - projection
   insert:
-#    - project
-#    - predefinedAcl
-#    - predefinedDefaultObjectAcl
+#     query parameters
+    - predefinedAcl
+    - predefinedDefaultObjectAcl
+    - project
+    - projection
+    - userProject
+#     body
     - name
-    - acl
+    - autoclass
     - billing
     - cors
     - customPlacementConfig
     - defaultEventBasedHold
-    - defaultObjectAcl
     - encryption
     - iamConfiguration
     - labels
     - lifecycle
     - location
     - logging
     - retentionPolicy
     - rpo
     - storageClass
     - versioning
     - website
+# TODO [DA]: Remove nested properties if separate Access Control resources are defined
+    - acl
+    - defaultObjectAcl
   update:
     - bucket # TODO: this is equal to name from insert so perhaps we should annotate equivalent properties with different names from the different methods
 #    - ifMetagenerationMatch
 #    - ifMetagenerationNotMatch
 #    - predefinedAcl
-    - acl
     - billing
     - cors
     - defaultEventBasedHold
-    - defaultObjectAcl
     - encryption
     - iamConfiguration
     - labels
     - lifecycle
     - logging
     - retentionPolicy
     - rpo
     - storageClass
     - versioning
     - website
+# TODO [DA]: Remove nested properties if separate Access Control resources are defined
+    - acl
+    - defaultObjectAcl
   delete:
+#   path parameters
     - bucket
-#    - ifMetagenerationMatch
-#    - ifMetagenerationNotMatch
+#   query parameters
+    - userProject
 #  equivalent_properties:
 #    - [metageneration, ifMetagenerationMatch, ifMetagenerationNotMatch]
 #    - [bucket, name]
 #  resource_id:
 #      - name
 #      - bucket
 #    metageneration:
 #      - ifMetagenerationMatch
 #      - ifMetagenerationNotMatch
+  readonly_return_props:
+    - metageneration
+  exclude_paths:
+    - iamConfiguration.bucketPolicyOnly
+#   read-only nested props - don't consider them in diff, but we still return them
+    - iamConfiguration.uniformBucketLevelAccess.lockedTime
+    - retentionPolicy.effectiveTime
+  exclude_properties_from_transformation:
+    - labels
+  nested_non_updatable_properties:
+    - acl[].bucket
+    - acl[].domain
+    - acl[].email
+    - acl[].entityId
+    - acl[].etag
+    - acl[].id
+    - acl[].kind
+    - acl[].projectTeam.projectNumber
+    - acl[].projectTeam.team
+    - acl[].selfLink
+    - defaultObjectAcl[].domain
+    - defaultObjectAcl[].email
+    - defaultObjectAcl[].entityId
+    - defaultObjectAcl[].etag
+    - defaultObjectAcl[].kind
+    - defaultObjectAcl[].projectTeam.team
+    - defaultObjectAcl[].projectTeam.projectNumber
+  missing_property_assumed_value:
+    autoclass:
+      enabled: False
+    billing:
+      requesterPays: False
+    cors: []
+    customPlacementConfig: null
+    defaultEventBasedHold: False
+    encryption: null
+    iamConfiguration:
+      publicAccessPrevention: inherited
+      uniformBucketLevelAccess:
+        enabled: False
+    lifecycle:
+      rule: []
+    location: US
+    logging: null
+    retentionPolicy: null
+    storageClass: STANDARD
+    versioning:
+      enabled: False
+    labels: {}
+    website:
+      mainPageSuffix: null
+      notFoundPage: null
+
 
 compute.resource_policy:
   get:
     - project
     - region
     - resourcePolicy
   insert:
@@ -643,23 +717,44 @@
     - enableFlowLogs
     - privateIpv6GoogleAccess
     - purpose
     - role
     - logConfig
     - stackType
     - ipv6AccessType
+  readonly_return_props:
+    - id
 
 compute.firewall:
+  manual_mapping:
+    body.allowed.ip_protocol: IPProtocol
+    body.denied.ip_protocol: IPProtocol
   get:
     - project
-    - firewall_id
-  insert:
+  fields_enum_type:
     - kind
     - id
     - creationTimestamp
+  insert:
+    - name
+    - description
+    - network
+    - priority
+    - sourceRanges
+    - destinationRanges
+    - sourceTags
+    - targetTags
+    - sourceServiceAccounts
+    - targetServiceAccounts
+    - allowed
+    - denied
+    - direction
+    - logConfig
+    - disabled
+  update:
     - name
     - description
     - network
     - priority
     - sourceRanges
     - destinationRanges
     - sourceTags
@@ -667,15 +762,14 @@
     - sourceServiceAccounts
     - targetServiceAccounts
     - allowed
     - denied
     - direction
     - logConfig
     - disabled
-    - selfLink
 
 compute.snapshot:
   get:
     - project
     - snapshot
   insert:
 #    path parameters
@@ -691,17 +785,457 @@
     - locationHint
     - description
     - sourceDisk
     - chainName
     - storageLocations
     - sourceDiskEncryptionKey
     - name
+  update:
+    - labels
+    - labelFingerprint
   delete:
 #   path parameters
     - project
     - snapshot
 #   query parameters
     - requestId
   exclude_paths:
     - labelFingerprint
   exclude_properties_from_transformation:
     - labels
+
+compute.health_check:
+  get:
+#     path parameters
+    - project
+    - resourceId
+#     query parameters
+    - requestId
+  insert:
+#     path parameters
+    - project
+#     query parameters
+    - requestId
+#     body
+    - name
+    - description
+    - checkIntervalSec
+    - timeoutSec
+    - unhealthyThreshold
+    - healthyThreshold
+    - type
+    - tcpHealthCheck
+    - sslHealthCheck
+    - httpHealthCheck
+    - httpsHealthCheck
+    - http2HealthCheck
+    - grpcHealthCheck
+    - logConfig
+  update:
+#     path parameters
+    - project
+#     query parameters
+    - requestId
+#     body
+    - description
+    - checkIntervalSec
+    - timeoutSec
+    - unhealthyThreshold
+    - healthyThreshold
+    - type
+    - tcpHealthCheck
+    - sslHealthCheck
+    - httpHealthCheck
+    - httpsHealthCheck
+    - http2HealthCheck
+    - grpcHealthCheck
+    - logConfig
+  delete:
+#     path parameters
+    - project
+    - resourceId
+#     query parameters
+    - requestId
+  readonly_return_props:
+    - name
+
+compute.instance_group:
+  get:
+    - project
+    - zone
+    - name
+  insert:
+#    path parameters
+    - project
+    - zone
+#    query parameters
+    - requestId
+#    body
+    - name
+    - description
+    - namedPorts
+    - network
+    - subnetwork
+  update:
+#    path parameters
+    - project
+    - zone
+    - name
+#    query parameters
+    - requestId
+#    body
+    - namedPorts
+  delete:
+#    path parameters
+    - project
+    - zone
+    - name
+#    query parameters
+    - requestId
+  readonly_return_props:
+    - name
+    - description
+    - fingerprint
+    - network
+    - subnetwork
+
+compute.forwarding_rule:
+  manual_mapping:
+    body.ip_address: IPAddress
+    body.ip_protocol: IPProtocol
+  get:
+#     path parameters
+    - project
+    - region
+    - resourceId
+#     query parameters
+    - requestId
+  insert:
+#     path parameters
+    - project
+    - region
+#     query parameters
+    - requestId
+#     body
+    - name
+    - description
+    - region
+    - labels
+    - labelFingerprint
+    - allowGlobalAccess
+    - portRange
+    - serviceName
+    - backendService
+    - pscConnectionId
+    - serviceDirectoryRegistrations
+    - IPProtocol
+    - target
+    - ipVersion
+    - isMirroringCollector
+    - networkTier
+    - noAutomateDnsZone
+    - IPAddress
+    - network
+    - pscConnectionStatus
+    - subnetwork
+    - allPorts
+    - serviceLabel
+    - loadBalancingScheme
+    - ports
+    - metadataFilters
+  update:
+    #     path parameters
+    - project
+    - region
+    #     query parameters
+    - requestId
+    #     body
+    - labels
+    - labelFingerprint
+    - target
+    - networkTier
+  delete:
+#     path parameters
+    - project
+    - region
+    - resourceId
+#     query parameters
+    - requestId
+  fields_enum_type:
+    - kind
+    - id
+    - creationTimestamp
+    - IPProtocol
+    - ipVersion
+    - networkTier
+    - pscConnectionStatus
+    - loadBalancingScheme
+  exclude_paths:
+    - labelFingerprint
+
+compute.backend_service:
+  get:
+    - project
+    - region
+    - backendService
+  insert:
+    #     path parameters
+    - project
+    - region
+    #     query parameters
+    - requestId
+    #     body
+    - name
+    - description
+    - backends
+    - healthChecks
+    - timeoutSec
+    - port
+    - fingerprint
+    - portName
+    - enableCDN
+    - affinityCookieTtlSec
+    - failoverPolicy
+    - connectionDraining
+    - iap
+    - cdnPolicy
+    - customRequestHeaders
+    - customResponseHeaders
+    - logConfig
+    - securitySettings
+    - consistentHash
+    - circuitBreakers
+    - outlierDetection
+    - network
+    - subsetting
+    - connectionTrackingPolicy
+    - maxStreamDuration
+    - serviceBindings
+    - localityLbPolicies
+  update:
+    - description
+    - backends
+    - healthChecks
+    - timeoutSec
+    - port
+    - fingerprint
+    - portName
+    - enableCDN
+    - affinityCookieTtlSec
+    - region
+    - failoverPolicy
+    - connectionDraining
+    - iap
+    - cdnPolicy
+    - customRequestHeaders
+    - customResponseHeaders
+    - logConfig
+    - securitySettings
+    - consistentHash
+    - circuitBreakers
+    - outlierDetection
+    - network
+    - subsetting
+    - connectionTrackingPolicy
+    - maxStreamDuration
+    - serviceBindings
+    - localityLbPolicies
+  exclude_paths:
+    - project
+    - id
+    - fingerprint
+  delete:
+    #     path parameters
+    - project
+    - resourceId
+    - region
+    - backendService
+    #     query parameters
+    - requestId
+  fields_enum_type:
+    - id
+    - protocol
+    - sessionAffinity
+    - loadBalancingScheme
+    - localityLbPolicy
+    - compressionMode
+
+compute.region_backend_service:
+  get:
+    - project
+    - region
+    - backendService
+  insert:
+    #     path parameters
+    - project
+    - region
+    #     query parameters
+    - requestId
+    #     body
+    - name
+    - description
+    - backends
+    - healthChecks
+    - timeoutSec
+    - port
+    - fingerprint
+    - portName
+    - enableCDN
+    - affinityCookieTtlSec
+    - failoverPolicy
+    - connectionDraining
+    - iap
+    - cdnPolicy
+    - customRequestHeaders
+    - customResponseHeaders
+    - logConfig
+    - securitySettings
+    - consistentHash
+    - circuitBreakers
+    - outlierDetection
+    - network
+    - subsetting
+    - connectionTrackingPolicy
+    - maxStreamDuration
+    - serviceBindings
+    - localityLbPolicies
+  update:
+    - description
+    - backends
+    - healthChecks
+    - timeoutSec
+    - port
+    - fingerprint
+    - portName
+    - enableCDN
+    - affinityCookieTtlSec
+    - region
+    - failoverPolicy
+    - connectionDraining
+    - iap
+    - cdnPolicy
+    - customRequestHeaders
+    - customResponseHeaders
+    - logConfig
+    - securitySettings
+    - consistentHash
+    - circuitBreakers
+    - outlierDetection
+    - network
+    - subsetting
+    - connectionTrackingPolicy
+    - maxStreamDuration
+    - serviceBindings
+    - localityLbPolicies
+  exclude_paths:
+    - project
+    - id
+    - fingerprint
+  delete:
+    #     path parameters
+    - project
+    - resourceId
+    - region
+    - backendService
+    #     query parameters
+    - requestId
+  fields_enum_type:
+    - id
+    - protocol
+    - sessionAffinity
+    - loadBalancingScheme
+    - localityLbPolicy
+    - compressionMode
+
+iam.projects.service_account:
+  request_parameters:
+    list:
+      - name
+    get:
+      - name
+    create:
+      - name
+    delete:
+      - name
+    undelete:
+      - name
+    enable:
+      - name
+    disable:
+      - name
+    patch:
+      - name
+  response_fields:
+    list: accounts
+  get:
+#     path parameters
+    - project
+    - resourceId
+#     query parameters
+    - requestId
+  insert:
+    - displayName
+    - description
+  update:
+    - displayName
+    - description
+  resource_id:
+    - name
+  readonly_return_props:
+    - projectId
+    - uniqueId
+    - email
+    - name
+    - etag
+    - oauth2ClientId
+    - disabled
+
+compute.target_pool:
+  get:
+    - project
+    - region
+    - targetPool
+  insert:
+    - name
+    - description
+    - failoverRatio
+    - backupPool
+  readonly_return_props:
+    - kind
+    - id
+    - selfLink
+    - region
+  fields_enum_type:
+    - id
+    - sessionAffinity
+  resource_id:
+    - name
+
+iam.projects.service_accounts.key:
+  request_parameters:
+    list:
+      - name
+    get:
+      - name
+    create:
+      -name
+    delete:
+      -name
+    upload:
+      -name
+    disable:
+      -name
+    enable:
+      -name
+  resource_id:
+    - name
+  create:
+    - name
+    - privateKeyType
+    - keyAlgorithm
+    - privateKeyData
+    - publicKeyData
+    - validAfterTime
+    - validBeforeTime
+    - keyOrigin
+    - keyType
+    - disabled
```

### Comparing `idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/crypto_key.py` & `idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/crypto_key.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """State module for managing Cloud Key Management Service crypto keys."""
-import copy
-from copy import deepcopy
 from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 
 __contracts__ = ["resource"]
+RESOURCE_TYPE = "cloudkms.crypto_key"
+RESOURCE_TYPE_FULL = "cloudkms.projects.locations.key_rings.crypto_keys"
+GCP_RESOURCE_TYPE_FULL = "gcp.cloudkms.crypto_key"
 
 
 async def present(
     hub,
     ctx,
     name: str,
     crypto_key_id: str = None,
@@ -90,15 +91,15 @@
     labels: Dict[str, str] = None,
     import_only: bool = None,
     destroy_scheduled_duration: str = None,
     crypto_key_backend: str = None,
     rotation_period: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
-    """Create or update a `CryptoKey`_ within a `KeyRing`_.
+    r"""Create or update a `CryptoKey`_ within a `KeyRing`_.
 
     `CryptoKey.purpose`_ and `CryptoKey.version_template.algorithm`_ are required for a new `CryptoKey`_.
 
     Args:
         name(str):
             Idem name.
 
@@ -126,16 +127,18 @@
         create_time(str, Optional):
             Output only. The time at which this CryptoKey was created. A timestamp in RFC3339 UTC "Zulu" format, with
             nanosecond resolution and up to nine fractional digits. Examples: "2014-10-02T15:01:23Z" and
             "2014-10-02T15:01:23.045123456Z".
 
         next_rotation_time(str, Optional):
             At nextRotationTime, the Key Management Service will automatically:
-                - Create a new version of this CryptoKey.
-                - Mark the new version as primary.
+
+            - Create a new version of this CryptoKey.
+            - Mark the new version as primary.
+
             Key rotations performed manually via cryptoKeyVersions.create and cryptoKeys.updatePrimaryVersion do not
             affect nextRotationTime. Keys with purpose ENCRYPT_DECRYPT support automatic rotation. For other keys, this
             field must be omitted. A timestamp in RFC3339 UTC "Zulu" format, with nanosecond resolution and up to nine
             fractional digits. Examples: "2014-10-02T15:01:23Z" and "2014-10-02T15:01:23.045123456Z".
 
         version_template(Dict[str, Any], Optional):
             A template describing settings for new CryptoKeyVersion instances. The properties of new CryptoKeyVersion
@@ -211,81 +214,70 @@
         "result": True,
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
-    create_if_missing = False
-    if not resource_id:
-        if project_id and location_id and key_ring_id and crypto_key_id:
-            resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
-                "cloudkms.projects.locations.key_rings.crypto_keys",
-                {
-                    "project_id": project_id,
-                    "location_id": location_id,
-                    "key_ring_id": key_ring_id,
-                    "crypto_key_id": crypto_key_id,
-                },
-            )
-            create_if_missing = True
-        else:
-            result["result"] = False
-            result["comment"].append(
-                "When creating new resource crypto_key_id, project_id, location_id and key_ring_id parameters are required!"
+    get_resource_only_with_resource_id = hub.OPT.idem.get(
+        "get_resource_only_with_resource_id", False
+    )
+
+    if hub.tool.gcp.resource_prop_utils.properties_mismatch_resource_id(
+        RESOURCE_TYPE_FULL,
+        resource_id,
+        {
+            "project_id": project_id,
+            "location_id": location_id,
+            "key_ring_id": key_ring_id,
+            "crypto_key_id": crypto_key_id,
+        },
+    ):
+        result["comment"].append(
+            hub.tool.gcp.comment_utils.properties_mismatch_resource_id_comment(
+                RESOURCE_TYPE_FULL, name
             )
-            return result
-    else:
-        els = hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
-            "cloudkms.projects.locations.key_rings.crypto_keys", resource_id
         )
-        if project_id and location_id and key_ring_id and crypto_key_id:
-            if (
-                els.get("project_id") != project_id
-                or els.get("location_id") != location_id
-                or els.get("key_ring_id") != key_ring_id
-                or els.get("crypto_key_id") != crypto_key_id
-            ):
-                result["result"] = False
-                result["comment"].append(
-                    hub.tool.gcp.comment_utils.non_updatable_properties_comment(
-                        "gcp.cloudkms.crypto_key",
-                        resource_id,
-                        ["project_id", "location_id", "key_ring_id", "crypto_key_id"],
-                    )
-                )
-                return result
-        else:
-            project_id = els.get("project_id")
-            location_id = els.get("location_id")
-            key_ring_id = els.get("key_ring_id")
-            crypto_key_id = els.get("crypto_key_id")
 
-    is_create = False
     if resource_id:
         old_get_ret = await hub.exec.gcp.cloudkms.crypto_key.get(
             ctx, resource_id=resource_id
         )
-        if not old_get_ret["result"] or not old_get_ret["ret"]:
-            if not create_if_missing:
-                result["result"] = False
-                result["comment"] += old_get_ret["comment"]
-                return result
-            is_create = True
-        else:
-            result["old_state"] = {
-                "name": name,
+
+        if not old_get_ret["result"] or (
+            not old_get_ret["ret"] and get_resource_only_with_resource_id
+        ):
+            result["result"] = False
+            result["comment"] += old_get_ret["comment"]
+            return result
+
+        result["old_state"] = old_get_ret["ret"]
+    elif not get_resource_only_with_resource_id:
+        resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
+            RESOURCE_TYPE_FULL,
+            {
                 "project_id": project_id,
                 "location_id": location_id,
                 "key_ring_id": key_ring_id,
                 "crypto_key_id": crypto_key_id,
-                **copy.copy(old_get_ret["ret"]),
-            }
+            },
+        )
+        old_get_ret = await hub.exec.gcp.cloudkms.crypto_key.get(
+            ctx, resource_id=resource_id
+        )
 
-    if is_create:
+        if not old_get_ret["result"]:
+            result["result"] = False
+            result["comment"] += old_get_ret["comment"]
+            return result
+
+        if old_get_ret["ret"]:
+            result["old_state"] = old_get_ret["ret"]
+
+    if not result["old_state"]:
         resource_body = {
             "purpose": purpose,
             "next_rotation_time": next_rotation_time,
             "version_template": version_template,
             "labels": labels,
             "import_only": import_only,
             "destroy_scheduled_duration": destroy_scheduled_duration,
@@ -300,142 +292,175 @@
                 labels, result["old_state"].get("labels")
             ),
             "rotation_period": rotation_period,
         }
 
     resource_body = {k: v for (k, v) in resource_body.items() if v is not None}
 
-    if ctx["test"]:
-        if is_create:
-            result["comment"].append(
-                hub.tool.gcp.comment_utils.would_create_comment(
-                    "gcp.cloudkms.crypto_key", resource_id
-                )
-            )
-            result["new_state"] = {
-                "resource_id": resource_id,
-                "name": name,
-                "project_id": project_id,
-                "location_id": location_id,
-                "key_ring_id": key_ring_id,
-                "crypto_key_id": crypto_key_id,
-                **resource_body,
-            }
+    if result["old_state"]:
+        resource_id = result["old_state"].get("resource_id", None)
+        update_mask = hub.tool.gcp.cloudkms.patch.calc_update_mask(
+            resource_body, result["old_state"]
+        )
+        if (
+            primary
+            and primary.get("name")
+            and primary["name"]
+            != (result["old_state"].get("primary") or {}).get("name")
+        ):
+            update_primary_version = True
         else:
-            result["new_state"] = {**deepcopy(result["old_state"]), **resource_body}
-            update_mask = hub.tool.gcp.cloudkms.patch.calc_update_mask(
-                resource_body, result["old_state"]
-            )
-            if update_mask:
+            update_primary_version = False
+
+        if ctx["test"]:
+            if update_mask or update_primary_version:
+                result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                    {**result["old_state"], **resource_body}
+                )
                 result["comment"].append(
                     hub.tool.gcp.comment_utils.would_update_comment(
-                        "gcp.cloudkms.crypto_key", resource_id
+                        GCP_RESOURCE_TYPE_FULL, resource_id
                     )
                 )
             else:
                 result["comment"].append(
-                    hub.tool.gcp.comment_utils.already_exists_comment(
-                        "gcp.cloudkms.crypto_key", resource_id
+                    hub.tool.gcp.comment_utils.up_to_date_comment(
+                        GCP_RESOURCE_TYPE_FULL, resource_id
                     )
                 )
-        return result
+            return result
 
-    if is_create:
-        create_ret = await hub.exec.gcp_api.client.cloudkms.projects.locations.key_rings.crypto_keys.create(
-            ctx,
-            parent=hub.tool.gcp.resource_prop_utils.construct_resource_id(
-                "cloudkms.projects.locations.key_rings",
-                {
-                    "project_id": project_id,
-                    "location_id": location_id,
-                    "key_ring_id": key_ring_id,
-                },
-            ),
-            body=resource_body,
-            crypto_key_id=crypto_key_id,
-            skip_initial_version_creation=False,
+        els = hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
+            RESOURCE_TYPE_FULL, resource_id
         )
-        if not create_ret["result"]:
+        if (
+            els.get("project_id") != project_id
+            or els.get("location_id") != location_id
+            or els.get("key_ring_id") != key_ring_id
+            or els.get("crypto_key_id") != crypto_key_id
+        ):
             result["result"] = False
-            result["comment"] += create_ret["comment"]
-            return result
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.create_comment(
-                "gcp.cloudkms.crypto_key", resource_id
+            result["comment"].append(
+                hub.tool.gcp.comment_utils.non_updatable_properties_comment(
+                    GCP_RESOURCE_TYPE_FULL,
+                    resource_id,
+                    ["project_id", "location_id", "key_ring_id", "crypto_key_id"],
+                )
             )
-        )
-        result["new_state"] = {
-            "name": name,
-            "project_id": project_id,
-            "location_id": location_id,
-            "key_ring_id": key_ring_id,
-            "crypto_key_id": crypto_key_id,
-            **copy.copy(create_ret["ret"]),
-        }
-    else:
-        update_mask = hub.tool.gcp.cloudkms.patch.calc_update_mask(
-            resource_body, result["old_state"]
-        )
+            return result
+
         if update_mask:
             update_ret = await hub.exec.gcp_api.client.cloudkms.projects.locations.key_rings.crypto_keys.patch(
                 ctx, name_=resource_id, updateMask=update_mask, body=resource_body
             )
             if not update_ret["result"]:
                 result["result"] = False
                 result["comment"] += update_ret["comment"]
                 return result
 
-            result["comment"].append(
-                hub.tool.gcp.comment_utils.update_comment(
-                    "gcp.cloudkms.crypto_key", resource_id
-                )
-            )
             result["new_state"] = {
                 "name": name,
                 "project_id": project_id,
                 "location_id": location_id,
                 "key_ring_id": key_ring_id,
                 "crypto_key_id": crypto_key_id,
-                **copy.copy(update_ret["ret"]),
+                **update_ret["ret"],
             }
 
-        else:
-            result["comment"].append(
-                hub.tool.gcp.comment_utils.already_exists_comment(
-                    "gcp.cloudkms.crypto_key", resource_id
-                )
-            )
-            result["new_state"] = deepcopy(result["old_state"])
-
-    if primary and primary.get("name"):
-        if primary["name"] != (result["old_state"].get("primary") or {}).get("name"):
+        if update_primary_version:
             els = hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
                 "cloudkms.projects.locations.key_rings.crypto_keys.crypto_key_versions",
                 primary["name"],
             )
             update_version_ret = await hub.exec.gcp_api.client.cloudkms.projects.locations.key_rings.crypto_keys.updatePrimaryVersion(
                 ctx,
                 name_=resource_id,
                 body={"cryptoKeyVersionId": els["crypto_key_version_id"]},
             )
             if not update_version_ret["result"]:
                 result["result"] = False
                 result["comment"] += update_version_ret["comment"]
                 return result
 
-            result["new_state"]["primary"] = copy.copy(
-                update_version_ret["ret"]["primary"]
-            )
+            result["new_state"] = {
+                "name": name,
+                "project_id": project_id,
+                "location_id": location_id,
+                "key_ring_id": key_ring_id,
+                "crypto_key_id": crypto_key_id,
+                "primary": update_version_ret["ret"]["primary"],
+            }
+
+        if update_mask or update_primary_version:
             result["comment"].append(
                 hub.tool.gcp.comment_utils.update_comment(
-                    "gcp.cloudkms.crypto_key", resource_id
+                    GCP_RESOURCE_TYPE_FULL, resource_id
+                )
+            )
+        else:
+            result["comment"].append(
+                hub.tool.gcp.comment_utils.up_to_date_comment(
+                    GCP_RESOURCE_TYPE_FULL, resource_id
                 )
             )
+        return result
 
-    return result
+    else:
+        if ctx["test"]:
+            result["comment"].append(
+                hub.tool.gcp.comment_utils.would_create_comment(
+                    GCP_RESOURCE_TYPE_FULL, name
+                )
+            )
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                {
+                    "resource_id": resource_id,
+                    "name": name,
+                    "project_id": project_id,
+                    "location_id": location_id,
+                    "key_ring_id": key_ring_id,
+                    "crypto_key_id": crypto_key_id,
+                    **resource_body,
+                }
+            )
+            return result
+
+        create_ret = await hub.exec.gcp_api.client.cloudkms.projects.locations.key_rings.crypto_keys.create(
+            ctx,
+            parent=hub.tool.gcp.resource_prop_utils.construct_resource_id(
+                "cloudkms.projects.locations.key_rings",
+                {
+                    "project_id": project_id,
+                    "location_id": location_id,
+                    "key_ring_id": key_ring_id,
+                },
+            ),
+            body=resource_body,
+            crypto_key_id=crypto_key_id,
+            skip_initial_version_creation=False,
+        )
+        if not create_ret["result"]:
+            result["result"] = False
+            result["comment"] += create_ret["comment"]
+            return result
+        result["comment"].append(
+            hub.tool.gcp.comment_utils.create_comment(
+                GCP_RESOURCE_TYPE_FULL, resource_id
+            )
+        )
+        result["new_state"] = {
+            "name": name,
+            "project_id": project_id,
+            "location_id": location_id,
+            "key_ring_id": key_ring_id,
+            "crypto_key_id": crypto_key_id,
+            **create_ret["ret"],
+        }
+        result["old_state"] = {}
+        return result
 
 
 async def absent(hub, ctx, name: str) -> Dict[str, Any]:
     """Absent is not supported for this resource.
 
     Args:
         name(str):
@@ -452,15 +477,15 @@
             }
     """
     return {
         "name": name,
         "result": False,
         "comment": [
             hub.tool.gcp.comment_utils.no_resource_delete_comment(
-                "gcp.cloudkms.crypto_key"
+                GCP_RESOURCE_TYPE_FULL
             )
         ],
         "old_state": None,
         "new_state": None,
     }
 
 
@@ -511,21 +536,22 @@
                         result[resource_id] = {
                             "gcp.cloudkms.crypto_key.present": [
                                 {parameter_key: parameter_value}
                                 for parameter_key, parameter_value in crypto_key.items()
                             ]
                         }
                         els = hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
-                            "cloudkms.projects.locations.key_rings.crypto_keys",
+                            RESOURCE_TYPE_FULL,
                             resource_id,
                         )
                         p = result[resource_id]["gcp.cloudkms.crypto_key.present"]
                         p.append({"project_id": els["project_id"]})
                         p.append({"location_id": els["location_id"]})
                         p.append({"key_ring_id": els["key_ring_id"]})
                         p.append({"crypto_key_id": els["crypto_key_id"]})
 
     return result
 
 
 def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
+    """Default implemented for each module."""
     return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/crypto_key_version.py` & `idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/crypto_key_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,148 +1,77 @@
 """State module for managing Cloud Key Management Service crypto keys."""
-from copy import deepcopy
 from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
-from typing import List
 
 __contracts__ = ["resource"]
+RESOURCE_TYPE = "cloudkms.crypto_key_versions"
+RESOURCE_TYPE_FULL = (
+    "cloudkms.projects.locations.key_rings.crypto_keys.crypto_key_versions"
+)
+GCP_RESOURCE_TYPE_FULL = "gcp.cloudkms.crypto_key_versions"
 
 
 async def present(
     hub,
     ctx,
     name: str,
     crypto_key_version_id: str = None,
     project_id: str = None,
     location_id: str = None,
     key_ring_id: str = None,
     crypto_key_id: str = None,
     key_state: str = None,
-    protection_level: str = None,
     algorithm: str = None,
-    attestation: make_dataclass(
-        "KeyOperationAttestation",
-        [
-            ("format", str, field(default=None)),
-            ("content", str, field(default=None)),
-            (
-                "cert_chains",
-                make_dataclass(
-                    "CertificateChains",
-                    [
-                        ("cavium_certs", List[str], field(default=None)),
-                        ("google_card_certs", List[str], field(default=None)),
-                        ("google_partition_certs", List[str], field(default=None)),
-                    ],
-                ),
-                field(default=None),
-            ),
-        ],
-    ) = None,
-    create_time: str = None,
-    generate_time: str = None,
-    destroy_time: str = None,
-    destroy_event_time: str = None,
     import_job: str = None,
-    import_time: str = None,
-    import_failure_reason: str = None,
     external_protection_level_options: make_dataclass(
         "ExternalProtectionLevelOptions",
         [
             ("external_key_uri", str, field(default=None)),
             ("ekm_connection_key_path", str, field(default=None)),
         ],
     ) = None,
-    reimport_eligible: bool = None,
     resource_id: str = None,
     key_material: str = None,
 ) -> Dict[str, Any]:
     """Create or update a `CryptoKeyVersion`_ within a `CryptoKey`_.
 
     Args:
         name(str):
-            Idem name
+            Idem name.
 
         crypto_key_version_id(str, Optional):
             Output only. Set by the service.
 
         project_id(str, Optional):
             Project Id of the new crypto key version.
 
         location_id(str, Optional):
-            Location Id of the new crypto key version .
+            Location Id of the new crypto key version.
 
         key_ring_id(str, Optional):
             Keyring Id of the new crypto key version.
 
         crypto_key_id(str, Optional):
             Cryptokey Id of the new crypto key version.
 
         key_state(str, Optional):
             The current state of the `CryptoKeyVersion`_.
 
-        protection_level(str, Optional):
-            Output only. The `ProtectionLevel`_ describing how crypto operations are performed with this `CryptoKeyVersion`_.
-
         algorithm(str, Optional):
             Output only. The `CryptoKeyVersionAlgorithm`_ that this `CryptoKeyVersion`_ supports.
 
-        attestation(Dict[str, Any], Optional):
-            Output only. Statement that was generated and signed by the HSM at key creation time. Use this statement to
-            verify attributes of the key as stored on the HSM, independently of Google. Only provided for key versions
-            with `protectionLevel`_ `HSM`_.
-
-        create_time(str, Optional):
-            Output only. The time at which this `CryptoKeyVersion`_ was created.
-
-            A timestamp in RFC3339 UTC "Zulu" format, with nanosecond resolution and up to nine fractional digits.
-            Examples: "2014-10-02T15:01:23Z" and "2014-10-02T15:01:23.045123456Z".
-
-        generate_time(str, Optional):
-            Output only. The time this `CryptoKeyVersion`_'s key material was generated.
-
-            A timestamp in RFC3339 UTC "Zulu" format, with nanosecond resolution and up to nine fractional digits.
-            Examples: "2014-10-02T15:01:23Z" and "2014-10-02T15:01:23.045123456Z".
-
-        destroy_time(str, Optional):
-            Output only. The time this `CryptoKeyVersion`_'s key material is scheduled for destruction. Only present if
-            `state`_ is `DESTROY_SCHEDULED`_.
-
-            A timestamp in RFC3339 UTC "Zulu" format, with nanosecond resolution and up to nine fractional digits.
-            Examples: "2014-10-02T15:01:23Z" and "2014-10-02T15:01:23.045123456Z".
-
-        destroy_event_time(str, Optional):
-            Output only. The time this `CryptoKeyVersion`_'s key material was destroyed. Only present if `state`_ is `DESTROYED`_.
-
             A timestamp in RFC3339 UTC "Zulu" format, with nanosecond resolution and up to nine fractional digits.
             Examples: "2014-10-02T15:01:23Z" and "2014-10-02T15:01:23.045123456Z".
 
         import_job(str, Optional):
             Output only. The name of the `ImportJob`_ used in the most recent import of this `CryptoKeyVersion`_. Only
             present if the underlying key material was imported.
 
-        import_time(str, Optional):
-            Output only. The time at which this `CryptoKeyVersion`_'s key material was most recently imported.
-
-            A timestamp in RFC3339 UTC "Zulu" format, with nanosecond resolution and up to nine fractional digits.
-            Examples: "2014-10-02T15:01:23Z" and "2014-10-02T15:01:23.045123456Z".
-
-        import_failure_reason(str, Optional):
-            Output only. The root cause of the most recent import failure. Only present if state is `IMPORT_FAILED`_.
-
-        external_protection_level_options(Dict[str, Any], Optional):
-            `ExternalProtectionLevelOptions`_ stores a group of additional fields for configuring a `CryptoKeyVersion`_
-             that are specific to the `EXTERNAL`_ protection level and `EXTERNAL_VPC`_ protection levels.
-
-        reimport_eligible(bool, Optional):
-            Output only. Whether or not this key version is eligible for reimport, by being specified as a target in
-            `ImportCryptoKeyVersionRequest.crypto_key_version`_.
-
         resource_id(str, Optional): Idem resource id. Formatted as
 
             `projects/{project_id}/locations/{location_id}/keyRings/{key_ring_id}/cryptoKeys/{crypto_key_id}/cryptoKeyVersions/{crypto_key_version_id}`
 
         key_material(str, Optional): Base64 encoded key material. If this parameter is present will be attempted `import`_
             of the key material in the `CryptoKeyVersion`_ specified by the resource_id or in a new `CryptoKeyVersion`_
             if resource_id is missing. `import`_ requires also project_id, location_id, key_ring_id, crypto_key_id,
@@ -167,71 +96,80 @@
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
-        crypto_key_test:
-          gcp.cloudkms.crypto_key.present:
-            - project_id: tango-gcp
-            - location_id: us-east1
-            - key_ring_id: idem-gcp-1
-            - crypto_key_id: key-2
-
-        crypto_key_version_test:
-          gcp.cloudkms.crypto_key_version.present:
-            - key_state: ENABLED
-            - project_id: tango-gcp
-            - location_id: us-east1
-            - key_ring_id: idem-gcp-1
-            - crypto_key_id: "${gcp.cloudkms.crypto_key:crypto_key_test:crypto_key_id}"
-
-          # Update crypto key primary version with the one managed above
-          gcp.cloudkms.crypto_key.present:
-            - primary:
-                name: "${gcp.cloudkms.crypto_key_version:crypto_key_version_test:resource_id}"
-            - project_id: tango-gcp
-            - location_id: us-east1
-            - key_ring_id:  idem-gcp-1
-            - crypto_key_id: "${gcp.cloudkms.crypto_key:crypto_key_test:crypto_key_id}"
+            crypto_key_test:
+              gcp.cloudkms.crypto_key.present:
+                - project_id: tango-gcp
+                - location_id: us-east1
+                - key_ring_id: idem-gcp-1
+                - crypto_key_id: key-2
+
+            crypto_key_version_test:
+              gcp.cloudkms.crypto_key_version.present:
+                - key_state: ENABLED
+                - project_id: tango-gcp
+                - location_id: us-east1
+                - key_ring_id: idem-gcp-1
+                - crypto_key_id: "${gcp.cloudkms.crypto_key:crypto_key_test:crypto_key_id}"
+
+              # Update crypto key primary version with the one managed above
+              gcp.cloudkms.crypto_key.present:
+                - primary:
+                    name: "${gcp.cloudkms.crypto_key_version:crypto_key_version_test:resource_id}"
+                - project_id: tango-gcp
+                - location_id: us-east1
+                - key_ring_id:  idem-gcp-1
+                - crypto_key_id: "${gcp.cloudkms.crypto_key:crypto_key_test:crypto_key_id}"
     """
     result = {
         "result": True,
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
-    create_if_missing = False
-    if not resource_id:
-        if project_id and location_id and key_ring_id and crypto_key_id:
-            if crypto_key_version_id:
-                resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
-                    "cloudkms.projects.locations.key_rings.crypto_keys.crypto_key_versions",
-                    {
-                        "project_id": project_id,
-                        "location_id": location_id,
-                        "key_ring_id": key_ring_id,
-                        "crypto_key_id": crypto_key_id,
-                        "crypto_key_version_id": crypto_key_version_id,
-                    },
-                )
-            else:
-                create_if_missing = True
-        else:
-            result["result"] = False
-            result["comment"].append(
-                "When creating new resource crypto_key_version_id, project_id, location_id, key_ring_id and crypto_key_id parameters are required!"
+    get_resource_only_with_resource_id = hub.OPT.idem.get(
+        "get_resource_only_with_resource_id", False
+    )
+
+    if hub.tool.gcp.resource_prop_utils.properties_mismatch_resource_id(
+        RESOURCE_TYPE_FULL,
+        resource_id,
+        {
+            "project_id": project_id,
+            "location_id": location_id,
+            "key_ring_id": key_ring_id,
+            "crypto_key_id": crypto_key_id,
+            "crypto_key_version_id": crypto_key_version_id,
+        },
+    ):
+        result["comment"].append(
+            hub.tool.gcp.comment_utils.properties_mismatch_resource_id_comment(
+                RESOURCE_TYPE_FULL, name
             )
+        )
+    if resource_id:
+        old_get_ret = await hub.exec.gcp.cloudkms.crypto_key_version.get(
+            ctx, resource_id=resource_id
+        )
+
+        if not old_get_ret["result"] or (
+            not old_get_ret["ret"] and get_resource_only_with_resource_id
+        ):
+            result["result"] = False
+            result["comment"] += old_get_ret["comment"]
             return result
-    else:
+
         els = hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
-            "cloudkms.projects.locations.key_rings.crypto_keys.crypto_key_versions",
+            RESOURCE_TYPE_FULL,
             resource_id,
         )
         if (
             project_id
             and location_id
             and key_ring_id
             and crypto_key_id
@@ -262,107 +200,121 @@
         else:
             project_id = els.get("project_id")
             location_id = els.get("location_id")
             key_ring_id = els.get("key_ring_id")
             crypto_key_id = els.get("crypto_key_id")
             crypto_key_version_id = els.get("crypto_key_version_id")
 
-    is_create = False
-    if resource_id:
+        result["old_state"] = old_get_ret["ret"]
+    elif not get_resource_only_with_resource_id:
+        if project_id and location_id and key_ring_id and crypto_key_id:
+            if crypto_key_version_id:
+                resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
+                    RESOURCE_TYPE_FULL,
+                    {
+                        "project_id": project_id,
+                        "location_id": location_id,
+                        "key_ring_id": key_ring_id,
+                        "crypto_key_id": crypto_key_id,
+                        "crypto_key_version_id": crypto_key_version_id,
+                    },
+                )
+        else:
+            result["result"] = False
+            result["comment"].append(
+                "When creating new resource crypto_key_version_id, project_id, location_id, key_ring_id and "
+                "crypto_key_id parameters are required! "
+            )
+            return result
+
         old_get_ret = await hub.exec.gcp.cloudkms.crypto_key_version.get(
             ctx, resource_id=resource_id
         )
-        if not old_get_ret["result"] or not old_get_ret["ret"]:
-            if not create_if_missing:
-                result["result"] = False
-                result["comment"] += old_get_ret["comment"]
-                return result
-            is_create = True
-        else:
-            result["old_state"] = {
-                "name": name,
-                "project_id": project_id,
-                "location_id": location_id,
-                "key_ring_id": key_ring_id,
-                "crypto_key_id": crypto_key_id,
-                "crypto_key_version_id": crypto_key_version_id,
-                **hub.tool.gcp.cloudkms.crypto_key_version_utils.to_state(
-                    old_get_ret["ret"]
-                ),
-            }
-            if (
-                result["old_state"].get("key_state") != "PENDING_IMPORT"
-                and key_state == "PENDING_IMPORT"
-                and ctx.get("rerun_data")
-                and ctx.get("rerun_data").get("imported_key_material")
-            ):
-                key_state = result["old_state"].get("key_state")
 
-    else:
-        is_create = create_if_missing
+        if not old_get_ret["result"]:
+            result["result"] = False
+            result["comment"] += old_get_ret["comment"]
+            return result
+
+        if old_get_ret["ret"]:
+            result["old_state"] = old_get_ret["ret"]
 
     resource_body = {
         "state": key_state,
         "external_protection_level_options": external_protection_level_options,
     }
     resource_body = {k: v for (k, v) in resource_body.items() if v is not None}
 
     import_key_ret = (
         await hub.tool.gcp.cloudkms.crypto_key_version_utils.get_import_key_if_eligible(
             ctx,
             key_material is not None,
             algorithm is not None,
             import_job,
-            result["old_state"].get("key_state")
-            if not is_create and "old_state" in result
+            (result.get("old_state") or {}).get("key_state")
+            if "old_state" in result
             else None,
         )
     )
     if not import_key_ret["result"] and not (
         ctx.get("rerun_data") and ctx.get("rerun_data").get("imported_key_material")
     ):
         result["result"] = False
         result["comment"] += import_key_ret["comment"]
         return result
 
     if ctx["test"]:
+        resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
+            RESOURCE_TYPE_FULL,
+            {
+                "project_id": project_id,
+                "location_id": location_id,
+                "key_ring_id": key_ring_id,
+                "crypto_key_id": crypto_key_id,
+                "crypto_key_version_id": crypto_key_version_id,
+            },
+        )
         if import_key_ret["ret"]:
-            if is_create:
-                result["comment"] += (
-                    "Key material will be imported in new gcp.cloudkms.crypto_key_version",
+            if not result["old_state"]:
+                result["comment"].append(
+                    "Key material will be imported in new gcp.cloudkms.crypto_key_version"
                 )
             else:
-                result["comment"] += (
-                    f"Key material will be re-imported in gcp.cloudkms.crypto_key_version '{resource_id}'",
+                result["comment"].append(
+                    f"Key material will be re-imported in gcp.cloudkms.crypto_key_version '{resource_id}'"
                 )
             return result
-        if is_create:
+        if not result["old_state"]:
             result["comment"].append(
                 hub.tool.gcp.comment_utils.would_create_comment(
                     "gcp.cloudkms.crypto_key_version", resource_id
                 )
             )
-            result["new_state"] = {
-                "resource_id": resource_id,
-                "name": name,
-                "project_id": project_id,
-                "location_id": location_id,
-                "key_ring_id": key_ring_id,
-                "crypto_key_id": crypto_key_id,
-                "crypto_key_version_id": crypto_key_version_id,
-                **resource_body,
-            }
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                {
+                    "resource_id": resource_id,
+                    "name": name,
+                    "project_id": project_id,
+                    "location_id": location_id,
+                    "key_ring_id": key_ring_id,
+                    "crypto_key_id": crypto_key_id,
+                    "crypto_key_version_id": crypto_key_version_id,
+                    **resource_body,
+                }
+            )
         else:
-            result["new_state"] = {
-                **deepcopy(result["old_state"]),
-                **{
-                    "key_state" if k == "state" else k: v
-                    for k, v in resource_body.items()
-                },
-            }
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                {
+                    **result["old_state"],
+                    **{
+                        "key_state" if k == "state" else k: v
+                        for k, v in resource_body.items()
+                    },
+                }
+            )
             update_mask = hub.tool.gcp.cloudkms.patch.calc_update_mask(
                 resource_body,
                 {
                     "state" if k == "key_state" else k: v
                     for k, v in result["old_state"].items()
                 },
             )
@@ -370,15 +322,15 @@
                 result["comment"].append(
                     hub.tool.gcp.comment_utils.would_update_comment(
                         "gcp.cloudkms.crypto_key_version", resource_id
                     )
                 )
             else:
                 result["comment"].append(
-                    hub.tool.gcp.comment_utils.already_exists_comment(
+                    hub.tool.gcp.comment_utils.up_to_date_comment(
                         "gcp.cloudkms.crypto_key_version", resource_id
                     )
                 )
         return result
 
     parent = hub.tool.gcp.resource_prop_utils.construct_resource_id(
         "cloudkms.projects.locations.key_rings.crypto_keys",
@@ -413,45 +365,40 @@
             "crypto_key_version_id": crypto_key_version_id,
             **hub.tool.gcp.cloudkms.crypto_key_version_utils.to_state(
                 import_ret["ret"]
             ),
         }
         result["rerun_data"] = {"imported_key_material": True}
         result["comment"].append(
-            f"Key material {'imported' if is_create else 're-imported'} in gcp.cloudkms.crypto_key_version {result['new_state']['resource_id']}"
+            f"Key material {'imported' if not result['old_state'] else 're-imported'} in gcp.cloudkms"
+            f".crypto_key_version {result['new_state']['resource_id']} "
         )
         return result
 
-    if is_create:
-        create_ret = await hub.exec.gcp_api.client.cloudkms.projects.locations.key_rings.crypto_keys.crypto_key_versions.create(
-            ctx,
-            parent=parent,
-            body=resource_body,
-        )
-        if not create_ret["result"]:
-            result["result"] = False
-            result["comment"] += create_ret["comment"]
-            return result
-        result["new_state"] = {
+    if result["old_state"]:
+        resource_id = result["old_state"].get("resource_id", None)
+        result["old_state"] = {
             "name": name,
             "project_id": project_id,
             "location_id": location_id,
             "key_ring_id": key_ring_id,
             "crypto_key_id": crypto_key_id,
             "crypto_key_version_id": crypto_key_version_id,
             **hub.tool.gcp.cloudkms.crypto_key_version_utils.to_state(
-                create_ret["ret"]
+                old_get_ret["ret"]
             ),
         }
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.create_comment(
-                "gcp.cloudkms.crypto_key_version", result["new_state"]["resource_id"]
-            )
-        )
-    else:
+        if (
+            result["old_state"].get("key_state") != "PENDING_IMPORT"
+            and key_state == "PENDING_IMPORT"
+            and ctx.get("rerun_data")
+            and ctx.get("rerun_data").get("imported_key_material")
+        ):
+            key_state = result["old_state"].get("key_state")
+
         update_mask = hub.tool.gcp.cloudkms.patch.calc_update_mask(
             resource_body,
             {
                 "state" if k == "key_state" else k: v
                 for k, v in result["old_state"].items()
             },
         )
@@ -490,19 +437,45 @@
                 "crypto_key_version_id": crypto_key_version_id,
                 **hub.tool.gcp.cloudkms.crypto_key_version_utils.to_state(
                     update_ret["ret"]
                 ),
             }
         else:
             result["comment"].append(
-                hub.tool.gcp.comment_utils.already_exists_comment(
+                hub.tool.gcp.comment_utils.up_to_date_comment(
                     "gcp.cloudkms.crypto_key_version", resource_id
                 )
             )
-            result["new_state"] = deepcopy(result["old_state"])
+
+    else:
+        create_ret = await hub.exec.gcp_api.client.cloudkms.projects.locations.key_rings.crypto_keys.crypto_key_versions.create(
+            ctx,
+            parent=parent,
+            body=resource_body,
+        )
+        if not create_ret["result"]:
+            result["result"] = False
+            result["comment"] += create_ret["comment"]
+            return result
+        result["new_state"] = {
+            "name": name,
+            "project_id": project_id,
+            "location_id": location_id,
+            "key_ring_id": key_ring_id,
+            "crypto_key_id": crypto_key_id,
+            "crypto_key_version_id": crypto_key_version_id,
+            **hub.tool.gcp.cloudkms.crypto_key_version_utils.to_state(
+                create_ret["ret"]
+            ),
+        }
+        result["comment"].append(
+            hub.tool.gcp.comment_utils.create_comment(
+                "gcp.cloudkms.crypto_key_version", result["new_state"]["resource_id"]
+            )
+        )
 
     return result
 
 
 async def absent(
     hub,
     ctx,
@@ -564,38 +537,44 @@
         "comment": [],
         "old_state": ctx.get("old_state"),
         "new_state": None,
         "name": name,
         "result": True,
     }
 
-    if not resource_id:
-        resource_id = (ctx.old_state or {}).get("resource_id")
-        if (
-            not resource_id
-            and project_id
-            and location_id
-            and key_ring_id
-            and crypto_key_id
-            and crypto_key_version_id
-        ):
-            resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
-                "cloudkms.projects.locations.key_rings.crypto_keys.crypto_key_versions",
+    get_resource_only_with_resource_id = hub.OPT.idem.get(
+        "get_resource_only_with_resource_id", False
+    )
+
+    if not resource_id and not get_resource_only_with_resource_id:
+        resource_id = (
+            hub.tool.gcp.resource_prop_utils.construct_resource_id(
+                RESOURCE_TYPE_FULL,
                 {
                     "project_id": project_id,
                     "location_id": location_id,
                     "key_ring_id": key_ring_id,
                     "crypto_key_id": crypto_key_id,
                     "crypto_key_version_id": crypto_key_version_id,
                 },
             )
-        else:
-            result["result"] = False
-            result["comment"] += ["Can not determine resource_id."]
-            return result
+            if project_id
+            and location_id
+            and key_ring_id
+            and crypto_key_id
+            and crypto_key_version_id
+            else None
+        )
+
+    if not resource_id:
+        result["comment"].append(
+            hub.tool.gcp.comment_utils.already_absent_comment("gcp.compute.disk", name)
+        )
+        result["result"] = False
+        return result
 
     if ctx.test:
         result["comment"].append(
             hub.tool.gcp.comment_utils.would_delete_comment(
                 "gcp.cloudkms.crypto_key_version", resource_id
             )
         )
@@ -695,15 +674,15 @@
                                         {parameter_key: parameter_value}
                                         if parameter_key != "state"
                                         else {"key_state": parameter_value}
                                         for parameter_key, parameter_value in crypto_key_version.items()
                                     ]
                                 }
                                 els = hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
-                                    "cloudkms.projects.locations.key_rings.crypto_keys.crypto_key_versions",
+                                    RESOURCE_TYPE_FULL,
                                     resource_id,
                                 )
                                 p = result[resource_id][
                                     "gcp.cloudkms.crypto_key_version.present"
                                 ]
                                 p.append({"project_id": els["project_id"]})
                                 p.append({"location_id": els["location_id"]})
@@ -717,8 +696,9 @@
                                     }
                                 )
 
     return result
 
 
 def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
+    """Default implemented for each module."""
     return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/import_job.py` & `idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/import_job.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """State module for managing Cloud Key Management Service import job."""
-import copy
-from copy import deepcopy
 from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 
 __contracts__ = ["resource"]
+RESOURCE_TYPE = "cloudkms.import_jobs"
+RESOURCE_TYPE_FULL = "cloudkms.projects.locations.key_rings.import_jobs"
+GCP_RESOURCE_TYPE_FULL = "gcp.cloudkms.import_jobs"
 
 
 async def present(
     hub,
     ctx,
     name: str,
     import_method: str,
@@ -22,15 +23,15 @@
     key_ring_id: str = None,
     create_time: str = None,
     generate_time: str = None,
     expire_time: str = None,
     expire_event_time: str = None,
     job_state: str = None,
     public_key: str = None,
-    attestation=make_dataclass(
+    attestation: make_dataclass(
         "KeyOperationAttestation",
         [
             ("format", str, field(default=None)),
             ("content", str, field(default=None)),
             (
                 "cert_chains",
                 make_dataclass(
@@ -48,25 +49,25 @@
                             field(default=None),
                         ),
                     ],
                 ),
                 field(default=None),
             ),
         ],
-    ),
+    ) = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     """Create a new `ImportJob`_ within a `KeyRing`_.
 
     Args:
         name(str):
             Idem name.
 
         import_job_id(str, Optional):
-            Import job id. It must be unique within a KeyRing and match the regular expression [a-zA-Z0-9_-]{1,63}
+            Import job id. It must be unique within a KeyRing and match the regular expression ``[a-zA-Z0-9_-]{1,63}``
 
         project_id(str, Optional):
             Project Id of the new crypto key.
 
         location_id(str, Optional):
             Location Id of the new crypto key.
 
@@ -155,34 +156,72 @@
         "result": True,
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
-    if not resource_id:
-        if project_id and location_id and key_ring_id and import_job_id:
-            resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
-                "cloudkms.projects.locations.key_rings.import_jobs",
-                {
-                    "project_id": project_id,
-                    "location_id": location_id,
-                    "key_ring_id": key_ring_id,
-                    "import_job_id": import_job_id,
-                },
+    if hub.tool.gcp.resource_prop_utils.properties_mismatch_resource_id(
+        RESOURCE_TYPE_FULL,
+        resource_id,
+        {
+            "project_id": project_id,
+            "location_id": location_id,
+            "key_ring_id": key_ring_id,
+            "import_job_id": import_job_id,
+        },
+    ):
+        result["comment"].append(
+            hub.tool.gcp.comment_utils.properties_mismatch_resource_id_comment(
+                RESOURCE_TYPE_FULL, name
             )
-        else:
+        )
+
+    get_resource_only_with_resource_id = hub.OPT.idem.get(
+        "get_resource_only_with_resource_id", False
+    )
+    if resource_id:
+        old_get_ret = await hub.exec.gcp.cloudkms.import_job.get(
+            ctx, resource_id=resource_id
+        )
+
+        if not old_get_ret["result"] or (
+            not old_get_ret["ret"] and get_resource_only_with_resource_id
+        ):
             result["result"] = False
-            result["comment"].append(
-                "When creating new resource crypto_key_id, project_id, location_id and key_ring_id parameters are required!"
-            )
+            result["comment"] += old_get_ret["comment"]
+            return result
+
+        result["old_state"] = old_get_ret["ret"]
+    elif not get_resource_only_with_resource_id:
+        resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
+            RESOURCE_TYPE_FULL,
+            {
+                "project_id": project_id,
+                "location_id": location_id,
+                "key_ring_id": key_ring_id,
+                "import_job_id": import_job_id,
+            },
+        )
+        old_get_ret = await hub.exec.gcp.cloudkms.import_job.get(
+            ctx, resource_id=resource_id
+        )
+
+        if not old_get_ret["result"]:
+            result["result"] = False
+            result["comment"] += old_get_ret["comment"]
             return result
-    else:
+
+        if old_get_ret["ret"]:
+            result["old_state"] = old_get_ret["ret"]
+
+    if result["old_state"]:
+        resource_id = result["old_state"].get("resource_id", None)
         els = hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
-            "cloudkms.projects.locations.key_rings.import_jobs", resource_id
+            RESOURCE_TYPE_FULL, resource_id
         )
         if project_id and location_id and key_ring_id and import_job_id:
             if (
                 els.get("project_id") != project_id
                 or els.get("location_id") != location_id
                 or els.get("key_ring_id") != key_ring_id
                 or els.get("import_job_id") != import_job_id
@@ -192,38 +231,15 @@
                     hub.tool.gcp.comment_utils.non_updatable_properties_comment(
                         "gcp.cloudkms.import_job",
                         resource_id,
                         ["project_id", "location_id", "key_ring_id", "import_job_id"],
                     )
                 )
                 return result
-        else:
-            project_id = els.get("project_id")
-            location_id = els.get("location_id")
-            key_ring_id = els.get("key_ring_id")
-            import_job_id = els.get("import_job_id")
-
-    old_get_ret = await hub.exec.gcp.cloudkms.import_job.get(
-        ctx, resource_id=resource_id
-    )
-
-    if not old_get_ret["result"]:
-        result["result"] = False
-        result["comment"] += old_get_ret["comment"]
-        return result
 
-    if old_get_ret["ret"]:
-        result["old_state"] = {
-            "name": name,
-            "project_id": project_id,
-            "location_id": location_id,
-            "key_ring_id": key_ring_id,
-            "import_job_id": import_job_id,
-            **copy.copy(old_get_ret["ret"]),
-        }
         if (
             result["old_state"].get("import_method") != import_method
             or result["old_state"].get("protection_level") != protection_level
         ):
             result["result"] = False
             result["comment"].append(
                 hub.tool.gcp.comment_utils.no_resource_update_comment(
@@ -232,38 +248,40 @@
             )
         else:
             result["comment"].append(
                 hub.tool.gcp.comment_utils.already_exists_comment(
                     "gcp.cloudkms.import_job", resource_id
                 )
             )
-            result["new_state"] = deepcopy(result["old_state"])
+            result["new_state"] = result["old_state"]
 
         return result
 
     resource_body = {
         "importMethod": import_method,
         "protectionLevel": protection_level,
     }
 
     if ctx["test"]:
         result["comment"].append(
             hub.tool.gcp.comment_utils.would_create_comment(
                 "gcp.cloudkms.import_job", resource_id
             )
         )
-        result["new_state"] = {
-            "resource_id": resource_id,
-            "name": name,
-            "project_id": project_id,
-            "location_id": location_id,
-            "key_ring_id": key_ring_id,
-            "import_job_id": import_job_id,
-            **resource_body,
-        }
+        result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+            {
+                "resource_id": resource_id,
+                "name": name,
+                "project_id": project_id,
+                "location_id": location_id,
+                "key_ring_id": key_ring_id,
+                "import_job_id": import_job_id,
+                **resource_body,
+            }
+        )
         return result
 
     create_ret = await hub.exec.gcp_api.client.cloudkms.projects.locations.key_rings.import_jobs.create(
         ctx,
         parent=hub.tool.gcp.resource_prop_utils.construct_resource_id(
             "cloudkms.projects.locations.key_rings",
             {
@@ -287,15 +305,15 @@
     )
     result["new_state"] = {
         "name": name,
         "project_id": project_id,
         "location_id": location_id,
         "key_ring_id": key_ring_id,
         "import_job_id": import_job_id,
-        **copy.copy(create_ret["ret"]),
+        **create_ret["ret"],
     }
     return result
 
 
 async def absent(hub, ctx, name: str) -> Dict[str, Any]:
     """Absent is not supported for this resource.
 
@@ -375,21 +393,22 @@
                                 {parameter_key: parameter_value}
                                 if parameter_key != "state"
                                 else {"job_state": parameter_value}
                                 for parameter_key, parameter_value in import_job.items()
                             ]
                         }
                         els = hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
-                            "cloudkms.projects.locations.key_rings.import_jobs",
+                            RESOURCE_TYPE_FULL,
                             resource_id,
                         )
                         p = result[resource_id]["gcp.cloudkms.import_job.present"]
                         p.append({"project_id": els["project_id"]})
                         p.append({"location_id": els["location_id"]})
                         p.append({"key_ring_id": els["key_ring_id"]})
                         p.append({"import_job_id": els["import_job_id"]})
 
     return result
 
 
 def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
+    """Default implemented for each module."""
     return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/key_ring.py` & `idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/key_ring.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """State module for managing Cloud Key Management Service key rings."""
 from typing import Any
 from typing import Dict
 
 __contracts__ = ["resource"]
+RESOURCE_TYPE = "cloudkms.key_ring"
+RESOURCE_TYPE_FULL = "cloudkms.projects.locations.key_rings"
+GCP_RESOURCE_TYPE_FULL = "gcp.cloudkms.key_ring"
 
 
 async def present(
     hub,
     ctx,
     name: str,
     key_ring_id: str = None,
@@ -35,93 +38,120 @@
             `projects/{project_id}/locations/{location_id}/keyRings/{key_ring_id}`
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
+
             key_ring_present:
               gcp.cloudkms.key_ring.present:
                 - key_ring_id: idem-gcp
-                  project_id: tango-gcp
-                  location_id: us-east1
+                - project_id: tango-gcp
+                - location_id: us-east1
 
     """
     result = {
         "result": True,
         "name": name,
         "old_state": None,
         "new_state": None,
         "comment": [],
     }
 
-    create_if_missing = False
-    if not resource_id:
-        if project_id and location_id and key_ring_id:
-            resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
-                "cloudkms.projects.locations.key_rings",
-                {
-                    "project_id": project_id,
-                    "location_id": location_id,
-                    "key_ring_id": key_ring_id,
-                },
+    if hub.tool.gcp.resource_prop_utils.properties_mismatch_resource_id(
+        RESOURCE_TYPE_FULL,
+        resource_id,
+        {
+            "project_id": project_id,
+            "location_id": location_id,
+            "key_ring_id": key_ring_id,
+        },
+    ):
+        result["comment"].append(
+            hub.tool.gcp.comment_utils.properties_mismatch_resource_id_comment(
+                RESOURCE_TYPE_FULL, name
             )
-            create_if_missing = True
-        else:
+        )
+
+    get_resource_only_with_resource_id = hub.OPT.idem.get(
+        "get_resource_only_with_resource_id", False
+    )
+    if resource_id:
+        old_get_ret = await hub.exec.gcp.cloudkms.key_ring.get(
+            ctx, resource_id=resource_id
+        )
+
+        if not old_get_ret["result"] or (
+            not old_get_ret["ret"] and get_resource_only_with_resource_id
+        ):
             result["result"] = False
-            result["comment"].append(
-                "When creating new resource key_ring_id, project_id and location_id parameters are required!"
-            )
+            result["comment"] += old_get_ret["comment"]
             return result
 
-    if resource_id:
+        result["old_state"] = old_get_ret["ret"]
+    elif not get_resource_only_with_resource_id:
+        resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
+            RESOURCE_TYPE_FULL,
+            {
+                "project_id": project_id,
+                "location_id": location_id,
+                "key_ring_id": key_ring_id,
+            },
+        )
         old_get_ret = await hub.exec.gcp.cloudkms.key_ring.get(
             ctx, resource_id=resource_id
         )
-        if not old_get_ret["result"] or not old_get_ret["ret"]:
-            if not create_if_missing:
-                result["result"] = False
-                result["comment"] += old_get_ret["comment"]
-                return result
-        else:
-            els = hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
-                "cloudkms.projects.locations.key_rings", resource_id
-            )
-            if (
-                els.get("project_id") != project_id
-                or els.get("location_id") != location_id
-                or els.get("key_ring_id") != key_ring_id
-            ):
-                result["result"] = False
-                result["comment"].append(
-                    hub.tool.gcp.comment_utils.non_updatable_properties_comment(
-                        "gcp.cloudkms.key_ring",
-                        key_ring_id,
-                        ["project_id", "location_id", "key_ring_id"],
-                    )
-                )
-                return result
+
+        if not old_get_ret["result"]:
+            result["result"] = False
+            result["comment"] += old_get_ret["comment"]
+            return result
+
+        if old_get_ret["ret"]:
+            result["old_state"] = old_get_ret["ret"]
+
+    if result["old_state"]:
+        resource_id = result["old_state"].get("resource_id", None)
+
+        els = hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
+            RESOURCE_TYPE_FULL, resource_id
+        )
+        if (
+            els.get("project_id") != project_id
+            or els.get("location_id") != location_id
+            or els.get("key_ring_id") != key_ring_id
+        ):
+            result["result"] = False
             result["comment"].append(
-                hub.tool.gcp.comment_utils.already_exists_comment(
-                    "gcp.cloudkms.key_ring", key_ring_id
+                hub.tool.gcp.comment_utils.non_updatable_properties_comment(
+                    "gcp.cloudkms.key_ring",
+                    key_ring_id,
+                    ["project_id", "location_id", "key_ring_id"],
                 )
             )
-            result["old_state"] = old_get_ret["ret"]
-            result["new_state"] = old_get_ret["ret"]
-            result["new_state"]["name"] = name
             return result
+        result["comment"].append(
+            hub.tool.gcp.comment_utils.already_exists_comment(
+                "gcp.cloudkms.key_ring", key_ring_id
+            )
+        )
+        result["old_state"] = old_get_ret["ret"]
+        result["new_state"] = old_get_ret["ret"]
+        result["new_state"]["name"] = name
+        return result
 
     if ctx["test"]:
         plan_state = {"resource_id": resource_id, "name": name}
         result["comment"].append(
             hub.tool.gcp.comment_utils.would_create_comment(
                 "gcp.cloudkms.key_ring", key_ring_id
             )
         )
-        result["new_state"] = plan_state
+        result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(plan_state)
         return result
 
     create_ret = (
         await hub.exec.gcp_api.client.cloudkms.projects.locations.key_rings.create(
             ctx,
             parent=hub.tool.gcp.resource_prop_utils.construct_resource_id(
                 "cloudkms.projects.locations",
@@ -220,8 +250,9 @@
                     ]
                 }
 
     return result
 
 
 def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
+    """Default implemented for each module."""
     return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/location.py` & `idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/location.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,8 +104,9 @@
             ]
         }
 
     return result
 
 
 def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
+    """Default implemented for each module."""
     return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/disk.py` & `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/disk.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 """State module for managing Disks."""
-import copy
 from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 
-from idem_gcp.tool.gcp.utils import get_project_from_account
+from dict_tools.typing import Computed
+
+from idem_gcp.tool.gcp.state_operation_utils import StateOperations
+from idem_gcp.tool.gcp.utils import zonal_absent
+
+# prevent commit hook from removing the import
+absent = zonal_absent
 
 __contracts__ = ["resource"]
 
 
 async def present(
     hub,
     ctx,
     name: str = None,
     project: str = None,
     zone: str = None,
+    region: str = None,
     resource_id: str = None,
     request_id: str = None,
     source_image: str = None,
     size_gb: str = None,
     source_snapshot: str = None,
     source_storage_object: str = None,
     options: str = None,
-    type: str = None,
+    type_: (str, "alias=type") = None,
     licenses: List[str] = None,
     guest_os_features: List[
-        make_dataclass("GuestOsFeature", [("type", str, field(default=None))])
+        make_dataclass(
+            "GuestOsFeature", [("type_", (str, "alias=type"), field(default=None))]
+        )
     ] = None,
     disk_encryption_key: make_dataclass(
         "CustomerEncryptionKey",
         [
             ("raw_key", str, field(default=None)),
             ("rsa_encrypted_key", str, field(default=None)),
             ("kms_key_name", str, field(default=None)),
@@ -69,27 +77,31 @@
     params: make_dataclass(
         "DiskParams",
         [
             ("resource_manager_tags", Dict[str, str], field(default=None)),
         ],
     ) = None,
     description: str = None,
+    id_: (Computed[str], "alias=id") = None,
 ) -> Dict[str, Any]:
     r"""Creates or updates a persistent disk in the specified project using the data in the request.
 
     You can create a disk from a source (sourceImage, sourceSnapshot, or sourceDisk) or create an empty 500 GB data disk by omitting all properties.
     You can also create a disk that is larger than the default size by specifying the sizeGb property.
 
     Args:
         name(str):
             An Idem name of the resource.
 
-        zone(str):
+        zone(str, Optional):
             The name of the zone for this request.
 
+        region(str, Optional):
+            The name of the region for this request.
+
         project(str, Optional):
             Project ID for this request.
 
         resource_id(str, Optional):
             An identifier of the resource in the provider.
             Defaults to None.
 
@@ -125,17 +137,19 @@
             If you specify this field along with a source, the value of sizeGb must not
             be less than the size of the source. Acceptable values are 1 to 65536, inclusive.
             Defaults to None.
 
         source_snapshot(str, Optional):
             The source snapshot used to create this disk. You can provide this as a partial or full URL to the resource.
             For example, the following are valid values:
-                - https://www.googleapis.com/compute/v1/projects/project /global/snapshots/snapshot
-                - projects/project/global/snapshots/snapshot
-                - global/snapshots/snapshot
+
+            - https://www.googleapis.com/compute/v1/projects/project/global/snapshots/snapshot
+            - projects/project/global/snapshots/snapshot
+            - global/snapshots/snapshot
+
             Defaults to None.
 
         source_storage_object(str, Optional):
             The full Google Cloud Storage URI where the disk image is stored.
             This file must be a gzip-compressed tarball whose name ends in .tar.gz or virtual machine disk
             whose name ends in vmdk. Valid URIs may start with gs:// or https://storage.googleapis.com/.
             This flag is not optimized for creating multiple disks from a source storage object.
@@ -157,92 +171,104 @@
             Defaults to None.
 
         guest_os_features(List[Dict[str, Any]], Optional):
             A list of features to enable on the guest operating system. Applicable only for bootable images.
             Read Enabling guest operating system features to see a list of available options.
             Defaults to None.
 
-                * type (str, Optional):
-                    The ID of a supported feature. To add multiple values,
-                    use commas to separate values. Set to one or more of the following values:
-                        - VIRTIO_SCSI_MULTIQUEUE
-                        - WINDOWS
-                        - MULTI_IP_SUBNET
-                        - UEFI_COMPATIBLE
-                        - GVNIC
-                        - SEV_CAPABLE
-                        - SUSPEND_RESUME_COMPATIBLE
-                        - SEV_SNP_CAPABLE
-                    For more information, see Enabling guest operating system features.
+            * type (str, Optional):
+                The ID of a supported feature. To add multiple values,
+                use commas to separate values. Set to one or more of the following values:
+
+                - VIRTIO_SCSI_MULTIQUEUE
+                - WINDOWS
+                - MULTI_IP_SUBNET
+                - UEFI_COMPATIBLE
+                - GVNIC
+                - SEV_CAPABLE
+                - SUSPEND_RESUME_COMPATIBLE
+                - SEV_SNP_CAPABLE
+
+                For more information, see Enabling guest operating system features.
 
         disk_encryption_key(Dict[str, Any], Optional):
             Encrypts the disk using a customer-supplied encryption key or a customer-managed encryption key.
             Encryption keys do not protect access to metadata of the disk. After you encrypt a disk with a
             customer-supplied key, you must provide the same key if you use the disk later. For example,
             to create a disk snapshot, to create a disk image, to create a machine image, or to attach the disk to a
             virtual machine. After you encrypt a disk with a customer-managed key, the diskEncryptionKey.kmsKeyName
             is set to a key *version* name once the disk is created. The disk is encrypted with this version of the key.
             In the response, diskEncryptionKey.kmsKeyName appears in the following format:
+
             "diskEncryptionKey.kmsKeyName":
             "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key /cryptoKeysVersions/version"
+
             If you do not provide an encryption key when creating the disk, then the disk is encrypted using an
             automatically generated key and you don't need to provide a key to use the disk later.
             Defaults to None.
 
-                * raw_key(str, Optional):
-                    Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt
-                    or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey.
-                    For example: \"raw_key\": \"SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0=\"
-
-                * rsa_encrypted_key(str, Optional):
-                    Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to
-                    either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey.
-                    For example:
-                        \"rsa_encrypted_key\":
-                        \"ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/
-                        NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEM
-                        MoNUXMCZEIpg9Vtp9x2oe==\"
-                    The key must meet the following requirements before you can provide it to Compute Engine:
-                        1. The key is wrapped using a RSA public key certificate provided by Google.
-                        2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding.
-                    Gets the RSA public key certificate provided by Google at:
-                    https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
-
-                * kms_key_name(str, Optional):
-                    The name of the encryption key that is stored in Google Cloud KMS.
-                    For example:
-                        \"kms_key_name\":
-                        \"projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
-
-                * kms_key_service_account(str, Optional):
-                    The service account being used for the encryption request for the given KMS key. If absent,
-                    the Compute Engine default service account is used. For example:
-                        \"kms_key_service_account\":
-                        \"name@project_id.iam.gserviceaccount.com/
+            * raw_key(str, Optional):
+                Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt
+                or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey.
+                For example:
+
+                \"raw_key\": \"SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0=\"
+
+            * rsa_encrypted_key(str, Optional):
+                Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to
+                either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey.
+                For example:
+
+                \"rsa_encrypted_key\":
+                \"ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/
+                NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEM
+                MoNUXMCZEIpg9Vtp9x2oe==\"
+
+                The key must meet the following requirements before you can provide it to Compute Engine:
+
+                1. The key is wrapped using a RSA public key certificate provided by Google.
+                2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding.
+
+                Gets the RSA public key certificate provided by Google at:
+                https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+
+            * kms_key_name(str, Optional):
+                The name of the encryption key that is stored in Google Cloud KMS.
+                For example:
+
+                \"kms_key_name\":
+                \"projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+
+            * kms_key_service_account(str, Optional):
+                The service account being used for the encryption request for the given KMS key. If absent,
+                the Compute Engine default service account is used. For example:
+
+                \"kms_key_service_account\":
+                \"name@project_id.iam.gserviceaccount.com/
 
 
         source_image_encryption_key(Dict[str, Any], Optional):
             The customer-supplied encryption key of the source image.
             Required if the source image is protected by a customer-supplied encryption key.
             Defaults to None.
 
-                * raw_key(str, Optional)
-                * rsa_encrypted_key(str, Optional)
-                * kms_key_name(str, Optional)
-                * kms_key_service_account(str, Optional)
+            * raw_key(str, Optional)
+            * rsa_encrypted_key(str, Optional)
+            * kms_key_name(str, Optional)
+            * kms_key_service_account(str, Optional)
 
         source_snapshot_encryption_key(Dict[str, Any], Optional):
             The customer-supplied encryption key of the source snapshot.
             Required if the source snapshot is protected by a customer-supplied encryption key.
             Defaults to None.
 
-                * raw_key(str, Optional)
-                * rsa_encrypted_key(str, Optional)
-                * kms_key_name(str, Optional)
-                * kms_key_service_account(str, Optional)
+            * raw_key(str, Optional)
+            * rsa_encrypted_key(str, Optional)
+            * kms_key_name(str, Optional)
+            * kms_key_service_account(str, Optional)
 
         labels(Dict[str, Dict[str, str]], Optional):
             Labels to apply to this disk. These can be later modified by the setLabels method.
             Defaults to None.
 
         label_fingerprint(str, Optional):
             A fingerprint for the labels being applied to this disk,
@@ -267,26 +293,29 @@
             The currently supported size is 4096, other sizes may be added in the future.
             If an unsupported value is requested,
             the error message will list the supported values for the caller's project.
             Defaults to None.
 
         resource_policies(List[str], Optional):
             Resource policies applied to this disk for automatic snapshot creations.
+            To remove a policy set resource_policies to be an empty array e.g. []
             Defaults to None.
 
         source_disk(str, Optional):
             The source disk used to create this disk. You can provide this as a partial or full URL to the resource.
             For example, the following are valid values:
-                - https://www.googleapis.com/compute/v1/projects/project/zones/zone /disks/disk
-                - https://www.googleapis.com/compute/v1/projects/project/regions/region /disks/disk
-                - projects/project/zones/zone/disks/disk
-                - projects/project/regions/region/disks/disk
-                - zones/zone/disks/disk
-                - regions/region/disks/disk
-                Defaults to None.
+
+            - https://www.googleapis.com/compute/v1/projects/project/zones/zone/disks/disk
+            - https://www.googleapis.com/compute/v1/projects/project/regions/region/disks/disk
+            - projects/project/zones/zone/disks/disk
+            - projects/project/regions/region/disks/disk
+            - zones/zone/disks/disk
+            - regions/region/disks/disk
+
+            Defaults to None.
 
         provisioned_iops(str, Optional):
             Indicates how many IOPS to provision for the disk.
             This sets the number of I/O operations per second that the disk can handle.
             Values must be between 10,000 and 120,000. For more details, see the Extreme persistent disk documentation.
             Defaults to None.
 
@@ -300,23 +329,25 @@
             Defaults to None.
 
         params(Dict[str, Dict[str, str]], Optional):
             Input only. [Input Only] Additional params passed with the request,
             but not persisted as part of resource payload.
             Defaults to None.
 
-                * resourceManagerTags(Dict[str, str], Optional):
-                    Resource manager tags to be bound to the disk. Tag keys and values have the same definition as
-                    resource manager tags. Keys must be in the format `tagKeys/{tag_key_id}`, and values are in the format
-                    `tagValues/456`. The field is ignored (both PUT & PATCH) when empty.
+            * resourceManagerTags(Dict[str, str], Optional):
+                Resource manager tags to be bound to the disk. Tag keys and values have the same definition as
+                resource manager tags. Keys must be in the format `tagKeys/{tag_key_id}`, and values are in the format
+                `tagValues/456`. The field is ignored (both PUT & PATCH) when empty.
 
         description(str, Optional):
             An optional description of this resource.
             Defaults to None.
 
+        id(str, Optional): The unique identifier for the resource. This identifier is defined by the server. Read-only property
+
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
             example_resource_name:
@@ -333,474 +364,238 @@
         "result": True,
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
-    project = get_project_from_account(ctx, project)
-
-    # Get the resource_id from ESM
-    if not resource_id:
-        resource_id = (ctx.old_state or {}).get(
-            "resource_id"
-        ) or hub.tool.gcp.resource_prop_utils.construct_resource_id(
-            "compute.disk", {**locals(), "disk": name}
-        )
-
-    if ctx.get("rerun_data"):
-        handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, ctx.get("rerun_data"), "compute.disk"
-        )
-
-        if not handle_operation_ret["result"]:
-            result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
-            return result
-
-        resource_id = handle_operation_ret["resource_id"]
-
-    if resource_id:
-        old_get_ret = await hub.exec.gcp.compute.disk.get(
-            ctx, name=name, resource_id=resource_id
-        )
-
-        if not old_get_ret["result"]:
-            # error other than non-existing resource
-            result["result"] = False
-            result["comment"] += old_get_ret["comment"]
-            return result
-        if old_get_ret["ret"]:
-            # copy.copy(old_get_ret['ret']) is needed to convert any objects of type NamespaceDict to dict
-            # in old_get_ret['ret']. This is done so that comparisons with the plan_state which has
-            # objects of type dict works properly
-            result["old_state"] = copy.deepcopy(copy.copy(old_get_ret["ret"]))
-            zone = hub.tool.gcp.resource_prop_utils.parse_link_to_zone(
-                result["old_state"]["zone"]
-            )
-            result["old_state"]["zone"] = zone
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
-            # If rerun_data is set at this point this means that there has been a completed create or update operation
-            # so there is no need to run the code for create or update below again, and we stop here
-            if ctx.get("rerun_data"):
-                result["new_state"] = result["old_state"]
-                return result
+    if ctx.get("wrapper_result"):
+        result = ctx.get("wrapper_result")
 
     # to be autogenerated by pop-create based on insert/update props in properties.yaml
     resource_body = {
-        "type": type,
+        "type_": type_,
         "name": name,
         "source_image": source_image,
         "label_fingerprint": label_fingerprint,
         "architecture": architecture,
         "guest_os_features": guest_os_features,
         "source_disk": source_disk,
         "resource_policies": resource_policies,
         "options": options,
         "source_storage_object": source_storage_object,
         "licenses": licenses,
         "size_gb": size_gb,
         "license_codes": license_codes,
         "source_snapshot_encryption_key": source_snapshot_encryption_key,
         "zone": zone,
+        "region": region,
         "source_image_encryption_key": source_image_encryption_key,
         "physical_block_size_bytes": physical_block_size_bytes,
         "source_snapshot": source_snapshot,
         "description": description,
         "labels": labels,
         "params": params,
         "replica_zones": replica_zones,
         "location_hint": location_hint,
         "disk_encryption_key": disk_encryption_key,
         "provisioned_iops": provisioned_iops,
+        "id_": id_,
     }
 
-    # TODO: How to handle query params which are not returned in the response body of get
-    plan_state = {"resource_id": resource_id, **resource_body}
-
-    plan_state = {k: v for (k, v) in plan_state.items() if v is not None}
+    resource_body = {k: v for (k, v) in resource_body.items() if v is not None}
     operation = None
     if result["old_state"]:
-        # Resize
-        size_gb_updated = False
-        if size_gb is not None and str(result["old_state"]["size_gb"]) != str(size_gb):
-            if not ctx.get("test"):
-                resize_body = {"size_gb": size_gb}
-                update_ret = await hub.exec.gcp_api.client.compute.disk.resize(
+        # Update
+        resource_id = result["old_state"].get("resource_id", None)
+        zone = hub.tool.gcp.resource_prop_utils.parse_link_to_zone(
+            result["old_state"]["zone"]
+        )
+        result["old_state"]["zone"] = zone
+
+        # A dictionary of additional operations to perform on the object identified by the key
+        # the values are tuples with the first element - the method to call, the second element - arguments,
+        # third - the property is required in the end result
+        patch_operations_dict = {
+            "size_gb": (
+                hub.tool.gcp.compute.disk.update_size_gb,
+                (
                     ctx,
-                    resource_id=resource_id,
-                    body=resize_body,
-                    request_id=request_id,
-                )
-
-                if not update_ret["result"]:
-                    result["result"] = False
-                    result["comment"] += update_ret["comment"]
-                    return result
-
-                if "compute#operation" in update_ret["ret"].get("kind"):
-                    operation = update_ret["ret"]
-                    operation_id = (
-                        hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                            operation.get("selfLink"), "compute.zone_operation"
-                        )
-                    )
-                    op_ret = await hub.tool.gcp.operation_utils.handle_operation(
-                        ctx, operation_id, "compute.disk", True
-                    )
-                    if not op_ret["result"]:
-                        result["comment"] += op_ret["comment"]
-                        result["rerun_data"] = op_ret["rerun_data"]
-                        return result
-
-            size_gb_updated = True
-
-        # Update labels
-        labels_updated = False
-        if (
-            labels is not None
-            and not (labels == {} and result["old_state"].get("labels") is None)
-            and result["old_state"].get("labels") != labels
-        ):
-            if not ctx.get("test"):
-                set_labels_body = {
-                    "labels": labels,
-                    "label_fingerprint": label_fingerprint,
-                }
-                update_ret = await hub.exec.gcp_api.client.compute.disk.setLabels(
+                    str(result["old_state"].get("size_gb")),
+                    str(size_gb),
+                    resource_id,
+                    request_id,
+                ),
+            ),
+            "labels": (
+                hub.tool.gcp.compute.disk.update_labels,
+                (
                     ctx,
-                    project=project,
-                    zone=zone,
-                    resource=name,
-                    body=set_labels_body,
-                    request_id=request_id,
-                )
+                    result["old_state"].get("labels"),
+                    labels,
+                    label_fingerprint or result["old_state"].get("label_fingerprint"),
+                    request_id,
+                    project,
+                    name,
+                    zone,
+                    region,
+                ),
+            ),
+            "resource_policies": (
+                hub.tool.gcp.compute.disk.update_resource_policies,
+                (
+                    ctx,
+                    result["old_state"].get("resource_policies"),
+                    resource_policies,
+                    resource_id,
+                    request_id,
+                ),
+            ),
+        }
 
-                if not update_ret["result"]:
-                    result["result"] = False
-                    result["comment"] += update_ret["comment"]
-                    return result
-
-                if "compute#operation" in update_ret["ret"].get("kind"):
-                    operation = update_ret["ret"]
-                    operation_id = (
-                        hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                            operation.get("selfLink"), "compute.zone_operation"
-                        )
-                    )
-                    op_ret = await hub.tool.gcp.operation_utils.handle_operation(
-                        ctx, operation_id, "compute.disk", True
-                    )
-                    if not op_ret["result"]:
-                        result["comment"] += op_ret["comment"]
-                        result["rerun_data"] = op_ret["rerun_data"]
-                        return result
-
-            labels_updated = True
-
-        # Update resource policies
-        resource_policies_updated = False
-        if not hub.tool.gcp.state_comparison_utils.are_lists_identical(
-            result["old_state"].get("resource_policies"), resource_policies
-        ):
-            # If (some) resource policies are links, parse them to resource policy resource ids
-            new_resource_policies = [
-                hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                    policy, "compute.resource_policy"
-                )
-                for policy in (
-                    resource_policies if resource_policies is not None else []
+        state_operations = StateOperations(
+            hub, "compute.disk", patch_operations_dict, result, resource_body
+        )
+
+        changes = hub.tool.gcp.utils.compare_states(
+            result["old_state"],
+            {
+                "resource_id": resource_id,
+                **resource_body,
+            },
+            "compute.disk",
+            additional_exclude_paths=list(patch_operations_dict.keys()),
+        )
+
+        if changes:
+            changed_non_updatable_properties = (
+                hub.tool.gcp.resource_prop_utils.get_changed_non_updatable_properties(
+                    "compute.disk", changes
                 )
-            ]
-            current_resource_policies = [
-                hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                    policy, "compute.resource_policy"
+            )
+            if changed_non_updatable_properties:
+                result["result"] = False
+                result["comment"].append(
+                    hub.tool.gcp.comment_utils.non_updatable_properties_comment(
+                        "gcp.compute.disk",
+                        name,
+                        changed_non_updatable_properties,
+                    )
                 )
-                for policy in result["old_state"].get("resource_policies", [])
-            ]
-
-            resource_policies_to_remove = [
-                policy
-                for policy in current_resource_policies
-                if policy not in new_resource_policies
-            ]
-            resource_policies_to_add = [
-                policy
-                for policy in new_resource_policies
-                if policy not in current_resource_policies
-            ]
+                result["new_state"] = result["old_state"]
+                return result
 
-            if (
-                len(resource_policies_to_remove) > 0
-                or len(resource_policies_to_add) > 0
-            ):
-                if not ctx.get("test"):
-                    add_request_body = None
-                    if len(resource_policies_to_add) > 0:
-                        add_request_body = {
-                            "resource_policies": resource_policies_to_add
-                        }
-                    remove_request_body = None
-                    if len(resource_policies_to_remove) > 0:
-                        remove_request_body = {
-                            "resource_policies": resource_policies_to_remove
-                        }
-
-                    remove_ret = None
-                    if remove_request_body is not None:
-                        remove_ret = await hub.exec.gcp_api.client.compute.disk.removeResourcePolicies(
-                            ctx,
-                            resource_id=resource_id,
-                            body=remove_request_body,
-                            request_id=request_id,
-                        )
-
-                        if not remove_ret["result"]:
-                            result["result"] = False
-                            result["comment"] += remove_ret["comment"]
-                            return result
-
-                        if "compute#operation" in remove_ret["ret"].get("kind"):
-                            operation = remove_ret["ret"]
-                            operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                                operation.get("selfLink"), "compute.zone_operation"
-                            )
-                            op_ret = (
-                                await hub.tool.gcp.operation_utils.handle_operation(
-                                    ctx, operation_id, "compute.disk", True
-                                )
-                            )
-                            if not op_ret["result"]:
-                                result["comment"] += op_ret["comment"]
-                                result["rerun_data"] = op_ret["rerun_data"]
-                                return result
-
-                    if (
-                        remove_ret is None or remove_ret["result"]
-                    ) and add_request_body is not None:
-                        add_ret = await hub.exec.gcp_api.client.compute.disk.addResourcePolicies(
-                            ctx,
-                            resource_id=resource_id,
-                            body=add_request_body,
-                            request_id=request_id,
-                        )
-
-                        if not add_ret["result"]:
-                            result["result"] = False
-                            result["comment"] += add_ret["comment"]
-                            return result
-
-                        if "compute#operation" in add_ret["ret"].get("kind"):
-                            operation = add_ret["ret"]
-                            operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                                operation.get("selfLink"), "compute.zone_operation"
-                            )
-                            op_ret = (
-                                await hub.tool.gcp.operation_utils.handle_operation(
-                                    ctx, operation_id, "compute.disk", True
-                                )
-                            )
-                            if not op_ret["result"]:
-                                result["comment"] += op_ret["comment"]
-                                result["rerun_data"] = op_ret["rerun_data"]
-                                return result
+        operation = None
 
-                resource_policies_updated = True
+        if not any(state_operations.changed_properties_dict.values()):
+            result["result"] = True
+            result["comment"].append(
+                hub.tool.gcp.comment_utils.up_to_date_comment("gcp.compute.disk", name)
+            )
+            result["new_state"] = result["old_state"]
+            return result
 
-        # Reset the operation because we don't need it
-        # since we are waiting for the operations to finish in order to proceed
-        operation = None
-        resource_updated = (
-            size_gb_updated or labels_updated or resource_policies_updated
-        )
-        if resource_updated:
-            if ctx.get("test", False):
-                result["comment"].append(
-                    hub.tool.gcp.comment_utils.would_update_comment(
-                        "gcp.compute.disk", name
-                    )
-                )
-            else:
-                result["comment"].append(
-                    hub.tool.gcp.comment_utils.update_comment("gcp.compute.disk", name)
-                )
-        else:
+        if ctx.get("test", False):
             result["comment"].append(
-                hub.tool.gcp.comment_utils.already_exists_comment(
+                hub.tool.gcp.comment_utils.would_update_comment(
                     "gcp.compute.disk", name
                 )
             )
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                {
+                    "resource_id": resource_id,
+                    **result["old_state"],
+                    **resource_body,
+                }
+            )
+            result["new_state"]["resource_id"] = resource_id
+            return result
+
+        state_operations_ret = await state_operations.run_operations()
+
+        current_state = result["old_state"]
+        if "new_state" in state_operations_ret:
+            current_state = state_operations_ret["new_state"]
+        elif any(state_operations.changed_properties_dict.values()):
+            get_ret = await hub.exec.gcp.compute.disk.get(ctx, resource_id=resource_id)
+            if not get_ret["result"] or not get_ret["ret"]:
+                result["result"] = False
+                result["comment"] += get_ret["comment"]
+                return result
+            current_state = get_ret["ret"]
+        result["new_state"] = current_state
+
+        if not state_operations_ret["result"]:
+            result["comment"] += state_operations_ret["comment"]
+            result["result"] = False
+            return result
+
+        if any(state_operations.changed_properties_dict.values()):
+            get_ret = await hub.exec.gcp.compute.disk.get(
+                ctx, name=name, resource_id=resource_id
+            )
+            if not get_ret["result"] and not get_ret["ret"]:
+                result["result"] = False
+                result["comment"] += get_ret["comment"]
+                return result
+
+            result["new_state"] = get_ret["ret"]
+            result["comment"].append(
+                hub.tool.gcp.comment_utils.update_comment("gcp.compute.disk", name)
+            )
+            return result
+
     else:
         if ctx["test"]:
             result["comment"].append(
                 hub.tool.gcp.comment_utils.would_create_comment(
                     "gcp.compute.disk", name
                 )
             )
-            result["new_state"] = plan_state
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                {"resource_id": resource_id, **resource_body}
+            )
             result["new_state"]["resource_id"] = resource_id
             return result
 
         # Create
-        create_ret = await hub.exec.gcp_api.client.compute.disk.insert(
-            ctx, name=name, project=project, zone=zone, body=resource_body
-        )
+        kwargs = {"name": name, "project": project, "body": resource_body}
+        if zone:
+            kwargs.update({"zone": zone})
+        if region:
+            kwargs.update({"region": region})
+
+        create_ret = await hub.exec.gcp_api.client.compute.disk.insert(ctx, **kwargs)
         if not create_ret["result"]:
             result["result"] = False
             result["comment"] += create_ret["comment"]
         else:
             result["comment"].append(
                 hub.tool.gcp.comment_utils.create_comment("gcp.compute.disk", name)
             )
             resource_id = create_ret["ret"].get("resource_id")
         if create_ret["ret"] is not None:
-            if "compute#operation" in create_ret["ret"].get("kind"):
+            if hub.tool.gcp.operation_utils.is_operation(create_ret["ret"]):
                 operation = create_ret["ret"]
 
     if operation:
-        operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-            operation.get("selfLink"), "compute.zone_operation"
-        )
-        handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, operation_id, "compute.disk"
-        )
-
-        if not handle_operation_ret["result"]:
-            result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
-            return result
-
-        resource_id = handle_operation_ret["resource_id"]
-
-    # Try getting the resource again
-    # TODO: Check if this can be removed because insert and update may also return the necessary data on success
-    get_ret = await hub.exec.gcp.compute.disk.get(
-        ctx, name=name, resource_id=resource_id
-    )
-
-    if not get_ret["result"] or not get_ret["ret"]:
-        result["result"] = False
-        result["comment"] += get_ret["comment"]
-        return result
-
-    result["new_state"] = get_ret["ret"]
-
-    return result
-
-
-async def absent(
-    hub,
-    ctx,
-    name: str,
-    resource_id: str = None,
-    request_id: str = None,
-) -> Dict[str, Any]:
-    r"""Deletes the specified persistent disk.
-
-    Deleting a disk removes its data permanently and is irreversible.
-    However, deleting a disk does not delete any snapshots previously made from the disk.
-    You must separately delete snapshots.
-
-    Args:
-        name(str):
-            An Idem name of the resource.
-
-        resource_id(str, Optional):
-            An identifier of the resource in the provider.
-            Defaults to None.
-
-        request_id(str, Optional):
-            An optional request ID to identify requests.
-            Specify a unique request ID so that if you must retry your request,
-            the server will know to ignore the request if it has already been completed.
-            For example, consider a situation where you make an initial request and the request times out.
-            If you make the request again with the same request ID,
-            the server can check if original operation with the same request ID was received, and if so,
-            will ignore the second request. This prevents clients from accidentally creating duplicate commitments.
-            The request ID must be a valid UUID with the exception that zero UUID is not supported
-            ( 00000000-0000-0000-0000-000000000000).
-            Defaults to None.
-
-    Returns:
-        Dict[str, Any]
-
-    Examples:
-        .. code-block:: sls
-
-            resource_is_absent:
-              gcp.compute.disk.absent:
-                - resource_id: resource_id
-    """
-    result = {
-        "result": True,
-        "old_state": ctx.get("old_state"),
-        "new_state": None,
-        "name": name,
-        "comment": [],
-    }
-
-    resource_id = resource_id or (ctx.old_state or {}).get("resource_id")
-    if not resource_id:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.already_absent_comment("gcp.compute.disk", name)
+        operation_type = hub.tool.gcp.operation_utils.get_operation_type(
+            operation.get("selfLink")
         )
-        return result
-
-    if not ctx.get("rerun_data"):
-        get_ret = await hub.exec.gcp.compute.disk.get(ctx, resource_id=resource_id)
-
-        if not get_ret["result"]:
-            result["result"] = False
-            result["comment"] += get_ret["comment"]
-            return result
-
-        if not get_ret["ret"]:
-            result["comment"].append(
-                hub.tool.gcp.comment_utils.already_absent_comment(
-                    "gcp.compute.disk", name
-                )
-            )
-            return result
-
-        result["old_state"] = get_ret["ret"]
-
-    if ctx["test"]:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.would_delete_comment("gcp.compute.disk", name)
+        operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
+            operation.get("selfLink"), operation_type
         )
+        result["rerun_data"] = {
+            "operation_id": operation_id,
+            "old_state": result["old_state"],
+        }
         return result
 
-    if not ctx.get("rerun_data"):
-        # First iteration; invoke disk's delete()
-        delete_ret = await hub.exec.gcp_api.client.compute.disk.delete(
-            ctx, resource_id=resource_id
-        )
-        if delete_ret["ret"]:
-            if "compute#operation" in delete_ret["ret"].get("kind"):
-                result["result"] = False
-                result["comment"] += delete_ret["comment"]
-                result[
-                    "rerun_data"
-                ] = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                    delete_ret["ret"].get("selfLink"), "compute.zone_operation"
-                )
-                return result
-    else:
-        # delete() has been called on some previous iteration
-        handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, ctx.get("rerun_data"), "compute.disk"
-        )
-        if not handle_operation_ret["result"]:
-            result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
-            return result
-
-    result["comment"].append(
-        hub.tool.gcp.comment_utils.delete_comment("gcp.compute.disk", name)
-    )
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
     r"""Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
     Retrieves a list of persistent disks contained within the specified zone.
@@ -832,8 +627,9 @@
             ]
         }
 
     return result
 
 
 def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
+    """Default implemented for each module."""
     return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/image.py` & `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/image.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """State module for managing Images."""
 from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 
+from idem_gcp.tool.gcp.utils import global_absent
+
+# prevent commit hook from removing the import
+absent = global_absent
 
 __contracts__ = ["resource"]
 
 
 async def present(
     hub,
     ctx,
@@ -158,77 +162,77 @@
 
         source_type(str, Optional):
             The type of the image used to create this disk. The default and only valid value is RAW.
 
         raw_disk(Dict[str, Any], Optional):
             The parameters of the raw disk image.
 
-                * container_type(str, Optional):
-                    The format used to encode and transmit the block device, which should be TAR.
-                    This is just a container and transmission format and not a runtime format.
-                    Provided by the client when the disk image is created.
-
-                * source(str, Optional):
-                    The full Google Cloud Storage URL where the raw disk image archive is stored.
-                    The following are valid formats for the URL:
-                        - https://storage.googleapis.com/bucket_name/image_archive_name
-                        - https://storage.googleapis.com/bucket_name/folder_name/ image_archive_name
-                        In order to create an image, you must provide the full or partial URL of one of the following:
-                        - The rawDisk.source URL
-                        - The sourceDisk URL
-                        - The sourceImage URL
-                        - The sourceSnapshot URL
-
-                * sha1_checksum(str, Optional):
-                    [Deprecated] This field is deprecated.
-                    An optional SHA1 checksum of the disk image before unpackaging provided by the client
-                    when the disk image is created.
+            * container_type(str, Optional):
+                The format used to encode and transmit the block device, which should be TAR.
+                This is just a container and transmission format and not a runtime format.
+                Provided by the client when the disk image is created.
+            * source(str, Optional):
+                The full Google Cloud Storage URL where the raw disk image archive is stored.
+                The following are valid formats for the URL:
+
+                - https://storage.googleapis.com/bucket_name/image_archive_name
+                - https://storage.googleapis.com/bucket_name/folder_name/ image_archive_name
+
+                In order to create an image, you must provide the full or partial URL of one of the following:
+
+                - The rawDisk.source URL
+                - The sourceDisk URL
+                - The sourceImage URL
+                - The sourceSnapshot URL
+            * sha1_checksum(str, Optional):
+                [Deprecated] This field is deprecated.
+                An optional SHA1 checksum of the disk image before unpackaging provided by the client
+                when the disk image is created.
 
         deprecated(Dict[str, Any], Optional):
             Deprecation status for a public resource.
 
             * deleted(str, Optional):
                 An optional RFC3339 timestamp on or after which the state of this resource
                 is intended to change to DELETED. This is only informational and the status
                 will not change unless the client explicitly changes it.
-
             * state(str, Optional):
                 The deprecation state of this resource. This can be ACTIVE, DEPRECATED, OBSOLETE, or DELETED.
                 Operations which communicate the end of life date for an image, can use ACTIVE.
                 Operations which create a new resource using a DEPRECATED resource will return successfully,
                 but with a warning indicating the deprecated resource and recommending its replacement.
                 Operations which use OBSOLETE or DELETED resources will be rejected and result in an error.
-
             * deprecated(str, Optional):
                 An optional RFC3339 timestamp on or after which the state of this resource
                 is intended to change to DEPRECATED. This is only informational and the status
                 will not change unless the client explicitly changes it.
-
             * replacement(str, Optional):
                 The URL of the suggested replacement for a deprecated resource.
                 The suggested replacement resource must be the same kind of resource as the deprecated resource.
-
             * obsolete(str, Optional):
                 An optional RFC3339 timestamp on or after which the state of this resource
                 is intended to change to OBSOLETE. This is only informational and the status
                 will not change unless the client explicitly changes it.
 
         archive_size_bytes(str, Optional):
             Size of the image tar.gz archive stored in Google Cloud Storage (in bytes).
 
         disk_size_gb(str, Optional):
             Size of the image when restored onto a persistent disk (in GB).
 
         source_disk(str, Optional):
             URL of the source disk used to create this image.
             For example, the following are valid values:
-            - https://www.googleapis.com/compute/v1/projects/project/zones/zone /disks/disk
+
+            - https://www.googleapis.com/compute/v1/projects/project/zones/zone/disks/disk
             - projects/project/zones/zone/disks/disk
             - zones/zone/disks/disk
+
             In order to create an image, you must provide the full or partial URL of one of the following:
+
             - The rawDisk.source URL
             - The sourceDisk URL
             - The sourceImage URL
             - The sourceSnapshot URL
 
         licenses(List[str], Optional):
             Any applicable license URI.
@@ -236,53 +240,61 @@
         image_encryption_key(Dict[str, Any], Optional):
             Encrypts the image using a customer-supplied encryption key. After you encrypt an image with a
             customer-supplied key, you must provide the same key if you use the image later
             (e.g. to create a disk from the image). Customer-supplied encryption keys do not protect access to metadata
             of the disk. If you do not provide an encryption key when creating the image, then the disk will be
             encrypted using an automatically generated key and you do not need to provide a key to use the image later.
 
-                * raw_key(str, Optional):
-                        Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt
-                        or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey.
-                        For example: \"raw_key\": \"SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0=\"
-
-                * rsa_encrypted_key(str, Optional):
-                    Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to
-                    either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey.
+            * raw_key(str, Optional):
+                    Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt
+                    or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey.
                     For example:
-                        \"rsa_encrypted_key\":
-                        \"ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/
-                        NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEM
-                        MoNUXMCZEIpg9Vtp9x2oe==\"
-                    The key must meet the following requirements before you can provide it to Compute Engine:
-                        1. The key is wrapped using a RSA public key certificate provided by Google.
-                        2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding.
-                    Gets the RSA public key certificate provided by Google at:
-                    https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
 
-                * kms_key_name(str, Optional):
-                    The name of the encryption key that is stored in Google Cloud KMS.
-                    For example:
-                        \"kms_key_name\":
-                        \"projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+                    \"raw_key\": \"SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0=\"
+
+            * rsa_encrypted_key(str, Optional):
+                Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to
+                either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey.
+                For example:
+
+                \"rsa_encrypted_key\":
+                \"ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/
+                NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEM
+                MoNUXMCZEIpg9Vtp9x2oe==\"
+
+                The key must meet the following requirements before you can provide it to Compute Engine:
+
+                1. The key is wrapped using a RSA public key certificate provided by Google.
+                2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding.
+
+                Gets the RSA public key certificate provided by Google at:
+                https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+
+            * kms_key_name(str, Optional):
+                The name of the encryption key that is stored in Google Cloud KMS.
+                For example:
 
-                * kms_key_service_account(str, Optional):
-                    The service account being used for the encryption request for the given KMS key. If absent,
-                    the Compute Engine default service account is used. For example:
-                        \"kms_key_service_account\":
-                        \"name@project_id.iam.gserviceaccount.com/
+                \"kms_key_name\":
+                \"projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+
+            * kms_key_service_account(str, Optional):
+                The service account being used for the encryption request for the given KMS key. If absent,
+                the Compute Engine default service account is used. For example:
+
+                \"kms_key_service_account\":
+                \"name@project_id.iam.gserviceaccount.com/
 
         source_disk_encryption_key(Dict[str, Any], Optional):
             The customer-supplied encryption key of the source disk.
             Required if the source disk is protected by a customer-supplied encryption key."
 
-                * raw_key(str, Optional)
-                * rsa_encrypted_key(str, Optional)
-                * kms_key_name(str, Optional)
-                * kms_key_service_account(str, Optional)
+            * raw_key(str, Optional)
+            * rsa_encrypted_key(str, Optional)
+            * kms_key_name(str, Optional)
+            * kms_key_service_account(str, Optional)
 
         labels(Dict[str, str], Optional):
             Labels to apply to this image. These can be later modified by the setLabels method.
 
         label_fingerprint(str, Optional):
             A fingerprint for the labels being applied to this image, which is essentially a hash of the labels
             used for optimistic locking. The fingerprint is initially generated by Compute Engine and changes after
@@ -290,100 +302,107 @@
             in order to update or change labels, otherwise the request will fail with error 412 conditionNotMet.
             To see the latest fingerprint, make a get() request to retrieve an image.
 
         guest_os_features(List[Dict[str, Any]], Optional):
             A list of features to enable on the guest operating system. Applicable only for bootable images.
             To see a list of available options, see the guestOSfeatures[].type parameter.
 
-                * type (str, Optional):
+            * type (str, Optional):
                 The ID of a supported feature. To add multiple values,
                 use commas to separate values. Set to one or more of the following values:
-                    - VIRTIO_SCSI_MULTIQUEUE
-                    - WINDOWS
-                    - MULTI_IP_SUBNET
-                    - UEFI_COMPATIBLE
-                    - GVNIC
-                    - SEV_CAPABLE
-                    - SUSPEND_RESUME_COMPATIBLE
-                    - SEV_SNP_CAPABLE
+
+                - VIRTIO_SCSI_MULTIQUEUE
+                - WINDOWS
+                - MULTI_IP_SUBNET
+                - UEFI_COMPATIBLE
+                - GVNIC
+                - SEV_CAPABLE
+                - SUSPEND_RESUME_COMPATIBLE
+                - SEV_SNP_CAPABLE
+
                 For more information, see Enabling guest operating system features.
 
         license_codes(List[str], Optional):
             Integer license codes indicating which licenses are attached to this image.
 
         source_image(str, Optional):
             URL of the source image used to create this image. The following are valid formats for the URL:
-            - https://www.googleapis.com/compute/v1/projects/project_id/global/ images/image_name
+
+            - https://www.googleapis.com/compute/v1/projects/project_id/global/images/image_name
             - projects/project_id/global/images/image_name
+
             In order to create an image, you must provide the full or partial URL of one of the following:
+
             - The rawDisk.source URL
             - The sourceDisk URL
             - The sourceImage URL
             - The sourceSnapshot URL
 
         source_image_encryption_key(Dict[str, Any], Optional):
             The customer-supplied encryption key of the source image.
             Required if the source image is protected by a customer-supplied encryption key.
 
-                * raw_key(str, Optional)
-                * rsa_encrypted_key(str, Optional)
-                * kms_key_name(str, Optional)
-                * kms_key_service_account(str, Optional)
+            * raw_key(str, Optional)
+            * rsa_encrypted_key(str, Optional)
+            * kms_key_name(str, Optional)
+            * kms_key_service_account(str, Optional)
 
         source_snapshot(str, Optional):
             URL of the source snapshot used to create this image. The following are valid formats for the URL:
-            - https://www.googleapis.com/compute/v1/projects/project_id/global/ snapshots/snapshot_name
+
+            - https://www.googleapis.com/compute/v1/projects/project_id/global/snapshots/snapshot_name
             - projects/project_id/global/snapshots/snapshot_name
+
             In order to create an image, you must provide the full or partial URL of one of the following:
+
             - The rawDisk.source URL
             - The sourceDisk URL
             - The sourceImage URL
             - The sourceSnapshot URL
 
         source_snapshot_encryption_key(Dict[str, Any], Optional):
             The customer-supplied encryption key of the source snapshot.
             Required if the source snapshot is protected by a customer-supplied encryption key.
 
-                * raw_key(str, Optional)
-                * rsa_encrypted_key(str, Optional)
-                * kms_key_name(str, Optional)
-                * kms_key_service_account(str, Optional)
+            * raw_key(str, Optional)
+            * rsa_encrypted_key(str, Optional)
+            * kms_key_name(str, Optional)
+            * kms_key_service_account(str, Optional)
 
         storage_locations(List[str], Optional):
             Cloud Storage bucket storage location of the image (regional or multi-regional).
 
         shielded_instance_initial_state(Dict[str, Any], Optional):
             Set the secure boot keys of shielded instance.
 
-                * keks(List[Dict[str, Any]], Optional):
-                    The Key Exchange Key (KEK).
-
-                    * content(str, Optional):
-                        The raw content in the secure keys file.
+            * keks(List[Dict[str, Any]], Optional):
+                The Key Exchange Key (KEK).
 
-                    * file_type(str, Optional):
-                        The file type of source file.
+                * content(str, Optional):
+                    The raw content in the secure keys file.
+                * file_type(str, Optional):
+                    The file type of source file.
 
-                * pk(Dict[str, Any], Optional):
-                    The Platform Key (PK).
+            * pk(Dict[str, Any], Optional):
+                The Platform Key (PK).
 
-                    * content(str, Optional)
-                    * file_type(str, Optional)
+                * content(str, Optional)
+                * file_type(str, Optional)
 
-                * dbs(List[Dict[str, Any]], Optional):
-                    The Key Database (db).
+            * dbs(List[Dict[str, Any]], Optional):
+                The Key Database (db).
 
-                    * content(str, Optional)
-                    * file_type(str, Optional)
+                * content(str, Optional)
+                * file_type(str, Optional)
 
-                * dbxs(List[Dict[str, Any]], Optional):
-                    The forbidden key database (dbx).
+            * dbxs(List[Dict[str, Any]], Optional):
+                The forbidden key database (dbx).
 
-                    * content(str, Optional)
-                    * file_type(str, Optional)
+                * content(str, Optional)
+                * file_type(str, Optional)
 
         architecture(str, Optional):
             The architecture of the image. Valid values are ARM64 or X86_64.
 
     Returns:
         Dict[str, Any]
 
@@ -400,117 +419,23 @@
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
     # TODO uncomment below line, when implementation is added
-    # project = get_project_from_account(ctx, project)
+    # project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     result["comment"].append(
         "No-op: There is no create/update function for gcp.compute.image"
     )
 
     return result
 
 
-async def absent(
-    hub,
-    ctx,
-    name: str,
-    resource_id: str = None,
-    request_id: str = None,
-) -> Dict[str, Any]:
-    r"""Deletes the specified image.
-
-    Args:
-        name(str):
-            An Idem name of the resource.
-
-        resource_id(str, Optional):
-            An identifier of the resource in the provider.
-            Defaults to None.
-
-        request_id(str, Optional):
-            An optional request ID to identify requests.
-            Specify a unique request ID so that if you must retry your request,
-            the server will know to ignore the request if it has already been completed.
-            For example, consider a situation where you make an initial request and the request times out.
-            If you make the request again with the same request ID,
-            the server can check if original operation with the same request ID was received, and if so,
-            will ignore the second request. This prevents clients from accidentally creating duplicate commitments.
-            The request ID must be a valid UUID with the exception that zero UUID is not supported
-            ( 00000000-0000-0000-0000-000000000000).
-            Defaults to None.
-
-    Returns:
-        Dict[str, Any]
-
-    Examples:
-        .. code-block:: sls
-
-            resource_is_absent:
-              gcp.compute.image.absent:
-                - resource_id: resource_id
-    """
-    result = {
-        "result": True,
-        "old_state": ctx.old_state,
-        "new_state": None,
-        "name": name,
-        "comment": [],
-    }
-
-    if not resource_id:
-        resource_id = (ctx.old_state or {}).get("resource_id")
-
-    if ctx.test:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.would_delete_comment("gcp.compute.image", name)
-        )
-        return result
-
-    if not ctx.get("rerun_data"):
-        delete_ret = await hub.exec.gcp_api.client.compute.image.delete(
-            ctx, resource_id=resource_id
-        )
-        if delete_ret["ret"]:
-            if "compute#operation" in delete_ret["ret"].get("kind"):
-                result["result"] = False
-                result["comment"] += delete_ret["comment"]
-                result[
-                    "rerun_data"
-                ] = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                    delete_ret["ret"].get("selfLink"), "compute.zone_operation"
-                )
-                return result
-    else:
-        # delete() has been called on some previous iteration
-        handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, ctx.get("rerun_data"), "compute.image"
-        )
-        if not handle_operation_ret["result"]:
-            result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
-            return result
-
-        resource_id = handle_operation_ret["resource_id"]
-
-    if not resource_id:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.already_absent_comment("gcp.compute.image", name)
-        )
-        return result
-
-    result["comment"].append(
-        hub.tool.gcp.comment_utils.delete_comment("gcp.compute.image", name)
-    )
-    return result
-
-
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
     r"""Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
     Retrieves a list of images.
 
     Returns:
         Dict[str, Any]
@@ -539,8 +464,9 @@
             ]
         }
 
     return result
 
 
 def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
+    """Default implemented for each module."""
     return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/instance.py` & `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 """Google Cloud Platform compute instances state module.
 
 Copyright (c) 2022 VMware, Inc. All Rights Reserved.
 SPDX-License-Identifier: Apache-2.0
 
 """
-
-__contracts__ = ["resource"]
-
 from dataclasses import field
 from dataclasses import make_dataclass
-from typing import Dict, Any, List
-import copy
-from idem_gcp.tool.gcp.utils import get_project_from_account
+from typing import Any
+from typing import Dict
+from typing import List
+
+from dict_tools.typing import Computed
+
+from idem_gcp.tool.gcp.state_operation_utils import StateOperations
+from idem_gcp.tool.gcp.utils import zonal_absent
+
+# prevent commit hook from removing the import
+absent = zonal_absent
+
+__contracts__ = ["resource"]
 
 
 async def present(
     hub,
     ctx,
     name: str,
     zone: str,
@@ -62,15 +69,15 @@
                                     "external_ipv6_prefix_length",
                                     int,
                                     field(default=None),
                                 ),
                                 ("name", str, field(default=None)),
                                 ("kind", str, field(default=None)),
                                 ("external_ipv6", str, field(default=None)),
-                                ("type_", str, field(default=None)),
+                                ("type_", (str, "alias=type"), field(default=None)),
                                 ("set_public_ptr", bool, field(default=None)),
                                 ("public_ptr_domain_name", str, field(default=None)),
                                 ("nat_ip", str, field(default=None)),
                             ],
                         )
                     ],
                     field(default=None),
@@ -104,15 +111,15 @@
                                     "external_ipv6_prefix_length",
                                     int,
                                     field(default=None),
                                 ),
                                 ("name", str, field(default=None)),
                                 ("kind", str, field(default=None)),
                                 ("external_ipv6", str, field(default=None)),
-                                ("type_", str, field(default=None)),
+                                ("type_", (str, "alias=type"), field(default=None)),
                                 ("set_public_ptr", bool, field(default=None)),
                                 ("public_ptr_domain_name", str, field(default=None)),
                                 ("nat_ip", str, field(default=None)),
                             ],
                         )
                     ],
                     field(default=None),
@@ -202,15 +209,16 @@
                 ("disk_size_gb", str, field(default=None)),
                 ("auto_delete", bool, field(default=None)),
                 ("boot", bool, field(default=None)),
                 (
                     "guest_os_features",
                     List[
                         make_dataclass(
-                            "GuestOsFeature", [("type_", str, field(default=None))]
+                            "GuestOsFeature",
+                            [("type_", (str, "alias=type"), field(default=None))],
                         )
                     ],
                     field(default=None),
                 ),
                 ("source", str, field(default=None)),
                 (
                     "disk_encryption_key",
@@ -351,15 +359,15 @@
                     field(default=None),
                 ),
                 ("kind", str, field(default=None)),
                 ("index", int, field(default=None)),
                 ("interface", str, field(default=None)),
                 ("licenses", List[str], field(default=None)),
                 ("mode", str, field(default=None)),
-                ("type_", str, field(default=None)),
+                ("type_", (str, "alias=type"), field(default=None)),
             ],
         )
     ] = None,
     hostname: str = None,
     network_performance_config: make_dataclass(
         "NetworkPerformanceConfig",
         [("total_egress_bandwidth_tier", str, field(default=None))],
@@ -372,15 +380,15 @@
     metadata: make_dataclass(
         "Metadata",
         [
             (
                 "items",
                 List[
                     make_dataclass(
-                        "Classcc3f9d3b673e4a89805fea2c3069bd85",
+                        "MetadataItemsProperties",
                         [
                             ("key", str, field(default=None)),
                             ("value", str, field(default=None)),
                         ],
                     )
                 ],
                 field(default=None),
@@ -404,204 +412,183 @@
     min_cpu_platform: str = None,
     machine_type: str = None,
     source_instance_template: str = None,
     request_id: str = None,
     minimal_action: str = None,
     most_disruptive_allowed_action: str = None,
     resource_id: str = None,
+    id_: (Computed[str], "alias=id") = None,
 ) -> Dict[str, Any]:
-    r"""Create or update a compute instance resource.
+    """Create or update a compute instance resource.
 
     Creates an instance resource in the specified project using the data included in the request.
     or
     Updates an instance only if the necessary resources are available. This method can update only a specific set of instance properties. See Updating a running instance for a list of updatable instance properties.
+
     Args:
         name(str):
             An Idem name of the resource.
 
-        service_accounts(List[Dict[str, Any]], optional):
+        service_accounts(List[Dict[str, Any]], Optional):
             A list of service accounts, with their specified scopes, authorized for this instance. Only one service account per VM instance is supported. Service accounts generate access tokens that can be accessed through the metadata server and used to authenticate applications on the instance. See Service Accounts for more information. Defaults to None.
 
-                * scopes (List[str], optional):
-                    The list of scopes to be made available for this service account.
+            * scopes (List[str], Optional):
+                The list of scopes to be made available for this service account.
+            * email (str, Optional):
+                Email address of the service account.
 
-                * email (str, optional):
-                    Email address of the service account.
-
-        label_fingerprint(str, optional):
+        label_fingerprint(str, Optional):
             A fingerprint for this request, which is essentially a hash of the label's contents and used for optimistic locking. The fingerprint is initially generated by Compute Engine and changes after every request to modify or update labels. You must always provide an up-to-date fingerprint hash in order to update or change labels. To see the latest fingerprint, make get() request to the instance. Defaults to None.
 
-        fingerprint(str, optional):
+        fingerprint(str, Optional):
             Specifies a fingerprint for this resource, which is essentially a hash of the instance's contents and used for optimistic locking. The fingerprint is initially generated by Compute Engine and changes after every request to modify or update the instance. You must always provide an up-to-date fingerprint hash in order to update the instance. To see the latest fingerprint, make get() request to the instance. Defaults to None.
 
-        advanced_machine_features(Dict[str, Any], optional):
-            Controls for advanced machine-related behavior features.
+        advanced_machine_features(Dict[str, Any], Optional):
+            Specifies options for controlling advanced machine features. Options that would traditionally be configured in a BIOS belong here. Features that require operating system support may have corresponding entries in the GuestOsFeatures of an Image (e.g., whether or not the OS in the Image supports nested virtualization being enabled or disabled). Defaults to None.
+
+            * enable_nested_virtualization (bool, Optional):
+                Whether to enable nested virtualization or not (default is false).
+            * visible_core_count (int, Optional):
+                The number of physical cores to expose to an instance. Multiply by the number of threads per core to compute the total number of virtual CPUs to expose to the instance. If unset, the number of cores is inferred from the instance's nominal CPU count and the underlying platform's SMT width.
+            * enable_uefi_networking (bool, Optional):
+                Whether to enable UEFI networking for instance creation.
+            * threads_per_core (int, Optional):
+                The number of threads per physical core. To disable simultaneous multithreading (SMT) set this to 1. If unset, the maximum number of threads supported per core by the underlying processor is assumed.
 
-                AdvancedMachineFeatures: Specifies options for controlling advanced machine features. Options that would traditionally be configured in a BIOS belong here. Features that require operating system support may have corresponding entries in the GuestOsFeatures of an Image (e.g., whether or not the OS in the Image supports nested virtualization being enabled or disabled). Defaults to None.
-                * enable_nested_virtualization (bool, optional):
-                    Whether to enable nested virtualization or not (default is false).
-
-                * visible_core_count (int, optional):
-                    The number of physical cores to expose to an instance. Multiply by the number of threads per core to compute the total number of virtual CPUs to expose to the instance. If unset, the number of cores is inferred from the instance's nominal CPU count and the underlying platform's SMT width.
-
-                * enable_uefi_networking (bool, optional):
-                    Whether to enable UEFI networking for instance creation.
-
-                * threads_per_core (int, optional):
-                    The number of threads per physical core. To disable simultaneous multithreading (SMT) set this to 1. If unset, the maximum number of threads supported per core by the underlying processor is assumed.
-        can_ip_forward(bool, optional):
+        can_ip_forward(bool, Optional):
             Allows this instance to send and receive packets with non-matching destination or source IPs. This is required if you plan to use this instance to forward routes. For more information, see Enabling IP Forwarding . Defaults to None.
 
-        network_interfaces(List[Dict[str, Any]], optional):
+        network_interfaces(List[Dict[str, Any]], Optional):
             An array of network configurations for this instance. These specify how interfaces are configured to interact with other network services, such as connecting to the internet. Multiple interfaces are supported per instance. Defaults to None.
-                * kind (str, optional):
-                    [Output Only] Type of the resource. Always compute#networkInterface for network interfaces.
 
-                * network (str, optional):
-                    URL of the VPC network resource for this instance. When creating an instance, if neither the network nor the subnetwork is specified, the default network global/networks/default is used. If the selected project doesn't have the default network, you must specify a network or subnet. If the network is not specified but the subnetwork is specified, the network is inferred. If you specify this property, you can specify the network as a full or partial URL. For example, the following are all valid URLs: - https://www.googleapis.com/compute/v1/projects/project/global/networks/ network - projects/project/global/networks/network - global/networks/default
-
-                * stack_type (str, optional):
-                    The stack type for this network interface to identify whether the IPv6 feature is enabled or not. If not specified, IPV4_ONLY will be used. This field can be both set at instance creation and update network interface operations.
-                        Enum type. Allowed values:
+            * kind (str, Optional):
+                [Output Only] Type of the resource. Always compute#networkInterface for network interfaces.
+            * network (str, Optional):
+                URL of the VPC network resource for this instance. When creating an instance, if neither the network nor the subnetwork is specified, the default network global/networks/default is used. If the selected project doesn't have the default network, you must specify a network or subnet. If the network is not specified but the subnetwork is specified, the network is inferred. If you specify this property, you can specify the network as a full or partial URL. For example, the following are all valid URLs:
+
+                - https://www.googleapis.com/compute/v1/projects/project/global/networks/network
+                - projects/project/global/networks/network
+                - global/networks/default
+            * stack_type (str, Optional):
+                The stack type for this network interface to identify whether the IPv6 feature is enabled or not. If not specified, IPV4_ONLY will be used. This field can be both set at instance creation and update network interface operations.
+                    Enum type. Allowed values:
                         "IPV4_IPV6" - The network interface can have both IPv4 and IPv6 addresses.
                         "IPV4_ONLY" - The network interface will be assigned IPv4 address.
+            * name (str, Optional):
+                [Output Only] The name of the network interface, which is generated by the server. For a VM, the network interface uses the nicN naming format. Where N is a value between 0 and 7. The default interface value is nic0.
+            * subnetwork (str, Optional):
+                The URL of the Subnetwork resource for this instance. If the network resource is in legacy mode, do not specify this field. If the network is in auto subnet mode, specifying the subnetwork is optional. If the network is in custom subnet mode, specifying the subnetwork is required. If you specify this field, you can specify the subnetwork as a full or partial URL. For example, the following are all valid URLs:
+
+                - https://www.googleapis.com/compute/v1/projects/project/regions/region/subnetworks/subnetwork
+                - regions/region/subnetworks/subnetwork
+            * queue_count (int, Optional):
+                The networking queue count that's specified by users for the network interface. Both Rx and Tx queues will be set to this number. It'll be empty if not specified by the users.
+            * ipv6_access_configs (List[Dict[str, Any]], Optional):
+                An array of IPv6 access configurations for this interface. Currently, only one IPv6 access config, DIRECT_IPV6, is supported. If there is no ipv6AccessConfig specified, then this instance will have no external IPv6 Internet access.
 
-                * name (str, optional):
-                    [Output Only] The name of the network interface, which is generated by the server. For a VM, the network interface uses the nicN naming format. Where N is a value between 0 and 7. The default interface value is nic0.
-
-                * subnetwork (str, optional):
-                    The URL of the Subnetwork resource for this instance. If the network resource is in legacy mode, do not specify this field. If the network is in auto subnet mode, specifying the subnetwork is optional. If the network is in custom subnet mode, specifying the subnetwork is required. If you specify this field, you can specify the subnetwork as a full or partial URL. For example, the following are all valid URLs: - https://www.googleapis.com/compute/v1/projects/project/regions/region /subnetworks/subnetwork - regions/region/subnetworks/subnetwork
-
-                * queue_count (int, optional):
-                    The networking queue count that's specified by users for the network interface. Both Rx and Tx queues will be set to this number. It'll be empty if not specified by the users.
-
-                * ipv6_access_configs (List[Dict[str, Any]], optional):
-                    An array of IPv6 access configurations for this interface. Currently, only one IPv6 access config, DIRECT_IPV6, is supported. If there is no ipv6AccessConfig specified, then this instance will have no external IPv6 Internet access.
-
-                        * network_tier (str, optional):
-                            This signifies the networking tier used for configuring this access configuration and can only take the following values: PREMIUM, STANDARD. If an AccessConfig is specified without a valid external IP address, an ephemeral IP will be created with this networkTier. If an AccessConfig with a valid external IP address is specified, it must match that of the networkTier associated with the Address resource owning that IP.
-                                Enum type. Allowed values:
-                                "FIXED_STANDARD" - Public internet quality with fixed bandwidth.
-                                "PREMIUM" - High quality, Google-grade network tier, support for all networking products.
-                                "STANDARD" - Public internet quality, only limited support for other networking products.
-                                "STANDARD_OVERRIDES_FIXED_STANDARD" - (Output only) Temporary tier for FIXED_STANDARD when fixed standard tier is expired or not configured.
-
-                        * external_ipv6_prefix_length (int, optional):
-                            The prefix length of the external IPv6 range.
-
-                        * name (str, optional):
-                            The name of this access configuration. The default and recommended name is External NAT, but you can use any arbitrary string, such as My external IP or Network Access.
-
-                        * kind (str, optional):
-                            [Output Only] Type of the resource. Always compute#accessConfig for access configs.
-
-                        * external_ipv6 (str, optional):
-                            The first IPv6 address of the external IPv6 range associated with this instance, prefix length is stored in externalIpv6PrefixLength in ipv6AccessConfig. The field is output only, an IPv6 address from a subnetwork associated with the instance will be allocated dynamically.
-
-                        * type_ (str, optional):
-                            The type of configuration. The default and only option is ONE_TO_ONE_NAT.
-                                Enum type. Allowed values:
-                                "DIRECT_IPV6"
-                                "ONE_TO_ONE_NAT"
-
-                        * set_public_ptr (bool, optional):
-                            Specifies whether a public DNS 'PTR' record should be created to map the external IP address of the instance to a DNS domain name. This field is not used in ipv6AccessConfig. A default PTR record will be created if the VM has external IPv6 range associated.
-
-                        * public_ptr_domain_name (str, optional):
-                            The DNS domain name for the public PTR record. You can set this field only if the `setPublicPtr` field is enabled in accessConfig. If this field is unspecified in ipv6AccessConfig, a default PTR record will be createc for first IP in associated external IPv6 range.
-
-                        * nat_ip (str, optional):
-                            An external IP address associated with this instance. Specify an unused static external IP address available to the project or leave this field undefined to use an IP from a shared ephemeral IP address pool. If you specify a static external IP address, it must live in the same region as the zone of the instance.
-
-                * internal_ipv6_prefix_length (int, optional):
-                    The prefix length of the primary internal IPv6 range.
-
-                * fingerprint (str, optional):
-                    Fingerprint hash of contents stored in this network interface. This field will be ignored when inserting an Instance or adding a NetworkInterface. An up-to-date fingerprint must be provided in order to update the NetworkInterface. The request will fail with error 400 Bad Request if the fingerprint is not provided, or 412 Precondition Failed if the fingerprint is out of date.
-
-                * alias_ip_ranges (List[Dict[str, Any]], optional):
-                    An array of alias IP ranges for this network interface. You can only specify this field for network interfaces in VPC networks.
-
-                        * ip_cidr_range (str, optional):
-                            The IP alias ranges to allocate for this interface. This IP CIDR range must belong to the specified subnetwork and cannot contain IP addresses reserved by system or used by other network interfaces. This range may be a single IP address (such as 10.2.3.4), a netmask (such as /24) or a CIDR-formatted string (such as 10.1.2.0/24).
-
-                        * subnetwork_range_name (str, optional):
-                            The name of a subnetwork secondary IP range from which to allocate an IP alias range. If not specified, the primary range of the subnetwork is used.
-
-                * ipv6_access_type (str, optional):
-                    [Output Only] One of EXTERNAL, INTERNAL to indicate whether the IP can be accessed from the Internet. This field is always inherited from its subnetwork. Valid only if stackType is IPV4_IPV6.
+                * network_tier (str, Optional):
+                    This signifies the networking tier used for configuring this access configuration and can only take the following values: PREMIUM, STANDARD. If an AccessConfig is specified without a valid external IP address, an ephemeral IP will be created with this networkTier. If an AccessConfig with a valid external IP address is specified, it must match that of the networkTier associated with the Address resource owning that IP.
                         Enum type. Allowed values:
-                        "EXTERNAL" - This network interface can have external IPv6.
-                        "INTERNAL" - This network interface can have internal IPv6.
-
-                * network_ip (str, optional):
-                    An IPv4 internal IP address to assign to the instance for this network interface. If not specified by the user, an unused internal IP is assigned by the system.
-
-                * nic_type (str, optional):
-                    The type of vNIC to be used on this interface. This may be gVNIC or VirtioNet.
+                        "FIXED_STANDARD" - Public internet quality with fixed bandwidth.
+                        "PREMIUM" - High quality, Google-grade network tier, support for all networking products.
+                        "STANDARD" - Public internet quality, only limited support for other networking products.
+                        "STANDARD_OVERRIDES_FIXED_STANDARD" - (Output only) Temporary tier for FIXED_STANDARD when fixed standard tier is expired or not configured.
+                * external_ipv6_prefix_length (int, Optional):
+                    The prefix length of the external IPv6 range.
+                * name (str, Optional):
+                    The name of this access configuration. The default and recommended name is External NAT, but you can use any arbitrary string, such as My external IP or Network Access.
+                * kind (str, Optional):
+                    [Output Only] Type of the resource. Always compute#accessConfig for access configs.
+                * external_ipv6 (str, Optional):
+                    The first IPv6 address of the external IPv6 range associated with this instance, prefix length is stored in externalIpv6PrefixLength in ipv6AccessConfig. The field is output only, an IPv6 address from a subnetwork associated with the instance will be allocated dynamically.
+                * type (str, Optional):
+                    The type of configuration. The default and only option is ONE_TO_ONE_NAT.
                         Enum type. Allowed values:
-                        "GVNIC" - GVNIC
-                        "UNSPECIFIED_NIC_TYPE" - No type specified.
-                        "VIRTIO_NET" - VIRTIO
+                        "DIRECT_IPV6"
+                        "ONE_TO_ONE_NAT"
+                * set_public_ptr (bool, Optional):
+                    Specifies whether a public DNS 'PTR' record should be created to map the external IP address of the instance to a DNS domain name. This field is not used in ipv6AccessConfig. A default PTR record will be created if the VM has external IPv6 range associated.
+                * public_ptr_domain_name (str, Optional):
+                    The DNS domain name for the public PTR record. You can set this field only if the `setPublicPtr` field is enabled in accessConfig. If this field is unspecified in ipv6AccessConfig, a default PTR record will be createc for first IP in associated external IPv6 range.
+                * nat_ip (str, Optional):
+                    An external IP address associated with this instance. Specify an unused static external IP address available to the project or leave this field undefined to use an IP from a shared ephemeral IP address pool. If you specify a static external IP address, it must live in the same region as the zone of the instance.
+
+            * internal_ipv6_prefix_length (int, Optional):
+                The prefix length of the primary internal IPv6 range.
+            * fingerprint (str, Optional):
+                Fingerprint hash of contents stored in this network interface. This field will be ignored when inserting an Instance or adding a NetworkInterface. An up-to-date fingerprint must be provided in order to update the NetworkInterface. The request will fail with error 400 Bad Request if the fingerprint is not provided, or 412 Precondition Failed if the fingerprint is out of date.
+            * alias_ip_ranges (List[Dict[str, Any]], Optional):
+                An array of alias IP ranges for this network interface. You can only specify this field for network interfaces in VPC networks.
+
+                * ip_cidr_range (str, Optional):
+                    The IP alias ranges to allocate for this interface. This IP CIDR range must belong to the specified subnetwork and cannot contain IP addresses reserved by system or used by other network interfaces. This range may be a single IP address (such as 10.2.3.4), a netmask (such as /24) or a CIDR-formatted string (such as 10.1.2.0/24).
+                * subnetwork_range_name (str, Optional):
+                    The name of a subnetwork secondary IP range from which to allocate an IP alias range. If not specified, the primary range of the subnetwork is used.
 
-                * access_configs (List[Dict[str, Any]], optional):
-                    An array of configurations for this interface. Currently, only one access config, ONE_TO_ONE_NAT, is supported. If there are no accessConfigs specified, then this instance will have no external internet access.
-
-                        * network_tier (str, optional):
-                            This signifies the networking tier used for configuring this access configuration and can only take the following values: PREMIUM, STANDARD. If an AccessConfig is specified without a valid external IP address, an ephemeral IP will be created with this networkTier. If an AccessConfig with a valid external IP address is specified, it must match that of the networkTier associated with the Address resource owning that IP.
-                                Enum type. Allowed values:
-                                "FIXED_STANDARD" - Public internet quality with fixed bandwidth.
-                                "PREMIUM" - High quality, Google-grade network tier, support for all networking products.
-                                "STANDARD" - Public internet quality, only limited support for other networking products.
-                                "STANDARD_OVERRIDES_FIXED_STANDARD" - (Output only) Temporary tier for FIXED_STANDARD when fixed standard tier is expired or not configured.
-
-                        * external_ipv6_prefix_length (int, optional):
-                            The prefix length of the external IPv6 range.
-
-                        * name (str, optional):
-                            The name of this access configuration. The default and recommended name is External NAT, but you can use any arbitrary string, such as My external IP or Network Access.
-
-                        * kind (str, optional):
-                            [Output Only] Type of the resource. Always compute#accessConfig for access configs.
-
-                        * external_ipv6 (str, optional):
-                            The first IPv6 address of the external IPv6 range associated with this instance, prefix length is stored in externalIpv6PrefixLength in ipv6AccessConfig. The field is output only, an IPv6 address from a subnetwork associated with the instance will be allocated dynamically.
-
-                        * type_ (str, optional):
-                            The type of configuration. The default and only option is ONE_TO_ONE_NAT.
-                                Enum type. Allowed values:
-                                "DIRECT_IPV6"
-                                "ONE_TO_ONE_NAT"
-
-                        * set_public_ptr (bool, optional):
-                            Specifies whether a public DNS 'PTR' record should be created to map the external IP address of the instance to a DNS domain name. This field is not used in ipv6AccessConfig. A default PTR record will be created if the VM has external IPv6 range associated.
+            * ipv6_access_type (str, Optional):
+                [Output Only] One of EXTERNAL, INTERNAL to indicate whether the IP can be accessed from the Internet. This field is always inherited from its subnetwork. Valid only if stackType is IPV4_IPV6.
+                    Enum type. Allowed values:
+                    "EXTERNAL" - This network interface can have external IPv6.
+                    "INTERNAL" - This network interface can have internal IPv6.
+            * network_ip (str, Optional):
+                An IPv4 internal IP address to assign to the instance for this network interface. If not specified by the user, an unused internal IP is assigned by the system.
+            * nic_type (str, Optional):
+                The type of vNIC to be used on this interface. This may be gVNIC or VirtioNet.
+                    Enum type. Allowed values:
+                    "GVNIC" - GVNIC
+                    "UNSPECIFIED_NIC_TYPE" - No type specified.
+                    "VIRTIO_NET" - VIRTIO
 
-                        * public_ptr_domain_name (str, optional):
-                            The DNS domain name for the public PTR record. You can set this field only if the `setPublicPtr` field is enabled in accessConfig. If this field is unspecified in ipv6AccessConfig, a default PTR record will be createc for first IP in associated external IPv6 range.
+            * access_configs (List[Dict[str, Any]], Optional):
+                An array of configurations for this interface. Currently, only one access config, ONE_TO_ONE_NAT, is supported. If there are no accessConfigs specified, then this instance will have no external internet access.
 
-                        * nat_ip (str, optional):
-                            An external IP address associated with this instance. Specify an unused static external IP address available to the project or leave this field undefined to use an IP from a shared ephemeral IP address pool. If you specify a static external IP address, it must live in the same region as the zone of the instance.
+                * network_tier (str, Optional):
+                    This signifies the networking tier used for configuring this access configuration and can only take the following values: PREMIUM, STANDARD. If an AccessConfig is specified without a valid external IP address, an ephemeral IP will be created with this networkTier. If an AccessConfig with a valid external IP address is specified, it must match that of the networkTier associated with the Address resource owning that IP.
+                        Enum type. Allowed values:
+                        "FIXED_STANDARD" - Public internet quality with fixed bandwidth.
+                        "PREMIUM" - High quality, Google-grade network tier, support for all networking products.
+                        "STANDARD" - Public internet quality, only limited support for other networking products.
+                        "STANDARD_OVERRIDES_FIXED_STANDARD" - (Output only) Temporary tier for FIXED_STANDARD when fixed standard tier is expired or not configured.
+                * external_ipv6_prefix_length (int, Optional):
+                    The prefix length of the external IPv6 range.
+                * name (str, Optional):
+                    The name of this access configuration. The default and recommended name is External NAT, but you can use any arbitrary string, such as My external IP or Network Access.
+                * kind (str, Optional):
+                    [Output Only] Type of the resource. Always compute#accessConfig for access configs.
+                * external_ipv6 (str, Optional):
+                    The first IPv6 address of the external IPv6 range associated with this instance, prefix length is stored in externalIpv6PrefixLength in ipv6AccessConfig. The field is output only, an IPv6 address from a subnetwork associated with the instance will be allocated dynamically.
+                * type (str, Optional):
+                    The type of configuration. The default and only option is ONE_TO_ONE_NAT.
+                        Enum type. Allowed values:
+                        "DIRECT_IPV6"
+                        "ONE_TO_ONE_NAT"
+                * set_public_ptr (bool, Optional):
+                    Specifies whether a public DNS 'PTR' record should be created to map the external IP address of the instance to a DNS domain name. This field is not used in ipv6AccessConfig. A default PTR record will be created if the VM has external IPv6 range associated.
+                * public_ptr_domain_name (str, Optional):
+                    The DNS domain name for the public PTR record. You can set this field only if the `setPublicPtr` field is enabled in accessConfig. If this field is unspecified in ipv6AccessConfig, a default PTR record will be createc for first IP in associated external IPv6 range.
+                * nat_ip (str, Optional):
+                    An external IP address associated with this instance. Specify an unused static external IP address available to the project or leave this field undefined to use an IP from a shared ephemeral IP address pool. If you specify a static external IP address, it must live in the same region as the zone of the instance.
 
-                * ipv6_address (str, optional):
-                    An IPv6 internal network address for this network interface.
+            * ipv6_address (str, Optional):
+                An IPv6 internal network address for this network interface.
 
-        labels(Dict[str, Any], optional):
+        labels(Dict[str, Any], Optional):
             Labels to apply to this instance. These can be later modified by the setLabels method. Defaults to None.
 
-        display_device(Dict[str, Any], optional):
+        display_device(Dict[str, Any], Optional):
             Enables display device for the instance.
-                DisplayDevice: A set of Display Device options. Defaults to None.
+            DisplayDevice: A set of Display Device options. Defaults to None.
 
-                * enable_display (bool, optional):
-                    Defines whether the instance has Display enabled.
+            * enable_display (bool, Optional):
+                Defines whether the instance has Display enabled.
 
-        source_machine_image(str, optional):
+        source_machine_image(str, Optional):
             Source machine image. Defaults to None.
 
-        resource_policies(List[str], optional):
+        resource_policies(List[str], Optional):
             Resource policies applied to this instance. Defaults to None.
 
         status(str, Optional):
             The status of the instance. One of the following values: PROVISIONING, STAGING, RUNNING, STOPPING, SUSPENDING, SUSPENDED, REPAIRING, and TERMINATED. For more information about the status of the instance, see Instance life cycle.
                 Enum type. Allowed values:
                 "DEPROVISIONING" - The Nanny is halted and we are performing tear down tasks like network deprogramming, releasing quota, IP, tearing down disks etc.
                 "PROVISIONING" - Resources are being allocated for the instance.
@@ -610,587 +597,474 @@
                 "STAGING" - All required resources have been allocated and the instance is being started.
                 "STOPPED" - The instance has stopped successfully.
                 "STOPPING" - The instance is currently stopping (either being deleted or killed).
                 "SUSPENDED" - The instance has suspended.
                 "SUSPENDING" - The instance is suspending.
                 "TERMINATED" - The instance has stopped (either by explicit action or underlying failure). Defaults to None.
 
-        tags(Dict[str, Any], optional):
+        tags(Dict[str, Any], Optional):
             Tags to apply to this instance. Tags are used to identify valid sources or targets for network firewalls and are specified by the client during instance creation. The tags can be later modified by the setTags method. Each tag within the list must comply with RFC1035. Multiple tags can be specified via the 'tags.items' field.
-                Tags: A set of instance tags. Defaults to None.
+            Tags: A set of instance tags. Defaults to None.
 
-                * fingerprint (str, optional):
-                    Specifies a fingerprint for this request, which is essentially a hash of the tags' contents and used for optimistic locking. The fingerprint is initially generated by Compute Engine and changes after every request to modify or update tags. You must always provide an up-to-date fingerprint hash in order to update or change tags. To see the latest fingerprint, make get() request to the instance.
+            * fingerprint (str, Optional):
+                Specifies a fingerprint for this request, which is essentially a hash of the tags' contents and used for optimistic locking. The fingerprint is initially generated by Compute Engine and changes after every request to modify or update tags. You must always provide an up-to-date fingerprint hash in order to update or change tags. To see the latest fingerprint, make get() request to the instance.
+            * items (List[str], Optional):
+                An array of tags. Each tag must be 1-63 characters long, and comply with RFC1035.
 
-                * items (List[str], optional):
-                    An array of tags. Each tag must be 1-63 characters long, and comply with RFC1035.
-
-        key_revocation_action_type(str, optional):
+        key_revocation_action_type(str, Optional):
             KeyRevocationActionType of the instance. Supported options are "STOP" and "NONE". The default value is "NONE" if it is not specified.
                 Enum type. Allowed values:
                 "KEY_REVOCATION_ACTION_TYPE_UNSPECIFIED" - Default value. This value is unused.
                 "NONE" - Indicates user chose no operation.
                 "STOP" - Indicates user chose to opt for VM shutdown on key revocation. Defaults to None.
 
-        scheduling(Dict[str, Any], optional):
+        scheduling(Dict[str, Any], Optional):
             Sets the scheduling options for this instance.
-                Scheduling: Sets the scheduling options for an Instance. Defaults to None.
-
-                * on_host_maintenance (str, optional):
-                    Defines the maintenance behavior for this instance. For standard instances, the default behavior is MIGRATE. For preemptible instances, the default and only possible behavior is TERMINATE. For more information, see Set VM host maintenance policy.
-                        Enum type. Allowed values:
-                        "MIGRATE" - *[Default]* Allows Compute Engine to automatically migrate instances out of the way of maintenance events.
-                        "TERMINATE" - Tells Compute Engine to terminate and (optionally) restart the instance away from the maintenance activity. If you would like your instance to be restarted, set the automaticRestart flag to true. Your instance may be restarted more than once, and it may be restarted outside the window of maintenance events.
-
-                * preemptible (bool, optional):
-                    Defines whether the instance is preemptible. This can only be set during instance creation or while the instance is stopped and therefore, in a `TERMINATED` state. See Instance Life Cycle for more information on the possible instance states.
-
-                * min_node_cpus (int, optional):
-                    The minimum number of virtual CPUs this instance will consume when running on a sole-tenant node.
-
-                * automatic_restart (bool, optional):
-                    Specifies whether the instance should be automatically restarted if it is terminated by Compute Engine (not terminated by a user). You can only set the automatic restart option for standard instances. Preemptible instances cannot be automatically restarted. By default, this is set to true so an instance is automatically restarted if it is terminated by Compute Engine.
+            Scheduling: Sets the scheduling options for an Instance. Defaults to None.
 
-                * node_affinities (List[Dict[str, Any]], optional):
-                    A set of node affinity and anti-affinity configurations. Refer to Configuring node affinity for more information. Overrides reservationAffinity.
-
-                    * operator (str, optional):
-                        Defines the operation of node selection. Valid operators are IN for affinity and NOT_IN for anti-affinity.
-                            Enum type. Allowed values:
-                            "IN" - Requires Compute Engine to seek for matched nodes.
-                            "NOT_IN" - Requires Compute Engine to avoid certain nodes.
-                            "OPERATOR_UNSPECIFIED"
-
-                    * values (List[str], optional):
-                        Corresponds to the label values of Node resource.
-
-                    * key (str, optional):
-                        Corresponds to the label key of Node resource.
-
-                * instance_termination_action (str, optional):
-                    Specifies the termination action for the instance.
-                        Enum type. Allowed values:
-                        "DELETE" - Delete the VM.
-                        "INSTANCE_TERMINATION_ACTION_UNSPECIFIED" - Default value. This value is unused.
-                        "STOP" - Stop the VM without storing in-memory content. default action.
+            * on_host_maintenance (str, Optional):
+                Defines the maintenance behavior for this instance. For standard instances, the default behavior is MIGRATE. For preemptible instances, the default and only possible behavior is TERMINATE. For more information, see Set VM host maintenance policy.
+                    Enum type. Allowed values:
+                    "MIGRATE" - *[Default]* Allows Compute Engine to automatically migrate instances out of the way of maintenance events.
+                    "TERMINATE" - Tells Compute Engine to terminate and (optionally) restart the instance away from the maintenance activity. If you would like your instance to be restarted, set the automaticRestart flag to true. Your instance may be restarted more than once, and it may be restarted outside the window of maintenance events.
+            * preemptible (bool, Optional):
+                Defines whether the instance is preemptible. This can only be set during instance creation or while the instance is stopped and therefore, in a `TERMINATED` state. See Instance Life Cycle for more information on the possible instance states.
+            * min_node_cpus (int, Optional):
+                The minimum number of virtual CPUs this instance will consume when running on a sole-tenant node.
+            * automatic_restart (bool, Optional):
+                Specifies whether the instance should be automatically restarted if it is terminated by Compute Engine (not terminated by a user). You can only set the automatic restart option for standard instances. Preemptible instances cannot be automatically restarted. By default, this is set to true so an instance is automatically restarted if it is terminated by Compute Engine.
+            * node_affinities (List[Dict[str, Any]], Optional):
+                A set of node affinity and anti-affinity configurations. Refer to Configuring node affinity for more information. Overrides reservationAffinity.
 
-                * provisioning_model (str, optional):
-                    Specifies the provisioning model of the instance.
+                * operator (str, Optional):
+                    Defines the operation of node selection. Valid operators are IN for affinity and NOT_IN for anti-affinity.
                         Enum type. Allowed values:
-                        "SPOT" - Heavily discounted, no guaranteed runtime.
-                        "STANDARD" - Standard provisioning with user controlled runtime, no discounts.
+                        "IN" - Requires Compute Engine to seek for matched nodes.
+                        "NOT_IN" - Requires Compute Engine to avoid certain nodes.
+                        "OPERATOR_UNSPECIFIED"
+                * values (List[str], Optional):
+                    Corresponds to the label values of Node resource.
+                * key (str, Optional):
+                    Corresponds to the label key of Node resource.
 
-                * location_hint (str, optional):
-                    An opaque location hint used to place the instance close to other resources. This field is for use by internal tools that use the public API.
+            * instance_termination_action (str, Optional):
+                Specifies the termination action for the instance.
+                    Enum type. Allowed values:
+                    "DELETE" - Delete the VM.
+                    "INSTANCE_TERMINATION_ACTION_UNSPECIFIED" - Default value. This value is unused.
+                    "STOP" - Stop the VM without storing in-memory content. default action.
+            * provisioning_model (str, Optional):
+                Specifies the provisioning model of the instance.
+                    Enum type. Allowed values:
+                    "SPOT" - Heavily discounted, no guaranteed runtime.
+                    "STANDARD" - Standard provisioning with user controlled runtime, no discounts.
+            * location_hint (str, Optional):
+                An opaque location hint used to place the instance close to other resources. This field is for use by internal tools that use the public API.
 
-        private_ipv6_google_access(str, optional):
+        private_ipv6_google_access(str, Optional):
             The private IPv6 google access type for the VM. If not specified, use INHERIT_FROM_SUBNETWORK as default.
                 Enum type. Allowed values:
                 "ENABLE_BIDIRECTIONAL_ACCESS_TO_GOOGLE" - Bidirectional private IPv6 access to/from Google services. If specified, the subnetwork who is attached to the instance's default network interface will be assigned an internal IPv6 prefix if it doesn't have before.
                 "ENABLE_OUTBOUND_VM_ACCESS_TO_GOOGLE" - Outbound private IPv6 access from VMs in this subnet to Google services. If specified, the subnetwork who is attached to the instance's default network interface will be assigned an internal IPv6 prefix if it doesn't have before.
                 "INHERIT_FROM_SUBNETWORK" - Each network interface inherits PrivateIpv6GoogleAccess from its subnetwork. Defaults to None.
 
-        description(str, optional):
+        description(str, Optional):
             An optional description of this resource. Provide this property when you create the resource. Defaults to None.
 
-        guest_accelerators(List[Dict[str, Any]], optional):
+        guest_accelerators(List[Dict[str, Any]], Optional):
             A list of the type and count of accelerator cards attached to the instance. Defaults to None.
 
-                * accelerator_count (int, optional):
-                    The number of the guest accelerator cards exposed to this instance.
+            * accelerator_count (int, Optional):
+                The number of the guest accelerator cards exposed to this instance.
+            * accelerator_type (str, Optional):
+                Full or partial URL of the accelerator type resource to attach to this instance. For example: projects/my-project/zones/us-central1-c/acceleratorTypes/nvidia-tesla-p100 If you are creating an instance template, specify only the accelerator name. See GPUs on Compute Engine for a full list of accelerator types.
 
-                * accelerator_type (str, optional):
-                    Full or partial URL of the accelerator type resource to attach to this instance. For example: projects/my-project/zones/us-central1-c/acceleratorTypes/nvidia-tesla-p100 If you are creating an instance template, specify only the accelerator name. See GPUs on Compute Engine for a full list of accelerator types.
-
-        confidential_instance_config(Dict[str, Any], optional):
+        confidential_instance_config(Dict[str, Any], Optional):
             ConfidentialInstanceConfig: A set of Confidential Instance options. Defaults to None.
 
-            * enable_confidential_compute (bool, optional):
+            * enable_confidential_compute (bool, Optional):
                 Defines whether the instance should have confidential compute enabled.
 
-        shielded_instance_config(Dict[str, Any], optional):
+        shielded_instance_config(Dict[str, Any], Optional):
             ShieldedInstanceConfig: A set of Shielded Instance options. Defaults to None.
 
-                * enable_vtpm (bool, optional):
-                    Defines whether the instance has the vTPM enabled. Enabled by default.
+            * enable_vtpm (bool, Optional):
+                Defines whether the instance has the vTPM enabled. Enabled by default.
+            * enable_secure_boot (bool, Optional):
+                Defines whether the instance has Secure Boot enabled. Disabled by default.
+            * enable_integrity_monitoring (bool, Optional):
+                Defines whether the instance has integrity monitoring enabled. Enabled by default.
 
-                * enable_secure_boot (bool, optional):
-                    Defines whether the instance has Secure Boot enabled. Disabled by default.
+        source_machine_image_encryption_key(Dict[str, Any], Optional):
+            Source machine image encryption key when creating an instance from a machine image. Defaults to None.
 
-                * enable_integrity_monitoring (bool, optional):
-                    Defines whether the instance has integrity monitoring enabled. Enabled by default.
+            * kms_key_service_account (str, Optional):
+                The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/"
+            * sha256 (str, Optional):
+                [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
+            * rsa_encrypted_key (str, Optional):
+                Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+            * kms_key_name (str, Optional):
+                The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+            * raw_key (str, Optional):
+                Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
 
-        source_machine_image_encryption_key(Dict[str, Any], optional):
-            Source machine image encryption key when creating an instance from a machine image. Defaults to None.
+        disks(List[Dict[str, Any]], Optional):
+            Array of disks associated with this instance. Persistent disks must be created before you can assign them. Defaults to None.
 
-                * kms_key_service_account (str, optional):
-                    The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/
+            * disk_size_gb (str, Optional):
+                The size of the disk in GB.
+            * auto_delete (bool, Optional):
+                Specifies whether the disk will be auto-deleted when the instance is deleted (but not when the disk is detached from the instance).
+            * boot (bool, Optional):
+                Indicates that this is a boot disk. The virtual machine will use the first partition of the disk for its root filesystem.
+            * guest_os_features (List[Dict[str, Any]], Optional):
+                A list of features to enable on the guest operating system. Applicable only for bootable images. Read Enabling guest operating system features to see a list of available options.
 
-                * sha256 (str, optional):
+                * type (str, Optional):
+                    The ID of a supported feature. To add multiple values, use commas to separate values. Set to one or more of the following values: - VIRTIO_SCSI_MULTIQUEUE - WINDOWS - MULTI_IP_SUBNET - UEFI_COMPATIBLE - GVNIC - SEV_CAPABLE - SUSPEND_RESUME_COMPATIBLE - SEV_SNP_CAPABLE For more information, see Enabling guest operating system features.
+                        Enum type. Allowed values:
+                        "FEATURE_TYPE_UNSPECIFIED"
+                        "GVNIC"
+                        "MULTI_IP_SUBNET"
+                        "SECURE_BOOT"
+                        "SEV_CAPABLE"
+                        "UEFI_COMPATIBLE"
+                        "VIRTIO_SCSI_MULTIQUEUE"
+                        "WINDOWS"
+            * source (str, Optional):
+                Specifies a valid partial or full URL to an existing Persistent Disk resource. When creating a new instance, one of initializeParams.sourceImage or initializeParams.sourceSnapshot or disks.source is required except for local SSD. If desired, you can also attach existing non-root persistent disks using this property. This field is only applicable for persistent disks. Note that for InstanceTemplate, specify the disk name for zonal disk, and the URL for regional disk.
+            * disk_encryption_key (Dict[str, Any], Optional):
+                Encrypts or decrypts a disk using a customer-supplied encryption key. If you are creating a new disk, this field encrypts the new disk using an encryption key that you provide. If you are attaching an existing disk that is already encrypted, this field decrypts the disk using the customer-supplied encryption key. If you encrypt a disk using a customer-supplied key, you must provide the same key again when you attempt to use this resource at a later time. For example, you must provide the key when you create a snapshot or an image from the disk or when you attach the disk to a virtual machine instance. If you do not provide an encryption key, then the disk will be encrypted using an automatically generated key and you do not need to provide a key to use the disk later. Instance templates do not store customer-supplied encryption keys, so you cannot use your own keys to encrypt disks in a managed instance group.
+
+                * kms_key_service_account (str, Optional):
+                    The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/"
+                * sha256 (str, Optional):
                     [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
-
-                * rsa_encrypted_key (str, optional):
+                * rsa_encrypted_key (str, Optional):
                     Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
-
-                * kms_key_name (str, optional):
+                * kms_key_name (str, Optional):
                     The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
-
-                * raw_key (str, optional):
+                * raw_key (str, Optional):
                     Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
+            * force_attach (bool, Optional):
+                [Input Only] Whether to force attach the regional disk even if it's currently attached to another instance. If you try to force attach a zonal disk to an instance, you will receive an error.
+            * architecture (str, Optional):
+                [Output Only] The architecture of the attached disk. Valid values are ARM64 or X86_64.
+                    Enum type. Allowed values:
+                    "ARCHITECTURE_UNSPECIFIED" - Default value indicating Architecture is not set.
+                    "ARM64" - Machines with architecture ARM64
+                    "X86_64" - Machines with architecture X86_64
+            * device_name (str, Optional):
+                Specifies a unique device name of your choice that is reflected into the /dev/disk/by-id/google-* tree of a Linux operating system running within the instance. This name can be used to reference the device for mounting, resizing, and so on, from within the instance. If not specified, the server chooses a default device name to apply to this disk, in the form persistent-disk-x, where x is a number assigned by Google Compute Engine. This field is only applicable for persistent disks.
+            * shielded_instance_initial_state (Dict[str, Any], Optional):
+                [Output Only] shielded vm initial state stored on disk.
+                InitialStateConfig: Initial State for shielded instance, these are public keys which are safe to store in public
 
-        disks(List[Dict[str, Any]], optional):
-            Array of disks associated with this instance. Persistent disks must be created before you can assign them. Defaults to None.
-
-                * disk_size_gb (str, optional):
-                    The size of the disk in GB.
-
-                * auto_delete (bool, optional):
-                    Specifies whether the disk will be auto-deleted when the instance is deleted (but not when the disk is detached from the instance).
-
-                * boot (bool, optional):
-                    Indicates that this is a boot disk. The virtual machine will use the first partition of the disk for its root filesystem.
-
-                * guest_os_features (List[Dict[str, Any]], optional):
-                    A list of features to enable on the guest operating system. Applicable only for bootable images. Read Enabling guest operating system features to see a list of available options.
-
-                        * type_ (str, optional):
-                            The ID of a supported feature. To add multiple values, use commas to separate values. Set to one or more of the following values: - VIRTIO_SCSI_MULTIQUEUE - WINDOWS - MULTI_IP_SUBNET - UEFI_COMPATIBLE - GVNIC - SEV_CAPABLE - SUSPEND_RESUME_COMPATIBLE - SEV_SNP_CAPABLE For more information, see Enabling guest operating system features.
-                                Enum type. Allowed values:
-                                "FEATURE_TYPE_UNSPECIFIED"
-                                "GVNIC"
-                                "MULTI_IP_SUBNET"
-                                "SECURE_BOOT"
-                                "SEV_CAPABLE"
-                                "UEFI_COMPATIBLE"
-                                "VIRTIO_SCSI_MULTIQUEUE"
-                                "WINDOWS"
-
-                * source (str, optional):
-                    Specifies a valid partial or full URL to an existing Persistent Disk resource. When creating a new instance, one of initializeParams.sourceImage or initializeParams.sourceSnapshot or disks.source is required except for local SSD. If desired, you can also attach existing non-root persistent disks using this property. This field is only applicable for persistent disks. Note that for InstanceTemplate, specify the disk name for zonal disk, and the URL for regional disk.
-
-                * disk_encryption_key (Dict[str, Any], optional):
-                    Encrypts or decrypts a disk using a customer-supplied encryption key. If you are creating a new disk, this field encrypts the new disk using an encryption key that you provide. If you are attaching an existing disk that is already encrypted, this field decrypts the disk using the customer-supplied encryption key. If you encrypt a disk using a customer-supplied key, you must provide the same key again when you attempt to use this resource at a later time. For example, you must provide the key when you create a snapshot or an image from the disk or when you attach the disk to a virtual machine instance. If you do not provide an encryption key, then the disk will be encrypted using an automatically generated key and you do not need to provide a key to use the disk later. Instance templates do not store customer-supplied encryption keys, so you cannot use your own keys to encrypt disks in a managed instance group.
-
-                        * kms_key_service_account (str, optional):
-                            The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/
+                * keks (List[Dict[str, Any]], Optional):
+                    The Key Exchange Key (KEK).
 
-                        * sha256 (str, optional):
-                            [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
+                    * file_type (str, Optional):
+                        The file type of source file.
+                            Enum type. Allowed values:
+                            "BIN"
+                            "UNDEFINED"
+                            "X509"
+                    * content (str, Optional):
+                        The raw content in the secure keys file.
+                * dbs (List[Dict[str, Any]], Optional):
+                    The Key Database (db).
 
-                        * rsa_encrypted_key (str, optional):
-                            Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+                    * file_type (str, Optional):
+                        The file type of source file.
+                            Enum type. Allowed values:
+                            "BIN"
+                            "UNDEFINED"
+                            "X509"
+                    * content (str, Optional):
+                        The raw content in the secure keys file.
 
-                        * kms_key_name (str, optional):
-                            The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+                * dbxs (List[Dict[str, Any]], Optional):
+                    The forbidden key database (dbx).
 
-                        * raw_key (str, optional):
-                            Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
+                    * file_type (str, Optional):
+                        The file type of source file.
+                            Enum type. Allowed values:
+                            "BIN"
+                            "UNDEFINED"
+                            "X509"
+                    * content (str, Optional):
+                        The raw content in the secure keys file.
+                * pk (Dict[str, Any], Optional):
+                    The Platform Key (PK).
 
-                * force_attach (bool, optional):
-                    [Input Only] Whether to force attach the regional disk even if it's currently attached to another instance. If you try to force attach a zonal disk to an instance, you will receive an error.
+                    * file_type (str, Optional):
+                        The file type of source file.
+                            Enum type. Allowed values:
+                            "BIN"
+                            "UNDEFINED"
+                            "X509"
+                    * content (str, Optional):
+                        The raw content in the secure keys file.
+            * initialize_params (Dict[str, Any], Optional):
+                [Input Only] Specifies the parameters for a new disk that will be created alongside the new instance. Use initialization parameters to create boot disks or local SSDs attached to the new instance. This property is mutually exclusive with the source property; you can only define one or the other, but not both.
+                AttachedDiskInitializeParams: [Input Only] Specifies the parameters for a new disk that will be created alongside the new instance. Use initialization parameters to create boot disks or local SSDs attached to the new instance. This field is persisted and returned for instanceTemplate and not returned in the context of instance. This property is mutually exclusive with the source property; you can only define one or the other, but not both.
+
+                * resource_manager_tags (Dict[str, Any], Optional):
+                    Resource manager tags to be bound to the disk. Tag keys and values have the same definition as resource manager tags. Keys must be in the format `tagKeys/{tag_key_id}`, and values are in the format `tagValues/456`. The field is ignored (both PUT & PATCH) when empty.
+                * source_image (str, Optional):
+                    The source image to create this disk. When creating a new instance, one of initializeParams.sourceImage or initializeParams.sourceSnapshot or disks.source is required except for local SSD. To create a disk with one of the public operating system images, specify the image by its family name. For example, specify family/debian-9 to use the latest Debian 9 image: projects/debian-cloud/global/images/family/debian-9 Alternatively, use a specific version of a public operating system image: projects/debian-cloud/global/images/debian-9-stretch-vYYYYMMDD To create a disk with a custom image that you created, specify the image name in the following format: global/images/my-custom-image You can also specify a custom image by its image family, which returns the latest version of the image in that family. Replace the image name with family/family-name: global/images/family/my-image-family If the source image is deleted later, this field will not be set.
+                * description (str, Optional):
+                    An optional description. Provide this property when creating the disk.
+                * disk_size_gb (str, Optional):
+                    Specifies the size of the disk in base-2 GB. The size must be at least 10 GB. If you specify a sourceImage, which is required for boot disks, the default size is the size of the sourceImage. If you do not specify a sourceImage, the default disk size is 500 GB.
+                * source_snapshot (str, Optional):
+                    The source snapshot to create this disk. When creating a new instance, one of initializeParams.sourceSnapshot or initializeParams.sourceImage or disks.source is required except for local SSD. To create a disk with a snapshot that you created, specify the snapshot name in the following format: global/snapshots/my-backup If the source snapshot is deleted later, this field will not be set.
+                * provisioned_iops (str, Optional):
+                    Indicates how many IOPS to provision for the disk. This sets the number of I/O operations per second that the disk can handle. Values must be between 10,000 and 120,000. For more details, see the Extreme persistent disk documentation.
+                * source_image_encryption_key (Dict[str, Any], Optional):
+                    The customer-supplied encryption key of the source image. Required if the source image is protected by a customer-supplied encryption key. InstanceTemplate and InstancePropertiesPatch do not store customer-supplied encryption keys, so you cannot create disks for instances in a managed instance group if the source images are encrypted with your own keys.
+
+                    * kms_key_service_account (str, Optional):
+                        The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/"
+                    * sha256 (str, Optional):
+                        [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
+                    * rsa_encrypted_key (str, Optional):
+                        Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+                    * kms_key_name (str, Optional):
+                        The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+                    * raw_key (str, Optional):
+                        Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
+                * on_update_action (str, Optional):
+                    Specifies which action to take on instance update with this disk. Default is to use the existing disk.
+                        Enum type. Allowed values:
+                        "RECREATE_DISK" - Always recreate the disk.
+                        "RECREATE_DISK_IF_SOURCE_CHANGED" - Recreate the disk if source (image, snapshot) of this disk is different from source of existing disk.
+                        "USE_EXISTING_DISK" - Use the existing disk, this is the default behaviour.
+                * source_snapshot_encryption_key (Dict[str, Any], Optional):
+                    The customer-supplied encryption key of the source snapshot.
+
+                    * kms_key_service_account (str, Optional):
+                        The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/"
+                    * sha256 (str, Optional):
+                        [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
+                    * rsa_encrypted_key (str, Optional):
+                        Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+                    * kms_key_name (str, Optional):
+                        The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+                    * raw_key (str, Optional):
+                        Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
 
-                * architecture (str, optional):
-                    [Output Only] The architecture of the attached disk. Valid values are ARM64 or X86_64.
+                * architecture (str, Optional):
+                    The architecture of the attached disk. Valid values are arm64 or x86_64.
                         Enum type. Allowed values:
                         "ARCHITECTURE_UNSPECIFIED" - Default value indicating Architecture is not set.
                         "ARM64" - Machines with architecture ARM64
                         "X86_64" - Machines with architecture X86_64
+                * licenses (List[str], Optional):
+                    A list of publicly visible licenses. Reserved for Google's use.
+                * labels (Dict[str, Any], Optional):
+                    Labels to apply to this disk. These can be later modified by the disks.setLabels method. This field is only applicable for persistent disks.
+                * disk_type (str, Optional):
+                    Specifies the disk type to use to create the instance. If not specified, the default is pd-standard, specified using the full URL. For example: https://www.googleapis.com/compute/v1/projects/project/zones/zone/diskTypes/pd-standard For a full list of acceptable values, see Persistent disk types. If you specify this field when creating a VM, you can provide either the full or partial URL. For example, the following values are valid: - https://www.googleapis.com/compute/v1/projects/project/zones/zone /diskTypes/diskType - projects/project/zones/zone/diskTypes/diskType - zones/zone/diskTypes/diskType If you specify this field when creating or updating an instance template or all-instances configuration, specify the type of the disk, not the URL. For example: pd-standard.
+                * disk_name (str, Optional):
+                    Specifies the disk name. If not specified, the default is to use the name of the instance. If a disk with the same name already exists in the given region, the existing disk is attached to the new instance and the new disk is not created.
+                * resource_policies (List[str], Optional):
+                    Resource policies applied to this disk for automatic snapshot creations. Specified using the full or partial URL. For instance template, specify only the resource policy name.
+
+            * kind (str, Optional):
+                [Output Only] Type of the resource. Always compute#attachedDisk for attached disks.
+            * index (int, Optional):
+                [Output Only] A zero-based index to this disk, where 0 is reserved for the boot disk. If you have many disks attached to an instance, each disk would have a unique index number.
+            * interface (str, Optional):
+                Specifies the disk interface to use for attaching this disk, which is either SCSI or NVME. For most machine types, the default is SCSI. Local SSDs can use either NVME or SCSI. In certain configurations, persistent disks can use NVMe. For more information, see About persistent disks.
+                    Enum type. Allowed values:
+                    "NVME"
+                    "SCSI"
+            * licenses (List[str], Optional):
+                [Output Only] Any valid publicly visible licenses.
+            * mode (str, Optional):
+                The mode in which to attach this disk, either READ_WRITE or READ_ONLY. If not specified, the default is to attach the disk in READ_WRITE mode.
+                    Enum type. Allowed values:
+                    "READ_ONLY" - Attaches this disk in read-only mode. Multiple virtual machines can use a disk in read-only mode at a time.
+                    "READ_WRITE" - *[Default]* Attaches this disk in read-write mode. Only one virtual machine at a time can be attached to a disk in read-write mode.
+            * type (str, Optional):
+                Specifies the type of the disk, either SCRATCH or PERSISTENT. If not specified, the default is PERSISTENT.
+                    Enum type. Allowed values:
+                    "PERSISTENT"
+                    "SCRATCH"
 
-                * device_name (str, optional):
-                    Specifies a unique device name of your choice that is reflected into the /dev/disk/by-id/google-* tree of a Linux operating system running within the instance. This name can be used to reference the device for mounting, resizing, and so on, from within the instance. If not specified, the server chooses a default device name to apply to this disk, in the form persistent-disk-x, where x is a number assigned by Google Compute Engine. This field is only applicable for persistent disks.
-
-                * shielded_instance_initial_state (Dict[str, Any], optional):
-                    [Output Only] shielded vm initial state stored on disk
-                        InitialStateConfig: Initial State for shielded instance, these are public keys which are safe to store in public
-
-                        * keks (List[Dict[str, Any]], optional):
-                            The Key Exchange Key (KEK).
-
-                                * file_type (str, optional):
-                                    The file type of source file.
-                                        Enum type. Allowed values:
-                                        "BIN"
-                                        "UNDEFINED"
-                                        "X509"
-
-                                * content (str, optional):
-                                    The raw content in the secure keys file.
-
-                        * dbs (List[Dict[str, Any]], optional):
-                            The Key Database (db).
-
-                                * file_type (str, optional):
-                                    The file type of source file.
-                                        Enum type. Allowed values:
-                                        "BIN"
-                                        "UNDEFINED"
-                                        "X509"
-
-                                * content (str, optional):
-                                    The raw content in the secure keys file.
-
-                        * dbxs (List[Dict[str, Any]], optional):
-                            The forbidden key database (dbx).
-
-                                * file_type (str, optional):
-                                    The file type of source file.
-                                        Enum type. Allowed values:
-                                        "BIN"
-                                        "UNDEFINED"
-                                        "X509"
-
-                                * content (str, optional):
-                                    The raw content in the secure keys file.
-
-                        * pk (Dict[str, Any], optional):
-                            The Platform Key (PK).
-
-                                * file_type (str, optional):
-                                    The file type of source file.
-                                        Enum type. Allowed values:
-                                        "BIN"
-                                        "UNDEFINED"
-                                        "X509"
-
-                                * content (str, optional):
-                                    The raw content in the secure keys file.
-
-                * initialize_params (Dict[str, Any], optional):
-                    [Input Only] Specifies the parameters for a new disk that will be created alongside the new instance. Use initialization parameters to create boot disks or local SSDs attached to the new instance. This property is mutually exclusive with the source property; you can only define one or the other, but not both.
-                        AttachedDiskInitializeParams: [Input Only] Specifies the parameters for a new disk that will be created alongside the new instance. Use initialization parameters to create boot disks or local SSDs attached to the new instance. This field is persisted and returned for instanceTemplate and not returned in the context of instance. This property is mutually exclusive with the source property; you can only define one or the other, but not both.
-
-                        * resource_manager_tags (Dict[str, Any], optional):
-                            Resource manager tags to be bound to the disk. Tag keys and values have the same definition as resource manager tags. Keys must be in the format `tagKeys/{tag_key_id}`, and values are in the format `tagValues/456`. The field is ignored (both PUT & PATCH) when empty.
-
-                        * source_image (str, optional):
-                            The source image to create this disk. When creating a new instance, one of initializeParams.sourceImage or initializeParams.sourceSnapshot or disks.source is required except for local SSD. To create a disk with one of the public operating system images, specify the image by its family name. For example, specify family/debian-9 to use the latest Debian 9 image: projects/debian-cloud/global/images/family/debian-9 Alternatively, use a specific version of a public operating system image: projects/debian-cloud/global/images/debian-9-stretch-vYYYYMMDD To create a disk with a custom image that you created, specify the image name in the following format: global/images/my-custom-image You can also specify a custom image by its image family, which returns the latest version of the image in that family. Replace the image name with family/family-name: global/images/family/my-image-family If the source image is deleted later, this field will not be set.
-
-                        * description (str, optional):
-                            An optional description. Provide this property when creating the disk.
-
-                        * disk_size_gb (str, optional):
-                            Specifies the size of the disk in base-2 GB. The size must be at least 10 GB. If you specify a sourceImage, which is required for boot disks, the default size is the size of the sourceImage. If you do not specify a sourceImage, the default disk size is 500 GB.
-
-                        * source_snapshot (str, optional):
-                            The source snapshot to create this disk. When creating a new instance, one of initializeParams.sourceSnapshot or initializeParams.sourceImage or disks.source is required except for local SSD. To create a disk with a snapshot that you created, specify the snapshot name in the following format: global/snapshots/my-backup If the source snapshot is deleted later, this field will not be set.
-
-                        * provisioned_iops (str, optional):
-                            Indicates how many IOPS to provision for the disk. This sets the number of I/O operations per second that the disk can handle. Values must be between 10,000 and 120,000. For more details, see the Extreme persistent disk documentation.
-
-                        * source_image_encryption_key (Dict[str, Any], optional):
-                            The customer-supplied encryption key of the source image. Required if the source image is protected by a customer-supplied encryption key. InstanceTemplate and InstancePropertiesPatch do not store customer-supplied encryption keys, so you cannot create disks for instances in a managed instance group if the source images are encrypted with your own keys.
-
-                                * kms_key_service_account (str, optional):
-                                    The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/
-
-                                * sha256 (str, optional):
-                                    [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
-
-                                * rsa_encrypted_key (str, optional):
-                                    Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
-
-                                * kms_key_name (str, optional):
-                                    The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
-
-                                * raw_key (str, optional):
-                                    Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
-
-                        * on_update_action (str, optional):
-                            Specifies which action to take on instance update with this disk. Default is to use the existing disk.
-                                Enum type. Allowed values:
-                                "RECREATE_DISK" - Always recreate the disk.
-                                "RECREATE_DISK_IF_SOURCE_CHANGED" - Recreate the disk if source (image, snapshot) of this disk is different from source of existing disk.
-                                "USE_EXISTING_DISK" - Use the existing disk, this is the default behaviour.
-
-                        * source_snapshot_encryption_key (Dict[str, Any], optional):
-                            The customer-supplied encryption key of the source snapshot.
-
-                                * kms_key_service_account (str, optional):
-                                    The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/
-
-                                * sha256 (str, optional):
-                                    [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
-
-                                * rsa_encrypted_key (str, optional):
-                                    Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
-
-                                * kms_key_name (str, optional):
-                                    The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
-
-                                * raw_key (str, optional):
-                                    Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
-
-                        * architecture (str, optional):
-                            The architecture of the attached disk. Valid values are arm64 or x86_64.
-                                Enum type. Allowed values:
-                                "ARCHITECTURE_UNSPECIFIED" - Default value indicating Architecture is not set.
-                                "ARM64" - Machines with architecture ARM64
-                                "X86_64" - Machines with architecture X86_64
-
-                        * licenses (List[str], optional):
-                            A list of publicly visible licenses. Reserved for Google's use.
-
-                        * labels (Dict[str, Any], optional):
-                            Labels to apply to this disk. These can be later modified by the disks.setLabels method. This field is only applicable for persistent disks.
-
-                        * disk_type (str, optional):
-                            Specifies the disk type to use to create the instance. If not specified, the default is pd-standard, specified using the full URL. For example: https://www.googleapis.com/compute/v1/projects/project/zones/zone /diskTypes/pd-standard For a full list of acceptable values, see Persistent disk types. If you specify this field when creating a VM, you can provide either the full or partial URL. For example, the following values are valid: - https://www.googleapis.com/compute/v1/projects/project/zones/zone /diskTypes/diskType - projects/project/zones/zone/diskTypes/diskType - zones/zone/diskTypes/diskType If you specify this field when creating or updating an instance template or all-instances configuration, specify the type of the disk, not the URL. For example: pd-standard.
-
-                        * disk_name (str, optional):
-                            Specifies the disk name. If not specified, the default is to use the name of the instance. If a disk with the same name already exists in the given region, the existing disk is attached to the new instance and the new disk is not created.
-
-                        * resource_policies (List[str], optional):
-                            Resource policies applied to this disk for automatic snapshot creations. Specified using the full or partial URL. For instance template, specify only the resource policy name.
-
-                * kind (str, optional):
-                    [Output Only] Type of the resource. Always compute#attachedDisk for attached disks.
-
-                * index (int, optional):
-                    [Output Only] A zero-based index to this disk, where 0 is reserved for the boot disk. If you have many disks attached to an instance, each disk would have a unique index number.
-
-                * interface (str, optional):
-                    Specifies the disk interface to use for attaching this disk, which is either SCSI or NVME. For most machine types, the default is SCSI. Local SSDs can use either NVME or SCSI. In certain configurations, persistent disks can use NVMe. For more information, see About persistent disks.
-                        Enum type. Allowed values:
-                        "NVME"
-                        "SCSI"
-
-                * licenses (List[str], optional):
-                    [Output Only] Any valid publicly visible licenses.
-
-                * mode (str, optional):
-                    The mode in which to attach this disk, either READ_WRITE or READ_ONLY. If not specified, the default is to attach the disk in READ_WRITE mode.
-                        Enum type. Allowed values:
-                        "READ_ONLY" - Attaches this disk in read-only mode. Multiple virtual machines can use a disk in read-only mode at a time.
-                        "READ_WRITE" - *[Default]* Attaches this disk in read-write mode. Only one virtual machine at a time can be attached to a disk in read-write mode.
-
-                * type_ (str, optional):
-                    Specifies the type of the disk, either SCRATCH or PERSISTENT. If not specified, the default is PERSISTENT.
-                        Enum type. Allowed values:
-                        "PERSISTENT"
-                        "SCRATCH"
-
-        hostname(str, optional):
+        hostname(str, Optional):
             Specifies the hostname of the instance. The specified hostname must be RFC1035 compliant. If hostname is not specified, the default hostname is [INSTANCE_NAME].c.[PROJECT_ID].internal when using the global DNS, and [INSTANCE_NAME].[ZONE].c.[PROJECT_ID].internal when using zonal DNS. Defaults to None.
 
-        network_performance_config(Dict[str, Any], optional):
-            . Defaults to None.
+        network_performance_config(Dict[str, Any], Optional):
+            Defaults to None.
 
-                * total_egress_bandwidth_tier (str, optional):
-                    Enum type. Allowed values:
-                        "DEFAULT"
-                        "TIER_1"
+            * total_egress_bandwidth_tier (str, Optional):
+                Enum type. Allowed values:
+                "DEFAULT"
+                "TIER_1"
 
-        params(Dict[str, Any], optional):
+        params(Dict[str, Any], Optional):
             Input only. [Input Only] Additional params passed with the request, but not persisted as part of resource payload.
-                InstanceParams: Additional instance params. Defaults to None.
+            InstanceParams: Additional instance params. Defaults to None.
 
-                * resource_manager_tags (Dict[str, Any], optional):
-                    Resource manager tags to be bound to the instance. Tag keys and values have the same definition as resource manager tags. Keys must be in the format `tagKeys/{tag_key_id}`, and values are in the format `tagValues/456`. The field is ignored (both PUT & PATCH) when empty.
+            * resource_manager_tags (Dict[str, Any], Optional):
+                Resource manager tags to be bound to the instance. Tag keys and values have the same definition as resource manager tags. Keys must be in the format `tagKeys/{tag_key_id}`, and values are in the format `tagValues/456`. The field is ignored (both PUT & PATCH) when empty.
 
                 ResourceStatus: Contains output only fields. Use this sub-message for actual values set on Instance attributes as compared to the value requested by the user (intent) in their instance CRUD calls. Defaults to None.
-                * physical_host (str, optional):
-                    [Output Only] An opaque ID of the host on which the VM is running.
+            * physical_host (str, Optional):
+                [Output Only] An opaque ID of the host on which the VM is running.
 
-        deletion_protection(bool, optional):
+        deletion_protection(bool, Optional):
             Whether the resource should be protected against deletion. Defaults to None.
 
-        metadata(Dict[str, Any], optional):
+        metadata(Dict[str, Any], Optional):
             The metadata key/value pairs assigned to this instance. This includes custom metadata and predefined keys.
             Metadata: A metadata key/value entry. Defaults to None.
 
-                * items (List[Dict[str, Any]], optional):
-                    Array of key/value pairs. The total size of all keys and values must be less than 512 KB.
-
-                        * key (str, optional):
-                            Key for the metadata entry. Keys must conform to the following regexp: [a-zA-Z0-9-_]+, and be less than 128 bytes in length. This is reflected as part of a URL in the metadata server. Additionally, to avoid ambiguity, keys must not conflict with any other metadata keys for the project.
-
-                        * value (str, optional):
-                            Value for the metadata entry. These are free-form strings, and only have meaning as interpreted by the image running in the instance. The only restriction placed on values is that their size must be less than or equal to 262144 bytes (256 KiB).
+            * items (List[Dict[str, Any]], Optional):
+                Array of key/value pairs. The total size of all keys and values must be less than 512 KB.
 
-                * kind (str, optional):
-                    [Output Only] Type of the resource. Always compute#metadata for metadata.
-
-                * fingerprint (str, optional):
-                    Specifies a fingerprint for this request, which is essentially a hash of the metadata's contents and used for optimistic locking. The fingerprint is initially generated by Compute Engine and changes after every request to modify or update metadata. You must always provide an up-to-date fingerprint hash in order to update or change metadata, otherwise the request will fail with error 412 conditionNotMet. To see the latest fingerprint, make a get() request to retrieve the resource.
+                * key (str, Optional):
+                    Key for the metadata entry. Keys must conform to the following regexp: [a-zA-Z0-9-_]+, and be less than 128 bytes in length. This is reflected as part of a URL in the metadata server. Additionally, to avoid ambiguity, keys must not conflict with any other metadata keys for the project.
+                * value (str, Optional):
+                    Value for the metadata entry. These are free-form strings, and only have meaning as interpreted by the image running in the instance. The only restriction placed on values is that their size must be less than or equal to 262144 bytes (256 KiB).
+
+            * kind (str, Optional):
+                [Output Only] Type of the resource. Always compute#metadata for metadata.
+            * fingerprint (str, Optional):
+                Specifies a fingerprint for this request, which is essentially a hash of the metadata's contents and used for optimistic locking. The fingerprint is initially generated by Compute Engine and changes after every request to modify or update metadata. You must always provide an up-to-date fingerprint hash in order to update or change metadata, otherwise the request will fail with error 412 conditionNotMet. To see the latest fingerprint, make a get() request to retrieve the resource.
 
         zone(str):
             The name of the zone for this request.
 
-        shielded_instance_integrity_policy(Dict[str, Any], optional):
+        shielded_instance_integrity_policy(Dict[str, Any], Optional):
             ShieldedInstanceIntegrityPolicy: The policy describes the baseline against which Instance boot integrity is measured. Defaults to None.
 
-                * update_auto_learn_policy (bool, optional):
-                    Updates the integrity policy baseline using the measurements from the VM instance's most recent boot.
+            * update_auto_learn_policy (bool, Optional):
+                Updates the integrity policy baseline using the measurements from the VM instance's most recent boot.
 
-        reservation_affinity(Dict[str, Any], optional):
+        reservation_affinity(Dict[str, Any], Optional):
             Specifies the reservations that this instance can consume from.
             ReservationAffinity: Specifies the reservations that this instance can consume from. Defaults to None.
 
-                * key (str, optional):
-                    Corresponds to the label key of a reservation resource. To target a SPECIFIC_RESERVATION by name, specify googleapis.com/reservation-name as the key and specify the name of your reservation as its value.
-
-                * values (List[str], optional):
-                    Corresponds to the label values of a reservation resource. This can be either a name to a reservation in the same project or "projects/different-project/reservations/some-reservation-name" to target a shared reservation in the same zone but in a different project.
-
-                * consume_reservation_type (str, optional):
-                    Specifies the type of reservation from which this instance can consume resources: ANY_RESERVATION (default), SPECIFIC_RESERVATION, or NO_RESERVATION. See Consuming reserved instances for examples.
-                        Enum type. Allowed values:
-                        "ANY_RESERVATION" - Consume any allocation available.
-                        "NO_RESERVATION" - Do not consume from any allocated capacity.
-                        "SPECIFIC_RESERVATION" - Must consume from a specific reservation. Must specify key value fields for specifying the reservations.
-                        "UNSPECIFIED"
+            * key (str, Optional):
+                Corresponds to the label key of a reservation resource. To target a SPECIFIC_RESERVATION by name, specify googleapis.com/reservation-name as the key and specify the name of your reservation as its value.
+            * values (List[str], Optional):
+                Corresponds to the label values of a reservation resource. This can be either a name to a reservation in the same project or "projects/different-project/reservations/some-reservation-name" to target a shared reservation in the same zone but in a different project.
+            * consume_reservation_type (str, Optional):
+                Specifies the type of reservation from which this instance can consume resources: ANY_RESERVATION (default), SPECIFIC_RESERVATION, or NO_RESERVATION. See Consuming reserved instances for examples.
+                    Enum type. Allowed values:
+                    "ANY_RESERVATION" - Consume any allocation available.
+                    "NO_RESERVATION" - Do not consume from any allocated capacity.
+                    "SPECIFIC_RESERVATION" - Must consume from a specific reservation. Must specify key value fields for specifying the reservations.
+                    "UNSPECIFIED"
 
-        min_cpu_platform(str, optional):
+        min_cpu_platform(str, Optional):
             Specifies a minimum CPU platform for the VM instance. Applicable values are the friendly names of CPU platforms, such as minCpuPlatform: "Intel Haswell" or minCpuPlatform: "Intel Sandy Bridge". Defaults to None.
 
-        machine_type(str, optional):
+        machine_type(str, Optional):
             Full or partial URL of the machine type resource to use for this instance, in the format: zones/zone/machineTypes/machine-type. This is provided by the client when the instance is created. For example, the following is a valid partial url to a predefined machine type: zones/us-central1-f/machineTypes/n1-standard-1 To create a custom machine type, provide a URL to a machine type in the following format, where CPUS is 1 or an even number up to 32 (2, 4, 6, ... 24, etc), and MEMORY is the total memory for this instance. Memory must be a multiple of 256 MB and must be supplied in MB (e.g. 5 GB of memory is 5120 MB): zones/zone/machineTypes/custom-CPUS-MEMORY For example: zones/us-central1-f/machineTypes/custom-4-5120 For a full list of restrictions, read the Specifications for custom machine types. Defaults to None.
 
         project(str, Optional):
             Project ID for this request.
 
-        source_instance_template(str, optional):
-            Specifies instance template to create the instance. This field is optional. It can be a full or partial URL. For example, the following are all valid URLs to an instance template: - https://www.googleapis.com/compute/v1/projects/project /global/instanceTemplates/instanceTemplate - projects/project/global/instanceTemplates/instanceTemplate - global/instanceTemplates/instanceTemplate . Defaults to None.
+        source_instance_template(str, Optional):
+            Specifies instance template to create the instance. This field is optional. It can be a full or partial URL. For example, the following are all valid URLs to an instance template:
+
+            - https://www.googleapis.com/compute/v1/projects/project/global/instanceTemplates/instanceTemplate
+            - projects/project/global/instanceTemplates/instanceTemplate
+            - global/instanceTemplates/instanceTemplate
 
-        source_machine_image(str, optional):
-            Specifies the machine image to use to create the instance. This field is optional. It can be a full or partial URL. For example, the following are all valid URLs to a machine image: - https://www.googleapis.com/compute/v1/projects/project/global/global /machineImages/machineImage - projects/project/global/global/machineImages/machineImage - global/machineImages/machineImage . Defaults to None.
+            Defaults to None.
 
-        request_id(str, optional):
+        source_machine_image(str, Optional):
+            Specifies the machine image to use to create the instance. This field is optional. It can be a full or partial URL. Defaults to None. For example, the following are all valid URLs to a machine image:
+
+            - https://www.googleapis.com/compute/v1/projects/project/global/global/machineImages/machineImage
+            - projects/project/global/global/machineImages/machineImage
+            - global/machineImages/machineImage
+
+        request_id(str, Optional):
             An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
 
-        minimal_action(str, optional):
+        minimal_action(str, Optional):
             Specifies the action to take when updating an instance even if the updated properties do not require it. If not specified, then Compute Engine acts based on the minimum action that the updated properties require. Defaults to None.
 
-        most_disruptive_allowed_action(str, optional):
+        most_disruptive_allowed_action(str, Optional):
             Specifies the most disruptive action that can be taken on the instance as part of the update. Compute Engine returns an error if the instance properties require a more disruptive action as part of the instance update. Valid options from lowest to highest are NO_EFFECT, REFRESH, and RESTART. Defaults to None.
 
-        resource_id(str, optional):
+        resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
+        id(str, Optional):
+            The unique identifier for the resource. This identifier is defined by the server. Read-only property
+
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
-        example_resource_name:
-          gcp.compute.instance.present:
-          - project: example-project
-          - machine_type: https://www.googleapis.com/compute/v1/projects/example-project/zones/us-central1-a/machineTypes/g1-small
-          - zone: us-central1-a
-          - can_ip_forward: false
-          - network_interfaces:
-            - access_configs:
-              - kind: compute#accessConfig
-                name: External NAT
-                network_tier: PREMIUM
-                set_public_ptr: false
-                type: ONE_TO_ONE_NAT
-              kind: compute#networkInterface
-              name: nic0
-              network: https://www.googleapis.com/compute/v1/projects/project-name/global/networks/default
-              stack_type: IPV4_ONLY
-              subnetwork: https://www.googleapis.com/compute/v1/projects/project-name/regions/us-central1/subnetworks/default
-          - disks:
-            - auto_delete: true
-              boot: true
-              device_name: example_disk_1
-              source: https://www.googleapis.com/compute/v1/projects/project-name/zones/us-central1-a/disks/example_disk_1
-              mode: READ_WRITE
-              type: PERSISTENT
-              disk_size_gb: '10'
-              index: 0
-              interface: SCSI
-              kind: compute#attachedDisk
-          - scheduling:
-              automatic_restart: true
-              on_host_maintenance: MIGRATE
-              preemptible: false
-              provisioning_model: STANDARD
-          - deletion_protection: false
-          - tags:
-              items:
-                - test
-          - metadata:
-              kind: compute#metadata
-              items:
-                - key: sample_metadata_key
-                  value: sample_metadata_value
-
+            example-resource-name:
+              gcp.compute.instance.present:
+              - project: example-project
+              - machine_type: https://www.googleapis.com/compute/v1/projects/example-project/zones/us-central1-a/machineTypes/g1-small
+              - zone: us-central1-a
+              - can_ip_forward: false
+              - network_interfaces:
+                - access_configs:
+                  - kind: compute#accessConfig
+                    name: External NAT
+                    network_tier: PREMIUM
+                    set_public_ptr: false
+                    type_: ONE_TO_ONE_NAT
+                  kind: compute#networkInterface
+                  name: nic0
+                  network: https://www.googleapis.com/compute/v1/projects/project-name/global/networks/default
+                  stack_type: IPV4_ONLY
+                  subnetwork: https://www.googleapis.com/compute/v1/projects/project-name/regions/us-central1/subnetworks/default
+              - disks:
+                - auto_delete: true
+                  boot: true
+                  device_name: example_disk_1
+                  source: https://www.googleapis.com/compute/v1/projects/project-name/zones/us-central1-a/disks/example_disk_1
+                  mode: READ_WRITE
+                  type_: PERSISTENT
+                  disk_size_gb: '10'
+                  index: 0
+                  interface: SCSI
+                  kind: compute#attachedDisk
+              - scheduling:
+                  automatic_restart: true
+                  on_host_maintenance: MIGRATE
+                  preemptible: false
+                  provisioning_model: STANDARD
+              - deletion_protection: false
+              - tags:
+                  items:
+                    - test
+              - metadata:
+                  kind: compute#metadata
+                  items:
+                    - key: sample_metadata_key
+                      value: sample_metadata_value
     """
     result = {
         "result": True,
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
-    project = get_project_from_account(ctx, project)
-
-    if ctx.get("rerun_data"):
-        handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, ctx.get("rerun_data").get("operation_id"), "compute.instance"
-        )
-
-        if not handle_operation_ret["result"]:
-            result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = ctx.get("rerun_data")
-            return result
-
-        resource_id = handle_operation_ret["resource_id"]
-
-    get_resource_only_with_resource_id = hub.OPT.idem.get(
-        "get_resource_only_with_resource_id", False
-    )
-    if resource_id:
-        old_get_ret = await hub.exec.gcp.compute.instance.get(
-            ctx, resource_id=resource_id
-        )
-
-        if not old_get_ret["result"] or (
-            not old_get_ret["ret"] and get_resource_only_with_resource_id
-        ):
-            result["result"] = False
-            result["comment"] += old_get_ret["comment"]
-            return result
-
-        # long running operation has succeeded - both update and create
-        if ctx.get("rerun_data"):
-            result["new_state"] = old_get_ret["ret"]
-            result["old_state"] = ctx["rerun_data"]["old_state"]
-            if ctx["rerun_data"]["old_state"]:
-                result["comment"].append(
-                    hub.tool.gcp.comment_utils.update_comment(
-                        "gcp.compute.instance", name
-                    )
-                )
-            else:
-                result["comment"].append(
-                    hub.tool.gcp.comment_utils.create_comment(
-                        "gcp.compute.instance", name
-                    )
-                )
-            return result
-
-        result["old_state"] = copy.deepcopy(copy.copy(old_get_ret["ret"]))
-    elif not get_resource_only_with_resource_id:
-        resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
-            "compute.instance", {**locals(), "instance": name}
-        )
-        old_get_ret = await hub.exec.gcp.compute.instance.get(
-            ctx, resource_id=resource_id
-        )
-
-        if not old_get_ret["result"]:
-            result["result"] = False
-            result["comment"] += old_get_ret["comment"]
-            return result
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
-        if old_get_ret["ret"]:
-            result["old_state"] = copy.deepcopy(copy.copy(old_get_ret["ret"]))
+    if ctx.get("wrapper_result"):
+        result = ctx.get("wrapper_result")
 
     # to be autogenerated by pop-create based on insert/update props in properties.yaml
     resource_body = {
         "service_accounts": service_accounts,
         "name": name,
         "min_cpu_platform": min_cpu_platform,
         "disks": disks,
@@ -1216,22 +1090,21 @@
         "labels": labels,
         "deletion_protection": deletion_protection,
         "network_interfaces": network_interfaces,
         "can_ip_forward": can_ip_forward,
         "display_device": display_device,
         "zone": zone,
         "status": status,
+        "id_": id_,
     }
 
     resource_body = {k: v for (k, v) in resource_body.items() if v is not None}
     operation = None
     if result["old_state"]:
-        # copy.copy(old_get_ret['ret']) is needed to convert any objects of type NamespaceDict to dict
-        # in old_get_ret['ret']. This is done so that comparisons with the resource_body which has
-        # objects of type dict works properly
+        resource_id = result["old_state"].get("resource_id", None)
         zone = hub.tool.gcp.resource_prop_utils.parse_link_to_zone(
             result["old_state"]["zone"]
         )
         result["old_state"]["zone"] = zone
 
         # The fingerprint is required upon an update operation but in the time of creation the
         # resource still do not have fingerprint so, we cannot make it a required param for present method.
@@ -1247,14 +1120,19 @@
         # third - the property is required in the end result
         patch_operations_dict = {
             "network_interfaces": (
                 hub.tool.gcp.compute.instance.update_network_interfaces,
                 (ctx, result["old_state"], network_interfaces),
                 True,
             ),
+            "status": (
+                hub.tool.gcp.compute.instance.update_status,
+                (ctx, resource_id, result["old_state"].get("status"), status),
+                True,
+            ),
             "shielded_instance_config": (
                 hub.tool.gcp.compute.instance.update_shielded_instance_config,
                 (ctx, shielded_instance_config, None, None, None, resource_id),
                 False,
             ),
             "shielded_instance_integrity_policy": (
                 hub.tool.gcp.compute.instance.update_shielded_instance_integrity_policy,
@@ -1264,37 +1142,28 @@
                     None,
                     None,
                     None,
                     resource_id,
                 ),
                 False,
             ),
-            "status": (
-                hub.tool.gcp.compute.instance.update_status,
-                (ctx, resource_id, result["old_state"].get("status"), status),
-                True,
-            ),
         }
 
-        old_properties_dict = {
-            k: result["old_state"].get(k) for k in patch_operations_dict.keys()
-        }
-        changed_properties_dict = {
-            k: hub.tool.gcp.utils.compare_states(
-                {k: old_properties_dict.get(k, [])},
-                {k: resource_body.get(k, [])},
-                "compute.instance",
-            )
-            for k, v in patch_operations_dict.items()
-        }
+        state_operations = StateOperations(
+            hub, "compute.instance", patch_operations_dict, result, resource_body
+        )
 
         changes = hub.tool.gcp.utils.compare_states(
             result["old_state"],
-            {"resource_id": resource_id, **resource_body, **old_properties_dict},
+            {
+                "resource_id": resource_id,
+                **resource_body,
+            },
             "compute.instance",
+            additional_exclude_paths=list(patch_operations_dict.keys()),
         )
 
         if changes:
             changed_non_updatable_properties = (
                 hub.tool.gcp.resource_prop_utils.get_changed_non_updatable_properties(
                     "compute.instance", changes
                 )
@@ -1304,68 +1173,71 @@
                 result["comment"].append(
                     hub.tool.gcp.comment_utils.non_updatable_properties_comment(
                         "gcp.compute.instance",
                         name,
                         changed_non_updatable_properties,
                     )
                 )
-                result["new_state"] = copy.deepcopy(result["old_state"])
+                result["new_state"] = result["old_state"]
                 return result
 
-        if not changes and not any(changed_properties_dict.values()):
+        if not changes and not any(state_operations.changed_properties_dict.values()):
             result["result"] = True
             result["comment"].append(
                 hub.tool.gcp.comment_utils.up_to_date_comment(
                     "gcp.compute.instance", name
                 )
             )
-            result["new_state"] = copy.deepcopy(result["old_state"])
+            result["new_state"] = result["old_state"]
             return result
 
         if ctx["test"]:
             result["comment"].append(
                 hub.tool.gcp.comment_utils.would_update_comment(
                     "gcp.compute.instance", name
                 )
             )
-            result["new_state"] = resource_body
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                resource_body
+            )
             result["new_state"]["resource_id"] = resource_id
             return result
 
-        for k, op in patch_operations_dict.items():
-            if changed_properties_dict[k]:
-                ret = await op[0](*op[1])
-
-                if not ret["result"]:
-                    result["comment"] += ret["comment"]
-                    result["result"] = False
-                    return result
+        state_operations_ret = await state_operations.run_operations()
 
-        if changes:
-            if any(changed_properties_dict.values()):
-                get_ret = await hub.exec.gcp.compute.instance.get(
-                    ctx, resource_id=resource_id
-                )
-                if not get_ret["result"] and not get_ret["ret"]:
-                    result["result"] = False
-                    result["comment"] += get_ret["comment"]
-                    return result
+        current_state = result["old_state"]
+        if "new_state" in state_operations_ret:
+            current_state = state_operations_ret["new_state"]
+        elif any(state_operations.changed_properties_dict.values()):
+            get_ret = await hub.exec.gcp.compute.instance.get(
+                ctx, resource_id=resource_id
+            )
+            if not get_ret["result"] or not get_ret["ret"]:
+                result["result"] = False
+                result["comment"] += get_ret["comment"]
+                return result
+            current_state = get_ret["ret"]
+        result["new_state"] = current_state
+
+        if not state_operations_ret["result"]:
+            result["comment"] += state_operations_ret["comment"]
+            result["result"] = False
+            return result
 
+        if changes:
+            if any(state_operations.changed_properties_dict.values()):
                 for k in patch_operations_dict.keys():
-                    resource_body[k] = get_ret["ret"].get(k)
+                    resource_body[k] = current_state.get(k)
 
-                resource_body["fingerprint"] = get_ret["ret"].get("fingerprint")
-                resource_body["label_fingerprint"] = get_ret["ret"].get(
+                resource_body["fingerprint"] = current_state.get("fingerprint")
+                resource_body["label_fingerprint"] = current_state.get(
                     "label_fingerprint"
                 )
 
-            # put the old value of required properties in the resource body
-            for k, v in patch_operations_dict.items():
-                if v[2] and not resource_body.get(k):
-                    resource_body[k] = old_properties_dict[k]
+            state_operations.pre_process_resource_body(resource_body)
 
             update_ret = await hub.exec.gcp_api.client.compute.instance.update(
                 hub,
                 ctx,
                 name=name,
                 resource_id=resource_id,
                 minimal_action=minimal_action,
@@ -1374,18 +1246,18 @@
             )
 
             if not update_ret["result"] or not update_ret["ret"]:
                 result["result"] = False
                 result["comment"] += update_ret["comment"]
                 return result
 
-            if "compute#operation" in update_ret["ret"].get("kind", ""):
+            if hub.tool.gcp.operation_utils.is_operation(update_ret["ret"]):
                 operation = update_ret["ret"]
 
-        if not changes and any(changed_properties_dict.values()):
+        if not changes and any(state_operations.changed_properties_dict.values()):
             get_ret = await hub.exec.gcp.compute.instance.get(
                 ctx, resource_id=resource_id
             )
             if not get_ret["result"] and not get_ret["ret"]:
                 result["result"] = False
                 result["comment"] += get_ret["comment"]
                 return result
@@ -1399,15 +1271,17 @@
     else:
         if ctx["test"]:
             result["comment"].append(
                 hub.tool.gcp.comment_utils.would_create_comment(
                     "gcp.compute.instance", name
                 )
             )
-            result["new_state"] = resource_body
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                resource_body
+            )
             result["new_state"]["resource_id"] = resource_id
             return result
 
         # Create
         create_ret = await hub.exec.gcp_api.client.compute.instance.insert(
             ctx,
             name=name,
@@ -1432,149 +1306,34 @@
                         "gcp.compute.instance", name
                     )
                 )
             else:
                 result["comment"] += create_ret["comment"]
             return result
 
-        if "compute#operation" in create_ret["ret"].get("kind", ""):
+        if hub.tool.gcp.operation_utils.is_operation(create_ret["ret"]):
             operation = create_ret["ret"]
 
     if operation:
         operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
             operation.get("selfLink"), "compute.zone_operation"
         )
         result["rerun_data"] = {
             "operation_id": operation_id,
             "old_state": result["old_state"],
+            "on_completion": {
+                "handler": "hub.tool.gcp.compute.instance.on_completion",
+                "aux_ctx": {"status": status},
+            },
         }
         return result
 
     return result
 
 
-async def absent(
-    hub,
-    ctx,
-    name: str = None,
-    zone: str = None,
-    project: str = None,
-    resource_id: str = None,
-    request_id: str = None,
-) -> Dict[str, Any]:
-    r"""Deletes the specified Instance resource. For more information, see Deleting an instance.
-
-    Args:
-        name(str):
-            The name of the resource
-
-        resource_id(str, Optional):
-            The resource_id of the resource
-
-        zone:(str, Optional):
-            The name of the zone for this request.
-        project:(str, Optional):
-            Project ID for this request.
-
-        request_id(str, Optional):
-            An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed.
-            For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments.
-            The request ID must be a valid UUID with the exception that zero UUID is not supported (00000000-0000-0000-0000-000000000000).
-
-    Returns:
-        Dict[str, Any]
-
-    Examples:
-        .. code-block:: sls
-
-        example_resource_name:
-          gcp.compute.instance.absent
-
-    """
-    result = {
-        "comment": [],
-        "old_state": ctx.get("old_state"),
-        "new_state": None,
-        "name": name,
-        "result": True,
-    }
-
-    if not resource_id and not hub.OPT.idem.get(
-        "get_resource_only_with_resource_id", False
-    ):
-        resource_id = (ctx.get("old_state") or {}).get(
-            "resource_id"
-        ) or hub.tool.gcp.resource_prop_utils.construct_resource_id(
-            "compute.instance", {**locals(), "instance": name}
-        )
-
-    if not resource_id:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.already_absent_comment(
-                "gcp.compute.instance", name
-            )
-        )
-        return result
-
-    if not ctx.get("rerun_data"):
-        get_ret = await hub.exec.gcp.compute.instance.get(ctx, resource_id=resource_id)
-
-        if not get_ret["result"]:
-            result["result"] = False
-            result["comment"] += get_ret["comment"]
-            return result
-
-        if not get_ret["ret"]:
-            result["comment"].append(
-                hub.tool.gcp.comment_utils.already_absent_comment(
-                    "gcp.compute.instance", name
-                )
-            )
-            return result
-
-        result["old_state"] = get_ret["ret"]
-
-    if ctx["test"]:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.would_delete_comment(
-                "gcp.compute.instance", name
-            )
-        )
-        return result
-
-    if not ctx.get("rerun_data"):
-        # First iteration; invoke instance's delete()
-        delete_ret = await hub.exec.gcp_api.client.compute.instance.delete(
-            ctx, resource_id=resource_id, request_id=request_id
-        )
-        if "compute#operation" in delete_ret.get("ret", {}).get("kind"):
-            result["result"] = False
-            result["comment"] += delete_ret["comment"]
-            result[
-                "rerun_data"
-            ] = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                delete_ret["ret"].get("selfLink"), "compute.zone_operation"
-            )
-            return result
-    else:
-        # delete() has been called on some previous iteration
-        handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, ctx.get("rerun_data"), "compute.instance"
-        )
-        if not handle_operation_ret["result"]:
-            result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
-            return result
-
-    result["comment"].append(
-        hub.tool.gcp.comment_utils.delete_comment("gcp.compute.instance", name)
-    )
-    return result
-
-
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
     r"""Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
     Retrieves the list of instances contained within the specified zone.
 
     Returns:
         Dict[str, Dict[str, Any]]
@@ -1603,8 +1362,9 @@
                 for parameter_key, parameter_value in resource.items()
             ]
         }
     return result
 
 
 def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
+    """Default implemented for each module."""
     return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/machine_image.py` & `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/firewall.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,396 +1,410 @@
-"""State module for managing Machine Images."""
-import copy
+"""Google Cloud Platform firewalls state module.
+
+Copyright (c) 2023 VMware, Inc. All Rights Reserved.
+SPDX-License-Identifier: Apache-2.0
+
+"""
 from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 
-from idem_gcp.tool.gcp.utils import get_project_from_account
+from idem_gcp.tool.gcp.utils import global_absent
+
+# prevent commit hook from removing the import
+absent = global_absent
 
 __contracts__ = ["resource"]
+RESOURCE_TYPE = "compute.firewall"
+RESOURCE_TYPE_FULL = "gcp.compute.firewall"
 
 
 async def present(
     hub,
     ctx,
     name: str,
     project: str = None,
-    resource_id: str = None,
-    source_instance: str = None,
-    storage_locations: List[str] = None,
-    source_disk_encryption_keys: List[
+    target_tags: List[str] = None,
+    source_service_accounts: List[str] = None,
+    denied: List[
         make_dataclass(
-            "SourceDiskEncryptionKey",
+            "items",
             [
-                ("sourceDisk", str, field(default=None)),
-                ("diskEncryptionKey", {}, field(default=None)),
+                ("ip_protocol", str, field(default=None)),
+                ("ports", List[str], field(default=None)),
             ],
-        )
+        ),
     ] = None,
     description: str = None,
-    saved_disks: List[
+    direction: str = None,
+    destination_ranges: List[str] = None,
+    allowed: List[
         make_dataclass(
-            "SavedDisk",
+            "items",
             [
-                ("kind", str, field(default="compute#savedDisk")),
-                ("storageBytesStatus", str, field(default=None)),
-                ("architecture", str, field(default=None)),
-                ("storageBytes", str, field(default=None)),
-                ("sourceDisk", str, field(default=None)),
+                ("ports", List[str], field(default=None)),
+                ("ip_protocol", str, field(default=None)),
             ],
-        )
+        ),
     ] = None,
-    guest_flush: bool = None,
-    machine_image_encryption_key: make_dataclass(
-        "CustomerEncryptionKey",
-        [
-            ("kmsKeyServiceAccount", str, field(default=None)),
-            ("rsaEncryptedKey", str, field(default=None)),
-            ("rawKey", str, field(default=None)),
-            ("kmsKeyName", str, field(default=None)),
-        ],
-    ) = None,
+    disabled: bool = None,
+    network: str = None,
+    priority: int = None,
+    log_config: Dict[str, Any] = None,
+    target_service_accounts: List[str] = None,
+    source_tags: List[str] = None,
+    source_ranges: List[str] = None,
+    resource_id: str = None,
 ) -> Dict[str, Any]:
-    r"""Creates a machine image in the specified project using the data that is included in the request. If you are creating a new machine image to update an existing instance, your new machine image should use the same network or, if applicable, the same subnetwork as the original instance.
+    r"""Creates or updates a firewall rule in the specified project using the data included in the request.
 
     Args:
-
-        name(str):
-            An Idem name of the resource.
-
-        project(str, Optional):
-            Project ID for this request.
-
+        name(str): An Idem name of the resource.
+        project(str, Optional): Project ID for this request.
+        target_tags(List[str], Optional):
+            A list of tags that controls which instances the firewall rule applies to. If targetTags are specified,
+            then the firewall rule applies only to instances in the VPC network that have one of those tags. If no
+            targetTags are specified, the firewall rule applies to all instances on the specified network. Defaults to None.
+        source_service_accounts(List[str], Optional):
+            If source service accounts are specified, the firewall rules apply only to traffic originating from an
+            instance with a service account in this list. Source service accounts cannot be used to control traffic to
+            an instance's external IP address because service accounts are associated with an instance, not an IP
+            address. sourceRanges can be set at the same time as sourceServiceAccounts. If both are set, the firewall
+            applies to traffic that has a source IP address within the sourceRanges OR a source IP that belongs to an
+            instance with service account listed in sourceServiceAccount. The connection does not need to match both
+            fields for the firewall to apply. sourceServiceAccounts cannot be used at the same time as sourceTags or
+            targetTags. Defaults to None.
+        denied(List[Dict[str, Any]], Optional):
+            The list of DENY rules specified by this firewall. Each rule specifies a protocol and port-range tuple that
+            describes a denied connection. Defaults to None.
+
+            * ip_protocol (str, Optional): The IP protocol to which this rule applies. The protocol type is required when
+              creating a firewall rule. This value can either be one of the following well known protocol strings
+              (tcp, udp, icmp, esp, ah, ipip, sctp) or the IP protocol number.
+            * ports (list[str], Optional): An optional list of ports to which this rule applies. This field is only
+              applicable for the UDP or TCP protocol. Each entry must be either an integer or a range. If not specified,
+              this rule applies to connections through any port. Example inputs include: ["22"], ["80","443"], and
+              ["12345-12349"].
+        description(str, Optional):
+            An optional description of this resource. Provide this field when you create the resource. Defaults to None.
+        direction(str, Optional):
+            Direction of traffic to which this firewall applies, either `INGRESS` or `EGRESS`. The default is `INGRESS`.
+            For `EGRESS` traffic, you cannot specify the sourceTags fields. Defaults to None.
+        destination_ranges(List[str], Optional):
+            If destination ranges are specified, the firewall rule applies only to traffic that has destination IP
+            address in these ranges. These ranges must be expressed in CIDR format. Both IPv4 and IPv6 are supported.
+            Defaults to None.
+        allowed(List[Dict[str, Any]], Optional):
+            The list of ALLOW rules specified by this firewall. Each rule specifies a protocol and port-range tuple that
+            describes a permitted connection. Defaults to None.
+
+            * ports (List[str], Optional): An optional list of ports to which this rule applies. This field is only
+              applicable for the UDP or TCP protocol. Each entry must be either an integer or a range. If not specified,
+              this rule applies to connections through any port. Example inputs include: ["22"], ["80","443"], and ["12345-12349"].
+            * ip_protocol (str, Optional): The IP protocol to which this rule applies. The protocol type is required when
+              creating a firewall rule. This value can either be one of the following well known protocol strings
+              (tcp, udp, icmp, esp, ah, ipip, sctp) or the IP protocol number.
+        disabled(bool, Optional):
+            Denotes whether the firewall rule is disabled. When set to true, the firewall rule is not enforced and the
+            network behaves as if it did not exist. If this is unspecified, the firewall rule will be enabled. Defaults to None.
+        network(str, Optional):
+            URL of the network resource for this firewall rule. If not specified when creating a firewall rule, the
+            default network is used: global/networks/default If you choose to specify this field, you can specify the
+            network as a full or partial URL. For example, the following are all valid
+            URLs: - https://www.googleapis.com/compute/v1/projects/myproject/global/networks/my-network -
+            projects/myproject/global/networks/my-network - global/networks/default . Defaults to None.
+        priority(int, Optional):
+            Priority for this rule. This is an integer between `0` and `65535`, both inclusive. The default value is
+            `1000`. Relative priorities determine which rule takes effect if multiple rules apply. Lower values indicate
+            higher priority. For example, a rule with priority `0` has higher precedence than a rule with priority `1`.
+            DENY rules take precedence over ALLOW rules if they have equal priority. Note that VPC networks have implied
+            rules with a priority of `65535`. To avoid conflicts with the implied rules, use a priority number less than
+            `65535`. Defaults to None.
+        log_config(Dict[str, Any], Optional):
+            This field denotes the logging options for a particular firewall rule. If logging is enabled, logs will be
+            exported to Cloud Logging. Defaults to None.
+        target_service_accounts(List[str], Optional):
+            A list of service accounts indicating sets of instances located in the network that may make network
+            connections as specified in allowed[]. targetServiceAccounts cannot be used at the same time as targetTags
+            or sourceTags. If neither targetServiceAccounts nor targetTags are specified, the firewall rule applies to
+            all instances on the specified network. Defaults to None.
+        source_tags(List[str], Optional):
+            If source tags are specified, the firewall rule applies only to traffic with source IPs that match the
+            primary network interfaces of VM instances that have the tag and are in the same VPC network. Source tags
+            cannot be used to control traffic to an instance's external IP address, it only applies to traffic between
+            instances in the same virtual network. Because tags are associated with instances, not IP addresses. One or
+            both of sourceRanges and sourceTags may be set. If both fields are set, the firewall applies to traffic that
+            has a source IP address within sourceRanges OR a source IP from a resource with a matching tag listed in the
+            sourceTags field. The connection does not need to match both fields for the firewall to apply. Defaults to None.
+        source_ranges(List[str], Optional):
+            If source ranges are specified, the firewall rule applies only to traffic that has a source IP address in
+            these ranges. These ranges must be expressed in CIDR format. One or both of sourceRanges and sourceTags may
+            be set. If both fields are set, the rule applies to traffic that has a source IP address within sourceRanges
+            OR a source IP from a resource with a matching tag listed in the sourceTags field. The connection does not
+            need to match both fields for the rule to apply. Both IPv4 and IPv6 are supported. Defaults to None.
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
-        source_instance(str, Optional):
-            The source instance used to create the machine image. You can provide this as a partial or full URL to the resource. For example, the following are valid values: - https://www.googleapis.com/compute/v1/projects/project/zones/zone /instances/instance - projects/project/zones/zone/instances/instance . Defaults to None.
-
-        storage_locations(list[str], Optional):
-            The regional or multi-regional Cloud Storage bucket location where the machine image is stored. Defaults to None.
-
-        source_disk_encryption_keys(list[Dict[str, Any]], Optional):
-            [Input Only] The customer-supplied encryption key of the disks attached to the source instance. Required if the source disk is protected by a customer-supplied encryption key. Defaults to None.
-            * properties (Dict[str, Dict[str, Any]], optional): None
-                * sourceDisk (str, optional): URL of the disk attached to the source instance. This can be a full or valid partial URL. For example, the following are valid values: - https://www.googleapis.com/compute/v1/projects/project/zones/zone /disks/disk - projects/project/zones/zone/disks/disk - zones/zone/disks/disk
-                * diskEncryptionKey ({}, optional): The customer-supplied encryption key of the source disk. Required if the source disk is protected by a customer-supplied encryption key.
-
-        description(str, Optional):
-            An optional description of this resource. Provide this property when you create the resource. Defaults to None.
-
-        saved_disks(list[Dict[str, Any]], Optional):
-            An array of Machine Image specific properties for disks attached to the source instance. Defaults to None.
-            * properties (Dict[str, Dict[str, Any]], optional): An instance-attached disk resource.
-                * kind (str, optional): [Output Only] Type of the resource. Always compute#savedDisk for attached disks.
-                * storageBytesStatus (str, optional): [Output Only] An indicator whether storageBytes is in a stable state or it is being adjusted as a result of shared storage reallocation. This status can either be UPDATING, meaning the size of the snapshot is being updated, or UP_TO_DATE, meaning the size of the snapshot is up-to-date.
-                * architecture (str, optional): [Output Only] The architecture of the attached disk.
-                * storageBytes (str, optional): [Output Only] Size of the individual disk snapshot used by this machine image.
-                * sourceDisk (str, optional): Specifies a URL of the disk attached to the source instance.
-
-        guest_flush(bool, Optional):
-            [Input Only] Whether to attempt an application consistent machine image by informing the OS to prepare for the snapshot process. Defaults to None.
-
-        machine_image_encryption_key({}, Optional):
-            Encrypts the machine image using a customer-supplied encryption key. After you encrypt a machine image using a customer-supplied key, you must provide the same key if you use the machine image later. For example, you must provide the encryption key when you create an instance from the encrypted machine image in a future request. Customer-supplied encryption keys do not protect access to metadata of the machine image. If you do not provide an encryption key when creating the machine image, then the machine image will be encrypted using an automatically generated key and you do not need to provide a key to use the machine image later. Defaults to None.
-
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
-            example_resource_name:
-                gcp.compute.machine_image.present:
-                  - project: project-name
-                  - source_instance: https://www.googleapis.com/compute/v1/projects/project-name/zones/zone-name/instances/instance-name
+            firewall-present:
+              gcp.compute.firewall.present:
+              - name: my-firewall-name
+              - description: Free text description
+              - network: https://www.googleapis.com/compute/v1/projects/project-name/global/networks/default
+              - source_ranges:
+                - 0.0.0.0/0
+              - allowed:
+                - ip_protocol: tcp
+                  ports:
+                  - '22'
+              - direction: INGRESS
+              - log_config:
+                  enable: false
+              - disabled: false
     """
     result = {
         "result": True,
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
+    resource_type_camel = hub.tool.gcp.case.camel(RESOURCE_TYPE_FULL.split(".")[-1])
 
-    # Get the resource_id from ESM
-    if not resource_id:
-        resource_id = (ctx.get("old_state") or {}).get(
-            "resource_id"
-        ) or hub.tool.gcp.resource_prop_utils.construct_resource_id(
-            "compute.machine_image", {**locals(), "machineImage": name}
+    if hub.tool.gcp.resource_prop_utils.properties_mismatch_resource_id(
+        RESOURCE_TYPE, resource_id, {**locals(), resource_type_camel: name}
+    ):
+        result["comment"].append(
+            hub.tool.gcp.comment_utils.properties_mismatch_resource_id_comment(
+                RESOURCE_TYPE_FULL, name
+            )
         )
-    old = None
 
-    # TODO: Handle operation result state
     if ctx.get("rerun_data"):
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, ctx.get("rerun_data"), "compute.machine_image"
+            ctx, ctx.get("rerun_data"), RESOURCE_TYPE
         )
 
         if not handle_operation_ret["result"]:
             result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
+            if handle_operation_ret.get("rerun_data"):
+                result["rerun_data"] = handle_operation_ret["rerun_data"]
+                if handle_operation_ret["rerun_data"].get("has_error", False):
+                    result["result"] = False
+            else:
+                result["result"] = False
+
             return result
 
         resource_id = handle_operation_ret["resource_id"]
 
+    get_resource_only_with_resource_id = hub.OPT.idem.get(
+        "get_resource_only_with_resource_id", False
+    )
     if resource_id:
-        old_get_ret = await hub.exec.gcp_api.client.compute.machine_image.get(
+        old_get_ret = await hub.exec.gcp.compute.firewall.get(
+            ctx, resource_id=resource_id
+        )
+
+        if not old_get_ret["result"] or (
+            not old_get_ret["ret"] and get_resource_only_with_resource_id
+        ):
+            result["result"] = False
+            result["comment"] += old_get_ret["comment"]
+            return result
+
+        # long running operation has succeeded - both update and create
+        if ctx.get("rerun_data"):
+            result["new_state"] = old_get_ret["ret"]
+            result["old_state"] = ctx["rerun_data"]["old_state"]
+            if ctx["rerun_data"]["old_state"]:
+                result["comment"].append(
+                    hub.tool.gcp.comment_utils.update_comment(RESOURCE_TYPE_FULL, name)
+                )
+            else:
+                result["comment"].append(
+                    hub.tool.gcp.comment_utils.create_comment(RESOURCE_TYPE_FULL, name)
+                )
+            return result
+
+        result["old_state"] = old_get_ret["ret"]
+    elif not get_resource_only_with_resource_id:
+        resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
+            RESOURCE_TYPE, {"project": project, "firewall": name}
+        )
+        old_get_ret = await hub.exec.gcp.compute.firewall.get(
             ctx, resource_id=resource_id
         )
 
         if not old_get_ret["result"]:
-            # error other than non-existing resource
             result["result"] = False
             result["comment"] += old_get_ret["comment"]
             return result
 
         if old_get_ret["ret"]:
-            # resource already exists
+            result["old_state"] = old_get_ret["ret"]
 
-            # copy.copy(old_get_ret['ret']) is needed to convert any objects of type NamespaceDict to dict
-            # in old_get_ret['ret']. This is done so that comparisons with the plan_state which has
-            # objects of type dict works properly
-            old = copy.deepcopy(copy.copy(old_get_ret["ret"]))
-            result["old_state"] = old
-
-            # If rerun_data is set at this point this means that there has been a completed create or update operation
-            # so there is no need to run the code for create or update below again and we stop here
-            if ctx.get("rerun_data"):
-                result["new_state"] = result["old_state"]
-                return result
-
-    # TODO: Check if body contains the same parameters as old
-    # to be autogenerated by pop-create based on insert/update props in properties.yaml
     resource_body = {
-        "storage_locations": storage_locations,
-        "guest_flush": guest_flush,
-        "source_instance": source_instance,
-        "description": description,
+        "priority": priority,
+        "log_config": log_config,
+        "direction": direction,
+        "source_ranges": source_ranges,
+        "source_service_accounts": source_service_accounts,
+        "allowed": allowed,
+        "target_tags": target_tags,
+        "source_tags": source_tags,
+        "denied": denied,
+        "target_service_accounts": target_service_accounts,
+        "network": network,
+        "destination_ranges": destination_ranges,
+        "disabled": disabled,
         "name": name,
-        "saved_disks": saved_disks,
-        "machine_image_encryption_key": machine_image_encryption_key,
-        "source_disk_encryption_keys": source_disk_encryption_keys,
-    }
-
-    # TODO: How to handle query params which are not returned in the response body of get
-    plan_state = {
-        # "project": project,
-        # "predefined_acl": predefined_acl,
-        # "predefined_default_object_acl": predefined_default_object_acl,
-        "resource_id": resource_id,
-        **resource_body,
+        "description": description,
     }
 
-    plan_state = {k: v for (k, v) in plan_state.items() if v is not None}
+    resource_body = {k: v for (k, v) in resource_body.items() if v is not None}
     operation = None
-    if old:
+    if result["old_state"]:
         changes = hub.tool.gcp.utils.compare_states(
-            old, plan_state, "compute.machine_image"
+            result["old_state"], resource_body, RESOURCE_TYPE
         )
         if not changes:
             result["result"] = True
             result["comment"].append(
-                hub.tool.gcp.comment_utils.already_exists_comment(
-                    "gcp.compute.machine_image", name
-                )
+                hub.tool.gcp.comment_utils.up_to_date_comment(RESOURCE_TYPE_FULL, name)
             )
             result["new_state"] = result["old_state"]
             return result
 
-        result["comment"].append(
-            "No-op: There is no update function for gcp.compute.machine_image"
-        )
-
-    else:
         if ctx["test"]:
             result["comment"].append(
-                hub.tool.gcp.comment_utils.would_create_comment(
-                    "gcp.compute.machine_image", name
+                hub.tool.gcp.comment_utils.would_update_comment(
+                    RESOURCE_TYPE_FULL, name
                 )
             )
-            result["new_state"] = plan_state
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                {"resource_id": resource_id, **resource_body}
+            )
             return result
 
-        # Create
-        create_ret = await hub.exec.gcp_api.client.compute.machine_image.insert(
-            ctx, project=project, body=resource_body
+        update_ret = await hub.exec.gcp_api.client.compute.firewall.patch(
+            hub, ctx, resource_id=resource_id, body=resource_body
         )
-        if not create_ret["result"]:
+        if not update_ret["result"] or not update_ret["ret"]:
             result["result"] = False
-            result["comment"] += create_ret["comment"]
+            result["comment"] += update_ret["comment"]
             return result
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.create_comment("gcp.compute.machine_image", name)
-        )
-        result["old_state"] = {}
-        resource_id = create_ret["ret"].get("resource_id")
-        if "compute#operation" in create_ret["ret"].get("kind"):
-            operation = create_ret["ret"]
 
-    if operation:
-        operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-            operation.get("selfLink"), "compute.global_operation"
-        )
-        handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, operation_id, "compute.machine_image"
-        )
+        if hub.tool.gcp.operation_utils.is_operation(update_ret.get("ret")):
+            operation = update_ret["ret"]
 
-        if not handle_operation_ret["result"]:
-            result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
+        get_ret = await hub.exec.gcp.compute.firewall.get(ctx, resource_id=resource_id)
+        if not get_ret["result"] and not get_ret["ret"]:
+            result["result"] = False
+            result["comment"] += get_ret["comment"]
             return result
 
-        resource_id = handle_operation_ret["resource_id"]
-
-    # Try getting the resource again
-    # TODO: Reconciliation or waiter loop?
-    # TODO: Check if this can be removed because insert and update may also return the necessary data on success
-    get_ret = await hub.exec.gcp_api.client.compute.machine_image.get(
-        ctx, resource_id=resource_id
-    )
-
-    if not get_ret["result"] and not get_ret["ret"]:
-        result["result"] = False
-        result["comment"] += get_ret["comment"]
-        return result
-
-    result["new_state"] = get_ret["ret"]
-
-    return result
-
-
-async def absent(
-    hub,
-    ctx,
-    name: str,
-    resource_id: str = None,
-    request_id: str = None,
-) -> Dict[str, Any]:
-    r"""Deletes the specified machine image. Deleting a machine image is permanent and cannot be undone.
-
-    Args:
-        name(str):
-            An Idem name of the resource.
-
-        resource_id(str, Optional):
-            An identifier of the resource in the provider. Defaults to None.
-
-        request_id(str, Optional):
-            An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
-
-    Returns:
-        Dict[str, Any]
-
-    Examples:
-        .. code-block:: sls
-
-            resource_is_absent:
-              gcp.compute.machine_image.absent:
-                - name: value
-                - project: value
-                - machine_image: value
-    """
-    result = {
-        "comment": [],
-        "old_state": ctx.get("old_state"),
-        "new_state": None,
-        "name": name,
-        "result": True,
-    }
-
-    if not resource_id:
-        resource_id = (ctx.get("old_state") or {}).get("resource_id")
-
-    if ctx.test:
+        result["new_state"] = get_ret["ret"]
         result["comment"].append(
-            hub.tool.gcp.comment_utils.would_delete_comment(
-                "gcp.compute.machine_image", name
-            )
+            hub.tool.gcp.comment_utils.update_comment(RESOURCE_TYPE_FULL, name)
         )
         return result
-
-    if not ctx.get("rerun_data"):
-        # First iteration; invoke machine image's delete()
-        delete_ret = await hub.exec.gcp_api.client.compute.machine_image.delete(
-            ctx, resource_id=resource_id
-        )
-        if delete_ret["ret"]:
-            if "compute#operation" in delete_ret["ret"].get("kind"):
-                result["result"] = False
-                result["comment"] += delete_ret["comment"]
-                result[
-                    "rerun_data"
-                ] = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                    delete_ret["ret"].get("selfLink"), "compute.global_operation"
-                )
-                return result
-
     else:
-        # delete() has been called on some previous iteration
-        handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, ctx.get("rerun_data"), "compute.machine_image"
+        if ctx.get("test", False):
+            result["comment"].append(
+                hub.tool.gcp.comment_utils.would_create_comment(
+                    RESOURCE_TYPE_FULL, name
+                )
+            )
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                {"resource_id": resource_id, **resource_body}
+            )
+            return result
+        create_ret = await hub.exec.gcp_api.client.compute.firewall.insert(
+            ctx, project=project, body=resource_body
         )
-        if not handle_operation_ret["result"]:
-            result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
+        if not create_ret["result"] or not create_ret["ret"]:
+            result["result"] = False
+            if create_ret["comment"] and next(
+                (
+                    comment
+                    for comment in create_ret["comment"]
+                    if "alreadyExists" in comment
+                ),
+                None,
+            ):
+                result["comment"].append(
+                    hub.tool.gcp.comment_utils.already_exists_comment(
+                        RESOURCE_TYPE_FULL, name
+                    )
+                )
+            else:
+                result["comment"] += create_ret["comment"]
             return result
 
-        resource_id = handle_operation_ret["resource_id"]
+        if hub.tool.gcp.operation_utils.is_operation(create_ret.get("ret")):
+            operation = create_ret["ret"]
 
-    if not resource_id:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.already_absent_comment(
-                "gcp.compute.machine_image", name
-            )
+    if operation:
+        operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
+            operation.get("selfLink"), "compute.global_operation"
         )
+        result["rerun_data"] = {
+            "operation_id": operation_id,
+            "old_state": result["old_state"],
+        }
+        result["result"] = False
         return result
 
-    result["comment"].append(
-        hub.tool.gcp.comment_utils.delete_comment("gcp.compute.machine_image", name)
-    )
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
     r"""Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
-    Retrieves a list of machine images that are contained within the specified project.
+    Retrieves the list of firewall rules available to the specified project.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: bash
 
-            $ idem describe gcp.compute.machine_image
+            $ idem describe gcp.compute.firewall
     """
     result = {}
 
-    describe_ret = await hub.exec.gcp_api.client.compute.machine_image.list(
+    describe_ret = await hub.exec.gcp.compute.firewall.list(
         ctx, project=ctx.acct.project_id
     )
 
     if not describe_ret["result"]:
         hub.log.debug(
-            f"Could not describe gcp.compute.machine_image {describe_ret['comment']}"
+            f"Could not describe gcp.compute.firewall {describe_ret['comment']}"
         )
-        return {}
+        return result
 
-    for resource in describe_ret["ret"]["items"]:
+    for resource in describe_ret["ret"]:
         resource_id = resource.get("resource_id")
+
         result[resource_id] = {
-            "gcp.compute.machine_image.present": [
+            "gcp.compute.firewall.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
+
     return result
 
 
 def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
+    """Default implemented for each module."""
     return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/network.py` & `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/network.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 """State module for managing Networks."""
-import copy
 from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 
-from idem_gcp.tool.gcp.utils import get_project_from_account
+from dict_tools.typing import Computed
+
+from idem_gcp.tool.gcp.utils import global_absent
+
+# prevent commit hook from removing the import
+absent = global_absent
 
 __contracts__ = ["resource"]
+RESOURCE_TYPE = "compute.network"
+RESOURCE_TYPE_FULL = "gcp.compute.network"
 
 
 async def present(
     hub,
     ctx,
     name: str,
     resource_id: str = None,
@@ -46,14 +52,15 @@
                 ("state_details", str, field(default=None)),
                 ("export_subnet_routes_with_public_ip", bool, field(default=None)),
                 ("exchange_subnet_routes", bool, field(default=None)),
                 ("stack_type", str, field(default=None)),
             ],
         )
     ] = None,
+    id_: (Computed[str], "alias=id") = None,
 ) -> Dict[str, Any]:
     r"""Creates a network in the specified project using the data included in the request.
 
     Args:
         name(str):
             An Idem name of the resource.
 
@@ -86,45 +93,49 @@
 
         mtu(int, Optional):
             Maximum Transmission Unit in bytes. The minimum value for this field is 1300 and the maximum value is 8896. The suggested value is 1500, which is the default MTU used on the Internet, or 8896 if you want to use Jumbo frames. If unspecified, the value defaults to 1460. Defaults to None.
 
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
-        peerings(List[Dict[str, Any]], Optional): [Output Only] A list of network peerings for the resource. Defaults to None.
+        peerings(List[Dict[str, Any]], Optional):
+            A list of network peerings for the resource. Defaults to None.
+
             * export_custom_routes(bool, Optional):
                 Whether to export the custom routes to peer network. The default value is false.
             * auto_create_routes(bool, Optional):
                 This field will be deprecated soon. Use the exchange_subnet_routes field instead. Indicates whether full mesh connectivity is created and managed automatically between peered networks. Currently this field should always be true since Google Compute Engine will automatically create and manage subnetwork routes between two networks when peering state is ACTIVE.
             * network(str, Optional):
                 The URL of the peer network. It can be either full URL or partial URL. The peer network may belong to a different project. If the partial URL does not contain project, it is assumed that the peer network is in the same project as the current network.
             * name(str, Optional):
                 Name of this peering. Provided by the client when the peering is created. The name must comply with RFC1035. Specifically, the name must be 1-63 characters long and match regular expression `[a-z]([-a-z0-9]*[a-z0-9])?`. The first character must be a lowercase letter, and all the following characters must be a dash, lowercase letter, or digit, except the last character, which cannot be a dash.
             * state(str, Optional):
                 [Output Only] State for the peering, either `ACTIVE` or `INACTIVE`. The peering is `ACTIVE` when there's a matching configuration in the peer network.
-                Enum type. Allowed values:
-                "ACTIVE" - Matching configuration exists on the peer.
-                "INACTIVE" - There is no matching configuration on the peer, including the case when peer does not exist.
+                    Enum type. Allowed values:
+                    "ACTIVE" - Matching configuration exists on the peer.
+                    "INACTIVE" - There is no matching configuration on the peer, including the case when peer does not exist.
             * peer_mtu(int, Optional):
                 Maximum Transmission Unit in bytes.
             * import_subnet_routes_with_public_ip(bool, Optional):
                 Whether subnet routes with public IP range are imported. The default value is false. IPv4 special-use ranges are always imported from peers and are not controlled by this field.
             * import_custom_routes(bool, Optional):
                 Whether to import the custom routes from peer network. The default value is false.
             * state_details(str, Optional):
                 [Output Only] Details about the current state of the peering.
             * export_subnet_routes_with_public_ip(bool, Optional):
                 Whether subnet routes with public IP range are exported. The default value is true, all subnet routes are exported. IPv4 special-use ranges are always exported to peers and are not controlled by this field.
             * exchange_subnet_routes(bool, Optional):
                 Indicates whether full mesh connectivity is created and managed automatically between peered networks. Currently this field should always be true since Google Compute Engine will automatically create and manage subnetwork routes between two networks when peering state is ACTIVE.
             * stack_type(str, Optional):
                 Which IP version(s) of traffic and routes are allowed to be imported or exported between peer networks. The default value is IPV4_ONLY.
-                Enum type. Allowed values:
-                "IPV4_IPV6" - This Peering will allow IPv4 traffic and routes to be exchanged. Additionally if the matching peering is IPV4_IPV6, IPv6 traffic and routes will be exchanged as well.
-                "IPV4_ONLY" - This Peering will only allow IPv4 traffic and routes to be exchanged, even if the matching peering is IPV4_IPV6.
+                    Enum type. Allowed values:
+                    "IPV4_IPV6" - This Peering will allow IPv4 traffic and routes to be exchanged. Additionally if the matching peering is IPV4_IPV6, IPv6 traffic and routes will be exchanged as well.
+                    "IPV4_ONLY" - This Peering will only allow IPv4 traffic and routes to be exchanged, even if the matching peering is IPV4_IPV6.
+
+        id(str, Optional): The unique identifier for the resource. This identifier is defined by the server. Read-only property
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
@@ -137,311 +148,295 @@
         "result": True,
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
+    resource_type_camel = hub.tool.gcp.case.camel(RESOURCE_TYPE_FULL.split(".")[-1])
 
-    # Get the resource_id from ESM
-    if not resource_id:
-        resource_id = (ctx.get("old_state") or {}).get(
-            "resource_id"
-        ) or hub.tool.gcp.resource_prop_utils.construct_resource_id(
-            "compute.network", {**locals(), "network": name}
+    if hub.tool.gcp.resource_prop_utils.properties_mismatch_resource_id(
+        RESOURCE_TYPE, resource_id, {**locals(), resource_type_camel: name}
+    ):
+        result["comment"].append(
+            hub.tool.gcp.comment_utils.properties_mismatch_resource_id_comment(
+                RESOURCE_TYPE_FULL, name
+            )
         )
 
-    old = None
-
     if ctx.get("rerun_data"):
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, ctx.get("rerun_data"), "compute.network"
         )
 
         if not handle_operation_ret["result"]:
             result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
+            if handle_operation_ret.get("rerun_data"):
+                result["rerun_data"] = handle_operation_ret["rerun_data"]
+                if handle_operation_ret["rerun_data"].get("has_error", False):
+                    result["result"] = False
+            else:
+                result["result"] = False
+
             return result
 
         resource_id = handle_operation_ret["resource_id"]
 
+    get_resource_only_with_resource_id = hub.OPT.idem.get(
+        "get_resource_only_with_resource_id", False
+    )
     if resource_id:
-        old_get_ret = await hub.exec.gcp_api.client.compute.network.get(
-            ctx, name=name, resource_id=resource_id
+        old_get_ret = await hub.exec.gcp.compute.network.get(
+            ctx, resource_id=resource_id
         )
 
-        if not old_get_ret["result"]:
-            # error other than non-existing resource
+        if not old_get_ret["result"] or (
+            not old_get_ret["ret"] and get_resource_only_with_resource_id
+        ):
             result["result"] = False
             result["comment"] += old_get_ret["comment"]
             return result
 
-        if old_get_ret["ret"]:
-            # resource already exists
+        # long running operation has succeeded - both update and create
+        if ctx.get("rerun_data"):
+            result["new_state"] = old_get_ret["ret"]
+            result["old_state"] = ctx["rerun_data"]["old_state"]
+            if ctx["rerun_data"]["old_state"]:
+                result["comment"].append(
+                    hub.tool.gcp.comment_utils.update_comment(
+                        "gcp.compute.network", name
+                    )
+                )
+            else:
+                result["comment"].append(
+                    hub.tool.gcp.comment_utils.create_comment(
+                        "gcp.compute.network", name
+                    )
+                )
+                # Handle the peerings addition when new network is created
+                if not result["new_state"].get("peerings") and peerings:
+                    add_peerings_ret = await hub.tool.gcp.compute.network.add_peerings(
+                        ctx, resource_id, peerings
+                    )
+                    if not add_peerings_ret["result"]:
+                        result["result"] = False
+                        result["comment"] += add_peerings_ret["comment"]
+                        return result
+
+                # Make a new get request containing the peerings in their form in gcp api
+                get_ret = await hub.exec.gcp_api.client.compute.network.get(
+                    ctx, name=name, resource_id=resource_id
+                )
+                if not get_ret["result"] and not get_ret["ret"]:
+                    result["result"] = False
+                    result["comment"] += get_ret["comment"]
+                    return result
+                result["new_state"] = get_ret["ret"]
 
-            # copy.copy(old_get_ret['ret']) is needed to convert any objects of type NamespaceDict to dict
-            # in old_get_ret['ret']. This is done so that comparisons with the plan_state which has
-            # objects of type dict works properly
-            old = copy.deepcopy(copy.copy(old_get_ret["ret"]))
-            result["old_state"] = old
+            return result
 
-        # do not return here even after fetching network post operation return,
-        # as there are further update operations below which might need to run
+        result["old_state"] = old_get_ret["ret"]
+    elif not get_resource_only_with_resource_id:
+        resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
+            "compute.network", {**locals(), "network": name}
+        )
+        old_get_ret = await hub.exec.gcp.compute.network.get(
+            ctx, resource_id=resource_id
+        )
+        if not old_get_ret["result"]:
+            result["result"] = False
+            result["comment"] += old_get_ret["comment"]
+            return result
+
+        if old_get_ret["ret"]:
+            result["old_state"] = old_get_ret["ret"]
 
     request_body = {
         "name": name,
         "description": description,
         "auto_create_subnetworks": auto_create_subnetworks,
         "enable_ula_internal_ipv6": enable_ula_internal_ipv6,
         "internal_ipv6_range": internal_ipv6_range,
         "i_pv4_range": i_pv4_range,
         "mtu": mtu,
         "network_firewall_policy_enforcement_order": network_firewall_policy_enforcement_order,
         "routing_config": routing_config,
         "peerings": peerings,
+        "id_": id_,
     }
 
     request_body = {k: v for (k, v) in request_body.items() if v is not None}
     operation = None
-    if old:
-        new_state_for_whole_resource_comparison = {
-            "resource_id": resource_id,
-            **request_body,
-        }
-        if hasattr(old, "peerings"):
-            new_state_for_whole_resource_comparison["peerings"] = old.get("peerings")
-        else:
-            new_state_for_whole_resource_comparison.pop("peerings", None)
-
+    if result["old_state"]:
         changes = hub.tool.gcp.utils.compare_states(
-            old, new_state_for_whole_resource_comparison, "compute.network"
+            result["old_state"],
+            request_body,
+            "compute.network",
         )
-        are_peerings_changed = (
-            not hub.tool.gcp.state_comparison_utils.are_lists_identical(
-                old.get("peerings"), peerings
+        if changes:
+            changed_non_updatable_properties = (
+                hub.tool.gcp.resource_prop_utils.get_changed_non_updatable_properties(
+                    "compute.network", changes
+                )
             )
+            if changed_non_updatable_properties:
+                result["result"] = False
+                result["comment"].append(
+                    hub.tool.gcp.comment_utils.non_updatable_properties_comment(
+                        "gcp.compute.network",
+                        name,
+                        changed_non_updatable_properties,
+                    )
+                )
+                result["new_state"] = result["old_state"]
+                return result
+
+        peerings = hub.tool.gcp.compute.network.build_new_peerings_on_top_of_old(
+            result["old_state"].get("peerings"), peerings
         )
 
-        if not changes and not are_peerings_changed:
+        # We want to make sure that the network in the current and new peerings have the same format.
+        for peering in result["old_state"].get("peerings", []):
+            peering[
+                "network"
+            ] = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
+                peering["network"], "compute.network"
+            )
+        for peering in peerings or []:
+            peering[
+                "network"
+            ] = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
+                peering["network"], "compute.network"
+            )
+
+        peerings_changes = None
+        if peerings is not None:
+            request_body["peerings"] = peerings
+            peerings_changes = hub.tool.gcp.utils.compare_states(
+                {"peerings": result["old_state"].get("peerings") or []},
+                {"peerings": peerings},
+                resource_type=None,
+                additional_exclude_paths=[
+                    "peerings[].peer_mtu",
+                    "peerings[].auto_create_routes",
+                ],
+            )
+
+        if not changes and not peerings_changes:
             result["result"] = True
             result["comment"].append(
-                hub.tool.gcp.comment_utils.already_exists_comment(
+                hub.tool.gcp.comment_utils.up_to_date_comment(
                     "gcp.compute.network", name
                 )
             )
             result["new_state"] = result["old_state"]
             return result
 
         if ctx["test"]:
             result["comment"].append(
                 hub.tool.gcp.comment_utils.would_update_comment(
                     "gcp.compute.network", name
                 )
             )
-            result["new_state"] = request_body
-            result["new_state"]["resource_id"] = resource_id
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                {"resource_id": resource_id, **request_body}
+            )
             return result
 
-        if are_peerings_changed:
+        if peerings_changes:
             update_peerings_ret = await hub.tool.gcp.compute.network.update_peerings(
-                ctx, resource_id, old.get("peerings"), peerings
+                ctx, resource_id, result["old_state"].get("peerings"), peerings
             )
             if not update_peerings_ret["result"]:
                 result["result"] = False
-                result["comment"].append(update_peerings_ret["comment"])
+                result["comment"] += update_peerings_ret["comment"]
                 return result
 
         if changes:
-            if are_peerings_changed:
+            if peerings_changes:
                 get_ret = await hub.exec.gcp.compute.network.get(
                     ctx, resource_id=resource_id
                 )
                 if not get_ret["result"] and not get_ret["ret"]:
                     result["result"] = False
                     result["comment"] += get_ret["comment"]
                     return result
 
-                # The network interfaces should be the same so update does not happen there
+                # The peerings should be the same so update does not happen there
                 request_body["peerings"] = get_ret["ret"].get("peerings")
 
             patch_ret = await hub.exec.gcp_api.client.compute.network.patch(
                 ctx, resource_id=resource_id, body=request_body
             )
 
             if not patch_ret["result"]:
                 result["result"] = False
-                result["comment"].append(patch_ret["comment"])
+                result["comment"] += patch_ret["comment"]
                 return result
             if patch_ret["ret"] is not None:
-                if "compute#operation" in patch_ret["ret"].get("kind"):
+                if hub.tool.gcp.operation_utils.is_operation(patch_ret["ret"]):
                     operation = patch_ret["ret"]
 
+        get_ret = await hub.exec.gcp.compute.network.get(ctx, resource_id=resource_id)
+        if not get_ret["result"] and not get_ret["ret"]:
+            result["result"] = False
+            result["comment"] += get_ret["comment"]
+            return result
+
+        result["new_state"] = get_ret["ret"]
         result["comment"].append(
             hub.tool.gcp.comment_utils.update_comment("gcp.compute.network", name)
         )
     else:
         if ctx["test"]:
             result["comment"].append(
                 hub.tool.gcp.comment_utils.would_create_comment(
                     "gcp.compute.network", name
                 )
             )
-            result["new_state"] = request_body
-            result["new_state"]["resource_id"] = resource_id
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                {"resource_id": resource_id, **request_body}
+            )
             return result
 
-        # Create
         create_ret = await hub.exec.gcp_api.client.compute.network.insert(
             ctx, name=name, project=project, body=request_body
         )
-        if not create_ret["result"]:
+        if not create_ret["result"] or not create_ret["ret"]:
             result["result"] = False
-            result["comment"] += create_ret["comment"]
+            if create_ret["comment"] and next(
+                (
+                    comment
+                    for comment in create_ret["comment"]
+                    if "alreadyExists" in comment
+                ),
+                None,
+            ):
+                result["comment"].append(
+                    hub.tool.gcp.comment_utils.already_exists_comment(
+                        "gcp.compute.network", name
+                    )
+                )
+            else:
+                result["comment"] += create_ret["comment"]
             return result
 
-        result["old_state"] = {}
-        resource_id = create_ret["ret"].get("resource_id")
-        if "compute#operation" in create_ret["ret"].get("kind"):
+        if hub.tool.gcp.operation_utils.is_operation(create_ret.get("ret")):
             operation = create_ret["ret"]
 
     if operation:
         operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
             operation.get("selfLink"), "compute.global_operation"
         )
-        handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, operation_id, "compute.network"
-        )
-
-        if not handle_operation_ret["result"]:
-            result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
-            return result
-
-        resource_id = handle_operation_ret["resource_id"]
-
-    # Try getting the resource again
-    # TODO: Reconciliation or waiter loop?
-    # TODO: Check if this can be removed because insert and update may also return the necessary data on success
-    get_ret = await hub.exec.gcp_api.client.compute.network.get(
-        ctx, name=name, resource_id=resource_id
-    )
-    if not get_ret["result"] and not get_ret["ret"]:
-        result["result"] = False
-        result["comment"] += get_ret["comment"]
-        return result
-    result["new_state"] = get_ret["ret"]
-
-    # Handle the peerings addition when new network is created
-    if not result["new_state"].get("peerings") and peerings:
-        add_peerings_ret = await hub.tool.gcp.compute.network.add_peerings(
-            ctx, resource_id, peerings
-        )
-        if not add_peerings_ret["result"]:
-            result["result"] = False
-            result["comment"] += add_peerings_ret["comment"]
-            return result
-
-    # Make a new get request containing the peerings in their form in gcp api
-    get_ret = await hub.exec.gcp_api.client.compute.network.get(
-        ctx, name=name, resource_id=resource_id
-    )
-    if not get_ret["result"] and not get_ret["ret"]:
-        result["result"] = False
-        result["comment"] += get_ret["comment"]
-        return result
-    result["new_state"] = get_ret["ret"]
-    return result
-
-
-async def absent(
-    hub,
-    ctx,
-    name: str = None,
-    resource_id: str = None,
-    request_id: str = None,
-) -> Dict[str, Any]:
-    r"""Deletes the specified network.
-
-    Args:
-        name(str):
-            An Idem name of the resource.
-
-        resource_id(str, Optional):
-            An identifier of the resource in the provider. Defaults to None.
-
-        request_id(str, Optional):
-            An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
-
-    Returns:
-        Dict[str, Any]
-
-    Examples:
-        .. code-block:: sls
-
-            my-network:
-              gcp.compute.network.absent:
-                - resource_id: projects/project-name/global/networks/my-network
-
-    """
-    result = {
-        "comment": [],
-        "old_state": ctx.get("old_state"),
-        "new_state": None,
-        "name": name,
-        "result": True,
-    }
-
-    if not resource_id:
-        resource_id = (ctx.old_state or {}).get("resource_id")
-
-    if ctx.test:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.would_delete_comment("gcp.compute.network", name)
-        )
-        return result
-
-    if not ctx.get("rerun_data"):
-        # First iteration; invoke instance's delete()
-        delete_ret = await hub.exec.gcp_api.client.compute.network.delete(
-            ctx, resource_id=resource_id
-        )
-        if delete_ret["ret"]:
-            if "compute#operation" in delete_ret["ret"].get("kind"):
-                result["result"] = False
-                result["comment"] += delete_ret["comment"]
-                result[
-                    "rerun_data"
-                ] = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                    delete_ret["ret"].get("selfLink"), "compute.global_operation"
-                )
-                return result
-
-    else:
-        # delete() has been called on some previous iteration
-        handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, ctx.get("rerun_data"), "compute.network"
-        )
-        if not handle_operation_ret["result"]:
-            result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
-            return result
-
-        resource_id = handle_operation_ret["resource_id"]
-
-    if not resource_id:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.already_absent_comment(
-                "gcp.compute.network", name
-            )
-        )
+        result["rerun_data"] = {
+            "operation_id": operation_id,
+            "old_state": result["old_state"],
+        }
 
-    result["comment"].append(
-        hub.tool.gcp.comment_utils.delete_comment("gcp.compute.network", name)
-    )
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
     r"""Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
     Retrieves the list of networks available to the specified project.
@@ -464,22 +459,23 @@
 
     if not describe_ret["result"]:
         hub.log.debug(
             f"Could not describe gcp.compute.network {describe_ret['comment']}"
         )
         return {}
 
-    for resource in describe_ret["ret"]["items"]:
+    for resource in describe_ret["ret"].get("items", []):
         resource_id = resource.get("resource_id")
 
         result[resource_id] = {
             "gcp.compute.network.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
 
     return result
 
 
 def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
+    """Default implemented for each module."""
     return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/node_template.py` & `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/node_template.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """State module for managing Node Templates."""
 from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 
+from idem_gcp.tool.gcp.utils import regional_absent
+
+# prevent commit hook from removing the import
+absent = regional_absent
 
 __contracts__ = ["resource"]
 
 
 async def present(
     hub,
     ctx,
@@ -109,112 +113,23 @@
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
     # TODO uncomment below line, when implementation is added
-    # project = get_project_from_account(ctx, project)
+    # project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     result["comment"].append(
         "No-op: There is no create/update function for gcp.compute.node_template"
     )
 
     return result
 
 
-async def absent(
-    hub,
-    ctx,
-    name: str = None,
-    resource_id: str = None,
-    request_id: str = None,
-) -> Dict[str, Any]:
-    r"""Deletes the specified network.
-
-    Args:
-        name(str):
-            An Idem name of the resource.
-
-        resource_id(str, Optional):
-            An identifier of the resource in the provider. Defaults to None.
-
-        request_id(str, Optional):
-            An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
-
-    Returns:
-        Dict[str, Any]
-
-    Examples:
-        .. code-block:: sls
-
-            delete-my-node-template:
-              gcp.compute.node_template.absent:
-                - resource_id: projects/project-name/regions/europe-west2/node_templates/node_template-123
-    """
-    result = {
-        "comment": [],
-        "old_state": ctx.get("old_state"),
-        "new_state": None,
-        "name": name,
-        "result": True,
-    }
-
-    if not resource_id:
-        resource_id = (ctx.old_state or {}).get("resource_id")
-
-    if ctx.test:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.would_delete_comment(
-                "gcp.compute.node_template", name
-            )
-        )
-        return result
-
-    if not ctx.get("rerun_data"):
-        # First iteration; invoke instance's delete()
-        delete_ret = await hub.exec.gcp_api.client.compute.node_template.delete(
-            ctx, resource_id=resource_id
-        )
-        if delete_ret["ret"]:
-            if "compute#operation" in delete_ret["ret"].get("kind"):
-                result["result"] = False
-                result["comment"] += delete_ret["comment"]
-                result[
-                    "rerun_data"
-                ] = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                    delete_ret["ret"].get("selfLink"), "compute.region_operation"
-                )
-                return result
-
-    else:
-        # delete() has been called on some previous iteration
-        handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, ctx.get("rerun_data"), "compute.node_template"
-        )
-        if not handle_operation_ret["result"]:
-            result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
-            return result
-
-        resource_id = handle_operation_ret["resource_id"]
-
-    if not resource_id:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.already_absent_comment(
-                "gcp.compute.node_template", name
-            )
-        )
-
-    result["comment"].append(
-        hub.tool.gcp.comment_utils.delete_comment("gcp.compute.node_template", name)
-    )
-    return result
-
-
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
     r"""Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
     Retrieves an aggregated list of node templates.
 
     Returns:
         Dict[str, Dict[str, Any]]
@@ -233,22 +148,23 @@
 
     if not describe_ret["result"]:
         hub.log.debug(
             f"Could not describe gcp.compute.node_template {describe_ret['comment']}"
         )
         return {}
 
-    for resource in describe_ret["ret"]["items"]:
+    for resource in describe_ret["ret"].get("items", []):
         resource_id = resource.get("resource_id")
 
         result[resource_id] = {
             "gcp.compute.node_template.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
 
     return result
 
 
 def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
+    """Default implemented for each module."""
     return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/reservation.py` & `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/target_pool.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,253 +1,177 @@
-"""State module for managing Reservations."""
-from dataclasses import field
-from dataclasses import make_dataclass
+"""State module for managing target tools."""
 from typing import Any
 from typing import Dict
 from typing import List
 
-
 __contracts__ = ["resource"]
 
 
 async def present(
     hub,
     ctx,
     name: str,
-    resource_id: str = None,
-    request_id: str = None,
+    region: str = None,
     project: str = None,
-    zone: str = None,
+    instances: List[str] = None,
+    session_affinity: str = None,
     description: str = None,
-    share_settings: make_dataclass(
-        "ShareSettings",
-        [
-            (
-                "project_map",
-                make_dataclass(
-                    "ShareSettingsProjectConfig",
-                    [("project_id", str, field(default=None))],
-                ),
-                field(default=None),
-            ),
-            ("share_type", str, field(default="LOCAL")),
-        ],
-    ) = None,
-    specific_reservation: make_dataclass(
-        "AllocationSpecificSKUReservation",
-        [
-            ("count", str, field(default=None)),
-            (
-                "instance_properties",
-                make_dataclass(
-                    "AllocationSpecificSKUAllocationReservedInstanceProperties",
-                    [
-                        ("machine_type", str, field(default=None)),
-                        (
-                            "local_ssds",
-                            List[
-                                make_dataclass(
-                                    "AllocationSpecificSKUAllocationAllocatedInstancePropertiesReservedDisk",
-                                    [
-                                        ("disk_size_gb", str, field(default=None)),
-                                        ("interface", str, field(default=None)),
-                                    ],
-                                )
-                            ],
-                            field(default=None),
-                        ),
-                        ("location_hint", str, field(default=None)),
-                        ("guest_accelerators", str, field(default=None)),
-                        ("min_cpu_platform", str, field(default=None)),
-                    ],
-                ),
-                field(default=None),
-            ),
-        ],
-    ) = None,
-    specific_reservation_required: bool = False,
+    failover_ratio: float = None,
+    health_checks: List[str] = None,
+    backup_pool: str = None,
+    request_id: str = None,
+    resource_id: str = None,
 ) -> Dict[str, Any]:
-    r"""Creates a new reservation. For more information, read Reserving zonal resources.
+    r"""Creates a target pool in the specified project and region using the data included in the request.
 
     Args:
-        name(str):
+        name (str):
             An Idem name of the resource.
-
-        request_id(str, Optional):
-            An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
-
+        instances (List[str], Optional):
+            A list of resource URLs to the virtual machine instances serving this pool. They must live in zones contained in the same region as this pool. Defaults to None.
+        session_affinity (str, Optional):
+            Session affinity option, must be one of the following values:
+            NONE: Connections from the same client IP may go to any instance in the pool.
+            CLIENT_IP: Connections from the same client IP will go to the same instance in the pool while that instance remains healthy.
+            CLIENT_IP_PROTO: Connections from the same client IP with the same IP protocol will go to the same instance in the pool while that instance remains healthy.
+        description (str, Optional):
+            An optional description of this resource. Provide this property when you create the resource. Defaults to None.
+        region(str, Optional):
+            Name of the region scoping this request.
+        failover_ratio(float, Optional):
+            This field is applicable only when the containing target pool is serving a forwarding rule as the primary pool (i.e., not as a backup pool to some other target pool). The value of the field must be in [0, 1]. If set, backupPool must also be set. They together define the fallback behavior of the primary target pool: if the ratio of the healthy instances in the primary pool is at or below this number, traffic arriving at the load-balanced IP will be directed to the backup pool. In case where failoverRatio is not set or all the instances in the backup pool are unhealthy, the traffic will be directed back to the primary pool in the "force" mode, where traffic will be spread to the healthy instances with the best effort, or to all instances when no instance is healthy. Defaults to None.
+        health_checks(List[str], Optional):
+            The URL of the HttpHealthCheck resource. A member instance in this pool is considered healthy if and only if the health checks pass. Only legacy HttpHealthChecks are supported. Only one health check may be specified. Defaults to None.
+        backup_pool(str, Optional):
+            The server-defined URL for the resource. This field is applicable only when the containing target pool is serving a forwarding rule as the primary pool, and its failoverRatio field is properly set to a value between [0, 1]. backupPool and failoverRatio together define the fallback behavior of the primary target pool: if the ratio of the healthy instances in the primary pool is at or below failoverRatio, traffic arriving at the load-balanced IP will be directed to the backup pool. In case where failoverRatio and backupPool are not set, or all the instances in the backup pool are unhealthy, the traffic will be directed back to the primary pool in the "force" mode, where traffic will be spread to the healthy instances with the best effort, or to all instances when no instance is healthy. Defaults to None.
         project(str, Optional):
             Project ID for this request.
-
-        zone(str, Optional):
-            Name of the zone for this request.
-
-        description(str, Optional):
-            An optional description of this resource. Provide this field when you create the resource. Defaults to None.
-
-        share_settings(ShareSettings, Optional):
-            Share-settings for shared-reservation
-
-        specific_reservation(AllocationSpecificSKUReservation, Optional):
-            Reservation for instances with specific machine shapes.
-
-        specific_reservation_required(bool, Optional):
-            Indicates whether the reservation can be consumed by VMs with affinity for \"any\" reservation. If the field is set, then only VMs that target the reservation by name can consume from this reservation.
-
+        request_id(str, Optional):
+            An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
+            resource_is_present:
+              gcp.compute.target_pool.present:
+                - name: value
+                - region: value
+                - project: value
     """
     result = {
         "result": True,
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
     # TODO uncomment below line, when implementation is added
-    # project = get_project_from_account(ctx, project)
+    # project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     result["comment"].append(
-        "No-op: There is no create/update function for gcp.compute.reservation"
+        hub.tool.gcp.comment_utils.no_resource_create_update_comment(
+            "gcp.compute.target_pool"
+        )
     )
 
     return result
 
 
 async def absent(
     hub,
     ctx,
-    name: str = None,
-    resource_id: str = None,
+    name: str,
+    project: str = None,
+    region: str = None,
     request_id: str = None,
+    resource_id: str = None,
 ) -> Dict[str, Any]:
-    r"""Deletes the specified reservation.
+    r"""Deletes the specified target pool.
 
     Args:
-        name(str):
-            An Idem name of the resource.
-
-        resource_id(str, Optional):
-            An identifier of the resource in the provider. Defaults to None.
-
-        request_id(str, Optional):
+        name (str): An Idem name of the resource.
+        project(str, Optional):
+            Project ID for this request.
+        region (str, Optional):
+            Name of the region scoping this request.
+        request_id (str, Optional):
             An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
+        resource_id (str, Optional):
+            An identifier of the resource in the provider. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
-            my-reservation:
-              gcp.compute.reservation.absent:
-                - resource_id: projects/project-name/zones/us-central1-a/reservations/my-reservation
+            resource_is_absent:
+              gcp.compute.target_pool.absent:
+                - name: value
+                - project: value
+                - region: value
     """
     result = {
-        "comment": [],
-        "old_state": ctx.get("old_state"),
+        "result": True,
+        "old_state": None,
         "new_state": None,
         "name": name,
-        "result": True,
+        "comment": [],
     }
 
-    if not resource_id:
-        resource_id = (ctx.old_state or {}).get("resource_id")
-
-    if ctx.test:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.would_delete_comment(
-                "gcp.compute.reservation", name
-            )
-        )
-        return result
-
-    if not ctx.get("rerun_data"):
-        # First iteration; invoke reservation's delete()
-        delete_ret = await hub.exec.gcp_api.client.compute.reservation.delete(
-            ctx, resource_id=resource_id
-        )
-        if delete_ret["ret"]:
-            if "compute#operation" in delete_ret["ret"].get("kind"):
-                result["result"] = False
-                result["comment"] += delete_ret["comment"]
-                result[
-                    "rerun_data"
-                ] = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                    delete_ret["ret"].get("selfLink"), "compute.zone_operation"
-                )
-                return result
-
-    else:
-        # delete() has been called on some previous iteration
-        handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, ctx.get("rerun_data"), "compute.reservation"
-        )
-        if not handle_operation_ret["result"]:
-            result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
-            return result
-
-        resource_id = handle_operation_ret["resource_id"]
-
-    if not resource_id:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.already_absent_comment(
-                "gcp.compute.reservation", name
-            )
-        )
+    # TODO uncomment below line, when implementation is added
+    # project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     result["comment"].append(
-        hub.tool.gcp.comment_utils.delete_comment("gcp.compute.reservation", name)
+        hub.tool.gcp.comment_utils.no_resource_delete_comment("gcp.compute.target_pool")
     )
+
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
     r"""Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
-    Retrieves a list of all the reservations that have been configured for the specified project in specified zone.
+    Retrieves a list of target pools available to the specified project and region.
 
     Returns:
-        Dict[str, Dict[str, Any]]
+        Dict[str, Any]
 
     Examples:
         .. code-block:: bash
 
-            $ idem describe gcp.compute.reservation
+            $ idem describe gcp.compute.target_pool
     """
     result = {}
 
     # TODO: Pagination
-    describe_ret = await hub.exec.gcp_api.client.compute.reservation.aggregatedList(
+    describe_ret = await hub.exec.gcp.compute.target_pool.list(
         ctx, project=ctx.acct.project_id
     )
 
     if not describe_ret["result"]:
         hub.log.debug(
-            f"Could not describe gcp.compute.reservation {describe_ret['comment']}"
+            f"Could not describe gcp.compute.target_pool {describe_ret['comment']}"
         )
         return {}
 
-    for resource in describe_ret["ret"]["items"]:
+    for resource in describe_ret["ret"]:
         resource_id = resource.get("resource_id")
-
         result[resource_id] = {
-            "gcp.compute.reservation.present": [
+            "gcp.compute.target_pool.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
 
     return result
 
 
 def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
+    """Default implemented for each module."""
     return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/resource_policy.py` & `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/disk.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,449 +1,375 @@
-"""State module for managing Resource Policies."""
-from dataclasses import field
-from dataclasses import make_dataclass
-from typing import Any
-from typing import Dict
-from typing import List
+"""Exec module for managing Disks."""
+__func_alias__ = {"list_": "list"}
 
+from dataclasses import make_dataclass, field
+from typing import Dict, Any, List
 
-__contracts__ = ["resource"]
+from idem_gcp.tool.gcp.generate.exec_context import ExecutionContext
 
 
-async def present(
+async def list_(
     hub,
     ctx,
-    name: str = None,
     project: str = None,
+    zone: str = None,
     region: str = None,
-    resource_id: str = None,
-    description: str = None,
-    snapshot_schedule_policy: make_dataclass(
-        "ResourcePolicySnapshotSchedulePolicy",
-        [
-            (
-                "schedule",
-                make_dataclass(
-                    "ResourcePolicySnapshotSchedulePolicySchedule",
-                    [
-                        (
-                            "daily_schedule",
-                            make_dataclass(
-                                "ResourcePolicyDailyCycle",
-                                [
-                                    ("days_in_cycle", int, field(default=0)),
-                                    ("start_time", str, field(default=None)),
-                                ],
-                            ),
-                            field(default=None),
-                        ),
-                        (
-                            "weekly_schedule",
-                            make_dataclass(
-                                "ResourcePolicyWeeklyCycle",
-                                [
-                                    (
-                                        "day_of_weeks",
-                                        List[
-                                            make_dataclass(
-                                                "ResourcePolicyWeeklyCycleDayOfWeek",
-                                                [
-                                                    (
-                                                        "start_time",
-                                                        str,
-                                                        field(default=None),
-                                                    ),
-                                                    ("day", str, field(default=None)),
-                                                ],
-                                            )
-                                        ],
-                                        field(default=None),
-                                    ),
-                                ],
-                            ),
-                            field(default=None),
-                        ),
-                        (
-                            "hourly_schedule",
-                            make_dataclass(
-                                "ResourcePolicyHourlyCycle",
-                                [
-                                    ("hours_in_cycle", int, field(default=0)),
-                                    ("start_time", str, field(default=None)),
-                                ],
-                            ),
-                            field(default=None),
-                        ),
-                    ],
-                ),
-                field(default=None),
-            ),
-            (
-                "retention_policy",
-                make_dataclass(
-                    "ResourcePolicySnapshotSchedulePolicyRetentionPolicy",
-                    [
-                        ("max_retention_days", int, field(default=0)),
-                        ("on_source_disk_delete", str, field(default=None)),
-                    ],
-                ),
-                field(default=None),
-            ),
-            (
-                "snapshotProperties",
-                make_dataclass(
-                    "ResourcePolicySnapshotSchedulePolicySnapshotProperties",
-                    [
-                        ("guest_flush", bool, field(default=False)),
-                        ("chain_name", str, field(default=None)),
-                        ("storage_locations", List[str], field(default=None)),
-                        ("labels", Dict[str, str], field(default=None)),
-                    ],
-                ),
-                field(default=None),
-            ),
-        ],
-    ) = None,
-    group_placement_policy: make_dataclass(
-        "ResourcePolicyGroupPlacementPolicy",
-        [
-            ("vm_count", int, field(default=0)),
-            ("collocation", str, field(default=None)),
-            ("availability_domain_count", int, field(default=0)),
-        ],
-    ) = None,
-    instance_schedule_policy: make_dataclass(
-        "ResourcePolicyInstanceSchedulePolicy",
-        [
-            ("start_time", str, field(default=None)),
-            ("time_zone", str, field(default=None)),
-            ("expiration_time", str, field(default=None)),
-            (
-                "vm_start_schedule",
-                make_dataclass(
-                    "ResourcePolicyInstanceSchedulePolicySchedule",
-                    [
-                        ("schedule", str, field(default=None)),
-                    ],
-                ),
-                field(default=None),
-            ),
-            (
-                "vm_stop_schedule",
-                make_dataclass(
-                    "ResourcePolicyInstanceSchedulePolicySchedule",
-                    [
-                        ("schedule", str, field(default=None)),
-                    ],
-                ),
-                field(default=None),
-            ),
-        ],
-    ) = None,
-) -> Dict[str, Any]:
-    r"""Creates a new resource policy.
-
-    You can use resource policies to schedule actions for some Compute Engine resources.
-    For example, you can use them to schedule persistent disk snapshots.
+    filter_: (str, "alias=filter") = None,
+    order_by: str = None,
+):
+    r"""Retrieves a list of persistent disks.
 
     Args:
-        name(str, Optional):
-            An Idem name of the resource.
-
         project(str, Optional):
-            Project ID for this request. Defaults to None.
-
-        region(str, Optional):
-            Name of the region for this request. Defaults to None.
-
-        resource_id(str, Optional):
-            An identifier of the resource in the provider. Defaults to None.
-
-        description(str, Optional):
-            An optional description of this resource. Defaults to None.
-
-        snapshot_schedule_policy(Dict[str, Any], Optional):
-            Resource policy for persistent disks for creating snapshots. Defaults to None.
-            A snapshot schedule policy specifies when and how frequently snapshots are to be created for
-            the target disk. Also specifies how many and how long these scheduled snapshots should be retained.
-
-            * schedule(Dict[str, Any], Optional):
-                A Vm Maintenance Policy specifies what kind of infrastructure maintenance we are allowed to perform on
-                this VM and when. Schedule that is applied to disks covered by this policy.
-                A schedule for disks where the scheduled operations are performed.
-
-                * daily_schedule(Dict[str, Any], Optional):
-                    Time window specified for daily operations.
-
-                    * days_in_cycle(int, Optional):
-                        Defines a schedule with units measured in days.
-                        The value determines how many days pass between the start of each cycle.
-
-                    * start_time(str, Optional):
-                        Start time of the window. This must be in UTC format that resolves to one of
-                        00:00, 04:00, 08:00, 12:00, 16:00, or 20:00. For example, both 13:00-5 and 08:00 are valid.
-
-                * weekly_schedule(Dict[str, Any], Optional):
-                    Time window specified for weekly operations.
-
-                    * day_of_weeks(List[Dict[str, Any]], Optional):
-                        Up to 7 intervals/windows, one for each day of the week.
-
-                        * start_time(str, Optional):
-                            Time within the window to start the operations.
-                            It must be in format \"HH:MM\", where HH : [00-23] and MM : [00-00] GMT.
-
-                        * day(str, Optional):
-                            Defines a schedule that runs on specific days of the week. Specify one or more days.
-                            The following options are available:
-                            MONDAY, TUESDAY, WEDNESDAY, THURSDAY, FRIDAY, SATURDAY, SUNDAY.
-
-                * hourly_schedule(Dict[str, Any], Optional):
-                    Time window specified for hourly operations.
-
-                    * hours_in_cycle(int, Optional):
-                        Defines a schedule with units measured in hours.
-                        The value determines how many hours pass between the start of each cycle.
-
-                    * start_time(str, Optional):
-                        Time within the window to start the operations.
-                        It must be in format \"HH:MM\", where HH : [00-23] and MM : [00-00] GMT.
-
-            * retention_policy(Dict[str, Any], Optional):
-                Retention policy applied to snapshots created by this resource policy.
-                Policy for retention of scheduled snapshots.
-
-                * max_retention_days(int, Optional):
-                    Maximum age of the snapshot that is allowed to be kept.
+            Project ID for this request.
 
-                * on_source_disk_delete(str, Optional):
-                    Specifies the behavior to apply to scheduled snapshots when the source disk is deleted.
-                    The following options are available:
-                    APPLY_RETENTION_POLICY, KEEP_AUTO_SNAPSHOTS, UNSPECIFIED_ON_SOURCE_DISK_DELETE
+        zone(str, Optional):
+            The name of the zone for this request.
 
+        region(str, Optional):
+            The name of the region for this request.
 
-            * snapshot_properties(Dict[str, Any], Optional):
-                Properties with which snapshots are created such as labels, encryption keys.
-                Specified snapshot properties for scheduled snapshots created by this policy.
-
-                * guest_flush(bool, Optional):
-                    Indication to perform a 'guest aware' snapshot.
-
-                * chain_name(str, Optional):
-                    Chain name that the snapshot is created in.
-
-                * storage_locations(List[str, str], Optional):
-                    Cloud Storage bucket storage location of the auto snapshot (regional or multi-regional).
+        filter(str, Optional):
+            A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name "instance", you would use `name ne .*instance`.
 
-                * labels(List[str, str], Optional):
-                    Labels to apply to scheduled snapshots. These can be later modified by the setLabels method.
-                    Label values may be empty.
+        order_by(str, Optional):
+            Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
 
-        group_placement_policy(Dict[str, Any], Optional):
-            Resource policy for instances for placement configuration. Defaults to None.
-            A GroupPlacementPolicy specifies resource placement configuration.
-            It specifies the failure bucket separation as well as network locality
+    Examples:
+        .. code-block:: sls
 
-            * vm_count(int, Optional):
-                Number of VMs in this placement group. Google does not recommend that you use this field unless
-                you use a compact policy, and you want your policy to work only if it contains this exact number of VMs.
+            random-name:
+              exec.run:
+              - path: gcp.compute.disk.list
+              - kwargs:
+                  project: project-name
+                  zone: zone-name
+    """
+    result = {
+        "comment": [],
+        "ret": None,
+        "result": True,
+    }
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
-            * collocation(str, Optional):
-                Specifies network collocation. The following options are available:
-                COLLOCATED, UNSPECIFIED_COLLOCATION
+    if zone:
+        ret = await hub.exec.gcp_api.client.compute.disk.list(
+            ctx,
+            project=project,
+            zone=zone,
+            filter=filter_,
+            orderBy=order_by,
+        )
+    elif region:
+        ret = await hub.exec.gcp_api.client.compute.disk.list(
+            ctx,
+            project=project,
+            region=region,
+            filter=filter_,
+            orderBy=order_by,
+        )
+    else:
+        ret = await hub.exec.gcp_api.client.compute.disk.aggregatedList(
+            ctx,
+            project=project,
+            filter=filter_,
+            orderBy=order_by,
+        )
 
-            * availability_domain_count(int, Optional):
-                The number of availability domains to spread instances across.
-                If two instances are in different availability domain, they are not in the same low latency network.
+    if not ret["result"]:
+        result["comment"] += ret["comment"]
+        result["result"] = False
+        return result
 
-        instance_schedule_policy(Dict[str, Any], Optional):
-            Resource policy for scheduling instance operations. Defaults to None.
-            An InstanceSchedulePolicy specifies when and how frequent certain operations are performed on the instance.
+    result["ret"] = ret["ret"].get("items", [])
+    return result
 
-            * start_time(str, Optional):
-                The start time of the schedule. The timestamp is an RFC3339 string.
 
-            * time_zone(str, Optional):
-                Specifies the time zone to be used in interpreting Schedule.schedule.
-                The value of this field must be a time zone name from the tz database:
-                http://en.wikipedia.org/wiki/Tz_database.
+async def get(
+    hub,
+    ctx,
+    project: str = None,
+    zone: str = None,
+    region: str = None,
+    name: str = None,
+    resource_id: str = None,
+):
+    r"""Returns a specified persistent disk.
 
-            * expiration_time(str, Optional):
-                The expiration time of the schedule. The timestamp is an RFC3339 string.
+    Use an un-managed disk as a data-source. Supply one of the inputs as the filter.
+    Gets a list of available persistent disks by making a list() request.
 
-            * vm_start_schedule(Dict[str, Any], Optional):
-                Specifies the schedule for starting instances.
+    Args:
+        project(str, Optional):
+            Project ID for this request. Defaults to None.
 
-                * schedule(str, Optional):
-                    Specifies the frequency for the operation, using the unix-cron format.
+        zone(str, Optional):
+            The name of the zone for this request. Defaults to None.
 
-            * vm_stop_schedule(Dict[str, Any], Optional):
-                Specifies the schedule for stopping instances.
+        region(str, Optional):
+            The name of the region for this request. Defaults to None.
 
-                * schedule(str, Optional):
-                    Specifies the frequency for the operation, using the unix-cron format.
+        name(str, Optional):
+            Name of the persistent disk to return. Defaults to None.
 
-    Returns:
-        Dict[str, Any]
+        resource_id(str, Optional):
+            An identifier of the resource in the provider. Defaults to None.
 
     Examples:
         .. code-block:: sls
 
-            example_resource_name:
-              gcp.compute.resource_policy.present:
-                - name: value
-                - project: value
-                - region: value
+            random-name:
+              exec.run:
+              - path: gcp.compute.disk.get
+              - kwargs:
+                  name: disk-name
+                  project: project-name
+                  zone: zone-name
     """
     result = {
-        "result": True,
-        "old_state": None,
-        "new_state": None,
-        "name": name,
         "comment": [],
+        "ret": None,
+        "result": True,
     }
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
-    # TODO uncomment below line, when implementation is added
-    # project = get_project_from_account(ctx, project)
+    if resource_id:
+        ret = await hub.exec.gcp_api.client.compute.disk.get(
+            ctx,
+            resource_id=resource_id,
+        )
+    elif project and zone and name:
+        ret = await hub.exec.gcp_api.client.compute.disk.get(
+            ctx, project=project, zone=zone, disk=name
+        )
+    elif project and region and name:
+        ret = await hub.exec.gcp_api.client.compute.disk.get(
+            ctx, project=project, region=region, disk=name
+        )
+    else:
+        result["result"] = False
+        result["comment"] = [
+            f"gcp.compute.disk#get(): {name} either resource_id or project, zone/region and name"
+            f" should be specified."
+        ]
+        return result
 
-    result["comment"].append(
-        "No-op: There is no create/update function for gcp.compute.resource_policy"
-    )
+    result["comment"] += ret["comment"]
+    if not ret["result"]:
+        result["result"] = False
+        return result
 
+    result["ret"] = ret["ret"]
     return result
 
 
-async def absent(
+async def create_snapshot(
     hub,
     ctx,
     name: str,
+    project: str = None,
+    zone: str = None,
+    region: str = None,
+    disk: str = None,
     resource_id: str = None,
+    storage_locations: List[str] = None,
+    location_hint: str = None,
+    label_fingerprint: str = None,
+    description: str = None,
+    labels: Dict[str, Any] = None,
+    source_disk_encryption_key: make_dataclass(
+        "CustomerEncryptionKey",
+        [
+            ("kms_key_service_account", str, field(default=None)),
+            ("sha256", str, field(default=None)),
+            ("rsa_encrypted_key", str, field(default=None)),
+            ("kms_key_name", str, field(default=None)),
+            ("raw_key", str, field(default=None)),
+        ],
+    ) = None,
+    source_disk: str = None,
+    chain_name: str = None,
+    snapshot_type: str = None,
+    snapshot_encryption_key: make_dataclass(
+        "CustomerEncryptionKey",
+        [
+            ("kms_key_service_account", str, field(default=None)),
+            ("sha256", str, field(default=None)),
+            ("rsa_encrypted_key", str, field(default=None)),
+            ("kms_key_name", str, field(default=None)),
+            ("raw_key", str, field(default=None)),
+        ],
+    ) = None,
     request_id: str = None,
-) -> Dict[str, Any]:
-    r"""Deletes the specified resource policy.
+):
+    r"""Creates a snapshot of a specified persistent disk. For regular snapshot creation, consider using snapshots.insert instead, as that method supports more features, such as creating snapshots in a project different from the source disk project.
 
     Args:
         name(str):
-            An Idem name of the resource.
+            Name of the resource; provided by the client when the resource is created. The name must be 1-63 characters long, and comply with RFC1035. Specifically, the name must be 1-63 characters long and match the regular expression `[a-z]([-a-z0-9]*[a-z0-9])?` which means the first character must be a lowercase letter, and all following characters must be a dash, lowercase letter, or digit, except the last character, which cannot be a dash.",
+                                "pattern": "[a-z](?:[-a-z0-9]{0,61}[a-z0-9])?
+
+        project(str, Optional):
+            Project ID for this request. Defaults to None.
+
+        zone(str, Optional):
+            The name of the zone for this request. Defaults to None.
+
+        region(str, Optional):
+            The name of the region for this request. Defaults to None.
+
+        disk(str, Optional):
+            Name of the persistent disk to snapshot.
 
         resource_id(str, Optional):
-            An identifier of the resource in the provider.
-            Defaults to None.
+            An identifier of the resource in the provider. Defaults to None.
 
         request_id(str, Optional):
-            An optional request ID to identify requests.
-            Specify a unique request ID so that if you must retry your request,
-            the server will know to ignore the request if it has already been completed.
-            For example, consider a situation where you make an initial request and the request times out.
-            If you make the request again with the same request ID,
-            the server can check if original operation with the same request ID was received, and if so,
-            will ignore the second request. This prevents clients from accidentally creating duplicate commitments.
-            The request ID must be a valid UUID with the exception that zero UUID is not supported
-            ( 00000000-0000-0000-0000-000000000000).
-            Defaults to None.
-
-    Returns:
-        Dict[str, Any]
+            An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000).
 
     Examples:
         .. code-block:: sls
 
-            resource_is_absent:
-              gcp.compute.resource_policy.absent:
-                - resource_id: resource_id
+            random-name:
+              exec.run:
+              - path: gcp.compute.disk.create_snapshot
+              - kwargs:
+                  name: snapshot-name
+                  disk: disk-name
+                  project: project-name
+                  zone: zone-name
     """
-    result = {
-        "result": True,
-        "old_state": ctx.old_state,
-        "new_state": None,
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
+
+    request_body = {
         "name": name,
-        "comment": [],
+        "storage_locations": storage_locations,
+        "location_hint": location_hint,
+        "label_fingerprint": label_fingerprint,
+        "description": description,
+        "labels": labels,
+        "source_disk_encryption_key": source_disk_encryption_key,
+        "source_disk": source_disk,
+        "chain_name": chain_name,
+        "snapshot_type": snapshot_type,
+        "snapshot_encryption_key": snapshot_encryption_key,
     }
 
-    if not resource_id:
-        resource_id = (ctx.old_state or {}).get("resource_id")
+    execution_context = ExecutionContext(
+        resource_type="compute.disk",
+        method_name="createSnapshot",
+        method_params={
+            "ctx": ctx,
+            "resource_id": resource_id,
+            "body": request_body,
+            "requestId": request_id,
+            "project": project,
+            "zone": zone,
+            "region": region,
+            "disk": disk,
+        },
+    )
+    return await hub.tool.gcp.generate.generic_exec.execute(execution_context)
 
-    if ctx.test:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.would_delete_comment(
-                "gcp.compute.resource_policy", name
-            )
-        )
-        return result
 
-    if not ctx.get("rerun_data"):
-        delete_ret = await hub.exec.gcp_api.client.compute.resource_policy.delete(
-            ctx, resource_id=resource_id
-        )
-        if delete_ret["ret"]:
-            if "compute#operation" in delete_ret["ret"].get("kind"):
-                result["result"] = False
-                result["comment"] += delete_ret["comment"]
-                result[
-                    "rerun_data"
-                ] = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                    delete_ret["ret"].get("selfLink"), "compute.zone_operation"
-                )
-                return result
-    else:
-        # delete() has been called on some previous iteration
-        handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, ctx.get("rerun_data"), "compute.resource_policy"
-        )
-        if not handle_operation_ret["result"]:
-            result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
-            return result
-
-        resource_id = handle_operation_ret["resource_id"]
-
-    if not resource_id:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.already_absent_comment(
-                "gcp.compute.resource_policy", name
-            )
-        )
-        return result
+async def create_from_snapshot(
+    hub,
+    ctx,
+    source_snapshot: str,
+    size_gb: str,
+    type_: (str, "alias=type") = None,
+    name: str = None,
+    project: str = None,
+    zone: str = None,
+    region: str = None,
+    resource_id: str = None,
+    request_id: str = None,
+):
+    r"""Create a disk from a snapshot.
 
-    result["comment"].append(
-        hub.tool.gcp.comment_utils.delete_comment("gcp.compute.resource_policy", name)
-    )
-    return result
+    If you backed up a boot or non-boot disk with a snapshot, you can create a new disk based on the snapshot.
 
+    Restrictions:
+        The new disk must be at least the same size as the original source disk for the snapshot. If you create a disk that is larger than the original source disk for the snapshot, you must resize the file system on that persistent disk to include the additional disk space. Depending on your operating system and file system type, you might need to use a different file system resizing tool. For more information, see your operating system documentation.
 
-async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r"""Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
+        You can create a new zonal disk from a given snapshot at most once every ten minutes. If you want to issue a burst of requests to snapshot your disks, you can issue at most 6 requests in 60 minutes. This limit does not apply when creating regional disks from a snapshot.
 
-    Retrieves a list of resource policies contained within the specified region.
+    Args:
+        name(str):
+            Name of the resource; provided by the client when the resource is created. The name must be 1-63 characters long, and comply with RFC1035. Specifically, the name must be 1-63 characters long and match the regular expression `[a-z]([-a-z0-9]*[a-z0-9])?` which means the first character must be a lowercase letter, and all following characters must be a dash, lowercase letter, or digit, except the last character, which cannot be a dash.",
 
-    Returns:
-        Dict[str, Any]
+            "pattern": "[a-z](?:[-a-z0-9]{0,61}[a-z0-9])?
 
-    Examples:
-        .. code-block:: bash
+        project(str, Optional):
+            Project ID for this request. Defaults to None.
 
-            $ idem describe gcp.compute.resource_policy
-    """
-    result = {}
+        zone(str, Optional):
+            The name of the zone for this request. Defaults to None.
 
-    describe_ret = await hub.exec.gcp.compute.resource_policy.list(
-        ctx, project=ctx.acct.project_id
-    )
+        region(str, Optional):
+            The name of the region for this request. Defaults to None.
 
-    if not describe_ret["result"]:
-        hub.log.debug(f"Could not describe resource policies {describe_ret['comment']}")
-        return {}
-
-    for resource in describe_ret["ret"]:
-        resource_id = resource.get("resource_id")
-        result[resource_id] = {
-            "gcp.compute.resource_policy.present": [
-                {parameter_key: parameter_value}
-                for parameter_key, parameter_value in resource.items()
-            ]
-        }
+        resource_id(str, Optional):
+            An identifier of the resource in the provider. Defaults to None.
 
-    return result
+        request_id(str, Optional):
+            An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000).
+
+        source_snapshot(str):
+            The source snapshot used to create this disk. You can provide this as a partial or full URL to the resource.
+            For example, the following are valid values:
+
+            - https://www.googleapis.com/compute/v1/projects/project/global/snapshots/snapshot
+            - projects/project/global/snapshots/snapshot
+            - global/snapshots/snapshot
+
+        size_gb(str):
+            Size, in GB, of the persistent disk.
+            You can specify this field when creating a persistent disk using the sourceImage, sourceSnapshot,
+            or sourceDisk parameter, or specify it alone to create an empty persistent disk.
+            If you specify this field along with a source, the value of sizeGb must not
+            be less than the size of the source. Acceptable values are 1 to 65536, inclusive.
+            Defaults to None.
+
+        type(str, Optional):
+            URL of the disk type resource describing which disk type to use to create the disk.
+            Provide this when creating the disk. For example: projects/project /zones/zone/diskTypes/pd-ssd.
+            See Persistent disk types.
+            Defaults to None.
 
+    Examples:
+        .. code-block:: sls
+
+            random-name:
+              exec.run:
+              - path: gcp.compute.disk.create_from_snapshot
+              - kwargs:
+                  source_snapshot: snapshot_resource_id
+                  name: restored-disk-name
+                  project: project-name
+                  zone: zone-name
+                  size_gb: disk-size
+    """
+    request_body = {
+        "type": type_,
+        "name": name,
+        "size_gb": size_gb,
+        "zone": zone,
+        "region": region,
+        "source_snapshot": source_snapshot,
+    }
+
+    execution_context = ExecutionContext(
+        resource_type="compute.disk",
+        method_name="insert",
+        method_params={
+            "ctx": ctx,
+            "resource_id": resource_id,
+            "project": project,
+            "zone": zone,
+            "region": region,
+            "body": request_body,
+            "requestId": request_id,
+        },
+    )
 
-def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
-    return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
+    return await hub.tool.gcp.generate.generic_exec.execute(execution_context)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/snapshot.py` & `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/snapshot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,66 @@
+"""State module for managing Snapshots."""
 __contracts__ = ["resource"]
 
-import copy
 from dataclasses import make_dataclass, field
 from typing import Dict, Any, List
 
-from idem_gcp.tool.gcp.utils import get_project_from_account
+from dataclasses import field
+from dataclasses import make_dataclass
+from typing import Any
+from typing import Dict
+from typing import List
+
+from idem_gcp.tool.gcp.utils import global_absent
+
+# prevent commit hook from removing the import
+absent = global_absent
+
+__contracts__ = ["resource"]
 
 
 async def present(
     hub,
     ctx,
     name: str,
     project: str = None,
     resource_id: str = None,
+    source_disk: str = None,
     storage_locations: List[str] = None,
     location_hint: str = None,
     label_fingerprint: str = None,
     description: str = None,
     labels: Dict[str, Any] = None,
     source_disk_encryption_key: make_dataclass(
         "CustomerEncryptionKey",
         [
             ("kms_key_service_account", str, field(default=None)),
-            ("sha256", str, field(default=None)),
             ("rsa_encrypted_key", str, field(default=None)),
             ("kms_key_name", str, field(default=None)),
             ("raw_key", str, field(default=None)),
         ],
     ) = None,
-    source_disk: str = None,
     chain_name: str = None,
     snapshot_type: str = None,
     snapshot_encryption_key: make_dataclass(
         "CustomerEncryptionKey",
         [
             ("kms_key_service_account", str, field(default=None)),
-            ("sha256", str, field(default=None)),
             ("rsa_encrypted_key", str, field(default=None)),
             ("kms_key_name", str, field(default=None)),
             ("raw_key", str, field(default=None)),
         ],
     ) = None,
     request_id: str = None,
 ) -> Dict[str, Any]:
-    r"""Creates a snapshot in the specified project using the data included in the request. For regular snapshot creation, consider using this method instead of disks.createSnapshot, as this method supports more features, such as creating snapshots in a project different from the source disk project.
+    r"""Creates a snapshot in the specified project using the data included in the request.
 
-    Args:
-        name(str):
-            An Idem name of the resource.
+    For regular snapshot creation, consider using this method instead of disks.createSnapshot, as this method supports more features, such as creating snapshots in a project different from the source disk project.
 
+    Args:
         storage_locations(List[str], Optional):
             Cloud Storage bucket storage location of the snapshot (regional or multi-regional). Defaults to None.
 
         location_hint(str, Optional):
             An opaque location hint used to place the snapshot close to other resources. This field is for use by internal tools that use the public API. Defaults to None.
 
         label_fingerprint(str, Optional):
@@ -62,39 +70,39 @@
             An optional description of this resource. Provide this property when you create the resource. Defaults to None.
 
         labels(Dict[str, Any], Optional):
             Labels to apply to this snapshot. These can be later modified by the setLabels method. Label values may be empty. Defaults to None.
 
         source_disk_encryption_key(Dict[str, Any], Optional):
             The customer-supplied encryption key of the source disk. Required if the source disk is protected by a customer-supplied encryption key. Defaults to None.
-            * kms_key_service_account (str, Optional): The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/
-            * sha256 (str, optional): [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
+            * kms_key_service_account (str, Optional): The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/"
+            * sha256 (str, Optional): [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
             * rsa_encrypted_key (str, Optional): Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
             * kms_key_name (str, Optional): The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
             * raw_key (str, Optional): Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
 
-        source_disk(str, optional):
+        source_disk(str, Optional):
             The source disk used to create this snapshot. Defaults to None.
 
         chain_name(str, Optional):
             Creates the new snapshot in the snapshot chain labeled with the specified name. The chain name must be 1-63 characters long and comply with RFC1035. This is an uncommon option only for advanced service owners who needs to create separate snapshot chains, for example, for chargeback tracking. When you describe your snapshot resource, this field is visible only if it has a non-empty value. Defaults to None.
 
         snapshot_type(str, Optional):
             Indicates the type of the snapshot.
-            Enum type. Allowed values:
-            "ARCHIVE"
-            "STANDARD". Defaults to None.
+                Enum type. Allowed values:
+                "ARCHIVE"
+                "STANDARD". Defaults to None.
 
         snapshot_encryption_key(Dict[str, Any], Optional):
             Encrypts the snapshot using a customer-supplied encryption key. After you encrypt a snapshot using a customer-supplied key, you must provide the same key if you use the snapshot later. For example, you must provide the encryption key when you create a disk from the encrypted snapshot in a future request. Customer-supplied encryption keys do not protect access to metadata of the snapshot. If you do not provide an encryption key when creating the snapshot, then the snapshot will be encrypted using an automatically generated key and you do not need to provide a key to use the snapshot later. Defaults to None.
-            * kms_key_service_account (str, optional): The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/
-            * sha256 (str, optional): [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
-            * rsa_encrypted_key (str, optional): Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
-            * kms_key_name (str, optional): The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
-            * raw_key (str, optional): Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
+            * kms_key_service_account (str, Optional): The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/"
+            * sha256 (str, Optional): [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
+            * rsa_encrypted_key (str, Optional): Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+            * kms_key_name (str, Optional): The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+            * raw_key (str, Optional): Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
 
         request_id(str, Optional):
             An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
 
         project(str):
             Project ID for this request.
 
@@ -112,88 +120,26 @@
 
             resource_is_present:
               gcp.compute.snapshot.present:
                 - name: value
                 - project: value
                 - snapshot: value
     """
-
     result = {
         "result": True,
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
-    project = get_project_from_account(ctx, project)
-
-    if ctx.get("rerun_data"):
-        handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, ctx.get("rerun_data"), "compute.snapshot"
-        )
-
-        if not handle_operation_ret["result"]:
-            result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
-            return result
-
-        resource_id = handle_operation_ret["resource_id"]
-
-    get_resource_only_with_resource_id = hub.OPT.idem.get(
-        "get_resource_only_with_resource_id", False
-    )
-
-    if resource_id:
-        old_get_ret = await hub.exec.gcp.compute.snapshot.get(
-            ctx, resource_id=resource_id
-        )
-
-        if not old_get_ret["result"] or (
-            not old_get_ret["ret"] and get_resource_only_with_resource_id
-        ):
-            result["result"] = False
-            result["comment"] += old_get_ret["comment"]
-            return result
-
-        # long-running operation has succeeded - both update and create
-        if ctx.get("rerun_data"):
-            result["new_state"] = old_get_ret["ret"]
-            result["old_state"] = ctx["rerun_data"].get("old_state")
-            if result["old_state"]:
-                result["comment"].append(
-                    hub.tool.gcp.comment_utils.update_comment(
-                        "gcp.compute.snapshot", name
-                    )
-                )
-            else:
-                result["comment"].append(
-                    hub.tool.gcp.comment_utils.create_comment(
-                        "gcp.compute.snapshot", name
-                    )
-                )
-            return result
-
-        result["old_state"] = copy.deepcopy(copy.copy(old_get_ret["ret"]))
-
-    elif not get_resource_only_with_resource_id:
-        resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
-            "compute.snapshot", {**locals(), "snapshot": name}
-        )
-        old_get_ret = await hub.exec.gcp.compute.snapshot.get(
-            ctx, resource_id=resource_id
-        )
-
-        if not old_get_ret["result"]:
-            result["result"] = False
-            result["comment"] += old_get_ret["comment"]
-            return result
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
-        if old_get_ret["ret"]:
-            result["old_state"] = copy.deepcopy(copy.copy(old_get_ret["ret"]))
+    if ctx.get("wrapper_result"):
+        result = ctx.get("wrapper_result")
 
     # to be autogenerated by pop-create based on insert/update props in properties.yaml
     resource_body = {
         "name": name,
         "storage_locations": storage_locations,
         "location_hint": location_hint,
         "label_fingerprint": label_fingerprint,
@@ -206,105 +152,118 @@
         "snapshot_encryption_key": snapshot_encryption_key,
     }
 
     resource_body = {k: v for (k, v) in resource_body.items() if v is not None}
     operation = None
 
     if result["old_state"]:
-
         resource_body["label_fingerprint"] = label_fingerprint or result[
             "old_state"
         ].get("label_fingerprint")
 
-        labels_updated = False
-        if (
+        changes = hub.tool.gcp.utils.compare_states(
+            result["old_state"],
+            {"resource_id": resource_id, **resource_body},
+            "compute.snapshot",
+        )
+
+        # This check is necessary because "changes" does not detect label removal
+        are_labels_changed = (
             labels is not None
             and not (labels == {} and result["old_state"].get("labels") is None)
             and result["old_state"].get("labels") != labels
-        ):
-            if not ctx.get("test"):
-                set_labels_body = {
-                    "labels": labels,
-                }
-                if label_fingerprint:
-                    set_labels_body.update(
-                        {
-                            "label_fingerprint": label_fingerprint,
-                        }
-                    )
-                elif result["old_state"].get("label_fingerprint"):
-                    set_labels_body.update(
-                        {
-                            "label_fingerprint": result["old_state"].get(
-                                "label_fingerprint"
-                            ),
-                        }
-                    )
+        )
 
-                update_ret = await hub.exec.gcp_api.client.compute.snapshot.setLabels(
-                    ctx,
-                    project=project,
-                    resource=name,
-                    body=set_labels_body,
+        if not changes and not are_labels_changed:
+            result["comment"].append(
+                hub.tool.gcp.comment_utils.up_to_date_comment(
+                    "gcp.compute.snapshot", name
                 )
+            )
+            result["new_state"] = result["old_state"]
+            return result
 
-                if not update_ret["result"]:
-                    result["result"] = False
-                    result["comment"] += update_ret["comment"]
-                    return result
-
-                if "compute#operation" in update_ret["ret"].get("kind"):
-                    operation = update_ret["ret"]
-                    operation_id = (
-                        hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                            operation.get("selfLink"), "compute.global_operation"
-                        )
-                    )
-                    op_ret = await hub.tool.gcp.operation_utils.handle_operation(
-                        ctx, operation_id, "compute.snapshot", True
-                    )
-                    if not op_ret["result"]:
-                        result["comment"] += op_ret["comment"]
-                        result["rerun_data"] = op_ret["rerun_data"]
-                        return result
-
-            labels_updated = True
+        changed_non_updatable_properties = (
+            hub.tool.gcp.resource_prop_utils.get_changed_non_updatable_properties(
+                "compute.snapshot", changes
+            )
+        )
 
-        if labels_updated:
-            if ctx.get("test", False):
-                result["comment"].append(
-                    hub.tool.gcp.comment_utils.would_update_comment(
-                        "gcp.compute.snapshot", name
-                    )
-                )
-                result["new_state"] = resource_body
-                result["new_state"]["resource_id"] = resource_id
-                return result
-            else:
-                result["comment"].append(
-                    hub.tool.gcp.comment_utils.update_comment(
-                        "gcp.compute.snapshot", name
-                    )
+        if changed_non_updatable_properties:
+            result["result"] = False
+            result["comment"].append(
+                hub.tool.gcp.comment_utils.non_updatable_properties_comment(
+                    "gcp.compute.snapshot",
+                    name,
+                    changed_non_updatable_properties,
                 )
-        else:
+            )
+            result["new_state"] = result["old_state"]
+            return result
+
+        if ctx.get("test", False):
             result["comment"].append(
-                hub.tool.gcp.comment_utils.up_to_date_comment(
+                hub.tool.gcp.comment_utils.would_update_comment(
                     "gcp.compute.snapshot", name
                 )
             )
-            result["new_state"] = copy.deepcopy(result["old_state"])
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                resource_body
+            )
+            result["new_state"]["resource_id"] = resource_id
+            return result
+
+        set_labels_body = {
+            "labels": labels,
+        }
+        if label_fingerprint:
+            set_labels_body.update(
+                {
+                    "label_fingerprint": label_fingerprint,
+                }
+            )
+        elif result["old_state"].get("label_fingerprint"):
+            set_labels_body.update(
+                {
+                    "label_fingerprint": result["old_state"].get("label_fingerprint"),
+                }
+            )
+
+        # the setLabels() method accepts "resource" as the name of the snapshot, so
+        # the resource_id is split into its properties ("project" and "snapshot") here to map "resource" to "snapshot
+        resource_id_props = (
+            hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
+                "compute.snapshot", resource_id
+            )
+        )
+        update_ret = await hub.exec.gcp_api.client.compute.snapshot.setLabels(
+            ctx,
+            project=resource_id_props.get("project"),
+            resource=resource_id_props.get("snapshot"),
+            body=set_labels_body,
+        )
+
+        if not update_ret["result"] or not update_ret["ret"]:
+            result["result"] = False
+            result["comment"] += update_ret["comment"]
+            return result
+
+        if hub.tool.gcp.operation_utils.is_operation(update_ret["ret"]):
+            operation = update_ret["ret"]
 
     else:
         if ctx["test"]:
             result["comment"].append(
                 hub.tool.gcp.comment_utils.would_create_comment(
                     "gcp.compute.snapshot", name
                 )
             )
-            result["new_state"] = resource_body
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                resource_body
+            )
             result["new_state"]["resource_id"] = resource_id
             return result
 
         # Create
         create_ret = await hub.exec.gcp_api.client.compute.snapshot.insert(
             ctx,
             name=name,
@@ -328,173 +287,42 @@
                     )
                 )
                 return result
             else:
                 result["comment"] += create_ret["comment"]
 
         if create_ret["ret"]:
-            if "compute#operation" in create_ret["ret"].get("kind", ""):
+            if hub.tool.gcp.operation_utils.is_operation(create_ret["ret"]):
                 operation = create_ret["ret"]
 
     if operation:
         operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
             operation.get("selfLink"), "compute.global_operation"
         )
         result["rerun_data"] = {
             "operation_id": operation_id,
             "old_state": result["old_state"],
         }
-        result["result"] = False
-
-    return result
-
-
-async def absent(
-    hub,
-    ctx,
-    name: str = None,
-    project: str = None,
-    resource_id: str = None,
-    request_id: str = None,
-) -> Dict[str, Any]:
-    r"""Deletes the specified Snapshot resource. Keep in mind that deleting a single snapshot might not necessarily delete all the data on that snapshot. If any data on the snapshot that is marked for deletion is needed for subsequent snapshots, the data will be moved to the next corresponding snapshot. For more information, see Deleting snapshots.
-
-    Args:
-        name(str):
-            An Idem name of the resource.
-
-        project(str, Optional):
-            Project ID for this request.
-
-        request_id(str, Optional):
-            An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
-
-        resource_id(str, Optional):
-            An identifier of the resource in the provider. Defaults to None.
-
-    Returns:
-        Dict[str, Any]
-
-    Examples:
-        .. code-block:: sls
-
-            resource_is_absent:
-              gcp.compute.snapshot.absent:
-                - name: value
-                - snapshot: value
-                - project: value
-    """
-
-    result = {
-        "result": True,
-        "old_state": None,
-        "new_state": None,
-        "name": name,
-        "comment": [],
-    }
-
-    if ctx.get("rerun_data"):
-        # delete() has been called on a previous iteration
-        handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, ctx.get("rerun_data"), "compute.snapshot"
-        )
-        if not handle_operation_ret["result"]:
-            result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
-            return result
-
-        result["old_state"] = ctx["rerun_data"].get("old_state")
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.delete_comment(
-                "gcp.compute.snapshot", result["old_state"].get("name", None)
-            )
-        )
-        return result
-
-    get_resource_only_with_resource_id = hub.OPT.idem.get(
-        "get_resource_only_with_resource_id", False
-    )
-
-    if not resource_id:
-        if get_resource_only_with_resource_id:
-            result["comment"].append(
-                hub.tool.gcp.comment_utils.already_absent_comment(
-                    "gcp.compute.snapshot", name
-                )
-            )
-            return result
-
-        resource_id = (ctx.get("old_state") or {}).get(
-            "resource_id"
-        ) or hub.tool.gcp.resource_prop_utils.construct_resource_id(
-            "compute.snapshot", {**locals(), "snapshot": name}
-        )
-
-    get_ret = await hub.exec.gcp.compute.snapshot.get(ctx, resource_id=resource_id)
-
-    if not get_ret["result"]:
-        result["result"] = False
-        result["comment"] += get_ret["comment"]
-        return result
-
-    if not get_ret["ret"]:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.already_absent_comment(
-                "gcp.compute.snapshot", name
-            )
-        )
-        return result
-
-    result["old_state"] = get_ret["ret"]
-
-    if ctx["test"]:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.would_delete_comment(
-                "gcp.compute.snapshot", name
-            )
-        )
-        return result
-
-    # First iteration; invoke snapshot's delete()
-    delete_ret = await hub.exec.gcp_api.client.compute.snapshot.delete(
-        ctx, resource_id=resource_id, request_id=request_id
-    )
-    if not delete_ret["result"] or not delete_ret["ret"]:
-        result["result"] = False
-        result["comment"] += delete_ret["comment"]
-        return result
-
-    if "compute#operation" in delete_ret.get("ret", {}).get("kind"):
-        result["result"] = False
-        result["comment"] += delete_ret["comment"]
-        operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-            delete_ret["ret"].get("selfLink"), "compute.global_operation"
-        )
-        result["rerun_data"] = {
-            "operation_id": operation_id,
-            "old_state": result["old_state"],
-        }
 
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r"""Describe the resource in a way that can be recreated/managed with the corresponding "present" function
+    r"""Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
     Retrieves the list of Snapshot resources contained within the specified project.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: bash
 
             $ idem describe gcp.compute.snapshot
     """
-
     result = {}
 
     describe_ret = await hub.exec.gcp.compute.snapshot.list(
         ctx, project=ctx.acct.project_id
     )
 
     if not describe_ret["result"]:
@@ -510,8 +338,9 @@
             ]
         }
 
     return result
 
 
 def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
+    """Default implemented for each module."""
     return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/subnetwork.py` & `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/subnetwork.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 """State module for managing subnetworks."""
-import copy
 from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 
-__contracts__ = ["resource"]
+from dict_tools.typing import Computed
+
+from idem_gcp.tool.gcp.utils import regional_absent
+
+# prevent commit hook from removing the import
+absent = regional_absent
 
-from idem_gcp.tool.gcp.utils import get_project_from_account
+from idem_gcp.tool.gcp.state_operation_utils import StateOperations
+
+__contracts__ = ["resource"]
 
 
 async def present(
     hub,
     ctx,
     name: str,
     region: str = None,
@@ -47,25 +53,26 @@
         )
     ] = None,
     purpose: str = None,
     private_ipv6_google_access: str = None,
     ip_cidr_range: str = None,
     drain_timeout_seconds: int = None,
     resource_id: str = None,
+    id_: (Computed[str], "alias=id") = None,
 ) -> Dict[str, Any]:
     r"""Creates a subnetwork in the specified project using the data included in the request.
 
     Args:
         name(str):
             An Idem name of the resource.
 
         project(str, Optional):
             Project ID for this request.
 
-        region(str):
+        region(str, Optional):
             Name of the region scoping this request.
 
         request_id(str, Optional):
             An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
 
         enable_flow_logs(bool, Optional):
             Whether to enable flow logging for this subnetwork. If this field is not explicitly set, it will not appear in get listings. If not set the default behavior is determined by the org policy, if there is no org policy specified, then it will default to disabled. This field isn't supported with the purpose field set to INTERNAL_HTTPS_LOAD_BALANCER. Defaults to None.
@@ -77,84 +84,99 @@
             An optional description of this resource. Provide this property when you create the resource. This field can be set only at resource creation time. Defaults to None.
 
         network(str, Optional):
             The URL of the network to which this subnetwork belongs, provided by the client when initially creating the subnetwork. This field can be set only at resource creation time. Defaults to None.
 
         stack_type(str, Optional):
             The stack type for the subnet. If set to IPV4_ONLY, new VMs in the subnet are assigned IPv4 addresses only. If set to IPV4_IPV6, new VMs in the subnet can be assigned both IPv4 and IPv6 addresses. If not specified, IPV4_ONLY is used. This field can be both set at resource creation time and updated using patch.
-            Enum type. Allowed values:
-            "IPV4_IPV6" - New VMs in this subnet can have both IPv4 and IPv6 addresses.
-            "IPV4_ONLY" - New VMs in this subnet will only be assigned IPv4 addresses. Defaults to None.
+                Enum type. Allowed values:
+                "IPV4_IPV6" - New VMs in this subnet can have both IPv4 and IPv6 addresses.
+                "IPV4_ONLY" - New VMs in this subnet will only be assigned IPv4 addresses. Defaults to None.
 
         log_config(Dict[str, Any], Optional):
             This field denotes the VPC flow logging options for this subnetwork. If logging is enabled, logs are exported to Cloud Logging.
             SubnetworkLogConfig: The available logging options for this subnetwork. Defaults to None.
-            * aggregation_interval (str, Optional): Can only be specified if VPC flow logging for this subnetwork is enabled. Toggles the aggregation interval for collecting flow logs. Increasing the interval time will reduce the amount of generated flow logs for long lasting connections. Default is an interval of 5 seconds per connection.
-                Enum type. Allowed values:
-                "INTERVAL_10_MIN"
-                "INTERVAL_15_MIN"
-                "INTERVAL_1_MIN"
-                "INTERVAL_30_SEC"
-                "INTERVAL_5_MIN"
-                "INTERVAL_5_SEC"
-            * filter_expr (str, Optional): Can only be specified if VPC flow logs for this subnetwork is enabled. The filter expression is used to define which VPC flow logs should be exported to Cloud Logging.
-            * enable (bool, Optional): Whether to enable flow logging for this subnetwork. If this field is not explicitly set, it will not appear in get listings. If not set the default behavior is determined by the org policy, if there is no org policy specified, then it will default to disabled.
-            * flow_sampling (float, Optional): Can only be specified if VPC flow logging for this subnetwork is enabled. The value of the field must be in [0, 1]. Set the sampling rate of VPC flow logs within the subnetwork where 1.0 means all collected logs are reported and 0.0 means no logs are reported. Default is 0.5 unless otherwise specified by the org policy, which means half of all collected logs are reported.
-            * metadata_fields (List[str], Optional): Can only be specified if VPC flow logs for this subnetwork is enabled and "metadata" was set to CUSTOM_METADATA.
-            * metadata (str, Optional): Can only be specified if VPC flow logs for this subnetwork is enabled. Configures whether all, none or a subset of metadata fields should be added to the reported VPC flow logs. Default is EXCLUDE_ALL_METADATA.
-                Enum type. Allowed values:
-                "CUSTOM_METADATA"
-                "EXCLUDE_ALL_METADATA"
-                "INCLUDE_ALL_METADATA"
+
+            * aggregation_interval (str, Optional):
+                Can only be specified if VPC flow logging for this subnetwork is enabled. Toggles the aggregation interval for collecting flow logs. Increasing the interval time will reduce the amount of generated flow logs for long lasting connections. Default is an interval of 5 seconds per connection.
+                    Enum type. Allowed values:
+                    "INTERVAL_10_MIN"
+                    "INTERVAL_15_MIN"
+                    "INTERVAL_1_MIN"
+                    "INTERVAL_30_SEC"
+                    "INTERVAL_5_MIN"
+                    "INTERVAL_5_SEC"
+
+            * filter_expr (str, Optional):
+                Can only be specified if VPC flow logs for this subnetwork is enabled. The filter expression is used to define which VPC flow logs should be exported to Cloud Logging.
+
+            * enable (bool, Optional):
+                Whether to enable flow logging for this subnetwork. If this field is not explicitly set, it will not appear in get listings. If not set the default behavior is determined by the org policy, if there is no org policy specified, then it will default to disabled.
+
+            * flow_sampling (float, Optional):
+                Can only be specified if VPC flow logging for this subnetwork is enabled. The value of the field must be in [0, 1]. Set the sampling rate of VPC flow logs within the subnetwork where 1.0 means all collected logs are reported and 0.0 means no logs are reported. Default is 0.5 unless otherwise specified by the org policy, which means half of all collected logs are reported.
+
+            * metadata_fields (List[str], Optional):
+                Can only be specified if VPC flow logs for this subnetwork is enabled and "metadata" was set to CUSTOM_METADATA.
+
+            * metadata (str, Optional):
+                Can only be specified if VPC flow logs for this subnetwork is enabled. Configures whether all, none or a subset of metadata fields should be added to the reported VPC flow logs. Default is EXCLUDE_ALL_METADATA.
+                    Enum type. Allowed values:
+                    "CUSTOM_METADATA"
+                    "EXCLUDE_ALL_METADATA"
+                    "INCLUDE_ALL_METADATA"
 
         role(str, Optional):
             The role of subnetwork. Currently, this field is only used when purpose = INTERNAL_HTTPS_LOAD_BALANCER. The value can be set to ACTIVE or BACKUP. An ACTIVE subnetwork is one that is currently being used for Internal HTTP(S) Load Balancing. A BACKUP subnetwork is one that is ready to be promoted to ACTIVE or is currently draining. This field can be updated with a patch request.
-            Enum type. Allowed values:
-            "ACTIVE" - The ACTIVE subnet that is currently used.
-            "BACKUP" - The BACKUP subnet that could be promoted to ACTIVE. Defaults to None.
+                Enum type. Allowed values:
+                "ACTIVE" - The ACTIVE subnet that is currently used.
+                "BACKUP" - The BACKUP subnet that could be promoted to ACTIVE. Defaults to None.
 
         ipv6_access_type(str, Optional):
             The access type of IPv6 address this subnet holds. It's immutable and can only be specified during creation or the first time the subnet is updated into IPV4_IPV6 dual stack.
-            Enum type. Allowed values:
-            "EXTERNAL" - VMs on this subnet will be assigned IPv6 addresses that are accessible via the Internet, as well as the VPC network.
-            "INTERNAL" - VMs on this subnet will be assigned IPv6 addresses that are only accessible over the VPC network. Defaults to None.
+                Enum type. Allowed values:
+                "EXTERNAL" - VMs on this subnet will be assigned IPv6 addresses that are accessible via the Internet, as well as the VPC network.
+                "INTERNAL" - VMs on this subnet will be assigned IPv6 addresses that are only accessible over the VPC network. Defaults to None.
 
         fingerprint(str, Optional):
             Fingerprint of this resource. A hash of the contents stored in this object. This field is used in optimistic locking. This field will be ignored when inserting a Subnetwork. An up-to-date fingerprint must be provided in order to update the Subnetwork, otherwise the request will fail with error 412 conditionNotMet. To see the latest fingerprint, make a get() request to retrieve a Subnetwork. Defaults to None.
 
         secondary_ip_ranges(List[Dict[str, Any]], Optional):
             An array of configurations for secondary IP ranges for VM instances contained in this subnetwork. The primary IP of such VM must belong to the primary ipCidrRange of the subnetwork. The alias IPs may belong to either primary or secondary ranges. This field can be updated with a patch request. Defaults to None.
-            * ip_cidr_range (str, optional): The range of IP addresses belonging to this subnetwork secondary range. Provide this property when you create the subnetwork. Ranges must be unique and non-overlapping with all primary and secondary IP ranges within a network. Only IPv4 is supported. The range can be any range listed in the Valid ranges list.
-            * range_name (str, optional): The name associated with this subnetwork secondary range, used when adding an alias IP range to a VM instance. The name must be 1-63 characters long, and comply with RFC1035. The name must be unique within the subnetwork.
+
+            * ip_cidr_range (str, Optional): The range of IP addresses belonging to this subnetwork secondary range. Provide this property when you create the subnetwork. Ranges must be unique and non-overlapping with all primary and secondary IP ranges within a network. Only IPv4 is supported. The range can be any range listed in the Valid ranges list.
+            * range_name (str, Optional): The name associated with this subnetwork secondary range, used when adding an alias IP range to a VM instance. The name must be 1-63 characters long, and comply with RFC1035. The name must be unique within the subnetwork.
 
         purpose(str, Optional):
             The purpose of the resource. This field can be either PRIVATE_RFC_1918 or INTERNAL_HTTPS_LOAD_BALANCER. A subnetwork with purpose set to INTERNAL_HTTPS_LOAD_BALANCER is a user-created subnetwork that is reserved for Internal HTTP(S) Load Balancing. If unspecified, the purpose defaults to PRIVATE_RFC_1918. The enableFlowLogs field isn't supported with the purpose field set to INTERNAL_HTTPS_LOAD_BALANCER.
-            Enum type. Allowed values:
-            "INTERNAL_HTTPS_LOAD_BALANCER" - Subnet reserved for Internal HTTP(S) Load Balancing.
-            "PRIVATE" - Regular user created or automatically created subnet.
-            "PRIVATE_RFC_1918" - Regular user created or automatically created subnet.
-            "PRIVATE_SERVICE_CONNECT" - Subnetworks created for Private Service Connect in the producer network.
-            "REGIONAL_MANAGED_PROXY" - Subnetwork used for Regional Internal/External HTTP(S) Load Balancing. Defaults to None.
+                Enum type. Allowed values:
+                "INTERNAL_HTTPS_LOAD_BALANCER" - Subnet reserved for Internal HTTP(S) Load Balancing.
+                "PRIVATE" - Regular user created or automatically created subnet.
+                "PRIVATE_RFC_1918" - Regular user created or automatically created subnet.
+                "PRIVATE_SERVICE_CONNECT" - Subnetworks created for Private Service Connect in the producer network.
+                "REGIONAL_MANAGED_PROXY" - Subnetwork used for Regional Internal/External HTTP(S) Load Balancing. Defaults to None.
 
         private_ipv6_google_access(str, Optional):
             This field is for internal use. This field can be both set at resource creation time and updated using patch.
-            Enum type. Allowed values:
-            "DISABLE_GOOGLE_ACCESS" - Disable private IPv6 access to/from Google services.
-            "ENABLE_BIDIRECTIONAL_ACCESS_TO_GOOGLE" - Bidirectional private IPv6 access to/from Google services.
-            "ENABLE_OUTBOUND_VM_ACCESS_TO_GOOGLE" - Outbound private IPv6 access from VMs in this subnet to Google services. Defaults to None.
+                Enum type. Allowed values:
+                "DISABLE_GOOGLE_ACCESS" - Disable private IPv6 access to/from Google services.
+                "ENABLE_BIDIRECTIONAL_ACCESS_TO_GOOGLE" - Bidirectional private IPv6 access to/from Google services.
+                "ENABLE_OUTBOUND_VM_ACCESS_TO_GOOGLE" - Outbound private IPv6 access from VMs in this subnet to Google services. Defaults to None.
 
         ip_cidr_range(str, Optional):
             The range of internal addresses that are owned by this subnetwork. Provide this property when you create the subnetwork. For example, 10.0.0.0/8 or 100.64.0.0/10. Ranges must be unique and non-overlapping within a network. Only IPv4 is supported. This field is set at resource creation time. The range can be any range listed in the Valid ranges list. The range can be expanded after creation using expandIpCidrRange. Defaults to None.
 
         drain_timeout_seconds(int, Optional):
             The drain timeout specifies the upper bound in seconds on the amount of time allowed to drain connections from the current ACTIVE subnetwork to the current BACKUP subnetwork. The drain timeout is only applicable when the following conditions are true: - the subnetwork being patched has purpose = INTERNAL_HTTPS_LOAD_BALANCER - the subnetwork being patched has role = BACKUP - the patch request is setting the role to ACTIVE. Note that after this patch operation the roles of the ACTIVE and BACKUP subnetworks will be swapped. Defaults to None.
 
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
+        id(str, Optional): The unique identifier for the resource. This identifier is defined by the server. Read-only property
+
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
             example_resource_name:
@@ -167,39 +189,18 @@
         "result": True,
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
-    project = get_project_from_account(ctx, project)
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
-    # Handle operation(s) in progress, if any
-    if ctx.get("rerun_data"):
-        op_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, ctx.get("rerun_data"), "compute.subnetwork"
-        )
-
-        if not op_ret["result"]:
-            result["comment"] += op_ret["comment"]
-            result["rerun_data"] = op_ret["rerun_data"]
-            return result
-
-        resource_id = op_ret["resource_id"]
-
-    if resource_id:
-        old = await hub.exec.gcp.compute.subnetwork.get(
-            ctx, name=name, resource_id=resource_id
-        )
-        if not old["result"] or not old["ret"]:
-            result["result"] = False
-            result["comment"] += old["comment"]
-            return result
-
-        result["old_state"] = copy.deepcopy(old["ret"])
+    if ctx.get("wrapper_result"):
+        result = ctx.get("wrapper_result")
 
     request_body = {
         "log_config": log_config,
         "purpose": purpose,
         "private_ipv6_google_access": private_ipv6_google_access,
         "private_ip_google_access": private_ip_google_access,
         "role": role,
@@ -207,73 +208,136 @@
         "name": name,
         "ip_cidr_range": ip_cidr_range,
         "description": description,
         "enable_flow_logs": enable_flow_logs,
         "stack_type": stack_type,
         "secondary_ip_ranges": secondary_ip_ranges,
         "network": network,
+        "id_": id_,
     }
 
     operation = None
     plan_state = {"resource_id": resource_id, **request_body}
     plan_state = {k: v for (k, v) in plan_state.items() if v is not None}
 
     if result["old_state"]:
+        resource_id = result["old_state"].get("resource_id", None)
         # Update subnetwork
+        patch_operations_dict = {
+            "ip_cidr_range": (
+                hub.tool.gcp.compute.subnetwork.update_ip_cidr_range,
+                (ctx, result["old_state"], ip_cidr_range),
+                True,
+            ),
+        }
+
+        state_operations = StateOperations(
+            hub, "compute.subnetwork", patch_operations_dict, result, request_body
+        )
+
         changes = hub.tool.gcp.utils.compare_states(
-            copy.copy(result["old_state"]),
-            {"resource_id": resource_id, **request_body},
+            result["old_state"],
+            {
+                "resource_id": resource_id,
+                **request_body,
+            },
             "compute.subnetwork",
+            additional_exclude_paths=list(patch_operations_dict.keys()),
         )
 
-        if not changes:
+        if not changes and not any(state_operations.changed_properties_dict.values()):
             result["result"] = True
             result["comment"].append(
-                hub.tool.gcp.comment_utils.already_exists_comment(
+                hub.tool.gcp.comment_utils.up_to_date_comment(
                     "gcp.compute.subnetwork", name
                 )
             )
-            result["new_state"] = copy.deepcopy(result["old_state"])
+            result["new_state"] = result["old_state"]
             return result
 
         if ctx["test"]:
             result["comment"].append(
                 hub.tool.gcp.comment_utils.would_update_comment(
                     "gcp.compute.subnetwork", name
                 )
             )
-            result["new_state"] = plan_state
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                plan_state
+            )
             return result
 
-        body = {**request_body, "fingerprint": result["old_state"].get("fingerprint")}
-        body.pop("ip_cidr_range")
-        update = await hub.exec.gcp_api.client.compute.subnetwork.patch(
-            ctx, resource_id=resource_id, body=body
-        )
-        if not update["result"]:
+        state_operations_ret = await state_operations.run_operations()
+
+        if not state_operations_ret["result"]:
+            result["comment"] += state_operations_ret["comment"]
             result["result"] = False
-            result["comment"] += update["comment"]
             return result
 
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.update_comment("gcp.compute.subnetwork", name)
-        )
+        if changes:
+            if any(state_operations.changed_properties_dict.values()):
+                get_ret = await hub.exec.gcp.compute.subnetwork.get(
+                    ctx, name=name, resource_id=resource_id
+                )
 
-        if "compute#operation" in update["ret"].get("kind"):
-            operation = update["ret"]
+                if not get_ret["result"] and not get_ret["ret"]:
+                    result["result"] = False
+                    result["comment"] += get_ret["comment"]
+                    return result
+
+                for k in patch_operations_dict.keys():
+                    request_body[k] = get_ret["ret"].get(k)
+
+                request_body["fingerprint"] = get_ret["ret"].get("fingerprint")
+
+            body = (
+                {**request_body, "fingerprint": result["old_state"].get("fingerprint")}
+                if not request_body.get("fingerprint")
+                else {**request_body}
+            )
+            body.pop("ip_cidr_range")
+            body.pop("network")
+            state_operations.pre_process_resource_body(body)
+            update = await hub.exec.gcp_api.client.compute.subnetwork.patch(
+                ctx, resource_id=resource_id, body=body
+            )
+            if not update["result"]:
+                result["result"] = False
+                result["comment"] += update["comment"]
+                return result
+
+            if hub.tool.gcp.operation_utils.is_operation(update["ret"]):
+                operation = update["ret"]
 
+        if not changes and any(state_operations.changed_properties_dict.values()):
+            get_ret = await hub.exec.gcp.compute.subnetwork.get(
+                ctx, name=name, resource_id=resource_id
+            )
+            if not get_ret["result"] and not get_ret["ret"]:
+                result["result"] = False
+                result["comment"] += get_ret["comment"]
+                return result
+
+            result["new_state"] = get_ret["ret"]
+            result["comment"].append(
+                hub.tool.gcp.comment_utils.update_comment(
+                    "gcp.compute.subnetwork", name
+                )
+            )
+            return result
     else:
         # Create subnetwork
         if ctx["test"]:
             result["comment"].append(
                 hub.tool.gcp.comment_utils.would_create_comment(
                     "gcp.compute.subnetwork", name
                 )
             )
-            result["new_state"] = plan_state
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                plan_state
+            )
             result["new_state"][
                 "resource_id"
             ] = hub.tool.gcp.resource_prop_utils.construct_resource_id(
                 "compute.subnetwork", {**locals(), "subnetwork": name}
             )
             return result
 
@@ -281,256 +345,27 @@
             ctx, project=project, region=region, body=request_body
         )
         if not create["result"]:
             result["result"] = False
             result["comment"] += create["comment"]
             return result
 
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.create_comment("gcp.compute.subnetwork", name)
-        )
-
-        if "compute#operation" in create["ret"].get("kind"):
+        if hub.tool.gcp.operation_utils.is_operation(create["ret"]):
             operation = create["ret"]
 
     if operation:
-        op_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
+        operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
             operation.get("selfLink"), "compute.region_operation"
         )
-        op_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, op_id, "compute.subnetwork"
-        )
-
-        if not op_ret["result"]:
-            result["comment"] += op_ret["comment"]
-            result["rerun_data"] = op_ret["rerun_data"]
-            return result
-
-        resource_id = op_ret["resource_id"]
-
-    new = await hub.exec.gcp.compute.subnetwork.get(
-        ctx, name=name, resource_id=resource_id
-    )
-
-    if not new["result"] and not new["ret"]:
-        result["result"] = False
-        result["comment"] += new["comment"]
-        return result
-
-    result["new_state"] = copy.deepcopy(new["ret"])
-
-    # Update individual properties of the subnetwork, if needed
-
-    prop_updated = False
-
-    if (
-        not ctx["test"]
-        and ip_cidr_range
-        and ip_cidr_range != result["new_state"].get("ip_cidr_range")
-    ):
-        request_body = {"ip_cidr_range": ip_cidr_range}
-
-        ret = await hub.exec.gcp_api.client.compute.subnetwork.expandIpCidrRange(
-            ctx, resource_id=resource_id, body=request_body
-        )
-
-        if not ret["result"] and not ret["ret"]:
-            result["result"] = False
-            result["comment"] += ret["comment"]
-            return result
-
-        if "compute#operation" in ret["ret"].get("kind"):
-            operation = ret["ret"]
-
-            operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                operation.get("selfLink"), "compute.region_operation"
-            )
-            handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-                ctx, operation_id, "compute.subnetwork", True
-            )
-
-            if not handle_operation_ret["result"]:
-                result["comment"] += handle_operation_ret["comment"]
-                result["rerun_data"] = handle_operation_ret["rerun_data"]
-                return result
-
-            resource_id = handle_operation_ret["resource_id"]
-            prop_updated = True
-
-    if (
-        not ctx["test"]
-        and private_ip_google_access is not None
-        and private_ip_google_access
-        != result["new_state"].get("private_ip_google_access")
-    ):
-        request_body = {"private_ip_google_access": private_ip_google_access}
-
-        ret = await hub.exec.gcp_api.client.compute.subnetwork.setPrivateIpGoogleAccess(
-            ctx, resource_id=resource_id, body=request_body
-        )
-
-        if not ret["result"] and not ret["ret"]:
-            result["result"] = False
-            result["comment"] += ret["comment"]
-            return result
-
-        if "compute#operation" in ret["ret"].get("kind"):
-            operation = ret["ret"]
-
-            operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                operation.get("selfLink"), "compute.region_operation"
-            )
-            handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-                ctx, operation_id, "compute.subnetwork", True
-            )
-
-            if not handle_operation_ret["result"]:
-                result["comment"] += handle_operation_ret["comment"]
-                result["rerun_data"] = handle_operation_ret["rerun_data"]
-                return result
-
-            resource_id = handle_operation_ret["resource_id"]
-            prop_updated = True
-
-    if prop_updated:
-        new = await hub.exec.gcp.compute.subnetwork.get(
-            ctx, name=name, resource_id=resource_id
-        )
-
-        if not new["result"] and not new["ret"]:
-            result["result"] = False
-            result["comment"] += new["comment"]
-            return result
-
-        result["new_state"] = copy.deepcopy(new["ret"])
-
-    return result
-
-
-async def absent(
-    hub,
-    ctx,
-    name: str,
-    region: str = None,
-    project: str = None,
-    request_id: str = None,
-    resource_id: str = None,
-) -> Dict[str, Any]:
-    r"""Deletes the specified subnetwork.
-
-    Args:
-        name(str):
-            An Idem name of the resource.
-
-        project(str, Optional):
-            Project ID for this request.
-
-        region(str):
-            Name of the region scoping this request.
-
-        request_id(str, Optional):
-            An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
-
-        resource_id(str, Optional):
-            An identifier of the resource in the provider. Defaults to None.
-
-    Returns:
-        Dict[str, Any]
-
-    Examples:
-        .. code-block:: sls
-
-            resource_is_absent:
-              gcp.compute.subnetwork.absent:
-                - name: value
-                - project: value
-                - region: value
-    """
-
-    result = {
-        "comment": [],
-        "old_state": ctx.get("old_state"),
-        "new_state": None,
-        "name": name,
-        "result": True,
-    }
-
-    if not resource_id:
-        resource_id = (ctx.old_state or {}).get("resource_id")
-
-    if not resource_id:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.already_absent_comment(
-                "gcp.compute.subnetwork", name
-            )
-        )
-        return result
-
-    if ctx.test:
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.would_delete_comment(
-                "gcp.compute.subnetwork", name
-            )
-        )
+        result["rerun_data"] = {
+            "operation_id": operation_id,
+            "old_state": result["old_state"],
+        }
         return result
 
-    if not ctx.get("rerun_data"):
-        # First iteration; invoke subnetwork's delete()
-        old = await hub.exec.gcp.compute.subnetwork.get(ctx, resource_id=resource_id)
-        if not old["result"]:
-            result["result"] = False
-            result["comment"] += old["comment"]
-            return result
-        if not old["ret"]:
-            result["comment"].append(
-                hub.tool.gcp.comment_utils.already_absent_comment(
-                    "gcp.compute.subnetwork", name
-                )
-            )
-            return result
-        elif ctx.test:
-            result["old_state"] = copy.deepcopy(old["ret"])
-            result["comment"].append(
-                hub.tool.gcp.comment_utils.would_delete_comment(
-                    "gcp.compute.subnetwork", name
-                )
-            )
-            return result
-        else:
-            result["old_state"] = copy.deepcopy(old["ret"])
-            delete = await hub.exec.gcp_api.client.compute.subnetwork.delete(
-                ctx, resource_id=resource_id
-            )
-            if delete["ret"]:
-                if "compute#operation" in delete["ret"].get("kind"):
-                    result["result"] = False
-                    result["comment"] += delete["comment"]
-                    result[
-                        "rerun_data"
-                    ] = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                        delete["ret"].get("selfLink"), "compute.region_operation"
-                    )
-                    return result
-    else:
-        # delete() has been called on some previous iteration
-        op_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, ctx.get("rerun_data"), "compute.subnetwork"
-        )
-        if not op_ret["result"]:
-            result["comment"] += op_ret["comment"]
-            result["rerun_data"] = op_ret["rerun_data"]
-            return result
-
-        resource_id = op_ret["resource_id"]
-
-    result["comment"].append(
-        hub.tool.gcp.comment_utils.delete_comment("gcp.compute.subnetwork", name)
-    )
-    return result
-
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
     r"""Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
     Retrieves a list of subnetworks available to the specified project.
 
     Returns:
@@ -560,8 +395,9 @@
             ]
         }
 
     return result
 
 
 def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
+    """Default implemented for each module."""
     return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/states/gcp/storage/buckets.py` & `idem_gcp-1.1.0/idem_gcp/states/gcp/iam/projects/service_account.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,352 +1,366 @@
-"""State module for managing Buckets."""
+"""State module for managing Service Accounts."""
 import copy
 from typing import Any
 from typing import Dict
-from typing import List
 
-from idem_gcp.tool.gcp.utils import get_project_from_account
 
 __contracts__ = ["resource"]
-
-
-# TODO:
-# TREQ = {
-#     "present": {
-#
-#     }
-# }
+RESOURCE_TYPE = "iam.projects.service_account"
+RESOURCE_TYPE_FULL = "gcp.iam.projects.service_account"
 
 
 async def present(
     hub,
     ctx,
     name: str,
     resource_id: str = None,
-    predefined_acl: str = None,
-    predefined_default_object_acl: str = None,
-    project: str = None,
-    # TODO: Remove user_project because it cannot be changed as it is set in the credentials
-    user_project: str = None,
-    acl: List = None,
-    billing: Dict = None,
-    cors: List = None,
-    custom_placement_config: Dict = None,
-    default_event_based_hold: bool = None,
-    default_object_acl: List = None,
-    encryption: Dict = None,
-    iam_configuration: Dict = None,
-    labels: Dict = None,
-    lifecycle: Dict = None,
-    location: str = None,
-    logging: Dict = None,
-    rpo: str = None,
-    storage_class: str = None,
-    versioning: Dict = None,
-    website: Dict = None,
-):
-    """Ensure a bucket exists pursuant to the requested state.
-
-    :param hub: The redistributed pop central hub.
-    :param ctx: A dict with the keys/values for the execution of the Idem run
-    located in `hub.idem.RUNS[ctx['run_name']]`.
-    :param name: The name of the state (e.g., "assure bucket present").
-    :param project: Name of the project in which to insert/update the bucket.
-    :param userProject: Project id of the user to bill.
-    :param body: A `Bucket`_ dictionary passed as the body to the GCP APIs
-    as they require.
-
-    Example SLS file usage:
-    .. code-block::
-        "Assure Bucket Present":
-            gcp.storage.buckets.present:
-                - project: MyProject
-                - userProject: None
-                - body:
-                    name: MyBucket
-                    cors:
-                    - maxAgeSeconds: 42
-                      method:
-                        - "GET"
-                        - "OPTIONS"
-                        - "POST"
-                        - "PATCH"
-                        - "DELETE"
-                      origin": [ '*' ]
-                      responseHeader:
-                        - "Cache-Control"
-                        - "Content-Language"
-                        - "Content-Length"
-                        - "Content-Type"
-                        - "Expires"
-                        - "Last-Modified"
-                        - "Pragma"
+    project_id: str = None,
+    account_id: str = None,
+    display_name: str = None,
+    description: str = None,
+    unique_id: str = None,
+    email: str = None,
+    etag: str = None,
+    disabled: bool = None,
+    oauth2_client_id: str = None,
+) -> Dict[str, Any]:
+    """Create or update a service account resource.
+
+    Args:
+        name(str, Optional): The resource name of the service account.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        project_id(str, Optional): A valid API project identifier.
+        account_id(str): Required on create. The account id that is used to generate the service account email address
+        and a stable unique id. It is unique within a project, must be 6-30 characters long, and match the regular
+        expression [a-z]([-a-z0-9]*[a-z0-9]) to comply with RFC1035.
+        display_name(str, Optional): A user-specified, human-readable name for the service account. The maximum length is 100 UTF-8 bytes.
+        description(str, Optional): A user-specified, human-readable description of the service account. The maximum length is 256 UTF-8 bytes.
+        unique_id(str, Optional): The unique, stable numeric ID for the service account.
+        email(str, Optional): The email address of the service account.
+        etag(str, Optional): A base64-encoded string.
+        disabled(str, Optional): Output only. Whether the service account is disabled.
+        oauth2_client_id(str, Optional): The OAuth 2.0 client ID for the service account.
+
+    Returns:
+        Dict[str, Any]
 
-    .. _Bucket: https://googleapis.github.io/google-api-python-client/docs/dyn/storage_v1.buckets.html#insert
+    Examples:
+        .. code-block:: sls
+
+            resource_is_present:
+              gcp.iam.projects.service_account.present:
+                - name: value
+                - project_id: value
     """
+    project_id = hub.tool.gcp.utils.get_project_from_account(ctx, project_id)
+
     result = {
         "result": True,
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
-    project = get_project_from_account(ctx, project)
+    resource_type_camel = hub.tool.gcp.case.camel(RESOURCE_TYPE_FULL.split(".")[-1])
 
-    # Get the resource_id from ESM
-    if not resource_id:
-        resource_id = (ctx.old_state or {}).get("resource_id")
+    if hub.tool.gcp.resource_prop_utils.properties_mismatch_resource_id(
+        RESOURCE_TYPE, resource_id, {**locals(), resource_type_camel: name}
+    ):
+        result["comment"].append(
+            hub.tool.gcp.comment_utils.properties_mismatch_resource_id_comment(
+                RESOURCE_TYPE_FULL, name
+            )
+        )
 
-    old = None
+    # Wait until resource is available in GCP
+    if ctx.get("rerun_data"):
+        service_account = ctx.get("rerun_data").get("old_state")
 
-    if resource_id:
-        old_get_ret = await hub.exec.gcp.storage.buckets.get(
-            ctx,
-            name=name,
+        old_get_ret = await hub.exec.gcp.iam.projects.service_account.get(
+            ctx, resource_id=service_account["resource_id"]
         )
 
-        if not old_get_ret["result"] or not old_get_ret["ret"]:
-            result["result"] = False
+        if not old_get_ret["result"]:
             result["comment"] += old_get_ret["comment"]
-            # TODO: Handle the case when resource does not exist
+            result["rerun_data"] = ctx.get("rerun_data")
             return result
 
-        # copy.copy(old_get_ret['ret']) is needed to convert any objects of type NamespaceDict to dict
-        # in old_get_ret['ret']. This is done so that comparisons with the plan_state which has
-        # objects of type dict works properly
-        old = copy.deepcopy(copy.copy(old_get_ret["ret"]))
-        result["old_state"] = old
-
-    # TODO: Check if body contains the same parameters as old
-    # to be autogenerated by pop-create based on insert/update props in properties.yaml
-    resource_body = {
-        "acl": acl,
-        "billing": billing,
-        "cors": cors,
-        "custom_placement_config": custom_placement_config,
-        "default_event_based_hold": default_event_based_hold,
-        "default_object_acl": default_object_acl,
-        "encryption": encryption,
-        "iam_configuration": iam_configuration,
-        "labels": labels,
-        "lifecycle": lifecycle,
-        "location": location,
-        "logging": logging,
-        "name": name,
-        "rpo": rpo,
-        "storage_class": storage_class,
-        "versioning": versioning,
-        "website": website,
-    }
+        result["old_state"] = old_get_ret["ret"]
+        result["new_state"] = old_get_ret["ret"]
 
-    # TODO: How to handle query params which are not returned in the response body of get
-    plan_state = {
-        # "project": project,
-        # "predefined_acl": predefined_acl,
-        # "predefined_default_object_acl": predefined_default_object_acl,
-        "resource_id": resource_id,
-        **resource_body,
-    }
+        return result
+
+    if resource_id:
+        old_get_ret = await hub.exec.gcp.iam.projects.service_account.get(
+            ctx, resource_id=resource_id
+        )
 
-    plan_state = {k: v for (k, v) in plan_state.items() if v is not None}
+        if not old_get_ret["result"]:
+            result["result"] = False
+            result["comment"] += old_get_ret["comment"]
+            return result
 
-    if old:
-        changes = hub.tool.gcp.utils.compare_states(old, plan_state)
+        result["old_state"] = copy.deepcopy(copy.copy(old_get_ret["ret"]))
 
+    if result["old_state"]:
+        new_state = {
+            "name": name,
+            "resource_id": resource_id,
+            "project_id": project_id,
+            "unique_id": unique_id,
+            "email": email,
+            "display_name": display_name,
+            "etag": etag,
+            "oauth2_client_id": oauth2_client_id,
+            "description": description,
+            "disabled": disabled,
+        }
+        new_state = {k: v for (k, v) in new_state.items() if v is not None}
+
+        changes = hub.tool.gcp.utils.compare_states(
+            result["old_state"],
+            new_state,
+            RESOURCE_TYPE,
+        )
         if not changes:
-            result["result"] = True
             result["comment"].append(
-                hub.tool.gcp.comment_utils.already_exists_comment(
-                    "gcp.storage.bucket", name
-                )
+                hub.tool.gcp.comment_utils.up_to_date_comment(RESOURCE_TYPE_FULL, name)
             )
-            result["new_state"] = plan_state
-
+            result["new_state"] = result["old_state"]
             return result
 
-        non_updatable_properties = (
-            hub.tool.gcp.resource_prop_utils.get_non_updatable_properties(
-                "storage.buckets"
+        changed_non_updatable_properties = (
+            hub.tool.gcp.resource_prop_utils.get_changed_non_updatable_properties(
+                RESOURCE_TYPE, changes
             )
         )
-
-        for key, value in plan_state.items():
-            if value == old.get(key):
-                non_updatable_properties.discard(key)
-
-        if non_updatable_properties:
+        if changed_non_updatable_properties:
             result["result"] = False
             result["comment"].append(
                 hub.tool.gcp.comment_utils.non_updatable_properties_comment(
-                    "gcp.storage.bucket", name, non_updatable_properties
+                    RESOURCE_TYPE_FULL,
+                    name,
+                    changed_non_updatable_properties,
                 )
             )
-            result["new_state"] = copy.deepcopy(old)
+            result["new_state"] = result["old_state"]
             return result
 
+        update_mask = []
+        service_account = {}
+        if display_name:
+            service_account["display_name"] = display_name
+            update_mask.append("displayName")
+        if description:
+            service_account["description"] = description
+            update_mask.append("description")
+
         if ctx["test"]:
             result["comment"].append(
-                hub.tool.gcp.comment_utils.would_update("gcp.storage.bucket", name)
+                hub.tool.gcp.comment_utils.would_update_comment(
+                    RESOURCE_TYPE_FULL, result["old_state"]["resource_id"]
+                )
+            )
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                {**result["old_state"], **service_account}
             )
-            result["new_state"] = plan_state
             return result
 
-        # Perform update
-        update_ret = await hub.exec.gcp_api.client.storage.buckets.update(
-            hub,
+        patch_ret = await hub.exec.gcp_api.client.iam.projects.service_account.patch(
             ctx,
-            name=name,
-            resource_id=resource_id,
-            body=resource_body,
-            userProject=user_project,
+            name=resource_id,
+            body={
+                "service_account": service_account,
+                "update_mask": ",".join(update_mask),
+            },
         )
-        if not update_ret["result"]:
+        if not patch_ret["result"]:
             result["result"] = False
-            result["comment"] += update_ret["comment"]
+            result["comment"] += patch_ret["comment"]
             return result
+
+        result["new_state"] = {**result["old_state"], **patch_ret["ret"]}
         result["comment"].append(
-            hub.tool.gcp.comment_utils.update_comment("gcp.storage.bucket", name)
+            hub.tool.gcp.comment_utils.update_comment(
+                RESOURCE_TYPE_FULL, result["new_state"]["resource_id"]
+            )
         )
-        result["new_state"] = update_ret["ret"]
-
+        return result
     else:
         if ctx["test"]:
             result["comment"].append(
                 hub.tool.gcp.comment_utils.would_create_comment(
-                    "gcp.storage.bucket", name
+                    RESOURCE_TYPE_FULL, resource_id
                 )
             )
-            result["new_state"] = plan_state
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                {
+                    "resource_id": resource_id,
+                    "name": name,
+                    "project_id": project_id,
+                    "unique_id": unique_id,
+                    "email": email,
+                    "display_name": display_name,
+                    "etag": etag,
+                    "oauth2_client_id": oauth2_client_id,
+                }
+            )
             return result
 
         # Create
-        create_ret = await hub.exec.gcp_api.client.storage.buckets.insert(
-            ctx,
-            name=name,
-            project=project,
-            body=resource_body,
-            userProject=user_project,
+        if not account_id:
+            result["result"] = False
+            result["comment"].append("Property 'account_id' is required.")
+            return result
+
+        resource_body = {"account_id": account_id}
+        service_account = {"display_name": display_name, "description": description}
+        service_account = {k: v for (k, v) in service_account.items() if v is not None}
+        if service_account:
+            resource_body["service_account"] = service_account
+
+        create_ret = await hub.exec.gcp_api.client.iam.projects.service_account.create(
+            ctx, name=f"projects/{project_id}", body=resource_body
         )
+
         if not create_ret["result"]:
             result["result"] = False
             result["comment"] += create_ret["comment"]
             return result
+
         result["comment"].append(
-            hub.tool.gcp.comment_utils.create_comment("gcp.storage.bucket", name)
+            hub.tool.gcp.comment_utils.create_comment(
+                RESOURCE_TYPE_FULL, create_ret["ret"]["resource_id"]
+            )
         )
-        result["old_state"] = {}
-        result["new_state"] = create_ret["ret"]
 
-    return result
+        result["rerun_data"] = {
+            "operation": "create",
+            "old_state": {
+                **copy.copy(create_ret["ret"]),
+            },
+        }
 
+        return result
 
-async def absent(
-    hub,
-    ctx,
-    name: str,
-    resource_id: str = None,
-    project: str = None,
-    user_project: str = None,
-):
-    """Ensure a bucket does not exist.
-
-    :param hub: The redistributed pop central hub.
-    :param ctx: A dict with the keys/values for the execution of the Idem run
-    located in `hub.idem.RUNS[ctx['run_name']]`.
-    :param name: The name of the state (e.g., "assure subnet absent").
-    :param project: The project in which the bucket should not exist.
-
-    Example usage:
-        .. code-block: yaml
-            gcp.storage.buckets.absent:
-                - project: {{ project }}
-                - bucket: {{ bucket_name }}
-                - user_project: {{ billto_project_name }}
+
+async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
+    r"""Deletes a service account.
+
+    Args:
+        name(str):
+            The name of the resource
+
+        resource_id(str, Optional):
+            The resource_id of the resource
+
+    Returns:
+        Dict[str, Any]
+
+    Examples:
+        .. code-block:: sls
+
+        resource_is_absent:
+          gcp.iam.projects.service_account.absent
     """
     result = {
         "result": True,
-        "old_state": None,
+        "old_state": ctx.get("old_state"),
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
     if not resource_id:
-        resource_id = (ctx.old_state or {}).get("resource_id")
+        # we don't have enough information to know what to delete
+        result["comment"].append(
+            hub.tool.gcp.comment_utils.already_absent_comment(RESOURCE_TYPE_FULL, name)
+        )
+        return result
 
-    if not resource_id:
+    get_ret = await hub.exec.gcp.iam.projects.service_account.get(
+        ctx, resource_id=resource_id
+    )
+
+    if not get_ret["result"]:
+        result["result"] = False
         result["comment"].append(
-            hub.tool.aws.comment_utils.already_absent_comment(
-                "gcp.storage.buckets", name
+            hub.tool.gcp.comment_utils.resource_not_found_comment(
+                RESOURCE_TYPE_FULL, resource_id
             )
         )
+        result["comment"].extend(get_ret["comment"])
         return result
 
-    get_ret = await hub.exec.gcp.storage.buckets.get(ctx, name=name)
-    if not get_ret["result"] or not get_ret["ret"]:
-        result["result"] = get_ret["result"]
-        result["comment"] += get_ret["comment"]
-        # TODO: Should we get the old state from the context?
+    if not get_ret["ret"]:
+        result["comment"].append(
+            hub.tool.gcp.comment_utils.already_absent_comment(RESOURCE_TYPE_FULL, name)
+        )
         return result
 
+    result["old_state"] = get_ret["ret"]
+
     if ctx["test"]:
         result["comment"].append(
-            hub.tool.gcp.comment_utils.would_delete_comment("gcp.storage.bucket", name)
+            hub.tool.gcp.comment_utils.would_delete_comment(RESOURCE_TYPE_FULL, name)
         )
-        result["old_state"] = get_ret["ret"]
         return result
-    else:
-        # Delete the existing bucket (async call).
-        del_ret = await hub.exec.gcp.storage.buckets.delete(
-            ctx, name=name, resource_id=resource_id, userProject=user_project
-        )
-        if not del_ret["result"]:
-            result["result"] = False
-            result["comment"] += del_ret["comment"]
-            return result
 
-        result["old_state"] = get_ret["ret"]
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.delete_comment("gcp.storage.bucket", name)
-        )
+    del_ret = await hub.exec.gcp_api.client.iam.projects.service_account.delete(
+        ctx, name=resource_id
+    )
+
+    if not del_ret["result"]:
+        result["result"] = False
+        result["comment"].extend(del_ret["comment"])
+        return result
+
+    result["comment"].append(
+        hub.tool.gcp.comment_utils.delete_comment(RESOURCE_TYPE_FULL, name)
+    )
 
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r"""Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
+    """Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
-    Retrieves a list of buckets.
+    Lists every ServiceAccount that belongs to a specific project.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: bash
 
-            $ idem describe gcp.storage.buckets
+            $ idem describe gcp.iam.projects.service_accounts
     """
     result = {}
 
-    # TODO: Pagination
-    describe_ret = await hub.exec.gcp.storage.buckets.list(
+    describe_ret = await hub.exec.gcp.iam.projects.service_account.list(
         ctx, project=ctx.acct.project_id
     )
 
     if not describe_ret["result"]:
-        hub.log.debug(f"Could not describe buckets {describe_ret['comment']}")
+        hub.log.debug(
+            f"Could not describe gcp.iam.projects.service_account {describe_ret['comment']}"
+        )
         return {}
 
-    for resource in describe_ret["ret"]["items"]:
+    for resource in describe_ret["ret"]:
         resource_id = resource.get("resource_id")
+
         result[resource_id] = {
-            "gcp.storage.buckets.present": [
+            "gcp.iam.projects.service_account.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
+
     return result
 
 
 def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
+    """Default implemented for each module."""
     return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/case.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/case.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import builtins
+import keyword
 import re
 
 
 def camel(hub, string: str, dromedary: bool = True) -> str:
     """
     Change a snake-cased string to a camel-cased string
     """
@@ -12,14 +14,18 @@
         # Replace underscores with spaces then call str()'s title() method, then get rid of spaces
         result = string.replace("_", " ").title().replace(" ", "")
         if dromedary:
             return result[0].swapcase() + result[1:]
         return result
 
 
+def is_camel_case(hub, value: str) -> bool:
+    return hub.tool.gcp.case.camel(value) == value
+
+
 # TODO: Write a test to validate corner cases like abcXTZ
 def snake(hub, string: str) -> str:
     """
     Change a camel-cased string to a snake-cased string
     """
 
     # Separate each camel-cased word into underscore delimited words
@@ -28,7 +34,28 @@
     # Replace special characters with underscores except for [] and .
     string = re.sub(r"[^\w\[\]\.]", "_", string)
     # make sure everything is lower-cased
     string = string.lower()
     string = string.replace("__", "_")
 
     return string
+
+
+def sanitize_key(hub, key: str) -> str:
+    return hub.tool.gcp.case.unclash(hub.tool.gcp.case.snake(key))
+
+
+def is_snake_case(hub, value: str) -> bool:
+    return hub.tool.gcp.case.snake(value) == value
+
+
+def is_unclashed(hub, value: str) -> bool:
+    return hub.tool.gcp.case.unclash(value) == value
+
+
+def unclash(hub, string: str) -> str:
+    """
+    If the string name clashes with a builtin, then append an underscore
+    """
+    if keyword.iskeyword(string) or string in dir(builtins):
+        return f"{string}_"
+    return string
```

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/cloudkms/patch.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/cloudkms/patch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 from typing import Dict
 
 import deepdiff
+from dict_tools.data import NamespaceDict
 
 
 def calc_update_mask(hub, sls_data: Dict[str, Any], gcp_data: Dict[str, Any]) -> str:
     """Calculate update mask needed for patch methods in cloudkms.
 
     Do not include in the update mask properties present only in gcp_data.
 
@@ -14,20 +15,30 @@
         gcp_data: Second object to diff
 
     Returns:
          List of fields to be updated in this request. None if there are no differences.
 
          This is a comma-separated list of fully qualified names of fields. Example: "user.displayName,photo".
     """
-    if type(sls_data) != type(gcp_data):
+    if (
+        type(sls_data) != type(gcp_data)
+        and type(sls_data) not in (NamespaceDict, dict)
+        and type(gcp_data) not in (NamespaceDict, dict)
+    ):
         raise Exception(
             f"Dictionary params are of different types ({type(sls_data)} - {type(gcp_data)}."
             " deepdiff will not work correctly"
         )
-    diff = deepdiff.DeepDiff(sls_data, gcp_data, ignore_order=True, view="tree")
+    diff = deepdiff.DeepDiff(
+        sls_data,
+        gcp_data,
+        ignore_order=True,
+        view="tree",
+        ignore_type_in_groups=[(NamespaceDict, dict)],
+    )
 
     paths = set()
     for k in diff.affected_paths:
         if (
             isinstance(k.t1, deepdiff.helper.NotPresent)
             and not k.get_root_key() == "labels"
         ):
```

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/comment_utils.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/comment_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import List
+
+
 def create_comment(hub, resource_type: str, name: str) -> str:
     return f"Created {resource_type} '{name}'"
 
 
 def would_create_comment(hub, resource_type: str, name: str) -> str:
     return f"Would create {resource_type} '{name}'"
 
@@ -11,19 +14,27 @@
 
 
 def would_update_comment(hub, resource_type: str, name: str) -> str:
     return f"Would update {resource_type} '{name}'"
 
 
 def no_resource_delete_comment(hub, resource_type: str) -> str:
-    return f"Delete operation for resource type {resource_type} is not supported."
+    return (
+        f"No-Op: Delete operation for resource type {resource_type} is not supported."
+    )
 
 
 def no_resource_create_update_comment(hub, resource_type: str) -> str:
-    return f"Create and update operations for resource type {resource_type} are not supported."
+    return f"No-Op: Create and update operations for resource type {resource_type} are not supported."
+
+
+def no_resource_update_comment(hub, resource_type: str) -> str:
+    return (
+        f"No-Op: Update operation for resource type {resource_type} is not supported."
+    )
 
 
 def delete_comment(hub, resource_type: str, name: str) -> str:
     return f"Deleted {resource_type} '{name}'"
 
 
 def would_delete_comment(hub, resource_type: str, name: str) -> str:
@@ -50,14 +61,22 @@
     return f"Would update tags: Add keys {tags_to_add.keys()} Remove keys {tags_to_remove.keys()}"
 
 
 def get_empty_comment(hub, resource_type: str, name: str) -> str:
     return f"Get {resource_type} '{name}' result is empty"
 
 
+def resource_not_found_comment(hub, resource_type: str, resource_id: str) -> str:
+    return f"Could not find {resource_type} with resource_id={resource_id}"
+
+
+def resource_discovered_comment(hub, resource_type: str, resource_id: str) -> str:
+    return f"Discovered existing {resource_type} with resource_id={resource_id}"
+
+
 def list_empty_comment(hub, resource_type: str, name: str) -> str:
     return f"List {resource_type} '{name}' result is empty"
 
 
 def find_more_than_one(hub, resource_type: str, resource_id: str) -> str:
     return (
         f"More than one {resource_type} resource was found. Use resource {resource_id}"
@@ -69,14 +88,27 @@
 ) -> str:
     sorted_props = list(non_updatable_properties)
     sorted_props.sort()
     return f"Forbidden modification of non-updatable properties: {str(sorted_props)} for {resource_type} '{name}'"
 
 
 def no_resource_update_comment(hub, resource_type: str, resource_id: str) -> str:
-    return f"Update operation for resource type {resource_type} is not supported for {resource_id}."
+    return f"Update operation for resource type {resource_type} is not supported for {resource_id}"
 
 
 def ill_formed_resource_id_comment(
-    hub, resource_type: str, resource_id: str, reason: str
+    hub, resource_type: str, resource_id: str, resource_paths: List
 ) -> str:
-    return f"Ill-formed {resource_type} resource ID '{resource_id}': {reason}"
+    return f"Ill-formed {resource_type} resource ID '{resource_id}' does not match patterns {resource_paths}"
+
+
+def resource_not_found_comment(hub, resource_type: str, resource_id: str) -> str:
+    return f"Resource {resource_type} with resource ID '{resource_id}' not found"
+
+
+def properties_mismatch_resource_id_comment(
+    hub, resource_type: str, name: str = None
+) -> str:
+    hub.log.warning(
+        f"Property values mismatch resource_id for resource type {resource_type} with name {name}."
+    )
+    return f"WARNING: Property values mismatch resource_id for resource type {resource_type} with name {name}."
```

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/compute/network.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/network.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 from typing import Any
 from typing import Dict
 from typing import List
 
 
 async def update_peerings(
     hub,
@@ -9,73 +10,88 @@
     resource_id: str,
     current_peerings: List[Dict[str, Any]],
     new_peerings: List[Dict[str, Any]],
 ) -> Dict[str, Any]:
     result = {"result": False, "comment": []}
 
     current_peerings = current_peerings if current_peerings is not None else []
-    new_peerings = new_peerings if new_peerings is not None else current_peerings
+    new_peerings = new_peerings if new_peerings is not None else []
+
+    existing_peering_names = {
+        peering.get("name"): peering for peering in current_peerings
+    }
+    new_peering_names = {peering.get("name"): peering for peering in new_peerings}
 
-    peerings_map = {peering.get("name"): peering for peering in current_peerings}
     peerings_to_add = []
     peerings_to_update = []
 
-    for peering in new_peerings:
-        if peering.get("name") not in peerings_map:
-            peerings_to_add.append(peering)
+    for new_peering in new_peerings:
+        if new_peering.get("name") not in existing_peering_names:
+            peerings_to_add.append(new_peering)
         else:
-            element = peerings_map.pop(peering.get("name"))
-            needs_update: bool = (
-                element.get("exchange_subnet_routes")
-                != peering.get("exchange_subnet_routes")
-                or element.get("export_custom_routes")
-                != peering.get("export_custom_routes")
-                or element.get("export_subnet_routes_with_public_ip")
-                != peering.get("export_subnet_routes_with_public_ip")
-                or element.get("import_custom_routes")
-                != peering.get("import_custom_routes")
-                or element.get("import_subnet_routes_with_public_ip")
-                != peering.get("import_subnet_routes_with_public_ip")
-                or element.get("name") != peering.get("name")
-                or element.get("network") != peering.get("network")
-                or element.get("peer_mtu") != peering.get("peer_mtu")
-                or element.get("stack_type") != peering.get("stack_type")
+            peering_changes = hub.tool.gcp.utils.compare_states(
+                {"peering": new_peering},
+                {
+                    "peering": next(
+                        current_peering
+                        for current_peering in current_peerings
+                        if current_peering.get("name") == new_peering.get("name")
+                    )
+                },
+                resource_type=None,
+                additional_exclude_paths=["auto_create_routes"],
             )
 
-            if needs_update:
-                peerings_to_update.append(peering)
+            if peering_changes:
+                peerings_to_update.append(new_peering)
+
+    peerings_to_remove = [
+        peering
+        for peering in current_peerings
+        if peering.get("name") not in new_peering_names
+    ]
 
-    for peering in peerings_map.values():
+    # Remove peerings
+    for peering in peerings_to_remove:
         remove_peering_request_body = {"name": peering.get("name")}
 
         remove_ret = await hub.exec.gcp_api.client.compute.network.removePeering(
             ctx, resource_id=resource_id, body=remove_peering_request_body
         )
 
         r = await hub.tool.gcp.operation_utils.await_operation_completion(
             ctx, remove_ret, "compute.network", "compute.global_operation"
         )
         if not r["result"]:
             result["comment"] += r["comment"]
             return result
 
+    # Update peerings
     for peering in peerings_to_update:
-        update_peering_request_body = build_peering_request_body(peering)
+        # We want to remove this property, as it will soon be deprecated.
+        # exchange_subnet_routes should be used instead.
+        peering.pop("auto_create_routes", None)
+
+        # Ignoring this property, until figuring out why get does not return it and how to update it.
+        peering.pop("peer_mtu", None)
+
+        update_peering_request_body = {"network_peering": peering}
 
         update_ret = await hub.exec.gcp_api.client.compute.network.updatePeering(
             ctx, resource_id=resource_id, body=update_peering_request_body
         )
 
         r = await hub.tool.gcp.operation_utils.await_operation_completion(
             ctx, update_ret, "compute.network", "compute.global_operation"
         )
         if not r["result"]:
             result["comment"] += r["comment"]
             return result
 
+    # Add peerings
     r = await hub.tool.gcp.compute.network.add_peerings(
         ctx, resource_id, peerings_to_add
     )
 
     if not r["result"]:
         result["comment"] += r["comment"]
         return result
@@ -86,15 +102,19 @@
 
 async def add_peerings(
     hub, ctx, resource_id: str, peerings_to_add: Dict[str, Any]
 ) -> Dict[str, Any]:
     result = {"result": False, "comment": []}
 
     for peering in peerings_to_add:
-        add_peering_request_body = build_peering_request_body(peering)
+        # We want to remove this property, as it will soon be deprecated.
+        # exchange_subnet_routes should be used instead.
+        peering.pop("auto_create_routes", None)
+
+        add_peering_request_body = {"network_peering": peering}
 
         add_ret = await hub.exec.gcp_api.client.compute.network.addPeering(
             ctx, resource_id=resource_id, body=add_peering_request_body
         )
 
         r = await hub.tool.gcp.operation_utils.await_operation_completion(
             ctx, add_ret, "compute.network", "compute.global_operation"
@@ -103,27 +123,38 @@
             result["comment"] += r["comment"]
             return result
 
     result["result"] = True
     return result
 
 
-def build_peering_request_body(
-    peering: Dict[str, Dict[str, Any]]
-) -> Dict[str, Dict[str, Any]]:
-    return {
-        "network_peering": {
-            "exchange_subnet_routes": peering.get("exchange_subnet_routes"),
-            "export_custom_routes": peering.get("export_custom_routes"),
-            "export_subnet_routes_with_public_ip": peering.get(
-                "export_subnet_routes_with_public_ip"
-            ),
-            "import_custom_routes": peering.get("import_custom_routes"),
-            "import_subnet_routes_with_public_ip": peering.get(
-                "import_subnet_routes_with_public_ip"
-            ),
-            "name": peering.get("name"),
-            "network": peering.get("network"),
-            "peer_mtu": peering.get("peer_mtu"),
-            "stack_type": peering.get("stack_type"),
-        }
-    }
+def build_new_peerings_on_top_of_old(
+    hub, old_peerings: List[Dict[str, Any]], new_peerings: List[Dict[str, Any]]
+) -> List[Dict[str, Any]]:
+    if new_peerings:
+        new_peerings = copy.deepcopy(new_peerings)
+        # Ignoring this property, until figuring out why get does not return it and how to update it.
+        for peering in new_peerings:
+            peering.pop("peer_mtu", None)
+    if not new_peerings or not old_peerings:
+        return new_peerings
+
+    new_peerings = new_peerings or []
+    old_peerings = old_peerings or []
+
+    new_peerings_body = []
+    for new_peering in new_peerings:
+        old_peering = next(
+            peering
+            for peering in old_peerings
+            if new_peering.get("name") == peering.get("name")
+        )
+        if old_peering:
+            new_peering_body = hub.tool.gcp.utils.create_dict_body_on_top_of_old(
+                old_peering, new_peering
+            )
+        else:
+            new_peering_body = new_peering
+
+        new_peerings_body.append(new_peering_body)
+
+    return new_peerings_body
```

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/exec_context.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/exec_context.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/generic_exec.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/generic_exec.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 from typing import Any
 from typing import Dict
 
 from idem_gcp.tool.gcp.generate.exec_context import ExecutionContext
 
 
 def __init__(hub):
-    hub.tool.gcp.generate.PRE_EXECS_ORDER = ["resource_id_extractor", "function_getter"]
+    hub.tool.gcp.generate.PRE_EXECS_ORDER = [
+        "resource_id_extractor",
+        "parameter_sanitizer",
+        "function_getter",
+    ]
     hub.tool.gcp.generate.POST_EXECS_ORDER = ["operation_processor", "item_getter"]
 
 
 async def execute(hub, execution_context: ExecutionContext) -> Dict[str, Any]:
     for operator_name in hub.tool.gcp.generate.PRE_EXECS_ORDER:
         operator = hub.tool.gcp.generate.generic_exec.get_pre_exec_operator(
             operator_name
         )
         if await operator.should_operate(execution_context):
-            await operator.operate(execution_context)
+            try:
+                await operator.operate(execution_context)
+            except ValueError as e:
+                return {"result": False, "ret": None, "comment": [str(e)]}
 
     execution_context.response = await execution_context.method(
         **execution_context.method_params
     )
 
     for operator_name in hub.tool.gcp.generate.POST_EXECS_ORDER:
         operator = hub.tool.gcp.generate.generic_exec.get_post_exec_operator(
```

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/post_exec/item_getter.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/post_exec/item_getter.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,8 +9,11 @@
         and execution_context.response.get("ret") is not None
         and "items" in execution_context.response.get("ret")
     )
 
 
 async def operate(hub, execution_context: ExecutionContext) -> None:
     response = execution_context.response
-    execution_context.response = {**response, "ret": response.get("ret").get("items")}
+    execution_context.response = {
+        **response,
+        "ret": response.get("ret").get("items", []),
+    }
```

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/post_exec/operation_processor.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/post_exec/operation_processor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 from idem_gcp.tool.gcp.generate.exec_context import ExecutionContext
 
 
 async def should_operate(hub, execution_context: ExecutionContext) -> bool:
     return (
         execution_context.response is not None
         and execution_context.response.get("ret") is not None
-        and "compute#operation" in execution_context.response["ret"].get("kind", "")
+        and hub.tool.gcp.operation_utils.is_operation(execution_context.response["ret"])
     )
 
 
 async def operate(hub, execution_context: ExecutionContext) -> None:
     operation = execution_context.response["ret"]
     operation_type = hub.tool.gcp.generate.operators.post_exec.operation_processor.get_operation_type(
         operation
     )
     if operation_type is None:
         execution_context.response["result"] = False
-        execution_context.response["comment"] += "Unexpected operation type returned"
+        execution_context.response["comment"].append(
+            "Unexpected operation type returned"
+        )
         return
     operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
         operation.get("selfLink"), operation_type
     )
-    op_ret = await hub.tool.gcp.operation_utils.handle_operation(
+    handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
         execution_context.method_params.get("ctx"),
-        operation_id,
+        {"operation_id": operation_id},
         execution_context.resource_type,
         wait_until_done=True,
     )
 
-    if not op_ret["result"]:
+    if not handle_operation_ret["result"]:
         execution_context.response["result"] = False
-        execution_context.response["comment"] += op_ret["comment"]
+        execution_context.response["comment"] += handle_operation_ret["comment"]
         return
 
     # if op_ret["result"] is True, then the operation is finished and resource_id is returned
-    resource_id = op_ret.get("resource_id")
+    resource_id = handle_operation_ret.get("resource_id")
     resource_get_result = await hub.tool.gcp.generate.operators.post_exec.operation_processor.invoke_get_operation_for_resource(
         execution_context, resource_id
     )
 
     if resource_get_result is None:
         execution_context.response["result"] = False
-        execution_context.response["comment"] += "Could not find resource"
+        execution_context.response["comment"].append("Could not find resource")
         return
     if not resource_get_result["result"]:
         execution_context.response["result"] = False
         execution_context.response["comment"] += resource_get_result["comment"]
         return
 
     execution_context.response["result"] = True
```

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/pre_exec/function_getter.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/pre_exec/function_getter.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/pre_exec/resource_id_extractor.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/pre_exec/resource_id_extractor.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,10 +14,18 @@
     resource_id = extended_params.pop("resource_id", None)
     if resource_id is not None:
         resource_id_params = (
             hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
                 execution_context.resource_type, resource_id
             )
         )
-        extended_params.update(resource_id_params)
+        aliases = execution_context.exec_params[ExecParam.PATH_PARAM_ALIASES]
+        if not aliases:
+            extended_params.update(resource_id_params)
+        else:
+            for resource_id_param in resource_id_params:
+                if resource_id_param in aliases:
+                    extended_params[aliases[resource_id_param]] = resource_id_params[
+                        resource_id_param
+                    ]
 
     execution_context.method_params = extended_params
```

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/init.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,14 +400,15 @@
         )
 
         ret = discovery.build(
             serviceName=self.name,
             version=api_version,
             credentials=ctx.acct["credentials"],
             cache=self._cache,
+            discoveryServiceUrl=ctx.acct.get("discovery_service_url"),
         )
         self._api_resource = ret
 
         return ret
 
     def __getattr__(self, attr: str):
         """Gets and returns the named _GCPApi child.
```

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/operation_utils.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/operation_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-import time
+import asyncio
 from typing import Any
 from typing import Dict
 
 
 async def handle_operation(
     hub, ctx, rerun_data, resource_type: str, wait_until_done: bool = False
 ) -> Dict[str, Any]:
     result = {
         "comment": [],
         "result": True,
         "rerun_data": None,
         "resource_id": None,
     }
 
-    rerun_dict = isinstance(rerun_data, dict)
-    operation_id = rerun_data["operation_id"] if rerun_dict else rerun_data
-
+    operation_id = rerun_data.get("operation_id")
     operation_type = hub.tool.gcp.operation_utils.get_operation_type(operation_id)
 
     if operation_type is None:
         result["result"] = False
         result["comment"].append(
             f"Cannot determine operation scope (zonal/regional/global) {operation_id}"
         )
+        result["rerun_data"] = {"has_error": True}
         return result
 
     if operation_type == "compute.zone_operation":
         get_ret = await hub.exec.gcp_api.client.compute.zone_operation.get(
             ctx, resource_id=operation_id
         )
     elif operation_type == "compute.region_operation":
@@ -37,51 +36,60 @@
         get_ret = await hub.exec.gcp_api.client.compute.global_operation.get(
             ctx, resource_id=operation_id
         )
 
     if not get_ret["result"] or not get_ret["ret"]:
         result["result"] = False
         result["comment"] = get_ret["comment"]
+        result["rerun_data"] = {"has_error": True}
         return result
 
     operation = get_ret["ret"]
+    op_ret = {}
     if operation["status"] != "DONE":
         if wait_until_done:
-            operation = await hub.tool.gcp.operation_utils.wait_for_operation(
+            op_ret = await hub.tool.gcp.operation_utils.wait_for_operation(
                 ctx, operation, operation_type
             )
+            operation = op_ret["ret"]
         else:
             result["result"] = False
             new_operation_id = (
                 hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
                     operation.get("selfLink"), operation_type
                 )
             )
-            if rerun_dict:
-                rerun_data["operation_id"] = new_operation_id
-            else:
-                rerun_data = new_operation_id
+            rerun_data["operation_id"] = new_operation_id
             result["rerun_data"] = rerun_data
 
             result["comment"] += get_ret["comment"]
             return result
 
-    if operation.get("error"):
+    op_ret_error_comments = [
+        comment for comment in op_ret.get("comment", []) if "errors" in comment
+    ]
+    if (operation and operation.get("error")) or op_ret_error_comments:
         result["result"] = False
-        result["comment"] += str(operation.get("error", {}))
+        if operation:
+            result["comment"].append(str(operation.get("error", {})))
+
+        result["comment"] += op_ret_error_comments
+        result["rerun_data"] = {"has_error": True}
         return result
 
     result["resource_id"] = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
         operation.get("targetLink"), resource_type
     )
 
     return result
 
 
 async def wait_for_operation(hub, ctx, operation, operation_type: str) -> Dict:
+    max_timeout_retries = 5
+    timeout_retries = 0
     while True:
         if operation_type == "compute.zone_operation":
             op_ret = await hub.exec.gcp_api.client.compute.zone_operation.wait(
                 ctx, resource_id=operation["selfLink"]
             )
         elif operation_type == "compute.region_operation":
             op_ret = await hub.exec.gcp_api.client.compute.region_operation.wait(
@@ -89,27 +97,39 @@
             )
         elif operation_type == "compute.global_operation":
             op_ret = await hub.exec.gcp_api.client.compute.global_operation.wait(
                 ctx, resource_id=operation["selfLink"]
             )
 
         if not op_ret or not op_ret["ret"] or not op_ret["result"]:
-            # wait() call timed out?
-            break
+            if timeout_retries < max_timeout_retries:
+                timeout_retries += 1
+                continue
+            else:
+                break
 
         operation = op_ret["ret"]
-        if operation["status"] == "DONE" or "error" in operation:
+        op_ret_error_comments = [
+            comment for comment in op_ret["comment"] if "errors" in comment
+        ]
+        if (
+            operation["status"] == "DONE"
+            or "error" in operation
+            or op_ret_error_comments
+        ):
             break
 
-        time.sleep(1)
+        await asyncio.sleep(1)
 
-    return operation
+    return op_ret
 
 
 def get_operation_type(hub, operation_id) -> str:
+    if not operation_id:
+        return None
     if "/zones/" in operation_id:
         return "compute.zone_operation"
     elif "/regions/" in operation_id:
         return "compute.region_operation"
     elif "/global/" in operation_id:
         return "compute.global_operation"
     else:
@@ -121,23 +141,29 @@
 ) -> Dict[str, Any]:
     result = {"result": False, "comment": []}
 
     if not api_call_ret["result"] and not api_call_ret["ret"]:
         result["comment"] += api_call_ret["comment"]
         return result
 
-    if "compute#operation" in api_call_ret["ret"].get("kind"):
+    if hub.tool.gcp.operation_utils.is_operation(api_call_ret["ret"]):
         operation = api_call_ret["ret"]
 
         operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
             operation.get("selfLink"), operation_type
         )
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, operation_id, resource_type, True
+            ctx, {"operation_id": operation_id}, resource_type, True
         )
 
         if not handle_operation_ret["result"]:
             result["comment"] += handle_operation_ret["comment"]
             return result
 
     result["result"] = True
     return result
+
+
+def is_operation(hub, candidate) -> bool:
+    return (
+        candidate and "kind" in candidate and candidate["kind"].endswith("#operation")
+    )
```

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/policy.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     auditConfigs: List[AuditConfig] = None
     etag: str = None
 
 
 async def set_iam_policy(
     hub, ctx, sub, resource: str, policy: Policy, update_mask: str
 ) -> Dict[str, Any]:
-
     ret = await sub.setIamPolicy(
         ctx, resource=resource, body={"policy": policy, "updateMask": update_mask}
     )
     return ret
 
 
 async def get_iam_policy(
```

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/resolver.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/resolver.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 
 will work, even though no exec subdirectories exist to match that call path.
 Instead, the API is dynamically discovered and built to match and tie
 them to the appropriate GCP Python SDK wrappers within the tool Sub of this
 project.
 """
 import copy
+import uuid
 from inspect import signature
 from typing import Dict
 from typing import List
+from typing import Optional
+from typing import Tuple
 
 from pop.loader import LoadedMod
 
 from idem_gcp.helpers.exc import NotFoundError
 
 _GCP_SUB_CACHE = {}
 _GCP_RESOURCE_TYPES_CACHE = {}
@@ -35,32 +38,40 @@
     :param hub: The Hub into which the resolved callable will get placed.
     :param ref: The call path reference. For example:
         "hub.exec.gcp.compute.instance.get".
     """
 
     def gen_sub(ref: str, gcp_api):
         callpath = ref.split(".")
+        method_name = callpath[-1]
         resource_type = ".".join(callpath[1:-1])
-        native_resource_type = hub.tool.gcp.resolver.find_native_resource_type(
+        native_resource_types = hub.tool.gcp.resolver.find_native_resource_types(
             resource_type
         )
-        method_name = callpath[-1]
-        callpath = callpath[0:1] + native_resource_type.split(".") + [callpath[-1]]
-        callpath[0:-1] = [hub.tool.gcp.case.camel(v) for v in callpath[0:-1]]
-
-        gcp_api_sub = gcp_api
-        for c in callpath[1:]:
-            gcp_api_sub = getattr(gcp_api_sub, c)
-        cm = ContractMod(
-            hub, gcp_api_sub, resource_type, native_resource_type, method_name
+        assert len(native_resource_types) > 0
+        cms = []
+        for nr_type in native_resource_types:
+            cpath = callpath[0:1] + nr_type.split(".") + [method_name]
+            cpath[0:-1] = [hub.tool.gcp.case.camel(v) for v in cpath[0:-1]]
+
+            gcp_api_sub = gcp_api
+            for c in cpath[1:]:
+                gcp_api_sub = getattr(gcp_api_sub, c)
+            cm = ContractMod(hub, gcp_api_sub, resource_type, nr_type, method_name)
+            cms.append(cm)
+
+        _GCP_SUB_CACHE[ref] = (
+            CompositeContractMod(hub, resource_type, method_name, cms)
+            if len(cms) > 1
+            else cms[0]
         )
-        _GCP_SUB_CACHE[ref] = cm
-        return cm
 
-    return _GCP_SUB_CACHE.get(ref, gen_sub(ref, gcp_api))
+        return _GCP_SUB_CACHE[ref]
+
+    return _GCP_SUB_CACHE.get(ref) or gen_sub(ref, gcp_api)
 
 
 class ContractMod(LoadedMod):
     """
     A Sub (class) to represent actually callable methods within Azure
     ...ManagementClient API sets.
 
@@ -127,44 +138,69 @@
                     self._resource_type, resource_id
                 )
             )
 
         if present_params.get("user_project") == "None":
             present_params["user_project"] = None
 
-        exclude_keys_from_transformation = None
+        exclude_keys_from_transformation = []
         if present_params.get("body", False):
             exclude_keys_from_transformation = self._hub.tool.gcp.resource_prop_utils.get_exclude_keys_from_transformation(
-                present_params["body"], self._resource_type
+                present_params["body"], self._resource_type, is_raw_resource=False
             )
 
+        manual_mappings = self._hub.tool.gcp.resource_prop_utils.get_manual_mappings(
+            self._resource_type
+        )
         raw_params = (
             self._hub.tool.gcp.conversion_utils.convert_present_resource_to_raw(
-                present_params, self._resource_type, exclude_keys_from_transformation
+                present_params,
+                self._resource_type,
+                exclude_keys_from_transformation,
+                manual_mappings,
             )
         )
 
         # TODO: Fix projection required or not
-        if self._method_name in {"create"} and not self._resource_type.startswith(
-            "cloudkms"
+        if (
+            self._method_name in {"create"}
+            and not self._resource_type.startswith("cloudkms")
+            and not self._resource_type.startswith("iam")
         ):
             raw_params["projection"] = "full"
 
+        if is_request_property(
+            self._hub, "name", self._resource_type, self._method_name
+        ):
+            raw_params["name"] = kwargs["name"]
+
+        raw_params = self._hub.tool.gcp.sanitizers.sanitize_resource_urls(raw_params)
+
         try:
             response = await self._gcp_method(ctx, *args, **raw_params)
             # Is it possible to get None for response. It looks like on error exceptions is thrown. If we are here
             # then the call was successful.
             if response is None:
                 result["result"] = False
                 return result
 
+            if not response:
+                result["ret"] = response
+                return result
+
             if "#operation" in response.get("kind", ""):
                 result["ret"] = response
                 return result
 
+            response_field = get_response_field(
+                self._hub, self._resource_type, self._method_name
+            )
+            if response_field:
+                response["items"] = response[response_field]
+
             items = response.get("items")
             if isinstance(items, dict):
                 response[
                     "items"
                 ] = self._hub.tool.gcp.resolver.convert_dict_items_to_list(
                     items, self._native_resource_type
                 )
@@ -180,109 +216,233 @@
             if response.get("nextPageToken"):
                 all_items = response.get("items", [])
                 raw_params["pageToken"] = response["nextPageToken"]
 
                 while response.get("nextPageToken"):
                     response = await self._gcp_method(ctx, *args, **raw_params)
 
-                    items = response.get("items")
+                    response_field = (
+                        get_response_field(
+                            self._hub, self._resource_type, self._method_name
+                        )
+                        or "items"
+                    )
+                    items = response.get(response_field)
                     if isinstance(items, dict):
                         response[
                             "items"
                         ] = self._hub.tool.gcp.resolver.convert_dict_items_to_list(
                             items, self._native_resource_type
                         )
 
                     resource_type_camel = self._hub.tool.gcp.case.camel(
                         self._native_resource_type.split(".")[-1]
                     )
                     if resource_type_camel in response:
-                        response["items"] = response[resource_type_camel]
+                        response[response_field] = response[resource_type_camel]
 
-                    all_items += response.get("items", [])
+                    all_items += response.get(response_field, [])
                     raw_params["pageToken"] = response.get("nextPageToken")
 
                 response["items"] = all_items
 
             result["ret"] = self._hub.tool.gcp.resolver.process_response(
                 response, self._resource_type, self._method_name
             )
+            result["ret"] = self._hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                result["ret"]
+            )
         except Exception as e:
             if self._method_name == "get" and isinstance(e, NotFoundError):
                 result["comment"].append(
                     self._hub.tool.gcp.comment_utils.get_empty_comment(
                         self._resource_type, name if name else resource_id
                     )
                 )
             else:
                 result["result"] = False
             result["comment"].append(str(e))
 
         return result
 
 
+class CompositeContractMod(LoadedMod):
+    def __init__(
+        self, hub, resource_type: str, method_name: str, mods: List[ContractMod]
+    ):
+        super().__init__(name=f"composite:{uuid.uuid4()}")
+        self._hub = hub
+        self._resource_type = resource_type
+        self._method_name = method_name
+        self._mods = mods
+
+    @property
+    def signature(self):
+        return signature(self.__call__)
+
+    def _missing(self, item: str):
+        return self
+
+    async def __call__(self, ctx, *args, **kwargs):
+        result = {"result": False, "ret": None, "comment": []}
+
+        pending_comments = []
+        mods_to_call = []
+        if self.should_aggregate_results():
+            mods_to_call.extend(self._mods)
+        else:
+            mod, err = self.find_best_matching_mod(**kwargs)
+            if mod:
+                mods_to_call.append(mod)
+            elif err:
+                result["comment"].append(err)
+
+        for mod in mods_to_call:
+            result_from_mod = await mod(ctx, *args, **kwargs)
+            if result_from_mod["result"]:
+                result["comment"] += result_from_mod["comment"]
+                result["result"] = True
+                if result["ret"]:
+                    result["ret"].extend(result_from_mod["ret"])
+                else:
+                    result["ret"] = result_from_mod["ret"]
+            else:
+                pending_comments += result_from_mod["comment"]
+
+        if not result["result"]:
+            result["comment"].extend(pending_comments)
+
+        return result
+
+    def find_best_matching_mod(
+        self, **kwargs
+    ) -> Tuple[Optional[ContractMod], Optional[str]]:
+        resource_paths = self._hub.tool.gcp.resource_prop_utils.get_resource_paths(
+            self._resource_type
+        )
+        assert len(self._mods) == len(resource_paths)
+
+        result = None
+        multiple_max_scores = False
+        max_score_so_far = -1
+        for idx, path in enumerate(resource_paths):
+            score = self.compute_matching_score(path, **kwargs)
+            if score > max_score_so_far:
+                max_score_so_far = score
+                result = self._mods[idx]
+                multiple_max_scores = False
+            elif score == max_score_so_far:
+                multiple_max_scores = True
+
+        if multiple_max_scores:
+            msg = f"Multiple resource paths of {self._resource_type} match the input arguments fully or partially."
+            self._hub.log.error(msg)
+            return None, msg
+
+        if not result:
+            msg = (
+                f"No resource paths of {self._resource_type} match the input arguments."
+            )
+            self._hub.log.warning(msg)
+            return None, msg
+
+        return result, None
+
+    def compute_matching_score(self, resource_path: str, **kwargs) -> int:
+        score = 0
+        params = self._hub.tool.gcp.resource_prop_utils.get_path_parameters_for_path(
+            resource_path
+        )
+
+        if "resource_id" in kwargs:
+            resource_id = kwargs.get("resource_id")
+            if (
+                self._hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id_and_path(
+                    resource_id, self._resource_type, resource_path
+                )
+                is not None
+            ):
+                score = len(params)
+        else:
+            for param in params:
+                if param in kwargs:
+                    score += 1
+
+        return score
+
+    def should_aggregate_results(self) -> bool:
+        return self._method_name in ["list", "aggregatedList"]
+
+
 def process_response(hub, response: Dict, resource_type: str, method_name: str) -> Dict:
     # TODO: Get does not return all the necessary properties which should be the present properties so
     #  decide what to do
 
     present_props_names = hub.tool.gcp.resource_prop_utils.get_present_properties(
         resource_type
     )
     singular_result_expected = hub.tool.gcp.resolver.has_singular_result(
         response, resource_type, method_name
     )
     if singular_result_expected:
+        if method_name == "get":
+            hub.tool.gcp.resource_prop_utils.populate_resource_with_assumed_values(
+                response, resource_type
+            )
+
         resource_id = hub.tool.gcp.resource_prop_utils.extract_resource_id(
             response, resource_type
         )
         if resource_id:
             present_item = hub.tool.gcp.resolver.filter_raw_properties_to_present(
                 response, present_props_names, resource_type, resource_id
             )
             return present_item
 
         return response
     else:
         # Multiple entries in call result, e.g. after list() call
         ret_items = []
-        for service_resource in response.get("items") or {}:
+        for service_resource in response.get("items") or []:
+            hub.tool.gcp.resource_prop_utils.populate_resource_with_assumed_values(
+                service_resource, resource_type
+            )
+
             resource_id = hub.tool.gcp.resource_prop_utils.extract_resource_id(
                 service_resource, resource_type
             )
 
             present_item = None
             if resource_id:
                 present_item = hub.tool.gcp.resolver.filter_raw_properties_to_present(
                     service_resource, present_props_names, resource_type, resource_id
                 )
 
             ret_items.append(present_item if present_item else service_resource)
 
         return {"items": ret_items}
 
-    return {}
-
 
 def filter_raw_properties_to_present(
     hub,
     raw_props: Dict,
     present_properties_names: List,
     resource_type: str,
     resource_id: str,
 ) -> Dict:
     filtered = {
         key: value
         for key, value in raw_props.items()
         if key in present_properties_names
     }
     filtered["resource_id"] = resource_id
-    filtered = hub.tool.gcp.resource_prop_utils.format_path_params(
+    hub.tool.gcp.resource_prop_utils.format_path_params(filtered, resource_type)
+    return hub.tool.gcp.conversion_utils.convert_raw_resource_to_present(
         filtered, resource_type
     )
-    return hub.tool.gcp.conversion_utils.convert_raw_resource_to_present(filtered)
 
 
 def convert_dict_items_to_list(hub, dict_items: Dict, resource_type: str) -> list:
     list_items = []
     simple_resource_type = resource_type.split(".")[-1]
     simple_resource_type_camel = hub.tool.gcp.case.camel(simple_resource_type)
 
@@ -307,20 +467,52 @@
     if isinstance(response.get("items"), list):
         return False
     if method_name in {"list", "aggregatedList", "describe"}:
         return False
     return True
 
 
-def find_native_resource_type(hub, resource_type: str) -> str:
+def find_native_resource_types(hub, resource_type: str) -> str:
     def fetch_res_type_mapping(res_type: str) -> str:
         hub_ref = hub.metadata.gcp
         for part in res_type.split("."):
             hub_ref = hub_ref[part]
         try:
-            return hub_ref["NATIVE_RESOURCE_TYPE"]
+            ret = hub_ref["NATIVE_RESOURCE_TYPE"]
         except AttributeError:
-            return res_type
+            hub.log.warning(f"Can't find native resource type for {resource_type}")
+            ret = res_type
 
-    return _GCP_RESOURCE_TYPES_CACHE.get(
-        resource_type, fetch_res_type_mapping(resource_type)
+        _GCP_RESOURCE_TYPES_CACHE[res_type] = ret if isinstance(ret, list) else [ret]
+        return _GCP_RESOURCE_TYPES_CACHE[res_type]
+
+    return _GCP_RESOURCE_TYPES_CACHE.get(resource_type) or fetch_res_type_mapping(
+        resource_type
     )
+
+
+def is_request_property(hub, prop: str, resource_type: str, method_name: str) -> bool:
+    """
+    Returns true if the specified property is a path parameter.
+    """
+    resource_methods_properties = hub.tool.gcp.RESOURCE_PROPS[resource_type]
+    requests_parameters = resource_methods_properties.get("request_parameters", {})
+    method_params = requests_parameters.get(method_name, [])
+    return prop in method_params
+
+
+def get_response_field(hub, resource_type: str, method_name: str) -> str:
+    """
+    Returns the name of the property which contains the actual resource inside the response body.
+
+    For example: the response body when listing service accounts has the following structure:
+    {
+      "accounts": [
+        object (ServiceAccount)
+      ],
+      "nextPageToken": string
+    }
+    In this case the result will be 'accounts'.
+    """
+    resource_methods_properties = hub.tool.gcp.RESOURCE_PROPS[resource_type]
+    response_fields = resource_methods_properties.get("response_fields", {})
+    return response_fields.get(method_name)
```

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/resource_prop_utils.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/resource_prop_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import copy
 import re
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Set
 
 import yaml
@@ -21,92 +20,93 @@
     #  to snake case here so that we do not have to do conversion
     #  very often anywhere these snake case properties names are needed.
     #  Check if hub.tool.gcp.RESOURCE_PROPS are always convert to snake case
 
     hub.tool.gcp.RESOURCE_PROPS = yaml.safe_load(file_text)
 
 
-def get_create_properties(hub, resource_type: str, convert_to_present=True) -> Set:
+def get_create_properties(
+    hub, resource_type: str, convert_to_present: bool = True
+) -> Set:
     resource_methods_properties = hub.tool.gcp.RESOURCE_PROPS[resource_type]
     raw_props = set(
         resource_methods_properties.get("insert", {})
         or resource_methods_properties.get("create", {})
     )
     if raw_props and convert_to_present:
         return hub.tool.gcp.conversion_utils.convert_raw_properties_to_present(
             raw_props
         )
     return raw_props
 
 
-def get_update_properties(hub, resource_type: str, convert_to_present=True) -> Set:
+def get_update_properties(
+    hub, resource_type: str, convert_to_present: bool = True
+) -> Set:
     raw_props = set(hub.tool.gcp.RESOURCE_PROPS[resource_type].get("update", {}))
-    if convert_to_present:
+    if raw_props and convert_to_present:
         return hub.tool.gcp.conversion_utils.convert_raw_properties_to_present(
             raw_props
         )
     return raw_props
 
 
-def get_fields_of_enum_type(hub, resource_type: str, convert_to_present=True) -> Set:
+def get_fields_of_enum_type(
+    hub, resource_type: str, convert_to_present: bool = True
+) -> Set:
     raw_props = set(
         hub.tool.gcp.RESOURCE_PROPS[resource_type].get("fields_enum_type", {})
     )
     if convert_to_present:
         return hub.tool.gcp.conversion_utils.convert_raw_properties_to_present(
             raw_props
         )
     return raw_props
 
 
-def get_get_properties(hub, resource_type: str, convert_to_present=True) -> Set:
-    raw_props = set(hub.tool.gcp.RESOURCE_PROPS[resource_type].get("get", {}))
-    if convert_to_present:
-        return hub.tool.gcp.conversion_utils.convert_raw_properties_to_present(
-            raw_props
-        )
-    return raw_props
-
+def get_non_updatable_properties(hub, resource_type: str) -> Set:
+    raw_non_updatable_properties = set()
 
-def get_delete_properties(hub, resource_type: str, convert_to_present=True) -> Set:
-    raw_props = set(hub.tool.gcp.RESOURCE_PROPS[resource_type].get("delete", {}))
-    if convert_to_present:
-        return hub.tool.gcp.conversion_utils.convert_raw_properties_to_present(
-            raw_props
+    raw_non_updatable_properties.update(
+        hub.tool.gcp.RESOURCE_PROPS[resource_type].get(
+            "nested_non_updatable_properties", []
         )
-    return raw_props
+    )
 
+    raw_non_updatable_properties.update(
+        hub.tool.gcp.resource_prop_utils.get_create_properties(resource_type)
+        - hub.tool.gcp.resource_prop_utils.get_update_properties(resource_type)
+    )
 
-def get_non_updatable_properties(hub, resource_type: str) -> Set:
-    raw_nested_non_updatable_properties = hub.tool.gcp.RESOURCE_PROPS[
-        resource_type
-    ].get("nested_non_updatable_properties", [])
+    raw_non_updatable_properties.update(
+        hub.tool.gcp.resource_prop_utils.get_readonly_return_props(resource_type)
+    )
 
     non_updatable_properties = set(
         hub.tool.gcp.conversion_utils.convert_raw_properties_to_present(
-            raw_nested_non_updatable_properties
+            raw_non_updatable_properties
         )
     )
 
-    non_updatable_properties.update(
-        hub.tool.gcp.resource_prop_utils.get_create_properties(resource_type)
-        - hub.tool.gcp.resource_prop_utils.get_update_properties(resource_type)
-    )
     return non_updatable_properties
 
 
 def get_changed_non_updatable_properties(
     hub, resource_type: str, changes: DeepDiff
 ) -> Set:
+    if not changes:
+        return set()
+
     non_updatable_properties = (
         hub.tool.gcp.resource_prop_utils.get_non_updatable_properties(resource_type)
     )
 
     changed_non_updatable_properties = set()
-    for changed_property_full_path in changes.affected_paths:
+
+    for changed_property_full_path in changes.get("relevant_changes", {}):
         # This formats changed_property_full_path from e.g. "root['network_interfaces'][0]['alias_ip_ranges']"
         # to "network_interfaces[].alias_ip_ranges"
         changed_property_path_elements = re.findall(
             r"(?<=\[).*?(?=\])", changed_property_full_path
         )
         formatted_path_elements = []
         for i in range(len(changed_property_path_elements)):
@@ -115,18 +115,16 @@
             else:
                 if i > 0:
                     formatted_path_elements.append(".")
                 formatted_path_elements.append(
                     changed_property_path_elements[i].strip("'")
                 )
         formatted_property_path = "".join(formatted_path_elements)
-        for non_updatable_property_path in non_updatable_properties:
-            if non_updatable_property_path in formatted_property_path:
-                changed_non_updatable_properties.add(non_updatable_property_path)
-                break
+        if formatted_property_path in non_updatable_properties:
+            changed_non_updatable_properties.add(formatted_property_path)
 
     return changed_non_updatable_properties
 
 
 def get_present_properties(hub, resource_type: str) -> Set:
     return (
         hub.tool.gcp.resource_prop_utils.get_create_properties(resource_type, False)
@@ -134,238 +132,446 @@
             hub.tool.gcp.resource_prop_utils.get_update_properties(resource_type, False)
         )
         .union(
             hub.tool.gcp.resource_prop_utils.get_fields_of_enum_type(
                 resource_type, False
             )
         )
+        .union(
+            hub.tool.gcp.resource_prop_utils.get_readonly_return_props(
+                resource_type, False
+            )
+        )
     )
 
 
 def get_exclude_paths(hub, resource_type: str) -> Set:
     raw_props_names = hub.tool.gcp.RESOURCE_PROPS[resource_type].get(
         "exclude_paths", []
     )
     return set(
         hub.tool.gcp.conversion_utils.convert_raw_properties_to_present(raw_props_names)
     )
 
 
 def get_exclude_properties_from_transformation(
-    hub, resource_type: str, convert_to_present=True
+    hub, resource_type: str, convert_to_present: bool
 ) -> Set:
     resource_methods_properties = hub.tool.gcp.RESOURCE_PROPS[resource_type]
     raw_props = set(
         resource_methods_properties.get("exclude_properties_from_transformation", {})
     )
     if raw_props and convert_to_present:
         return hub.tool.gcp.conversion_utils.convert_raw_properties_to_present(
             raw_props
         )
     return raw_props
 
 
 def get_exclude_keys_from_transformation(
-    hub, resource_body: Dict[str, Any], resource_type: str = None
+    hub, resource_body: Dict[str, Any], resource_type: str, is_raw_resource: bool
 ) -> List[str]:
     # Get the properties whose keys should be excluded from transformation
     exclude_properties_from_transformation = (
         hub.tool.gcp.resource_prop_utils.get_exclude_properties_from_transformation(
-            resource_type
+            resource_type, convert_to_present=(not is_raw_resource)
         )
     )
 
-    # Create a list, which has lists per each property and have the properties' keys as items
-    list_of_properties_key_lists = [
-        list(resource_body[item].keys()) if resource_body.get(item, False) else []
-        for item in exclude_properties_from_transformation
-    ]
-
-    # Map the list_of_properties_key_lists to a list containing only the keys to be excluded
     exclude_keys_from_transformation = []
-    for _list in list_of_properties_key_lists:
-        exclude_keys_from_transformation += _list
+    _populate_list_with_keys_from_specified_dict_properties(
+        resource_body,
+        exclude_properties_from_transformation,
+        exclude_keys_from_transformation,
+    )
 
     return exclude_keys_from_transformation
 
 
+def _populate_list_with_keys_from_specified_dict_properties(
+    resource,
+    properties: List[str],
+    key_list: List[str],
+    path_prefix: str = "",
+) -> List[str]:
+    if key_list is None:
+        return
+
+    if isinstance(resource, list) or isinstance(resource, set):
+        for item in resource:
+            _populate_list_with_keys_from_specified_dict_properties(
+                item, properties, key_list, path_prefix
+            )
+    elif isinstance(resource, dict):
+        for k, v in resource.items():
+            if k in properties:
+                if resource.get(k) and isinstance(resource[k], dict):
+                    key_list += list(resource[k].keys())
+            else:
+                _populate_list_with_keys_from_specified_dict_properties(
+                    v, properties, key_list, f"{path_prefix}{k}."
+                )
+    return
+
+
 def extract_resource_id(hub, input_props: Dict, resource_type: str) -> Dict:
     if "selfLink" in input_props:
         return hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
             input_props.get("selfLink"), resource_type
         )
 
     if "resource_id" in hub.tool.gcp.RESOURCE_PROPS[resource_type]:
         resource_id_fields = hub.tool.gcp.RESOURCE_PROPS[resource_type]["resource_id"]
         for resource_id_field in resource_id_fields:
             if resource_id_field in input_props:
                 return input_props[resource_id_field]
 
 
-def get_resource_path(hub, resource_type: str) -> str:
+def get_resource_paths(hub, resource_type: str) -> List[str]:
     resource_path = resource_type.split(".")
     hub_ref = hub.metadata.gcp
     for resource_path_segment in resource_path:
         hub_ref = hub_ref[resource_path_segment]
 
-    return hub_ref["PATH"]
+    result = hub_ref["PATH"]
+    return result if isinstance(result, list) else [result]
 
 
-def get_resource_id_property_name(hub, resource_type: str, method_name: str) -> str:
-    resource_id_props = hub.tool.gcp.RESOURCE_PROPS[resource_type]["resource_id"]
-    method_properties = {}
-    if method_name == "get":
-        method_properties = hub.tool.gcp.resource_prop_utils.get_get_properties(
-            resource_type
-        )
-    elif method_name == "insert" or method_name == "create":
-        method_properties = hub.tool.gcp.resource_prop_utils.get_create_properties(
-            resource_type
-        )
-    elif method_name == "update":
-        method_properties = hub.tool.gcp.resource_prop_utils.get_update_properties(
-            resource_type
-        )
-    elif method_name == "delete":
-        method_properties = hub.tool.gcp.resource_prop_utils.get_delete_properties(
-            resource_type
-        )
+def get_elements_from_resource_id(hub, resource_type: str, resource_id: str) -> Dict:
+    resource_paths = hub.tool.gcp.resource_prop_utils.get_resource_paths(resource_type)
 
-    for resource_id_prop in resource_id_props:
-        if resource_id_prop in method_properties:
-            return resource_id_prop
+    result = None
+    for path in resource_paths:
+        r = hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id_and_path(
+            resource_type, resource_id, path
+        )
+        if r:
+            if result:
+                msg = f"Resource ID {resource_id} matches multiple resource paths of {resource_type}"
+                hub.log.error(msg)
+                return {}
+            result = r
+
+    if not result:
+        comment = hub.tool.gcp.comment_utils.ill_formed_resource_id_comment(
+            resource_type, resource_id, resource_paths
+        )
+        raise ValueError(comment)
 
-    return ""
+    return result
 
 
-def get_elements_from_resource_id(hub, resource_type: str, resource_id: str) -> Dict:
-    resource_path = hub.tool.gcp.resource_prop_utils.get_resource_path(resource_type)
+def get_elements_from_resource_id_and_path(
+    hub, resource_type: str, resource_id: str, resource_path: str
+) -> Dict:
     src = resource_path.split("/")
     act = resource_id.split("/")
     result = {}
 
     if len(act) < len(src):
-        hub.log.warning(
-            hub.tool.gcp.comment_utils.ill_formed_resource_id_comment(
-                resource_type, resource_id, "insufficient number of segments."
-            )
-        )
         return {}
 
     idx = -1
     for s in reversed(src):
         val = act[idx]
         if s.startswith("{") and s.endswith("}"):
             key = s[1:-1]
             result[key] = val
         elif val != s:
-            hub.log.warning(
-                hub.tool.gcp.comment_utils.ill_formed_resource_id_comment(
-                    resource_type, resource_id, "segment names do not match."
-                )
-            )
             return {}
         idx -= 1
 
     return result
 
 
-def parse_link_to_resource_id(hub, link, resource_type: str):
-    resource_path = hub.tool.gcp.resource_prop_utils.get_resource_path(resource_type)
-    result = copy.deepcopy(resource_path)
+def parse_link_to_resource_id_and_path(
+    hub, link, resource_type: str, resource_path: str
+) -> str:
+    result = resource_path
     src = result.split("/")
     act = link.split("/")
 
     if len(act) < len(src):
         return None
 
     idx = -1
     for s in reversed(src):
         val = act[idx]
         if s.startswith("{") and s.endswith("}"):
             result = result.replace(s, val)
         elif val != s:
-            hub.log.warning(
-                f"Resource selfLink differs from the actual path for resource type: {resource_type}"
-                f"\nselfLink: {link}, PATH: {resource_path}"
-            )
             return None
         idx -= 1
 
     return result
 
 
+def parse_link_to_resource_id(
+    hub, link, resource_type: str, log_warnings: bool = True
+) -> str:
+    resource_paths = hub.tool.gcp.resource_prop_utils.get_resource_paths(resource_type)
+    result = None
+    for path in resource_paths:
+        r = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id_and_path(
+            link, resource_type, path
+        )
+        if r:
+            if result:
+                msg = f"Link {link} matches multiple resource paths of {resource_type}"
+                hub.log.error(msg)
+                return None
+            result = r
+
+    if not result:
+        if log_warnings:
+            msg = f"Link {link} matches no resource paths of {resource_type}"
+            hub.log.warning(msg)
+        return None
+
+    return result
+
+
 def construct_resource_id(hub, resource_type: str, input_props: Dict[str, Any]) -> str:
     if input_props is not None and input_props.get("name") is not None:
         # handle case where "name" contains full resource id
         name = input_props.get("name")
-        if (
-            hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                name, resource_type
-            )
-            is not None
-        ):
-            return name
-
-    resource_path = hub.tool.gcp.resource_prop_utils.get_resource_path(resource_type)
-    try:
-        filtered_without_none_properties = {
-            k: v for k, v in input_props.items() if v is not None
-        }
-        return resource_path.format(**filtered_without_none_properties)
-    except:
-        # a required input prop is missing or input_props is invalid format
+        try:
+            if (
+                hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
+                    name, resource_type, log_warnings=False
+                )
+                is not None
+            ):
+                return name
+        except ValueError:
+            ...
+
+    filtered_without_none_properties = (
+        {k: v for k, v in input_props.items() if v is not None}
+        if input_props is not None
+        else {}
+    )
+    resource_paths: List[str] = hub.tool.gcp.resource_prop_utils.get_resource_paths(
+        resource_type
+    )
+    result = None
+    for path in resource_paths:
+        try:
+            r = path.format(**filtered_without_none_properties)
+            if r.find("{") != -1 or r.find("}") != -1:
+                # not fully matched
+                r = None
+        except KeyError:
+            r = None
+        if r:
+            if result:
+                msg = f"Could not construct resource ID because multiple resource paths of {resource_type} match the input arguments."
+                hub.log.error(msg)
+                return None
+            result = r
+
+    if not result:
+        msg = f"Could not construct resource ID because no resource paths of {resource_type} match the input arguments."
+        hub.log.warning(msg)
         return None
 
+    return result
+
 
 def parse_link_to_zone(hub, link: str) -> str:
     return link.split("/")[-1]
 
 
-def get_path_parameters(hub, resource_type):
-    resource_path = hub.tool.gcp.resource_prop_utils.get_resource_path(resource_type)
+def get_path_parameters_for_path(hub, resource_path: str) -> Set[str]:
     src = resource_path.split("/")
     result = set()
 
     for s in src:
         if s.startswith("{") and s.endswith("}"):
             result.add(s[1:-1])
 
     return result
 
 
+def get_path_parameters(hub, resource_type: str, resource: str) -> Set[str]:
+    resource_paths = hub.tool.gcp.resource_prop_utils.get_resource_paths(resource_type)
+    all_parameters = []
+    for path in resource_paths:
+        r = hub.tool.gcp.resource_prop_utils.get_path_parameters_for_path(path)
+        if r:
+            all_parameters.append(r)
+
+    # Try to find best-matching path
+    result = None
+    for parameters in all_parameters:
+        missing = {p for p in parameters if p not in resource}
+        if not missing:
+            if result:
+                msg = f"Resource {resource} matches multiple resource paths of {resource_type}"
+                hub.log.error(msg)
+                return set()
+
+            result = parameters
+
+    if not result:
+        msg = f"Resource {resource} matches no resource paths of {resource_type}"
+        hub.log.warning(msg)
+        return set()
+
+    return result
+
+
+def get_path_parameters_combined(hub, resource_type: str, resource: str) -> Set[str]:
+    resource_paths = hub.tool.gcp.resource_prop_utils.get_resource_paths(resource_type)
+    all_parameters = []
+    for path in resource_paths:
+        r = hub.tool.gcp.resource_prop_utils.get_path_parameters_for_path(path)
+        if r:
+            all_parameters.append(r)
+
+    result = set()
+    for parameters in all_parameters:
+        result = result.union(parameters)
+
+    return result
+
+
 def format_path_params(hub, resource, resource_type):
-    resource_copy = copy.deepcopy(resource)
-    path_params = hub.tool.gcp.resource_prop_utils.get_path_parameters(resource_type)
+    path_params = hub.tool.gcp.resource_prop_utils.get_path_parameters_combined(
+        resource_type, resource
+    )
     for path_el in path_params:
-        if resource_copy.get(path_el):
-            resource_copy[path_el] = resource_copy[path_el].split("/")[-1]
-
-    return resource_copy
+        if resource.get(path_el):
+            resource[path_el] = resource[path_el].split("/")[-1]
 
 
 # TODO: Remove this logic once we have all the nested properties defined for a method
 def are_properties_allowed_for_update(hub, resource_type, request_body):
     can_update = True
     if resource_type == "compute.instance":
         for disk in request_body.get("disks" or {}):
             if disk.get("initialize_params"):
                 can_update = False
 
     return can_update
 
 
 def resource_type_matches(hub, resource_id: str, resource_type: str) -> bool:
-    resource_path = hub.tool.gcp.resource_prop_utils.get_resource_path(resource_type)
+    resource_paths = hub.tool.gcp.resource_prop_utils.get_resource_paths(resource_type)
+    result = False
+    for path in resource_paths:
+        r = hub.tool.gcp.resource_prop_utils.resource_type_matches_for_path(
+            resource_id, path
+        )
+        if r:
+            if result:
+                msg = f"Resource ID {resource_id} matches multiple resource paths of {resource_type}"
+                hub.log.error(msg)
+                return False
+            result = True
+
+    return result
+
+
+def resource_type_matches_for_path(hub, resource_id: str, resource_path: str) -> bool:
     rpath = resource_path.split("/")
     rid = resource_id.split("/")
 
     if len(rid) < len(rpath):
         return False
 
     idx = -1
     for s in reversed(rpath):
         if not (s.startswith("{") and s.endswith("}")) and rid[idx] != s:
             return False
         idx -= 1
 
     return True
+
+
+def get_manual_mappings(hub, resource_type: str) -> Dict[str, str]:
+    resource_methods_properties = hub.tool.gcp.RESOURCE_PROPS[resource_type]
+    manual_mappings = resource_methods_properties.get("manual_mapping", {})
+    return manual_mappings
+
+
+def get_missing_property_assumed_values(hub, resource_type: str) -> Dict[str, Any]:
+    resource_properties = hub.tool.gcp.RESOURCE_PROPS.get(resource_type, {})
+    return resource_properties.get("missing_property_assumed_value", {})
+
+
+def populate_resource_with_assumed_values(
+    hub, resource, resource_type, convert_to_present: bool = False
+):
+    assumed_values = (
+        hub.tool.gcp.resource_prop_utils.get_missing_property_assumed_values(
+            resource_type
+        )
+    )
+
+    if convert_to_present:
+        assumed_values = hub.tool.gcp.conversion_utils.convert_raw_resource_to_present(
+            assumed_values, resource_type
+        )
+
+    for missing_key, assumed_value in assumed_values.items():
+        if missing_key not in resource:
+            resource[missing_key] = assumed_value
+
+
+def get_readonly_return_props(
+    hub, resource_type: str, convert_to_present: bool = True
+) -> Set[str]:
+    resource_properties = hub.tool.gcp.RESOURCE_PROPS.get(resource_type, {})
+
+    raw_props = set(resource_properties.get("readonly_return_props", {}))
+
+    if raw_props and convert_to_present:
+        return hub.tool.gcp.conversion_utils.convert_raw_properties_to_present(
+            raw_props
+        )
+
+    return raw_props
+
+
+def properties_mismatch_resource_id(
+    hub, service_resource_type, resource_id, state_properties
+) -> bool:
+    constructed_resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
+        service_resource_type, state_properties
+    )
+    # This check is needed if properties or resource_id are not supplied
+    if not constructed_resource_id or not resource_id:
+        return False
+    if resource_id != constructed_resource_id:
+        return True
+    return False
+
+
+# TODO: Figure out a generic way to get the native resource path
+def get_service_resource_type(hub, state_resource_path: str) -> str:
+    service_resource_path = state_resource_path.replace("gcp.", "")
+    if "cloudkms" not in service_resource_path:
+        return service_resource_path
+
+    cloudkms_native_resource_paths_dict = {
+        "cloudkms.location": "cloudkms.projects.locations",
+        "cloudkms.key_ring": "cloudkms.projects.locations.key_rings",
+        "cloudkms.import_job": "cloudkms.projects.locations.key_rings.import_jobs",
+        "cloudkms.crypto_key": "cloudkms.projects.locations.key_rings.crypto_keys",
+        "cloudkms.crypto_key_version": "cloudkms.projects.locations.key_rings.crypto_keys.crypto_key_versions",
+    }
+
+    return cloudkms_native_resource_paths_dict[service_resource_path]
+
+
+def get_relevant_dict_items_removed(
+    hub, resource_type: str, convert_to_present: bool = True
+) -> List[str]:
+    resource_methods_properties = hub.tool.gcp.RESOURCE_PROPS.get(resource_type, {})
+    raw_props = set(resource_methods_properties.get("relevant_dict_items_removed", {}))
+    if raw_props and convert_to_present:
+        return hub.tool.gcp.conversion_utils.convert_raw_properties_to_present(
+            raw_props
+        )
+
+    return raw_props
```

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/session.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/session.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.9.0/idem_gcp/tool/gcp/state_comparison_utils.py` & `idem_gcp-1.1.0/idem_gcp/tool/gcp/state_comparison_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.9.0/idem_gcp.egg-info/PKG-INFO` & `idem_gcp-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
-Name: idem-gcp
-Version: 0.9.0
+Name: idem_gcp
+Version: 1.1.0
 Summary: GCP Cloud Provider for Idem
 Home-page: https://gitlab.com/vmware/idem/idem-gcp
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/idem-gcp
-Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-gcp/issues
+Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-gcp/-/issues
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: full
 Provides-Extra: autogen
 License-File: LICENSE
 
 ========
 idem-gcp
@@ -37,15 +37,15 @@
 
 .. image:: https://img.shields.io/badge/made%20with-idem-teal
    :alt: Made with idem, a Python implementation of Plugin Oriented Programming
    :target: https://www.idemproject.io/
 
 .. image:: https://img.shields.io/badge/docs%20on-docs.idemproject.io-blue
    :alt: Documentation is published with Sphinx on docs.idemproject.io
-   :target: https://docs.idemproject.io/idem-aws/en/latest/index.html
+   :target: https://docs.idemproject.io/idem-gcp/en/latest/index.html
 
 .. image:: https://img.shields.io/badge/made%20with-python-yellow
    :alt: Made with Python
    :target: https://www.python.org/
 
 GCP Cloud Provider for Idem.
 
@@ -82,22 +82,47 @@
 
 * `Idem Project Website <https://www.idemproject.io/>`__
 * `Idem Project docs portal <https://docs.idemproject.io/>`__
 
 Getting Started
 ===============
 
-DEVELOPMENT
-===========
+Prerequisites
+-------------
+
+* Python 3.8+
+* git *(if installing from source, or contributing to the project)*
+
+Installation
+------------
+
+.. note::
+
+   If wanting to contribute to the project, and setup your local development
+   environment, see the ``CONTRIBUTING.rst`` document in the source repository
+   for this project.
+
+If wanting to use ``idem-gcp``, you can do so by either
+installing from PyPI or from source.
+
+Install from PyPI
++++++++++++++++++
+
+.. code-block:: bash
+
+  pip install idem-gcp
+
+Install from source
++++++++++++++++++++
 
-Clone the `idem_gcp` repository and install with pip.
+Clone the `idem_gcp` repository.
 
 .. code:: bash
 
-    git clone git@gitlab.com:my-user/idem_gcp.git
+    git clone git@gitlab.com:vmware/idem/idem-gcp.git
     cd idem_gcp
 
 Create a virtual environment, and then activate it:
 
 .. code:: bash
 
     python3 -m venv venv
@@ -113,80 +138,104 @@
 
 Install the following packages in order to run the tests:
 
 .. code:: bash
 
     pip3 install -r requirements/py3.10/tests.txt
 
-**NOTE:**  Change py3.10 if needed with your  Python version. There is support for py3.7, py3.8, py3.9 and py3.10.
+**NOTE:**  Change py3.10 if needed with your  Python version. There is support for py3.8, py3.9, py3.10 and py3.11.
 
-ACCT
-====
+Setup
+=====
 
-After installation gcp Idem Provider execution and state modules will be accessible to the pop `hub`.
+After installation GCP Idem Provider execution and state modules will be accessible to the pop `hub`.
 In order to use them we need to set up our credentials.
 
-Create a new file called `credentials.yaml` and populate it with profiles.
-The `default` profile will be used automatically by `idem` unless you specify one with `--acct-profile=profile_name` on the cli.
-
-`acct backends <https://gitlab.com/saltstack/pop/acct-backends>`_ provide alternate methods for storing profiles.
+Create a new file called `credentials.yaml` and populate it with your credential profiles.
 
-The gcp provider uses the gcp acct plugin for authentication.
-A profile needs to specify the authentication parameters for gcp.
+To provide your GCP credentials in the file, use the "gcp" provider key.
+Under that key, add different profiles as needed.
+A profile specifies authentication parameters for GCP.
+The `default` profile will be automatically used by `idem`,
+but the other ones could be explicitly specified for each run or SLS file.
+This is done through the `--acct-profile` `idem` cli flag or the
+`acct_profile` SLS property.
+
+There is currently one GCP authentication mechanism supported by idem-gcp -
+providing service account keys.
+The following example gives the overall structure of the authentication
+parameters' expected format.
 
 credentials.yaml
 
 ..  code:: sls
 
     gcp:
       default:
-        username: my_user
-        password: my_good_password
-        endpoint_url: https://console.gcp.com/api
+        type: service_account
+        project_id: “<project>”
+        private_key_id: “<key_id>”
+        private_key: |
+          -----BEGIN PRIVATE KEY-----
+          <private_key>
+          ——END PRIVATE KEY-----
+        client_email: “<service_account_email>“
+        client_id: “<client_id>”
+        auth_uri: https://accounts.google.com/o/oauth2/auth
+        token_uri: https://oauth2.googleapis.com/token
+        auth_provider_x509_cert_url: https://www.googleapis.com/oauth2/v1/certs
+        client_x509_cert_url: “<certificate_url>“
+        universe_domain: googleapis.com
+      <other_profile_name>:
+        ...
+
+The values of these parameters can be obtained through the GCP console after creating a service account and generating a service account key in JSON format.
+Be sure to assign appropriate roles for the service account, such that it has the rights to access and manage the needed resources.
+For a better security posture, follow the principal of least privilege and do not use service accounts with excessive rights.
+For more information on the authentication parameters used, refer to the `Credentials <https://google-auth.readthedocs.io/en/master/reference/google.oauth2.service_account.html#google.oauth2.service_account.Credentials>`_ docs.
 
-Now encrypt the credentials file and add the encryption key and encrypted file path to the ENVIRONMENT.
+Encrypt the created credentials file:
 
-The `acct` command should be available as it is a requisite of `idem` and `idem_gcp`.
-Encrypt the the credential file.
 
 .. code:: bash
 
     acct encrypt credentials.yaml
 
-output::
 
-    -A9ZkiCSOjWYG_lbGmmkVh4jKLFDyOFH4e4S1HNtNwI=
+The output of this command is the ACCT_KEY which needs to be securely stored.
+A `credentials.yaml.fernet` encrypted file is also created in the working directory, whose path should be used as ACCT_FILE.
+These could be given to idem either through environment variables or directly as `idem` run parameters.
 
-Add these to your environment:
+Setting environment variables
+-----------------------------
 
 .. code:: bash
 
-    export ACCT_KEY="-A9ZkiCSOjWYG_lbGmmkVh4jKLFDyOFH4e4S1HNtNwI="
+    export ACCT_KEY="<ACCT_KEY>"
     export ACCT_FILE=$PWD/credentials.yaml.fernet
 
+Providing acct parameters to the idem run
+-----------------------------------------
 
-USAGE
-=====
-A profile can be specified for use with a specific state.
-If no profile is specified, the profile called "default", if one exists, will be used:
+.. code:: bash
 
-.. code:: sls
+    idem <subcommand> --acct-key "<ACCT_KEY>" --acct-file "$PWD/credentials.yaml.fernet" --acct-profile "<profile_name>"
 
-    ensure_user_exists:
-      gcp.user.present:
-        - acct_profile: my-staging-env
-        - name: a_user_name
-        - kwarg1: val1
+Specifying account profile in SLS files
+---------------------------------------
 
-It can also be specified from the command line when executing states.
-
-.. code:: bash
+.. code:: sls
 
-    idem state --acct-profile my-staging-env my_state.sls
+    ensure_resource:
+      gcp.<service>.<resource>.present:
+        - acct_profile: <profile_name>
+        - name: resource_name
+        - kwarg1: val1
 
-It can also be specified from the command line when calling an exec module directly.
 
-.. code:: bash
+For more information on the Idem ACCT authentication management subsystem, refer to the following resources:
 
-    idem exec --acct-profile my-staging-env gcp.user.list
+* `Account credentials file doc <https://docs.idemproject.io/idem/en/latest/topics/tutorials/acct_file.html>`_
+* `Multiple Account Management <https://docs.idemproject.io/idem/en/latest/topics/tutorials/acct.html>`_
+* `ACCT advanced features <https://docs.idemproject.io/idem/en/latest/topics/sls_acct.html>`_
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `idem_gcp-0.9.0/idem_gcp.egg-info/SOURCES.txt` & `idem_gcp-1.1.0/idem_gcp.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -7,110 +7,141 @@
 idem_gcp/version.py
 idem_gcp.egg-info/PKG-INFO
 idem_gcp.egg-info/SOURCES.txt
 idem_gcp.egg-info/dependency_links.txt
 idem_gcp.egg-info/entry_points.txt
 idem_gcp.egg-info/requires.txt
 idem_gcp.egg-info/top_level.txt
-idem_gcp/acct/gcp/basic_auth.py
-idem_gcp/acct/gcp/default_auth.py
-idem_gcp/acct/gcp/init.py
 idem_gcp/acct/gcp/service_account.py
 idem_gcp/acct/gcp/contracts/init.py
 idem_gcp/autogen/init.py
 idem_gcp/autogen/gcp/schema_parser.py
-idem_gcp/exec/gcp/sample.py
-idem_gcp/exec/gcp/None/init.py
-idem_gcp/exec/gcp/None/recursive_contracts/init.py
 idem_gcp/exec/gcp/cloudkms/crypto_key.py
 idem_gcp/exec/gcp/cloudkms/crypto_key_version.py
 idem_gcp/exec/gcp/cloudkms/import_job.py
 idem_gcp/exec/gcp/cloudkms/key_ring.py
 idem_gcp/exec/gcp/cloudkms/location.py
 idem_gcp/exec/gcp/compute/accelerator_type.py
+idem_gcp/exec/gcp/compute/backend_service.py
 idem_gcp/exec/gcp/compute/disk.py
 idem_gcp/exec/gcp/compute/disk_type.py
 idem_gcp/exec/gcp/compute/firewall.py
+idem_gcp/exec/gcp/compute/forwarding_rule.py
+idem_gcp/exec/gcp/compute/health_check.py
 idem_gcp/exec/gcp/compute/image.py
 idem_gcp/exec/gcp/compute/instance.py
+idem_gcp/exec/gcp/compute/instance_group.py
 idem_gcp/exec/gcp/compute/machine_image.py
 idem_gcp/exec/gcp/compute/machine_type.py
 idem_gcp/exec/gcp/compute/network.py
 idem_gcp/exec/gcp/compute/node_template.py
 idem_gcp/exec/gcp/compute/reservation.py
 idem_gcp/exec/gcp/compute/resource_policy.py
 idem_gcp/exec/gcp/compute/snapshot.py
 idem_gcp/exec/gcp/compute/subnetwork.py
+idem_gcp/exec/gcp/compute/target_pool.py
 idem_gcp/exec/gcp/compute/zone.py
 idem_gcp/exec/gcp/contracts/init.py
-idem_gcp/exec/gcp/storage/buckets.py
+idem_gcp/exec/gcp/iam/projects/service_account.py
+idem_gcp/exec/gcp/iam/projects/service_accounts/key.py
+idem_gcp/exec/gcp/storage/bucket.py
 idem_gcp/exec/gcp_api/init.py
 idem_gcp/helpers/exc.py
 idem_gcp/helpers/log.py
 idem_gcp/helpers/returns.py
 idem_gcp/metadata/gcp/cloudkms/projects/locations/init.py
 idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/init.py
 idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/crypto_key_versions.py
 idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/init.py
 idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/import_jobs/init.py
 idem_gcp/metadata/gcp/compute/accelerator_type.py
+idem_gcp/metadata/gcp/compute/backend_service.py
 idem_gcp/metadata/gcp/compute/disk.py
 idem_gcp/metadata/gcp/compute/disk_type.py
 idem_gcp/metadata/gcp/compute/firewall.py
+idem_gcp/metadata/gcp/compute/forwarding_rule.py
 idem_gcp/metadata/gcp/compute/global_operation.py
+idem_gcp/metadata/gcp/compute/health_check.py
 idem_gcp/metadata/gcp/compute/image.py
 idem_gcp/metadata/gcp/compute/instance.py
+idem_gcp/metadata/gcp/compute/instance_group.py
 idem_gcp/metadata/gcp/compute/machine_image.py
 idem_gcp/metadata/gcp/compute/machine_type.py
 idem_gcp/metadata/gcp/compute/network.py
 idem_gcp/metadata/gcp/compute/node_template.py
+idem_gcp/metadata/gcp/compute/region_backend_service.py
 idem_gcp/metadata/gcp/compute/region_operation.py
 idem_gcp/metadata/gcp/compute/reservation.py
 idem_gcp/metadata/gcp/compute/resource_policy.py
 idem_gcp/metadata/gcp/compute/snapshot.py
 idem_gcp/metadata/gcp/compute/subnetwork.py
+idem_gcp/metadata/gcp/compute/target_pool.py
 idem_gcp/metadata/gcp/compute/zone.py
 idem_gcp/metadata/gcp/compute/zone_operation.py
-idem_gcp/metadata/gcp/storage/buckets.py
+idem_gcp/metadata/gcp/iam/projects/service_account.py
+idem_gcp/metadata/gcp/iam/projects/service_accounts/key.py
+idem_gcp/metadata/gcp/storage/bucket.py
 idem_gcp/metadata/gcp/storage/objectAccessControls.py
 idem_gcp/resources/properties.yaml
 idem_gcp/states/gcp/init.py
 idem_gcp/states/gcp/cloudkms/crypto_key.py
 idem_gcp/states/gcp/cloudkms/crypto_key_version.py
 idem_gcp/states/gcp/cloudkms/import_job.py
 idem_gcp/states/gcp/cloudkms/key_ring.py
 idem_gcp/states/gcp/cloudkms/location.py
+idem_gcp/states/gcp/compute/backend_service.py
 idem_gcp/states/gcp/compute/disk.py
+idem_gcp/states/gcp/compute/firewall.py
+idem_gcp/states/gcp/compute/forwarding_rule.py
+idem_gcp/states/gcp/compute/health_check.py
 idem_gcp/states/gcp/compute/image.py
 idem_gcp/states/gcp/compute/instance.py
+idem_gcp/states/gcp/compute/instance_group.py
 idem_gcp/states/gcp/compute/machine_image.py
 idem_gcp/states/gcp/compute/network.py
 idem_gcp/states/gcp/compute/node_template.py
 idem_gcp/states/gcp/compute/reservation.py
 idem_gcp/states/gcp/compute/resource_policy.py
 idem_gcp/states/gcp/compute/snapshot.py
 idem_gcp/states/gcp/compute/subnetwork.py
-idem_gcp/states/gcp/storage/buckets.py
+idem_gcp/states/gcp/compute/target_pool.py
+idem_gcp/states/gcp/iam/projects/service_account.py
+idem_gcp/states/gcp/iam/projects/service_accounts/key.py
+idem_gcp/states/gcp/recursive_contracts/init.py
+idem_gcp/states/gcp/storage/bucket.py
 idem_gcp/tool/gcp/case.py
 idem_gcp/tool/gcp/comment_utils.py
 idem_gcp/tool/gcp/conversion_utils.py
+idem_gcp/tool/gcp/hub_resolver.py
 idem_gcp/tool/gcp/init.py
 idem_gcp/tool/gcp/operation_utils.py
 idem_gcp/tool/gcp/policy.py
 idem_gcp/tool/gcp/resolver.py
 idem_gcp/tool/gcp/resource_prop_utils.py
+idem_gcp/tool/gcp/sanitizers.py
 idem_gcp/tool/gcp/session.py
 idem_gcp/tool/gcp/state_comparison_utils.py
+idem_gcp/tool/gcp/state_operation_utils.py
 idem_gcp/tool/gcp/utils.py
 idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py
 idem_gcp/tool/gcp/cloudkms/patch.py
+idem_gcp/tool/gcp/compute/disk.py
 idem_gcp/tool/gcp/compute/instance.py
+idem_gcp/tool/gcp/compute/instance_group.py
 idem_gcp/tool/gcp/compute/network.py
+idem_gcp/tool/gcp/compute/subnetwork.py
 idem_gcp/tool/gcp/generate/exec_context.py
 idem_gcp/tool/gcp/generate/exec_param.py
 idem_gcp/tool/gcp/generate/generic_exec.py
 idem_gcp/tool/gcp/generate/scope.py
 idem_gcp/tool/gcp/generate/operators/post_exec/item_getter.py
 idem_gcp/tool/gcp/generate/operators/post_exec/operation_processor.py
 idem_gcp/tool/gcp/generate/operators/pre_exec/function_getter.py
+idem_gcp/tool/gcp/generate/operators/pre_exec/parameter_sanitizer.py
 idem_gcp/tool/gcp/generate/operators/pre_exec/resource_id_extractor.py
-idem_gcp/tool/gcp/generate/operators/recursive_contracts/init.py
+idem_gcp/tool/gcp/generate/operators/recursive_contracts/init.py
+idem_gcp/tool/gcp/schema/finding.py
+idem_gcp/tool/gcp/schema/results_collector.py
+idem_gcp/tool/gcp/schema/schema_compatibility_checker.py
+idem_gcp/tool/gcp/schema/schema_naming_checker.py
+idem_gcp/tool/gcp/schema/scm_utils.py
+idem_gcp/tool/gcp/storage/bucket.py
```

### Comparing `idem_gcp-0.9.0/setup.py` & `idem_gcp-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,35 +71,35 @@
     author="VMware, Inc.",
     author_email="idemproject@vmware.com",
     # This URL should be updated once docs are publishing,
     # Should point to the published Sphinx site
     url="https://gitlab.com/vmware/idem/idem-gcp",
     project_urls={
         "Code": "https://gitlab.com/vmware/idem/idem-gcp",
-        "Issue tracker": "https://gitlab.com/vmware/idem/idem-gcp/issues",
+        "Issue tracker": "https://gitlab.com/vmware/idem/idem-gcp/-/issues",
     },
     version=VERSION,
     install_requires=REQUIREMENTS,
     extras_require=REQUIREMENTS_EXTRA,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     license="Apache Software License 2.0",
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
     ],
     packages=discover_packages(),
     entry_points={"console_scripts": [""]},
     cmdclass={"clean": Clean},
     include_package_data=True,
```

