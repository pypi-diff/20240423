# Comparing `tmp/bce-python-sdk-0.9.6.tar.gz` & `tmp/bce_python_sdk-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bce-python-sdk-0.9.6.tar", last modified: Wed Mar 27 06:57:14 2024, max compression
+gzip compressed data, was "bce_python_sdk-0.9.7.tar", last modified: Tue Apr 23 12:37:08 2024, max compression
```

## Comparing `bce-python-sdk-0.9.6.tar` & `bce_python_sdk-0.9.7.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.361836 bce-python-sdk-0.9.6/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      314 2024-03-27 06:57:14.361644 bce-python-sdk-0.9.6/PKG-INFO
--rw-r--r--   0 liuzhongshan   (501) staff       (20)       40 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/README.txt
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.341234 bce-python-sdk-0.9.6/baidubce/
--rwxr-xr-x   0 liuzhongshan   (501) staff       (20)      813 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/__init__.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.341578 bce-python-sdk-0.9.6/baidubce/auth/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/auth/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1157 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/auth/bce_credentials.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3211 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/auth/bce_v1_signer.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3428 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/bce_base_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3055 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/bce_client_configuration.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1655 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/bce_response.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3467 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/compat.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1691 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/exception.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.342235 bce-python-sdk-0.9.6/baidubce/http/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/http/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     9877 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/http/bce_http_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     2930 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/http/handler.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      722 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/http/http_content_types.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     2659 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/http/http_headers.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      782 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/http/http_methods.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1151 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/protocol.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      835 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/region.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.342431 bce-python-sdk-0.9.6/baidubce/retry/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/retry/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     4926 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/retry/retry_policy.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.342592 bce-python-sdk-0.9.6/baidubce/services/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/__init__.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.343014 bce-python-sdk-0.9.6/baidubce/services/autoscaling/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/autoscaling/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    22179 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/autoscaling/as_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3332 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/autoscaling/as_handler.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     8501 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/autoscaling/as_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.343361 bce-python-sdk-0.9.6/baidubce/services/bbc/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bbc/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    35864 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bbc/bbc_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1595 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bbc/bbc_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.344055 bce-python-sdk-0.9.6/baidubce/services/bcc/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bcc/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)   233985 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bcc/bcc_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     5919 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bcc/bcc_model.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      948 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bcc/fpga_card_type.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1054 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bcc/gpu_card_type.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.344569 bce-python-sdk-0.9.6/baidubce/services/bcm/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bcm/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)   209237 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bcm/bcm_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3315 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bcm/bcm_handler.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    22095 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bcm/bcm_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.344914 bce-python-sdk-0.9.6/baidubce/services/bes/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bes/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    22810 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bes/bes_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1784 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bes/bes_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.345435 bce-python-sdk-0.9.6/baidubce/services/blb/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/blb/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)   128513 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/blb/app_blb_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    98620 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/blb/blb_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    17046 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/blb/user_service_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.345650 bce-python-sdk-0.9.6/baidubce/services/bmr/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bmr/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    20565 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bmr/bmr_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.346225 bce-python-sdk-0.9.6/baidubce/services/bos/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      813 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bos/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)   100010 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bos/bos_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1832 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bos/bos_handler.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      723 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bos/canned_acl.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      729 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bos/storage_class.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.346666 bce-python-sdk-0.9.6/baidubce/services/bts/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      749 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bts/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    21916 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bts/bts_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    11520 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bts/model.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1521 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/bts/util.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.346985 bce-python-sdk-0.9.6/baidubce/services/cdn/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/cdn/__init__.py
--rwxr-xr-x   0 liuzhongshan   (501) staff       (20)    59017 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/cdn/cdn_client.py
--rwxr-xr-x   0 liuzhongshan   (501) staff       (20)     1252 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/cdn/cdn_stats_param.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.347329 bce-python-sdk-0.9.6/baidubce/services/cert/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/cert/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     4659 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/cert/cert_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1622 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/cert/cert_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.347729 bce-python-sdk-0.9.6/baidubce/services/cfc/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/cfc/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    42843 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/cfc/cfc_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3037 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/cfc/cfc_handler.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     5722 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/cfc/models.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.348234 bce-python-sdk-0.9.6/baidubce/services/csn/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/csn/__init__.py
--rwxr-xr-x   0 liuzhongshan   (501) staff       (20)     7609 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/csn/csn_api.py
--rwxr-xr-x   0 liuzhongshan   (501) staff       (20)    35434 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/csn/csn_client.py
--rwxr-xr-x   0 liuzhongshan   (501) staff       (20)     1308 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/csn/csn_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.348443 bce-python-sdk-0.9.6/baidubce/services/ddc/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/ddc/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     6834 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/ddc/ddc_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.348693 bce-python-sdk-0.9.6/baidubce/services/dns/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/dns/__init__.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.348914 bce-python-sdk-0.9.6/baidubce/services/dns/api/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/dns/api/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     4350 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/dns/api/dns_api.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    15953 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/dns/dns_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.349163 bce-python-sdk-0.9.6/baidubce/services/dumap/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/dumap/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3955 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/dumap/dumap_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.350012 bce-python-sdk-0.9.6/baidubce/services/eip/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/eip/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    13055 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/eip/eip_bp_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    23965 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/eip/eip_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    18955 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/eip/eip_group_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1914 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/eip/eip_group_model.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     8798 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/eip/eip_tp_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1769 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/eip/model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.350393 bce-python-sdk-0.9.6/baidubce/services/endpoint/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/endpoint/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    12789 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/endpoint/endpoint_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1650 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/endpoint/model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.350739 bce-python-sdk-0.9.6/baidubce/services/eni/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/eni/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    27213 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/eni/eni_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1165 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/eni/eni_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.351079 bce-python-sdk-0.9.6/baidubce/services/et/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/et/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    31622 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/et/et_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      975 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/et/model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.351199 bce-python-sdk-0.9.6/baidubce/services/havip/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    13846 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/havip/havip_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.351458 bce-python-sdk-0.9.6/baidubce/services/iam/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      668 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/iam/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    24555 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/iam/iam_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.351832 bce-python-sdk-0.9.6/baidubce/services/infinite/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      655 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/infinite/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     8898 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/infinite/infinite_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.352287 bce-python-sdk-0.9.6/baidubce/services/ipv6gateway/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/ipv6gateway/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    19194 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/ipv6gateway/ipv6gateway_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1698 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/ipv6gateway/ipv6gateway_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.353088 bce-python-sdk-0.9.6/baidubce/services/kms/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/kms/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      794 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/kms/keyspec_class.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    17789 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/kms/kms_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      640 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/kms/origin_class.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      633 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/kms/protectedby_class.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      655 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/kms/publickeyencoding_class.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.353437 bce-python-sdk-0.9.6/baidubce/services/lbdc/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/lbdc/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    10679 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/lbdc/lbdc_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1625 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/lbdc/model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.353630 bce-python-sdk-0.9.6/baidubce/services/localdns/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/localdns/__init__.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.353839 bce-python-sdk-0.9.6/baidubce/services/localdns/api/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/localdns/api/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3294 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/localdns/api/ld_api.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    10461 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/localdns/ld_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.354172 bce-python-sdk-0.9.6/baidubce/services/media/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/media/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    25881 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/media/media_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     2460 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/media/media_handler.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.354407 bce-python-sdk-0.9.6/baidubce/services/mms/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      610 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/mms/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    19332 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/mms/mms_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.354675 bce-python-sdk-0.9.6/baidubce/services/mvs/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      610 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/mvs/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     5802 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/mvs/mvs_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.355107 bce-python-sdk-0.9.6/baidubce/services/oos/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/oos/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    10214 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/oos/oos_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     2869 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/oos/oos_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.357002 bce-python-sdk-0.9.6/baidubce/services/rds/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      707 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/rds/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    13869 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/rds/rds_backup_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     5695 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/rds/rds_database_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    17005 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/rds/rds_hot_active_instance_group_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     8479 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/rds/rds_http.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    33785 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/rds/rds_instance_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     9197 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/rds/rds_log_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    17318 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/rds/rds_parameter_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    17078 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/rds/rds_readonly_group_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     4115 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/rds/rds_recycler_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     5190 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/rds/rds_security_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3455 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/rds/rds_task_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    10387 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/rds/rds_users_manager.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.357396 bce-python-sdk-0.9.6/baidubce/services/route/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/route/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    13869 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/route/route_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      280 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/route/route_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.357764 bce-python-sdk-0.9.6/baidubce/services/scs/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      707 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/scs/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     8355 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/scs/model.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    27357 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/scs/scs_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.358170 bce-python-sdk-0.9.6/baidubce/services/sms/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      676 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/sms/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     6592 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/sms/model.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    31118 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/sms/sms_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.358386 bce-python-sdk-0.9.6/baidubce/services/sts/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      669 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/sts/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3687 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/sts/sts_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.358577 bce-python-sdk-0.9.6/baidubce/services/subnet/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/subnet/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    14627 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/subnet/subnet_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.359099 bce-python-sdk-0.9.6/baidubce/services/tsdb/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/tsdb/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     4845 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/tsdb/tsdb_admin_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     9337 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/tsdb/tsdb_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1744 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/tsdb/tsdb_handler.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.359293 bce-python-sdk-0.9.6/baidubce/services/vca/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/vca/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     5273 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/vca/vca_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.359558 bce-python-sdk-0.9.6/baidubce/services/vcr/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/vcr/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    13004 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/vcr/vcr_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.360392 bce-python-sdk-0.9.6/baidubce/services/vpc/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/vpc/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    11902 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/vpc/acl_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    36440 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/vpc/nat_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1688 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/vpc/nat_model.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    20077 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/vpc/peerconn_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1686 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/vpc/peerconn_model.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     9875 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/vpc/vpc_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.360716 bce-python-sdk-0.9.6/baidubce/services/vpn/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/vpn/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    28554 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/vpn/vpn_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3364 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/services/vpn/vpn_model.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    20194 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/baidubce/utils.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-03-27 06:57:14.361394 bce-python-sdk-0.9.6/bce_python_sdk.egg-info/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      314 2024-03-27 06:57:14.000000 bce-python-sdk-0.9.6/bce_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     6313 2024-03-27 06:57:14.000000 bce-python-sdk-0.9.6/bce_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        1 2024-03-27 06:57:14.000000 bce-python-sdk-0.9.6/bce_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 liuzhongshan   (501) staff       (20)       45 2024-03-27 06:57:14.000000 bce-python-sdk-0.9.6/bce_python_sdk.egg-info/requires.txt
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        9 2024-03-27 06:57:14.000000 bce-python-sdk-0.9.6/bce_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 liuzhongshan   (501) staff       (20)       38 2024-03-27 06:57:14.361876 bce-python-sdk-0.9.6/setup.cfg
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3255 2024-03-25 11:18:24.000000 bce-python-sdk-0.9.6/setup.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.709573 bce_python_sdk-0.9.7/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      314 2024-04-23 12:37:08.709384 bce_python_sdk-0.9.7/PKG-INFO
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)       40 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/README.txt
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.684641 bce_python_sdk-0.9.7/baidubce/
+-rwxr-xr-x   0 liuzhongshan   (501) staff       (20)      813 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/__init__.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.685120 bce_python_sdk-0.9.7/baidubce/auth/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/auth/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1157 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/auth/bce_credentials.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3211 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/auth/bce_v1_signer.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3428 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/bce_base_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3055 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/bce_client_configuration.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1655 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/bce_response.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3467 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/compat.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1691 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/exception.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.685909 bce_python_sdk-0.9.7/baidubce/http/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/http/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     9877 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/http/bce_http_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     2930 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/http/handler.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      722 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/http/http_content_types.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     2659 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/http/http_headers.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      782 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/http/http_methods.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1151 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/protocol.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      835 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/region.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.686144 bce_python_sdk-0.9.7/baidubce/retry/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/retry/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     4926 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/retry/retry_policy.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.686308 bce_python_sdk-0.9.7/baidubce/services/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/__init__.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.686800 bce_python_sdk-0.9.7/baidubce/services/autoscaling/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/autoscaling/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    22179 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/autoscaling/as_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3332 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/autoscaling/as_handler.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     8501 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/autoscaling/as_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.687231 bce_python_sdk-0.9.7/baidubce/services/bbc/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bbc/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    37306 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bbc/bbc_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1790 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bbc/bbc_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.688029 bce_python_sdk-0.9.7/baidubce/services/bcc/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcc/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)   237248 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcc/bcc_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     5919 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcc/bcc_model.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      948 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcc/fpga_card_type.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1054 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcc/gpu_card_type.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.690736 bce_python_sdk-0.9.7/baidubce/services/bcm/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcm/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)   209237 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcm/bcm_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3315 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcm/bcm_handler.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    22095 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcm/bcm_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.692081 bce_python_sdk-0.9.7/baidubce/services/bes/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bes/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    22810 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bes/bes_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1784 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bes/bes_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.692730 bce_python_sdk-0.9.7/baidubce/services/blb/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/blb/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)   128513 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/blb/app_blb_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    98620 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/blb/blb_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    17046 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/blb/user_service_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.692938 bce_python_sdk-0.9.7/baidubce/services/bmr/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bmr/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    20565 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bmr/bmr_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.693522 bce_python_sdk-0.9.7/baidubce/services/bos/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      813 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bos/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)   100010 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bos/bos_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1832 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bos/bos_handler.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      723 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bos/canned_acl.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      729 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bos/storage_class.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.693989 bce_python_sdk-0.9.7/baidubce/services/bts/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      749 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bts/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    21916 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bts/bts_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    11520 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bts/model.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1521 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bts/util.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.694315 bce_python_sdk-0.9.7/baidubce/services/cdn/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cdn/__init__.py
+-rwxr-xr-x   0 liuzhongshan   (501) staff       (20)    59017 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cdn/cdn_client.py
+-rwxr-xr-x   0 liuzhongshan   (501) staff       (20)     1252 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cdn/cdn_stats_param.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.694658 bce_python_sdk-0.9.7/baidubce/services/cert/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cert/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     4659 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cert/cert_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1622 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cert/cert_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.695088 bce_python_sdk-0.9.7/baidubce/services/cfc/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cfc/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    42843 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cfc/cfc_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3037 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cfc/cfc_handler.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     5722 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cfc/models.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.695564 bce_python_sdk-0.9.7/baidubce/services/csn/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/csn/__init__.py
+-rwxr-xr-x   0 liuzhongshan   (501) staff       (20)     7609 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/csn/csn_api.py
+-rwxr-xr-x   0 liuzhongshan   (501) staff       (20)    35434 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/csn/csn_client.py
+-rwxr-xr-x   0 liuzhongshan   (501) staff       (20)     1308 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/csn/csn_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.695754 bce_python_sdk-0.9.7/baidubce/services/ddc/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/ddc/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     6834 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/ddc/ddc_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.695980 bce_python_sdk-0.9.7/baidubce/services/dns/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/dns/__init__.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.696241 bce_python_sdk-0.9.7/baidubce/services/dns/api/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/dns/api/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     4350 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/dns/api/dns_api.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    15953 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/dns/dns_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.696469 bce_python_sdk-0.9.7/baidubce/services/dumap/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/dumap/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3955 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/dumap/dumap_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.697394 bce_python_sdk-0.9.7/baidubce/services/eip/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eip/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    13055 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eip/eip_bp_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    23965 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eip/eip_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    18955 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eip/eip_group_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1914 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eip/eip_group_model.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     8798 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eip/eip_tp_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1769 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eip/model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.697794 bce_python_sdk-0.9.7/baidubce/services/endpoint/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/endpoint/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    12789 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/endpoint/endpoint_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1650 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/endpoint/model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.698148 bce_python_sdk-0.9.7/baidubce/services/eni/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eni/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    27213 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eni/eni_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1165 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eni/eni_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.698472 bce_python_sdk-0.9.7/baidubce/services/et/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/et/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    31622 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/et/et_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      975 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/et/model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.698589 bce_python_sdk-0.9.7/baidubce/services/havip/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    13846 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/havip/havip_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.698874 bce_python_sdk-0.9.7/baidubce/services/iam/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      668 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/iam/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    24555 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/iam/iam_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.699097 bce_python_sdk-0.9.7/baidubce/services/infinite/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      655 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/infinite/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     8898 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/infinite/infinite_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.699435 bce_python_sdk-0.9.7/baidubce/services/ipv6gateway/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/ipv6gateway/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    19194 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/ipv6gateway/ipv6gateway_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1698 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/ipv6gateway/ipv6gateway_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.700065 bce_python_sdk-0.9.7/baidubce/services/kms/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/kms/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      794 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/kms/keyspec_class.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    17789 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/kms/kms_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      640 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/kms/origin_class.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      633 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/kms/protectedby_class.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      655 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/kms/publickeyencoding_class.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.700399 bce_python_sdk-0.9.7/baidubce/services/lbdc/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/lbdc/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    10679 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/lbdc/lbdc_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1625 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/lbdc/model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.700624 bce_python_sdk-0.9.7/baidubce/services/localdns/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/localdns/__init__.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.700893 bce_python_sdk-0.9.7/baidubce/services/localdns/api/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/localdns/api/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3294 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/localdns/api/ld_api.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    10461 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/localdns/ld_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.701255 bce_python_sdk-0.9.7/baidubce/services/media/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/media/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    25881 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/media/media_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     2460 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/media/media_handler.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.701494 bce_python_sdk-0.9.7/baidubce/services/mms/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      610 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/mms/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    19332 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/mms/mms_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.701757 bce_python_sdk-0.9.7/baidubce/services/mvs/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      610 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/mvs/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     5802 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/mvs/mvs_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.702182 bce_python_sdk-0.9.7/baidubce/services/oos/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/oos/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    10214 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/oos/oos_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     2869 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/oos/oos_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.704175 bce_python_sdk-0.9.7/baidubce/services/rds/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      707 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    13869 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_backup_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     5695 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_database_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    17005 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_hot_active_instance_group_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     8479 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_http.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    33785 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_instance_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     9197 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_log_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    17318 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_parameter_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    17078 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_readonly_group_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     4115 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_recycler_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     5190 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_security_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3455 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_task_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    10387 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_users_manager.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.704624 bce_python_sdk-0.9.7/baidubce/services/route/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/route/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    13869 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/route/route_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      280 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/route/route_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.705040 bce_python_sdk-0.9.7/baidubce/services/scs/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      707 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/scs/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     8355 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/scs/model.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    27357 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/scs/scs_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.705445 bce_python_sdk-0.9.7/baidubce/services/sms/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      676 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/sms/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     6592 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/sms/model.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    31118 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/sms/sms_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.705721 bce_python_sdk-0.9.7/baidubce/services/sts/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      669 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/sts/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3687 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/sts/sts_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.705957 bce_python_sdk-0.9.7/baidubce/services/subnet/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/subnet/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    14627 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/subnet/subnet_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.706538 bce_python_sdk-0.9.7/baidubce/services/tsdb/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/tsdb/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     4845 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/tsdb/tsdb_admin_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     9337 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/tsdb/tsdb_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1744 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/tsdb/tsdb_handler.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.706742 bce_python_sdk-0.9.7/baidubce/services/vca/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vca/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     5273 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vca/vca_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.707021 bce_python_sdk-0.9.7/baidubce/services/vcr/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vcr/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    13004 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vcr/vcr_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.707935 bce_python_sdk-0.9.7/baidubce/services/vpc/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpc/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    11902 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpc/acl_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    36440 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpc/nat_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1688 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpc/nat_model.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    20077 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpc/peerconn_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1686 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpc/peerconn_model.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     9875 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpc/vpc_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.708407 bce_python_sdk-0.9.7/baidubce/services/vpn/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpn/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    28554 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpn/vpn_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3364 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpn/vpn_model.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    20194 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/utils.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.709154 bce_python_sdk-0.9.7/bce_python_sdk.egg-info/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      314 2024-04-23 12:37:08.000000 bce_python_sdk-0.9.7/bce_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     6313 2024-04-23 12:37:08.000000 bce_python_sdk-0.9.7/bce_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        1 2024-04-23 12:37:08.000000 bce_python_sdk-0.9.7/bce_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)       45 2024-04-23 12:37:08.000000 bce_python_sdk-0.9.7/bce_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        9 2024-04-23 12:37:08.000000 bce_python_sdk-0.9.7/bce_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)       38 2024-04-23 12:37:08.709612 bce_python_sdk-0.9.7/setup.cfg
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3255 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/setup.py
```

### Comparing `bce-python-sdk-0.9.6/baidubce/__init__.py` & `bce_python_sdk-0.9.7/baidubce/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 This module defines some common string constants.
 """
 from builtins import str
 from builtins import bytes
 from . import protocol
 
 
-SDK_VERSION = b'0.9.06'
+SDK_VERSION = b'0.9.07'
 DEFAULT_SERVICE_DOMAIN = b'bcebos.com'
 URL_PREFIX = b'/v1'
 DEFAULT_ENCODING = 'UTF-8'
```

### Comparing `bce-python-sdk-0.9.6/baidubce/auth/bce_credentials.py` & `bce_python_sdk-0.9.7/baidubce/auth/bce_credentials.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/auth/bce_v1_signer.py` & `bce_python_sdk-0.9.7/baidubce/auth/bce_v1_signer.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/bce_base_client.py` & `bce_python_sdk-0.9.7/baidubce/bce_base_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/bce_client_configuration.py` & `bce_python_sdk-0.9.7/baidubce/bce_client_configuration.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/bce_response.py` & `bce_python_sdk-0.9.7/baidubce/bce_response.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/compat.py` & `bce_python_sdk-0.9.7/baidubce/compat.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/exception.py` & `bce_python_sdk-0.9.7/baidubce/exception.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/http/bce_http_client.py` & `bce_python_sdk-0.9.7/baidubce/http/bce_http_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/http/handler.py` & `bce_python_sdk-0.9.7/baidubce/http/handler.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/http/http_content_types.py` & `bce_python_sdk-0.9.7/baidubce/http/http_content_types.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/http/http_headers.py` & `bce_python_sdk-0.9.7/baidubce/http/http_headers.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/http/http_methods.py` & `bce_python_sdk-0.9.7/baidubce/http/http_methods.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/protocol.py` & `bce_python_sdk-0.9.7/baidubce/protocol.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/region.py` & `bce_python_sdk-0.9.7/baidubce/region.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/retry/retry_policy.py` & `bce_python_sdk-0.9.7/baidubce/retry/retry_policy.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/autoscaling/as_client.py` & `bce_python_sdk-0.9.7/baidubce/services/autoscaling/as_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/autoscaling/as_handler.py` & `bce_python_sdk-0.9.7/baidubce/services/autoscaling/as_handler.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/autoscaling/as_model.py` & `bce_python_sdk-0.9.7/baidubce/services/autoscaling/as_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bbc/bbc_client.py` & `bce_python_sdk-0.9.7/baidubce/services/bbc/bbc_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 
 class BbcClient(bce_base_client.BceBaseClient):
     """
     Bbc client sdk
     """
 
+    prefix_v2 = b'/v2'
     def __init__(self, config=None):
         bce_base_client.BceBaseClient.__init__(self, config)
 
     def _merge_config(self, config=None):
         if config is None:
             return self.config
         else:
@@ -681,14 +682,55 @@
         body = {
             'changeTags': change_tags
         }
 
         return self._send_request(http_methods.PUT, path, body=json.dumps(body),
                                   params=params, config=config)
 
+    @required(reserved_instance_ids=list,
+              tags=list)
+    def bind_reserved_instance_to_tags(self, reserved_instance_ids, tags, config=None):
+        """
+        :param reserved_instance_ids:
+        :param tags:
+        :param config:
+        :return:
+        """
+        path = b'/bbc/reserved/tag'
+        tag_list = [tag.__dict__ for tag in tags]
+        body = {
+            'changeTags': tag_list,
+            'reservedInstanceIds': reserved_instance_ids
+        }
+        params = {
+            'bind': None
+        }
+        return self._send_request(http_methods.PUT, path, json.dumps(body),
+                                  params=params, config=config, api_version=self.prefix_v2)
+
+    @required(reserved_instance_ids=list,
+              tags=list)
+    def unbind_reserved_instance_from_tags(self, reserved_instance_ids, tags, config=None):
+        """
+        :param reserved_instance_ids:
+        :param tags:
+        :param config:
+        :return:
+        """
+        path = b'/bbc/reserved/tag'
+        tag_list = [tag.__dict__ for tag in tags]
+        body = {
+            'changeTags': tag_list,
+            'reservedInstanceIds': reserved_instance_ids
+        }
+        params = {
+            'unbind': None
+        }
+        return self._send_request(http_methods.PUT, path, json.dumps(body),
+                                  params=params, config=config, api_version=self.prefix_v2)
 
     def list_flavors(self, config=None):
         """
         :return:
         :rtype baidubce.bce_response.BceResponse
 
         """
```

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bbc/bbc_model.py` & `bce_python_sdk-0.9.7/baidubce/services/vpc/peerconn_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,30 +12,31 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 """
-This module provides models for BBC-SDK.
+This module provides models for PEERCONN-SDK.
 """
 
 
 class Billing(object):
     """
-	This class define billing.
-	param: paymentTiming:
-		The pay time of the payment,
-		see more detail in https://bce.baidu.com/doc/BCC/API.html#Billing
-	param: reservationLength:
-		The duration to buy in specified time unit,
-		available values are [1,2,3,4,5,6,7,8,9,12,24,36] now.
-	param: reservationTimeUnit:
-		The time unit to specify the duration ,only "Month" can be used now.
-	"""
-    def __init__(self, paymentTiming=None, reservationLength=1, reservationTimeUnit='Month'):
+    This class define billing.
+    param: paymentTiming:
+        The pay time of the payment,
+        see more detail in https://bce.baidu.com/doc/BCC/API.html#Billing
+    param: reservationLength:
+        The duration to buy in specified time unit,
+        available values are [1,2,3,4,5,6,7,8,9,12,24,36] now.
+    param: reservationTimeUnit:
+        The time unit to specify the duration ,only "Month" can be used now.
+    """
+    def __init__(self, paymentTiming=None, reservationLength=1,
+                 reservationTimeUnit='Month'):
         if paymentTiming:
             self.paymentTiming = paymentTiming
         self.reservation = {
-			'reservationLength': reservationLength,
-			'reservationTimeUnit': reservationTimeUnit
-		}
+            'reservationLength': reservationLength,
+            'reservationTimeUnit': reservationTimeUnit
+        }
```

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bcc/bcc_client.py` & `bce_python_sdk-0.9.7/baidubce/services/bcc/bcc_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 class BccClient(bce_base_client.BceBaseClient):
     """
     Bcc base sdk client
     """
 
     prefix = b'/v2'
+    prefix_v3 = b'/v3'
 
     def __init__(self, config=None):
         bce_base_client.BceBaseClient.__init__(self, config)
 
     def _merge_config(self, config=None):
         if config is None:
             return self.config
@@ -1061,15 +1062,15 @@
 
         return self._send_request(http_methods.POST, path, json.dumps(body),
                                   params=params, config=config)
 
     def list_instances(self, marker=None, max_keys=None, internal_ip=None, dedicated_host_id=None,
                        zone_name=None, instance_ids=None, instance_names=None, cds_ids=None,
                        deployset_ids=None, security_group_ids=None, payment_timing=None, status=None, tags=None,
-                       vpc_id=None, private_ips=None, auto_renew=None, config=None):
+                       vpc_id=None, private_ips=None, ipv6_addresses=None, auto_renew=None, config=None):
         """
         Return a list of instances owned by the authenticated user.
 
         :param marker:
             The optional parameter marker specified in the original request to specify
             where in the results to begin listing.
             Together with the marker, specifies the list result which listing should begin.
@@ -1131,14 +1132,19 @@
         :type vpc_id: string
 
         :param private_ips:
             filter instance list with multiple private ips join by ',', the parameter should be used with
             vpc_id
         :type private_ips: string
 
+        :param ipv6_addresses:
+            filter instance list with multiple ipv6 private ips join by ',', the parameter should be used with
+            vpc_id
+        :type ipv6_addresses: string
+
         :param auto_renew:
         :type auto_renew: boolean
 
         :return:
         :rtype baidubce.bce_response.BceResponse
         """
         path = b'/instance'
@@ -1170,14 +1176,16 @@
             params['status'] = status
         if tags is not None:
             params['tags'] = tags
         if vpc_id is not None:
             params['vpcId'] = vpc_id
         if private_ips is not None:
             params['privateIps'] = private_ips
+        if ipv6_addresses is not None:
+            params['ipv6Addresses'] = ipv6_addresses
         if auto_renew is not None:
             params['autoRenew'] = auto_renew
         return self._send_request(http_methods.GET, path, params=params, config=config)
 
     @required(instance_id=(bytes, str))  # ***Unicode***
     def get_instance(self, instance_id, contains_failed=False, config=None):
         """
@@ -1636,14 +1644,102 @@
         }
         params = {
             'unbind': None
         }
         return self._send_request(http_methods.PUT, path, json.dumps(body),
                                   params=params, config=config)
 
+    @required(reserved_instance_ids=list,
+              tags=list)
+    def bind_reserved_instance_to_tags(self, reserved_instance_ids, tags, config=None):
+        """
+        :param reserved_instance_ids:
+        :param tags:
+        :param config:
+        :return:
+        """
+        path = b'/bcc/reserved/tag'
+        tag_list = [tag.__dict__ for tag in tags]
+        body = {
+            'changeTags': tag_list,
+            'reservedInstanceIds': reserved_instance_ids
+        }
+        params = {
+            'bind': None
+        }
+        return self._send_request(http_methods.PUT, path, json.dumps(body),
+                                  params=params, config=config)
+
+    @required(reserved_instance_ids=list,
+              tags=list)
+    def unbind_reserved_instance_from_tags(self, reserved_instance_ids, tags, config=None):
+        """
+        :param reserved_instance_ids:
+        :param tags:
+        :param config:
+        :return:
+        """
+        path = b'/bcc/reserved/tag'
+        tag_list = [tag.__dict__ for tag in tags]
+        body = {
+            'changeTags': tag_list,
+            'reservedInstanceIds': reserved_instance_ids
+        }
+        params = {
+            'unbind': None
+        }
+        return self._send_request(http_methods.PUT, path, json.dumps(body),
+                                  params=params, config=config)
+
+    def bind_tags_batch_by_resource_type(self, resource_type, resource_ids, tags, is_relation_tag, config=None):
+        """
+        :param resource_type:
+        :param resource_ids:
+        :param tags:
+        :param is_relation_tag:
+        :param config:
+        :return:
+        """
+        path = b'/bcc/tag'
+        tag_list = [tag.__dict__ for tag in tags]
+        body = {
+            'resourceType': resource_type,
+            'resourceIds': resource_ids,
+            'tags': tag_list,
+            'isRelationTag': is_relation_tag
+        }
+        params = {
+            'action': 'AttachTags'
+        }
+        return self._send_request(http_methods.POST, path, json.dumps(body),
+                                  params=params, config=config, prefix=self.prefix_v3)
+
+    def unbind_tags_batch_by_resource_type(self, resource_type, resource_ids, tags, is_relation_tag, config=None):
+        """
+        :param resource_type:
+        :param resource_ids:
+        :param tags:
+        :param is_relation_tag:
+        :param config:
+        :return:
+        """
+        path = b'/bcc/tag'
+        tag_list = [tag.__dict__ for tag in tags]
+        body = {
+            'resourceType': resource_type,
+            'resourceIds': resource_ids,
+            'tags': tag_list,
+            'isRelationTag': is_relation_tag
+        }
+        params = {
+            'action': 'DetachTags'
+        }
+        return self._send_request(http_methods.POST, path, json.dumps(body),
+                                  params=params, config=config, prefix=self.prefix_v3)
+
     @required(instance_id=(bytes, str),
               tags=list)
     def bind_instance_to_tags(self, instance_id, tags, config=None):
         """
         :param instance_id:
         :param tags:
         :param config:
```

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bcc/bcc_model.py` & `bce_python_sdk-0.9.7/baidubce/services/bcc/bcc_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bcc/fpga_card_type.py` & `bce_python_sdk-0.9.7/baidubce/services/bcc/fpga_card_type.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bcc/gpu_card_type.py` & `bce_python_sdk-0.9.7/baidubce/services/bcc/gpu_card_type.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bcm/bcm_client.py` & `bce_python_sdk-0.9.7/baidubce/services/bcm/bcm_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bcm/bcm_handler.py` & `bce_python_sdk-0.9.7/baidubce/services/bcm/bcm_handler.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bcm/bcm_model.py` & `bce_python_sdk-0.9.7/baidubce/services/bcm/bcm_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bes/bes_client.py` & `bce_python_sdk-0.9.7/baidubce/services/bes/bes_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bes/bes_model.py` & `bce_python_sdk-0.9.7/baidubce/services/bes/bes_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/blb/app_blb_client.py` & `bce_python_sdk-0.9.7/baidubce/services/blb/app_blb_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/blb/blb_client.py` & `bce_python_sdk-0.9.7/baidubce/services/blb/blb_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/blb/user_service_client.py` & `bce_python_sdk-0.9.7/baidubce/services/blb/user_service_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bmr/bmr_client.py` & `bce_python_sdk-0.9.7/baidubce/services/bmr/bmr_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bos/__init__.py` & `bce_python_sdk-0.9.7/baidubce/services/bos/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bos/bos_client.py` & `bce_python_sdk-0.9.7/baidubce/services/bos/bos_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bos/bos_handler.py` & `bce_python_sdk-0.9.7/baidubce/services/bos/bos_handler.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bos/canned_acl.py` & `bce_python_sdk-0.9.7/baidubce/services/bos/canned_acl.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bos/storage_class.py` & `bce_python_sdk-0.9.7/baidubce/services/bos/storage_class.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bts/__init__.py` & `bce_python_sdk-0.9.7/baidubce/services/bts/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bts/bts_client.py` & `bce_python_sdk-0.9.7/baidubce/services/bts/bts_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bts/model.py` & `bce_python_sdk-0.9.7/baidubce/services/bts/model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/bts/util.py` & `bce_python_sdk-0.9.7/baidubce/services/bts/util.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/cdn/cdn_client.py` & `bce_python_sdk-0.9.7/baidubce/services/cdn/cdn_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/cdn/cdn_stats_param.py` & `bce_python_sdk-0.9.7/baidubce/services/cdn/cdn_stats_param.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/cert/cert_client.py` & `bce_python_sdk-0.9.7/baidubce/services/cert/cert_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/cert/cert_model.py` & `bce_python_sdk-0.9.7/baidubce/services/cert/cert_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/cfc/cfc_client.py` & `bce_python_sdk-0.9.7/baidubce/services/cfc/cfc_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/cfc/cfc_handler.py` & `bce_python_sdk-0.9.7/baidubce/services/cfc/cfc_handler.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/cfc/models.py` & `bce_python_sdk-0.9.7/baidubce/services/cfc/models.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/csn/csn_api.py` & `bce_python_sdk-0.9.7/baidubce/services/csn/csn_api.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/csn/csn_client.py` & `bce_python_sdk-0.9.7/baidubce/services/csn/csn_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/csn/csn_model.py` & `bce_python_sdk-0.9.7/baidubce/services/csn/csn_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/ddc/ddc_client.py` & `bce_python_sdk-0.9.7/baidubce/services/ddc/ddc_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/dns/api/dns_api.py` & `bce_python_sdk-0.9.7/baidubce/services/dns/api/dns_api.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/dns/dns_client.py` & `bce_python_sdk-0.9.7/baidubce/services/dns/dns_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/dumap/dumap_client.py` & `bce_python_sdk-0.9.7/baidubce/services/dumap/dumap_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/eip/eip_bp_client.py` & `bce_python_sdk-0.9.7/baidubce/services/eip/eip_bp_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/eip/eip_client.py` & `bce_python_sdk-0.9.7/baidubce/services/eip/eip_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/eip/eip_group_client.py` & `bce_python_sdk-0.9.7/baidubce/services/eip/eip_group_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/eip/eip_group_model.py` & `bce_python_sdk-0.9.7/baidubce/services/eip/eip_group_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/eip/eip_tp_client.py` & `bce_python_sdk-0.9.7/baidubce/services/eip/eip_tp_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/eip/model.py` & `bce_python_sdk-0.9.7/baidubce/services/eip/model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/endpoint/endpoint_client.py` & `bce_python_sdk-0.9.7/baidubce/services/endpoint/endpoint_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/endpoint/model.py` & `bce_python_sdk-0.9.7/baidubce/services/endpoint/model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/eni/eni_client.py` & `bce_python_sdk-0.9.7/baidubce/services/eni/eni_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/eni/eni_model.py` & `bce_python_sdk-0.9.7/baidubce/services/eni/eni_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/et/et_client.py` & `bce_python_sdk-0.9.7/baidubce/services/et/et_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/et/model.py` & `bce_python_sdk-0.9.7/baidubce/services/et/model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/havip/havip_client.py` & `bce_python_sdk-0.9.7/baidubce/services/havip/havip_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/iam/__init__.py` & `bce_python_sdk-0.9.7/baidubce/services/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/iam/iam_client.py` & `bce_python_sdk-0.9.7/baidubce/services/iam/iam_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/infinite/__init__.py` & `bce_python_sdk-0.9.7/baidubce/services/infinite/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/infinite/infinite_client.py` & `bce_python_sdk-0.9.7/baidubce/services/infinite/infinite_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/ipv6gateway/ipv6gateway_client.py` & `bce_python_sdk-0.9.7/baidubce/services/ipv6gateway/ipv6gateway_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/ipv6gateway/ipv6gateway_model.py` & `bce_python_sdk-0.9.7/baidubce/services/ipv6gateway/ipv6gateway_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/kms/keyspec_class.py` & `bce_python_sdk-0.9.7/baidubce/services/kms/keyspec_class.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/kms/kms_client.py` & `bce_python_sdk-0.9.7/baidubce/services/kms/kms_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/kms/origin_class.py` & `bce_python_sdk-0.9.7/baidubce/services/kms/origin_class.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/kms/protectedby_class.py` & `bce_python_sdk-0.9.7/baidubce/services/kms/protectedby_class.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/kms/publickeyencoding_class.py` & `bce_python_sdk-0.9.7/baidubce/services/kms/publickeyencoding_class.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/lbdc/lbdc_client.py` & `bce_python_sdk-0.9.7/baidubce/services/lbdc/lbdc_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/lbdc/model.py` & `bce_python_sdk-0.9.7/baidubce/services/lbdc/model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/localdns/api/ld_api.py` & `bce_python_sdk-0.9.7/baidubce/services/localdns/api/ld_api.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/localdns/ld_client.py` & `bce_python_sdk-0.9.7/baidubce/services/localdns/ld_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/media/media_client.py` & `bce_python_sdk-0.9.7/baidubce/services/media/media_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/media/media_handler.py` & `bce_python_sdk-0.9.7/baidubce/services/media/media_handler.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/mms/__init__.py` & `bce_python_sdk-0.9.7/baidubce/services/mms/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/mms/mms_client.py` & `bce_python_sdk-0.9.7/baidubce/services/mms/mms_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/mvs/__init__.py` & `bce_python_sdk-0.9.7/baidubce/services/mvs/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/mvs/mvs_client.py` & `bce_python_sdk-0.9.7/baidubce/services/mvs/mvs_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/oos/oos_client.py` & `bce_python_sdk-0.9.7/baidubce/services/oos/oos_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/oos/oos_model.py` & `bce_python_sdk-0.9.7/baidubce/services/oos/oos_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/rds/__init__.py` & `bce_python_sdk-0.9.7/baidubce/services/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/rds/rds_backup_manager.py` & `bce_python_sdk-0.9.7/baidubce/services/rds/rds_backup_manager.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/rds/rds_database_manager.py` & `bce_python_sdk-0.9.7/baidubce/services/rds/rds_database_manager.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/rds/rds_hot_active_instance_group_manager.py` & `bce_python_sdk-0.9.7/baidubce/services/rds/rds_hot_active_instance_group_manager.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/rds/rds_http.py` & `bce_python_sdk-0.9.7/baidubce/services/rds/rds_http.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/rds/rds_instance_manager.py` & `bce_python_sdk-0.9.7/baidubce/services/rds/rds_instance_manager.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/rds/rds_log_manager.py` & `bce_python_sdk-0.9.7/baidubce/services/rds/rds_log_manager.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/rds/rds_parameter_manager.py` & `bce_python_sdk-0.9.7/baidubce/services/rds/rds_parameter_manager.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/rds/rds_readonly_group_manager.py` & `bce_python_sdk-0.9.7/baidubce/services/rds/rds_readonly_group_manager.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/rds/rds_recycler_manager.py` & `bce_python_sdk-0.9.7/baidubce/services/rds/rds_recycler_manager.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/rds/rds_security_manager.py` & `bce_python_sdk-0.9.7/baidubce/services/rds/rds_security_manager.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/rds/rds_task_manager.py` & `bce_python_sdk-0.9.7/baidubce/services/rds/rds_task_manager.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/rds/rds_users_manager.py` & `bce_python_sdk-0.9.7/baidubce/services/rds/rds_users_manager.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/route/route_client.py` & `bce_python_sdk-0.9.7/baidubce/services/route/route_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/scs/__init__.py` & `bce_python_sdk-0.9.7/baidubce/services/scs/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/scs/model.py` & `bce_python_sdk-0.9.7/baidubce/services/scs/model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/scs/scs_client.py` & `bce_python_sdk-0.9.7/baidubce/services/scs/scs_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/sms/__init__.py` & `bce_python_sdk-0.9.7/baidubce/services/sms/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/sms/model.py` & `bce_python_sdk-0.9.7/baidubce/services/sms/model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/sms/sms_client.py` & `bce_python_sdk-0.9.7/baidubce/services/sms/sms_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/sts/__init__.py` & `bce_python_sdk-0.9.7/baidubce/services/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/sts/sts_client.py` & `bce_python_sdk-0.9.7/baidubce/services/sts/sts_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/subnet/subnet_client.py` & `bce_python_sdk-0.9.7/baidubce/services/subnet/subnet_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/tsdb/tsdb_admin_client.py` & `bce_python_sdk-0.9.7/baidubce/services/tsdb/tsdb_admin_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/tsdb/tsdb_client.py` & `bce_python_sdk-0.9.7/baidubce/services/tsdb/tsdb_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/tsdb/tsdb_handler.py` & `bce_python_sdk-0.9.7/baidubce/services/tsdb/tsdb_handler.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/vca/vca_client.py` & `bce_python_sdk-0.9.7/baidubce/services/vca/vca_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/vcr/vcr_client.py` & `bce_python_sdk-0.9.7/baidubce/services/vcr/vcr_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/vpc/acl_client.py` & `bce_python_sdk-0.9.7/baidubce/services/vpc/acl_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/vpc/nat_client.py` & `bce_python_sdk-0.9.7/baidubce/services/vpc/nat_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/vpc/nat_model.py` & `bce_python_sdk-0.9.7/baidubce/services/vpc/nat_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/vpc/peerconn_client.py` & `bce_python_sdk-0.9.7/baidubce/services/vpc/peerconn_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/vpc/peerconn_model.py` & `bce_python_sdk-0.9.7/baidubce/services/bbc/bbc_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,31 +12,41 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 """
-This module provides models for PEERCONN-SDK.
+This module provides models for BBC-SDK.
 """
 
 
 class Billing(object):
     """
-    This class define billing.
-    param: paymentTiming:
-        The pay time of the payment,
-        see more detail in https://bce.baidu.com/doc/BCC/API.html#Billing
-    param: reservationLength:
-        The duration to buy in specified time unit,
-        available values are [1,2,3,4,5,6,7,8,9,12,24,36] now.
-    param: reservationTimeUnit:
-        The time unit to specify the duration ,only "Month" can be used now.
-    """
-    def __init__(self, paymentTiming=None, reservationLength=1,
-                 reservationTimeUnit='Month'):
+	This class define billing.
+	param: paymentTiming:
+		The pay time of the payment,
+		see more detail in https://bce.baidu.com/doc/BCC/API.html#Billing
+	param: reservationLength:
+		The duration to buy in specified time unit,
+		available values are [1,2,3,4,5,6,7,8,9,12,24,36] now.
+	param: reservationTimeUnit:
+		The time unit to specify the duration ,only "Month" can be used now.
+	"""
+
+    def __init__(self, paymentTiming=None, reservationLength=1, reservationTimeUnit='Month'):
         if paymentTiming:
             self.paymentTiming = paymentTiming
         self.reservation = {
             'reservationLength': reservationLength,
             'reservationTimeUnit': reservationTimeUnit
         }
+
+
+class TagModel(object):
+    """
+    TAGModel
+    """
+
+    def __init__(self, tagKey=None, tagValue=None):
+        self.tagKey = tagKey
+        self.tagValue = tagValue
```

### Comparing `bce-python-sdk-0.9.6/baidubce/services/vpc/vpc_client.py` & `bce_python_sdk-0.9.7/baidubce/services/vpc/vpc_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/vpn/vpn_client.py` & `bce_python_sdk-0.9.7/baidubce/services/vpn/vpn_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/services/vpn/vpn_model.py` & `bce_python_sdk-0.9.7/baidubce/services/vpn/vpn_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/baidubce/utils.py` & `bce_python_sdk-0.9.7/baidubce/utils.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/bce_python_sdk.egg-info/SOURCES.txt` & `bce_python_sdk-0.9.7/bce_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.9.6/setup.py` & `bce_python_sdk-0.9.7/setup.py`

 * *Files identical despite different names*

