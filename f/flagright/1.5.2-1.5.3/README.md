# Comparing `tmp/flagright-1.5.2.tar.gz` & `tmp/flagright-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flagright-1.5.2.tar", max compression
+gzip compressed data, was "flagright-1.5.3.tar", max compression
```

## Comparing `flagright-1.5.2.tar` & `flagright-1.5.3.tar`

### file list

```diff
@@ -1,163 +1,163 @@
--rw-r--r--   0        0        0      829 2024-04-19 15:19:49.417884 flagright-1.5.2/README.md
--rw-r--r--   0        0        0      404 2024-04-19 15:19:49.417884 flagright-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     9653 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/__init__.py
--rw-r--r--   0        0        0     3441 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/client.py
--rw-r--r--   0        0        0      519 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/core/api_error.py
--rw-r--r--   0        0        0     1078 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      168 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/environment.py
--rw-r--r--   0        0        0      358 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/errors/bad_request_error.py
--rw-r--r--   0        0        0      247 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/errors/forbidden_error.py
--rw-r--r--   0        0        0      253 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      250 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/errors/unauthorized_error.py
--rw-r--r--   0        0        0        0 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/py.typed
--rw-r--r--   0        0        0      647 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/business_user_events/__init__.py
--rw-r--r--   0        0        0    70170 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/business_user_events/client.py
--rw-r--r--   0        0        0      155 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/business_users/__init__.py
--rw-r--r--   0        0        0    38466 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/business_users/client.py
--rw-r--r--   0        0        0      180 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/business_users/types/__init__.py
--rw-r--r--   0        0        0      910 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/business_users/types/business_users_create_response.py
--rw-r--r--   0        0        0       65 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/consumer_user_events/__init__.py
--rw-r--r--   0        0        0    23686 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/consumer_user_events/client.py
--rw-r--r--   0        0        0      155 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/consumer_users/__init__.py
--rw-r--r--   0        0        0    20900 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/consumer_users/client.py
--rw-r--r--   0        0        0      180 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/consumer_users/types/__init__.py
--rw-r--r--   0        0        0      910 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/consumer_users/types/consumer_users_create_response.py
--rw-r--r--   0        0        0       65 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/transaction_events/__init__.py
--rw-r--r--   0        0        0    16377 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/transaction_events/client.py
--rw-r--r--   0        0        0      153 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/transactions/__init__.py
--rw-r--r--   0        0        0    19718 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/transactions/client.py
--rw-r--r--   0        0        0      176 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/transactions/types/__init__.py
--rw-r--r--   0        0        0      927 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/transactions/types/transactions_verify_response.py
--rw-r--r--   0        0        0    12233 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/__init__.py
--rw-r--r--   0        0        0     1947 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/ach_details.py
--rw-r--r--   0        0        0      143 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/ach_payment_method.py
--rw-r--r--   0        0        0     1167 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/acquisition_channel.py
--rw-r--r--   0        0        0     1637 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/address.py
--rw-r--r--   0        0        0     1667 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/alert_closed_details.py
--rw-r--r--   0        0        0     1160 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/amount.py
--rw-r--r--   0        0        0      448 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/boolean_string.py
--rw-r--r--   0        0        0     3230 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business.py
--rw-r--r--   0        0        0     1296 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business_base.py
--rw-r--r--   0        0        0     1080 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business_entity_link.py
--rw-r--r--   0        0        0     3090 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business_optional.py
--rw-r--r--   0        0        0     3143 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business_optional_saved_payment_details_item.py
--rw-r--r--   0        0        0     1658 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business_user_event.py
--rw-r--r--   0        0        0     1282 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business_user_segment.py
--rw-r--r--   0        0        0     1546 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business_users_response.py
--rw-r--r--   0        0        0     1470 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business_with_rules_result.py
--rw-r--r--   0        0        0     1247 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/card_brand.py
--rw-r--r--   0        0        0     3079 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/card_details.py
--rw-r--r--   0        0        0      920 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/card_expiry.py
--rw-r--r--   0        0        0      661 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/card_funding.py
--rw-r--r--   0        0        0     1200 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/card_merchant_details.py
--rw-r--r--   0        0        0      145 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/card_payment_method.py
--rw-r--r--   0        0        0      497 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/card_type.py
--rw-r--r--   0        0        0     1357 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/case_closed_details.py
--rw-r--r--   0        0        0     2130 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/case_management_event.py
--rw-r--r--   0        0        0      558 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/case_management_event_case_status.py
--rw-r--r--   0        0        0     1174 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/case_management_event_case_status_reason.py
--rw-r--r--   0        0        0     1169 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/case_opened_details.py
--rw-r--r--   0        0        0     1133 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/check_delivery_status.py
--rw-r--r--   0        0        0     1608 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/check_details.py
--rw-r--r--   0        0        0      147 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/check_payment_method.py
--rw-r--r--   0        0        0     1420 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/company_financial_details.py
--rw-r--r--   0        0        0     2026 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/company_general_details.py
--rw-r--r--   0        0        0     1878 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/company_registration_details.py
--rw-r--r--   0        0        0     1272 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/consumer_name.py
--rw-r--r--   0        0        0     1646 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/consumer_user_event.py
--rw-r--r--   0        0        0      511 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/consumer_user_segment.py
--rw-r--r--   0        0        0     1546 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/consumer_users_response.py
--rw-r--r--   0        0        0     1731 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/contact_details.py
--rw-r--r--   0        0        0    29271 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/country_code.py
--rw-r--r--   0        0        0    56920 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/currency_code.py
--rw-r--r--   0        0        0     1066 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/date.py
--rw-r--r--   0        0        0     2967 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/device_data.py
--rw-r--r--   0        0        0       79 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/email_id.py
--rw-r--r--   0        0        0     1685 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/employment_status.py
--rw-r--r--   0        0        0     1771 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/executed_rules_result.py
--rw-r--r--   0        0        0     1426 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/failed_rules_result.py
--rw-r--r--   0        0        0     1049 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/false_positive_details.py
--rw-r--r--   0        0        0      584 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/gender.py
--rw-r--r--   0        0        0      175 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/general_bank_account_payment_method.py
--rw-r--r--   0        0        0     2340 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/generic_bank_account_details.py
--rw-r--r--   0        0        0     1709 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/hit_rules_details.py
--rw-r--r--   0        0        0     2249 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/iban_details.py
--rw-r--r--   0        0        0      145 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/iban_payment_method.py
--rw-r--r--   0        0        0     1575 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/kyc_status.py
--rw-r--r--   0        0        0     1078 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/kyc_status_details.py
--rw-r--r--   0        0        0     2153 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/legal_document.py
--rw-r--r--   0        0        0     1939 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/legal_entity.py
--rw-r--r--   0        0        0     1115 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/list_data.py
--rw-r--r--   0        0        0     1162 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/list_existed.py
--rw-r--r--   0        0        0     1275 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/list_header.py
--rw-r--r--   0        0        0      958 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/list_item.py
--rw-r--r--   0        0        0      127 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/list_key_metadata.py
--rw-r--r--   0        0        0     1084 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/list_metadata.py
--rw-r--r--   0        0        0     2152 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/list_subtype.py
--rw-r--r--   0        0        0      697 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/list_type.py
--rw-r--r--   0        0        0     1006 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/mcc_details.py
--rw-r--r--   0        0        0     1573 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/mpesa_details.py
--rw-r--r--   0        0        0      147 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/mpesa_payment_method.py
--rw-r--r--   0        0        0     1312 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/mpesa_transaction_type.py
--rw-r--r--   0        0        0     1465 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/payment_method.py
--rw-r--r--   0        0        0     1029 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/pep_status.py
--rw-r--r--   0        0        0     1781 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/person.py
--rw-r--r--   0        0        0      884 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/risk_level.py
--rw-r--r--   0        0        0      921 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/rule_action.py
--rw-r--r--   0        0        0     1121 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/rule_failure_exception.py
--rw-r--r--   0        0        0      497 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/rule_hit_direction.py
--rw-r--r--   0        0        0     1562 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/rule_hit_meta.py
--rw-r--r--   0        0        0     2235 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/rule_labels.py
--rw-r--r--   0        0        0      735 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/rule_nature.py
--rw-r--r--   0        0        0     1293 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/rules_results.py
--rw-r--r--   0        0        0     1172 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/sanctions_details.py
--rw-r--r--   0        0        0     1694 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/sanctions_details_entity_type.py
--rw-r--r--   0        0        0     2433 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/source_of_funds.py
--rw-r--r--   0        0        0     2071 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/swift_details.py
--rw-r--r--   0        0        0      147 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/swift_payment_method.py
--rw-r--r--   0        0        0     1156 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/tag.py
--rw-r--r--   0        0        0      907 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction.py
--rw-r--r--   0        0        0     1291 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_amount_details.py
--rw-r--r--   0        0        0     1028 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_amount_limit.py
--rw-r--r--   0        0        0     1616 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_base.py
--rw-r--r--   0        0        0      996 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_count_limit.py
--rw-r--r--   0        0        0     1923 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_event.py
--rw-r--r--   0        0        0     1260 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_event_monitoring_result.py
--rw-r--r--   0        0        0     1408 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_limit.py
--rw-r--r--   0        0        0     1947 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_limits.py
--rw-r--r--   0        0        0     1686 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_limits_payment_method_limits.py
--rw-r--r--   0        0        0     1332 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_monitoring_result.py
--rw-r--r--   0        0        0     1122 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_risk_scoring_result.py
--rw-r--r--   0        0        0     1669 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_state.py
--rw-r--r--   0        0        0     1100 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_status_details.py
--rw-r--r--   0        0        0     1140 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_type.py
--rw-r--r--   0        0        0     3339 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_updatable.py
--rw-r--r--   0        0        0     3257 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_updatable_destination_payment_details.py
--rw-r--r--   0        0        0     3162 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_updatable_origin_payment_details.py
--rw-r--r--   0        0        0     1534 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_with_rules_result.py
--rw-r--r--   0        0        0     1635 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/upi_details.py
--rw-r--r--   0        0        0      143 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/upi_payment_method.py
--rw-r--r--   0        0        0      899 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user.py
--rw-r--r--   0        0        0     1141 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user_base.py
--rw-r--r--   0        0        0     1476 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user_details.py
--rw-r--r--   0        0        0     3056 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user_optional.py
--rw-r--r--   0        0        0      540 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user_registration_status.py
--rw-r--r--   0        0        0     1279 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user_risk_score_details.py
--rw-r--r--   0        0        0     1232 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user_state.py
--rw-r--r--   0        0        0     1060 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user_state_details.py
--rw-r--r--   0        0        0     1459 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user_with_rules_result.py
--rw-r--r--   0        0        0     2210 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/wallet_details.py
--rw-r--r--   0        0        0     3957 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/wallet_network.py
--rw-r--r--   0        0        0      149 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/wallet_payment_method.py
--rw-r--r--   0        0        0      987 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/webhook_event.py
--rw-r--r--   0        0        0     1387 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/webhook_event_base.py
--rw-r--r--   0        0        0      562 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/webhook_event_base_triggered_by.py
--rw-r--r--   0        0        0      578 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/webhook_event_data.py
--rw-r--r--   0        0        0     1201 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/webhook_event_type.py
--rw-r--r--   0        0        0     1335 1970-01-01 00:00:00.000000 flagright-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0      829 2024-04-23 15:36:21.233697 flagright-1.5.3/README.md
+-rw-r--r--   0        0        0      404 2024-04-23 15:36:21.233697 flagright-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     9653 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/__init__.py
+-rw-r--r--   0        0        0     3441 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/client.py
+-rw-r--r--   0        0        0      519 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/core/api_error.py
+-rw-r--r--   0        0        0     1078 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      168 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/environment.py
+-rw-r--r--   0        0        0      358 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/errors/forbidden_error.py
+-rw-r--r--   0        0        0      253 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      250 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/errors/unauthorized_error.py
+-rw-r--r--   0        0        0        0 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/py.typed
+-rw-r--r--   0        0        0      647 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/resources/business_user_events/__init__.py
+-rw-r--r--   0        0        0    10484 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/resources/business_user_events/client.py
+-rw-r--r--   0        0        0      155 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/resources/business_users/__init__.py
+-rw-r--r--   0        0        0    10024 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/resources/business_users/client.py
+-rw-r--r--   0        0        0      180 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/resources/business_users/types/__init__.py
+-rw-r--r--   0        0        0      910 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/resources/business_users/types/business_users_create_response.py
+-rw-r--r--   0        0        0       65 2024-04-23 15:36:21.233697 flagright-1.5.3/src/flagright/resources/consumer_user_events/__init__.py
+-rw-r--r--   0        0        0    10460 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/resources/consumer_user_events/client.py
+-rw-r--r--   0        0        0      155 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/resources/consumer_users/__init__.py
+-rw-r--r--   0        0        0    13448 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/resources/consumer_users/client.py
+-rw-r--r--   0        0        0      180 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/resources/consumer_users/types/__init__.py
+-rw-r--r--   0        0        0      910 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/resources/consumer_users/types/consumer_users_create_response.py
+-rw-r--r--   0        0        0       65 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/resources/transaction_events/__init__.py
+-rw-r--r--   0        0        0    11401 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/resources/transaction_events/client.py
+-rw-r--r--   0        0        0      153 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/resources/transactions/__init__.py
+-rw-r--r--   0        0        0    19448 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/resources/transactions/client.py
+-rw-r--r--   0        0        0      176 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/resources/transactions/types/__init__.py
+-rw-r--r--   0        0        0      927 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/resources/transactions/types/transactions_verify_response.py
+-rw-r--r--   0        0        0    12233 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/__init__.py
+-rw-r--r--   0        0        0     1947 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/ach_details.py
+-rw-r--r--   0        0        0      143 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/ach_payment_method.py
+-rw-r--r--   0        0        0     1167 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/acquisition_channel.py
+-rw-r--r--   0        0        0     1637 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/address.py
+-rw-r--r--   0        0        0     1667 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/alert_closed_details.py
+-rw-r--r--   0        0        0     1160 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/amount.py
+-rw-r--r--   0        0        0      448 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/boolean_string.py
+-rw-r--r--   0        0        0     3230 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/business.py
+-rw-r--r--   0        0        0     1296 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/business_base.py
+-rw-r--r--   0        0        0     1080 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/business_entity_link.py
+-rw-r--r--   0        0        0     3090 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/business_optional.py
+-rw-r--r--   0        0        0     3143 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/business_optional_saved_payment_details_item.py
+-rw-r--r--   0        0        0     1658 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/business_user_event.py
+-rw-r--r--   0        0        0     1282 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/business_user_segment.py
+-rw-r--r--   0        0        0     1546 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/business_users_response.py
+-rw-r--r--   0        0        0     1470 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/business_with_rules_result.py
+-rw-r--r--   0        0        0     1247 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/card_brand.py
+-rw-r--r--   0        0        0     3079 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/card_details.py
+-rw-r--r--   0        0        0      920 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/card_expiry.py
+-rw-r--r--   0        0        0      661 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/card_funding.py
+-rw-r--r--   0        0        0     1200 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/card_merchant_details.py
+-rw-r--r--   0        0        0      145 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/card_payment_method.py
+-rw-r--r--   0        0        0      497 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/card_type.py
+-rw-r--r--   0        0        0     1357 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/case_closed_details.py
+-rw-r--r--   0        0        0     2130 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/case_management_event.py
+-rw-r--r--   0        0        0      558 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/case_management_event_case_status.py
+-rw-r--r--   0        0        0     1174 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/case_management_event_case_status_reason.py
+-rw-r--r--   0        0        0     1169 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/case_opened_details.py
+-rw-r--r--   0        0        0     1133 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/check_delivery_status.py
+-rw-r--r--   0        0        0     1608 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/check_details.py
+-rw-r--r--   0        0        0      147 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/check_payment_method.py
+-rw-r--r--   0        0        0     1420 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/company_financial_details.py
+-rw-r--r--   0        0        0     2026 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/company_general_details.py
+-rw-r--r--   0        0        0     1878 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/company_registration_details.py
+-rw-r--r--   0        0        0     1272 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/consumer_name.py
+-rw-r--r--   0        0        0     1646 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/consumer_user_event.py
+-rw-r--r--   0        0        0      511 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/consumer_user_segment.py
+-rw-r--r--   0        0        0     1546 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/consumer_users_response.py
+-rw-r--r--   0        0        0     1731 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/contact_details.py
+-rw-r--r--   0        0        0    29271 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/country_code.py
+-rw-r--r--   0        0        0    56922 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/currency_code.py
+-rw-r--r--   0        0        0     1066 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/date.py
+-rw-r--r--   0        0        0     2967 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/device_data.py
+-rw-r--r--   0        0        0       79 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/email_id.py
+-rw-r--r--   0        0        0     1685 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/employment_status.py
+-rw-r--r--   0        0        0     1771 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/executed_rules_result.py
+-rw-r--r--   0        0        0     1426 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/failed_rules_result.py
+-rw-r--r--   0        0        0     1049 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/false_positive_details.py
+-rw-r--r--   0        0        0      584 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/gender.py
+-rw-r--r--   0        0        0      175 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/general_bank_account_payment_method.py
+-rw-r--r--   0        0        0     2340 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/generic_bank_account_details.py
+-rw-r--r--   0        0        0     1709 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/hit_rules_details.py
+-rw-r--r--   0        0        0     2249 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/iban_details.py
+-rw-r--r--   0        0        0      145 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/iban_payment_method.py
+-rw-r--r--   0        0        0     1575 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/kyc_status.py
+-rw-r--r--   0        0        0     1078 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/kyc_status_details.py
+-rw-r--r--   0        0        0     2153 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/legal_document.py
+-rw-r--r--   0        0        0     1939 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/legal_entity.py
+-rw-r--r--   0        0        0     1115 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/list_data.py
+-rw-r--r--   0        0        0     1162 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/list_existed.py
+-rw-r--r--   0        0        0     1275 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/list_header.py
+-rw-r--r--   0        0        0      958 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/list_item.py
+-rw-r--r--   0        0        0      127 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/list_key_metadata.py
+-rw-r--r--   0        0        0     1084 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/list_metadata.py
+-rw-r--r--   0        0        0     2152 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/list_subtype.py
+-rw-r--r--   0        0        0      697 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/list_type.py
+-rw-r--r--   0        0        0     1006 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/mcc_details.py
+-rw-r--r--   0        0        0     1573 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/mpesa_details.py
+-rw-r--r--   0        0        0      147 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/mpesa_payment_method.py
+-rw-r--r--   0        0        0     1312 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/mpesa_transaction_type.py
+-rw-r--r--   0        0        0     1465 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/payment_method.py
+-rw-r--r--   0        0        0     1029 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/pep_status.py
+-rw-r--r--   0        0        0     1781 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/person.py
+-rw-r--r--   0        0        0      884 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/risk_level.py
+-rw-r--r--   0        0        0      921 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/rule_action.py
+-rw-r--r--   0        0        0     1121 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/rule_failure_exception.py
+-rw-r--r--   0        0        0      497 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/rule_hit_direction.py
+-rw-r--r--   0        0        0     1562 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/rule_hit_meta.py
+-rw-r--r--   0        0        0     2235 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/rule_labels.py
+-rw-r--r--   0        0        0      735 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/rule_nature.py
+-rw-r--r--   0        0        0     1293 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/rules_results.py
+-rw-r--r--   0        0        0     1172 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/sanctions_details.py
+-rw-r--r--   0        0        0     1694 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/sanctions_details_entity_type.py
+-rw-r--r--   0        0        0     2433 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/source_of_funds.py
+-rw-r--r--   0        0        0     2071 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/swift_details.py
+-rw-r--r--   0        0        0      147 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/swift_payment_method.py
+-rw-r--r--   0        0        0     1156 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/tag.py
+-rw-r--r--   0        0        0      907 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction.py
+-rw-r--r--   0        0        0     1291 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_amount_details.py
+-rw-r--r--   0        0        0     1028 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_amount_limit.py
+-rw-r--r--   0        0        0     1616 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_base.py
+-rw-r--r--   0        0        0      996 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_count_limit.py
+-rw-r--r--   0        0        0     1923 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_event.py
+-rw-r--r--   0        0        0     1260 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_event_monitoring_result.py
+-rw-r--r--   0        0        0     1408 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_limit.py
+-rw-r--r--   0        0        0     1947 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_limits.py
+-rw-r--r--   0        0        0     1686 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_limits_payment_method_limits.py
+-rw-r--r--   0        0        0     1332 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_monitoring_result.py
+-rw-r--r--   0        0        0     1122 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_risk_scoring_result.py
+-rw-r--r--   0        0        0     1669 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_state.py
+-rw-r--r--   0        0        0     1100 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_status_details.py
+-rw-r--r--   0        0        0     1140 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_type.py
+-rw-r--r--   0        0        0     3339 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_updatable.py
+-rw-r--r--   0        0        0     3257 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_updatable_destination_payment_details.py
+-rw-r--r--   0        0        0     3162 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_updatable_origin_payment_details.py
+-rw-r--r--   0        0        0     1534 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/transaction_with_rules_result.py
+-rw-r--r--   0        0        0     1635 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/upi_details.py
+-rw-r--r--   0        0        0      143 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/upi_payment_method.py
+-rw-r--r--   0        0        0      899 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/user.py
+-rw-r--r--   0        0        0     1141 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/user_base.py
+-rw-r--r--   0        0        0     1476 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/user_details.py
+-rw-r--r--   0        0        0     3056 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/user_optional.py
+-rw-r--r--   0        0        0      540 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/user_registration_status.py
+-rw-r--r--   0        0        0     1279 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/user_risk_score_details.py
+-rw-r--r--   0        0        0     1232 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/user_state.py
+-rw-r--r--   0        0        0     1060 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/user_state_details.py
+-rw-r--r--   0        0        0     1459 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/user_with_rules_result.py
+-rw-r--r--   0        0        0     2210 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/wallet_details.py
+-rw-r--r--   0        0        0     3957 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/wallet_network.py
+-rw-r--r--   0        0        0      149 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/wallet_payment_method.py
+-rw-r--r--   0        0        0      987 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/webhook_event.py
+-rw-r--r--   0        0        0     1387 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/webhook_event_base.py
+-rw-r--r--   0        0        0      562 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/webhook_event_base_triggered_by.py
+-rw-r--r--   0        0        0      578 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/webhook_event_data.py
+-rw-r--r--   0        0        0     1201 2024-04-23 15:36:21.237697 flagright-1.5.3/src/flagright/types/webhook_event_type.py
+-rw-r--r--   0        0        0     1335 1970-01-01 00:00:00.000000 flagright-1.5.3/PKG-INFO
```

### Comparing `flagright-1.5.2/README.md` & `flagright-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/__init__.py` & `flagright-1.5.3/src/flagright/__init__.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/client.py` & `flagright-1.5.3/src/flagright/client.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/core/__init__.py` & `flagright-1.5.3/src/flagright/core/__init__.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/core/client_wrapper.py` & `flagright-1.5.3/src/flagright/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self.api_key = api_key
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "flagright",
-            "X-Fern-SDK-Version": "1.5.2",
+            "X-Fern-SDK-Version": "1.5.3",
         }
         headers["x-api-key"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `flagright-1.5.2/src/flagright/core/datetime_utils.py` & `flagright-1.5.3/src/flagright/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/core/jsonable_encoder.py` & `flagright-1.5.3/src/flagright/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/resources/__init__.py` & `flagright-1.5.3/src/flagright/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/resources/business_users/types/business_users_create_response.py` & `flagright-1.5.3/src/flagright/resources/business_users/types/business_users_create_response.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/resources/consumer_users/client.py` & `flagright-1.5.3/src/flagright/resources/transactions/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,499 +3,374 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
+from ...core.remove_none_from_dict import remove_none_from_dict
 from ...errors.bad_request_error import BadRequestError
+from ...errors.forbidden_error import ForbiddenError
 from ...errors.too_many_requests_error import TooManyRequestsError
 from ...errors.unauthorized_error import UnauthorizedError
-from ...types.user import User
-from ...types.user_with_rules_result import UserWithRulesResult
-from .types.consumer_users_create_response import ConsumerUsersCreateResponse
+from ...types.boolean_string import BooleanString
+from ...types.transaction import Transaction
+from ...types.transaction_with_rules_result import TransactionWithRulesResult
+from .types.transactions_verify_response import TransactionsVerifyResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class ConsumerUsersClient:
+class TransactionsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def create(self, *, request: User) -> ConsumerUsersCreateResponse:
+    def verify(
+        self,
+        *,
+        validate_origin_user_id: typing.Optional[BooleanString] = None,
+        validate_destination_user_id: typing.Optional[BooleanString] = None,
+        request: Transaction,
+    ) -> TransactionsVerifyResponse:
         """
-        ## POST Consumer User
+        ## POST Transactions
 
-        `/consumer/user` endpoint allows you to operate on the Consumer user entity.
+        `/transactions` endpoint allows you to operate on the [Transaction entity.](/guides/overview/entities#transaction)
 
-        In order to pass the payload of a User to Flagright and verify the User, you will need to call this endpoint with the User payload. Not all fields are mandatory, you will only need to pass in the fields that you have and are relevant for your compliance setup.
+        In order to pass the payload of a transaction to Flagright and verify the transaction, you will need to call this endpoint with the transaction payload. Not all fields are mandatory, you will only need to pass in the fields that you have and are relevant for your compliance setup.
 
         ### Payload
 
-        Each consumer user needs two mandatory fields:
+        Here are some of the most used payload fields explained (you can find the full payload [schema below](/api-reference/api-reference/transactions/verify#request) with 1 line descriptions):
 
-        - `userId` - Unique identifier for the user
-        - `createdTimestamp` - UNIX timestamp in _milliseconds_ for when the User is created in your system
+        - `type`: Type of transaction (Ex: `WITHDRAWAL`, `DEPOSIT`, `TRANSFER` etc).
+        - `transactionId` - Unique Identifier for the transaction. Flagright API will generate a `transactionId` if this field is left empty
+        - `timestamp` - UNIX timestamp in _milliseconds_ of when the transaction took place
+        - `transactionState` - The state of the transaction, set to `CREATED` by default. [More details here](/guides/overview/entities#transaction-lifecycle-through-transaction-events)
+        - `originUserId` - Unique identifier (if any) of the user who is sending the money. This user must be created within the Flagright system before using the [create a consumer user](/api-reference/api-reference/consumer-users/create) or [create a business user](/api-reference/api-reference/business-users/create) endpoint
+        - `destinationUserId` - Unique identifier (if any) of the user who is receiving the money. This user must be created within the Flagright system before using the [create a consumer user](/api-reference/api-reference/consumer-users/create) or [create a business user](/api-reference/api-reference/business-users/create) endpoint
+        - `originAmountDetails` - Details of the amount being sent from the origin
+        - `destinationAmountDetails` - Details of the amount being received at the destination
+        - `originPaymentDetails` - Payment details (if any) used at the origin (ex: `CARD`, `IBAN`, `WALLET` etc). You can click on the dropdown next to the field in the schema below to view all supported payment types.
+        - `destinationPaymentDetails` - Payment details (if any) used at the destination (ex: `CARD`, `IBAN`, `WALLET` etc). You can click on the dropdown next to the field in the schema below to view all supported payment types.
 
         Parameters:
-            - request: User.
+            - validate_origin_user_id: typing.Optional[BooleanString]. Boolean string whether Flagright should validate if provided originUserId exist. True by default
+
+            - validate_destination_user_id: typing.Optional[BooleanString]. Boolean string whether Flagright should validate if provided destinationUserId exist. True by default
+
+            - request: Transaction.
         ---
         from flagright import (
-            Address,
-            Amount,
-            ConsumerName,
-            ContactDetails,
             CountryCode,
             CurrencyCode,
-            LegalDocument,
+            DeviceData,
             Tag,
-            TransactionLimits,
-            User,
-            UserDetails,
+            Transaction,
+            TransactionAmountDetails,
+            TransactionType,
         )
         from flagright.client import Flagright
 
         client = Flagright(
             api_key="YOUR_API_KEY",
         )
-        client.consumer_users.create(
-            request=User(
-                user_details=UserDetails(
-                    name=ConsumerName(
-                        first_name="Baran",
-                        middle_name="Realblood",
-                        last_name="Ozkan",
-                    ),
-                    date_of_birth="1991-01-01",
-                    country_of_residence=CountryCode.US,
-                    country_of_nationality=CountryCode.DE,
+        client.transactions.verify(
+            request=Transaction(
+                origin_amount_details=TransactionAmountDetails(
+                    transaction_amount=800.0,
+                    transaction_currency=CurrencyCode.EUR,
+                    country=CountryCode.DE,
                 ),
-                legal_documents=[
-                    LegalDocument(
-                        document_type="passport",
-                        document_number="Z9431P",
-                        document_issued_date=1639939034000.0,
-                        document_expiration_date=1839939034000.0,
-                        document_issued_country=CountryCode.DE,
-                        tags=[
-                            Tag(
-                                key="customerType",
-                                value="wallet",
-                            ),
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                        ],
-                        name_on_document=ConsumerName(
-                            first_name="Baran",
-                            middle_name="Realblood",
-                            last_name="Ozkan",
-                        ),
-                    ),
-                    LegalDocument(
-                        document_type="passport",
-                        document_number="Z9431P",
-                        document_issued_date=1639939034000.0,
-                        document_expiration_date=1839939034000.0,
-                        document_issued_country=CountryCode.DE,
-                        tags=[
-                            Tag(
-                                key="customerType",
-                                value="wallet",
-                            ),
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                        ],
-                        name_on_document=ConsumerName(
-                            first_name="Baran",
-                            middle_name="Realblood",
-                            last_name="Ozkan",
-                        ),
-                    ),
-                ],
-                contact_details=ContactDetails(
-                    email_ids=["baran@flagright.com", "emailIds"],
-                    contact_numbers=["+37112345432", "contactNumbers"],
-                    websites=["flagright.com", "websites"],
-                    addresses=[
-                        Address(
-                            address_lines=["Klara-Franke Str 20"],
-                            postcode="10557",
-                            city="Berlin",
-                            state="Berlin",
-                            country="Germany",
-                            tags=[
-                                Tag(
-                                    key="customKey",
-                                    value="customValue",
-                                ),
-                                Tag(
-                                    key="customKey",
-                                    value="customValue",
-                                ),
-                            ],
-                        ),
-                        Address(
-                            address_lines=["Klara-Franke Str 20"],
-                            postcode="10557",
-                            city="Berlin",
-                            state="Berlin",
-                            country="Germany",
-                            tags=[
-                                Tag(
-                                    key="customKey",
-                                    value="customValue",
-                                ),
-                                Tag(
-                                    key="customKey",
-                                    value="customValue",
-                                ),
-                            ],
-                        ),
-                    ],
+                destination_amount_details=TransactionAmountDetails(
+                    transaction_amount=68351.34,
+                    transaction_currency=CurrencyCode.INR,
+                    country=CountryCode.IN,
+                ),
+                promotion_code_used=True,
+                reference="loan repayment",
+                origin_device_data=DeviceData(
+                    battery_level=95.0,
+                    device_latitude=13.0033,
+                    device_longitude=76.1004,
+                    ip_address="10.23.191.2",
+                    device_identifier="3c49f915d04485e34caba",
+                    vpn_used=False,
+                    operating_system="Android 11.2",
+                    device_maker="ASUS",
+                    device_model="Zenphone M2 Pro Max",
+                    device_year="2018",
+                    app_version="1.1.0",
                 ),
-                transaction_limits=TransactionLimits(
-                    maximum_daily_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_weekly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_monthly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_quarterly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_yearly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
+                destination_device_data=DeviceData(
+                    battery_level=95.0,
+                    device_latitude=13.0033,
+                    device_longitude=76.1004,
+                    ip_address="10.23.191.2",
+                    device_identifier="3c49f915d04485e34caba",
+                    vpn_used=False,
+                    operating_system="Android 11.2",
+                    device_maker="ASUS",
+                    device_model="Zenphone M2 Pro Max",
+                    device_year="2018",
+                    app_version="1.1.0",
                 ),
                 tags=[
                     Tag(
                         key="customKey",
                         value="customValue",
-                    ),
-                    Tag(
-                        key="customKey",
-                        value="customValue",
-                    ),
+                    )
                 ],
-                user_id="96647cfd9e8fe66ee0f3362e011e34e8",
-                created_timestamp=1641654664000.0,
+                type=TransactionType.DEPOSIT,
+                transaction_id="7b80a539eea6e78acbd6d458e5971482",
+                timestamp=1641654664000.0,
+                origin_user_id="8650a2611d0771cba03310f74bf6",
+                destination_user_id="9350a2611e0771cba03310f74bf6",
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "consumer/users"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "transactions"),
+            params=remove_none_from_dict(
+                {
+                    "validateOriginUserId": validate_origin_user_id,
+                    "validateDestinationUserId": validate_destination_user_id,
+                }
+            ),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ConsumerUsersCreateResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TransactionsVerifyResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, user_id: str) -> UserWithRulesResult:
+    def get(self, transaction_id: str) -> TransactionWithRulesResult:
         """
-        ### GET Consumer User
+        ### GET Transactions
 
-        `/consumer/user` endpoint allows you to operate on the Consumer User entity.
+        `/transactions` endpoint allows you to operate on the [Transaction entity](/guides/overview/entities#transaction).
 
-        Calling `GET /consumer/user/{userId}` will return the entire user payload and rule execution results for the user with the corresponding `userId`
+        Calling `GET /transactions/{transactionId}` will return the entire transaction payload and rule execution results for the transaction with the corresponding `transactionId`
 
         Parameters:
-            - user_id: str.
+            - transaction_id: str. Unique Transaction Identifier
         ---
         from flagright.client import Flagright
 
         client = Flagright(
             api_key="YOUR_API_KEY",
         )
-        client.consumer_users.get(
-            user_id="userId",
+        client.transactions.get(
+            transaction_id="transactionId",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"consumer/users/{user_id}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"transactions/{transaction_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UserWithRulesResult, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TransactionWithRulesResult, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncConsumerUsersClient:
+class AsyncTransactionsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def create(self, *, request: User) -> ConsumerUsersCreateResponse:
+    async def verify(
+        self,
+        *,
+        validate_origin_user_id: typing.Optional[BooleanString] = None,
+        validate_destination_user_id: typing.Optional[BooleanString] = None,
+        request: Transaction,
+    ) -> TransactionsVerifyResponse:
         """
-        ## POST Consumer User
+        ## POST Transactions
 
-        `/consumer/user` endpoint allows you to operate on the Consumer user entity.
+        `/transactions` endpoint allows you to operate on the [Transaction entity.](/guides/overview/entities#transaction)
 
-        In order to pass the payload of a User to Flagright and verify the User, you will need to call this endpoint with the User payload. Not all fields are mandatory, you will only need to pass in the fields that you have and are relevant for your compliance setup.
+        In order to pass the payload of a transaction to Flagright and verify the transaction, you will need to call this endpoint with the transaction payload. Not all fields are mandatory, you will only need to pass in the fields that you have and are relevant for your compliance setup.
 
         ### Payload
 
-        Each consumer user needs two mandatory fields:
+        Here are some of the most used payload fields explained (you can find the full payload [schema below](/api-reference/api-reference/transactions/verify#request) with 1 line descriptions):
 
-        - `userId` - Unique identifier for the user
-        - `createdTimestamp` - UNIX timestamp in _milliseconds_ for when the User is created in your system
+        - `type`: Type of transaction (Ex: `WITHDRAWAL`, `DEPOSIT`, `TRANSFER` etc).
+        - `transactionId` - Unique Identifier for the transaction. Flagright API will generate a `transactionId` if this field is left empty
+        - `timestamp` - UNIX timestamp in _milliseconds_ of when the transaction took place
+        - `transactionState` - The state of the transaction, set to `CREATED` by default. [More details here](/guides/overview/entities#transaction-lifecycle-through-transaction-events)
+        - `originUserId` - Unique identifier (if any) of the user who is sending the money. This user must be created within the Flagright system before using the [create a consumer user](/api-reference/api-reference/consumer-users/create) or [create a business user](/api-reference/api-reference/business-users/create) endpoint
+        - `destinationUserId` - Unique identifier (if any) of the user who is receiving the money. This user must be created within the Flagright system before using the [create a consumer user](/api-reference/api-reference/consumer-users/create) or [create a business user](/api-reference/api-reference/business-users/create) endpoint
+        - `originAmountDetails` - Details of the amount being sent from the origin
+        - `destinationAmountDetails` - Details of the amount being received at the destination
+        - `originPaymentDetails` - Payment details (if any) used at the origin (ex: `CARD`, `IBAN`, `WALLET` etc). You can click on the dropdown next to the field in the schema below to view all supported payment types.
+        - `destinationPaymentDetails` - Payment details (if any) used at the destination (ex: `CARD`, `IBAN`, `WALLET` etc). You can click on the dropdown next to the field in the schema below to view all supported payment types.
 
         Parameters:
-            - request: User.
+            - validate_origin_user_id: typing.Optional[BooleanString]. Boolean string whether Flagright should validate if provided originUserId exist. True by default
+
+            - validate_destination_user_id: typing.Optional[BooleanString]. Boolean string whether Flagright should validate if provided destinationUserId exist. True by default
+
+            - request: Transaction.
         ---
         from flagright import (
-            Address,
-            Amount,
-            ConsumerName,
-            ContactDetails,
             CountryCode,
             CurrencyCode,
-            LegalDocument,
+            DeviceData,
             Tag,
-            TransactionLimits,
-            User,
-            UserDetails,
+            Transaction,
+            TransactionAmountDetails,
+            TransactionType,
         )
         from flagright.client import AsyncFlagright
 
         client = AsyncFlagright(
             api_key="YOUR_API_KEY",
         )
-        await client.consumer_users.create(
-            request=User(
-                user_details=UserDetails(
-                    name=ConsumerName(
-                        first_name="Baran",
-                        middle_name="Realblood",
-                        last_name="Ozkan",
-                    ),
-                    date_of_birth="1991-01-01",
-                    country_of_residence=CountryCode.US,
-                    country_of_nationality=CountryCode.DE,
+        await client.transactions.verify(
+            request=Transaction(
+                origin_amount_details=TransactionAmountDetails(
+                    transaction_amount=800.0,
+                    transaction_currency=CurrencyCode.EUR,
+                    country=CountryCode.DE,
                 ),
-                legal_documents=[
-                    LegalDocument(
-                        document_type="passport",
-                        document_number="Z9431P",
-                        document_issued_date=1639939034000.0,
-                        document_expiration_date=1839939034000.0,
-                        document_issued_country=CountryCode.DE,
-                        tags=[
-                            Tag(
-                                key="customerType",
-                                value="wallet",
-                            ),
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                        ],
-                        name_on_document=ConsumerName(
-                            first_name="Baran",
-                            middle_name="Realblood",
-                            last_name="Ozkan",
-                        ),
-                    ),
-                    LegalDocument(
-                        document_type="passport",
-                        document_number="Z9431P",
-                        document_issued_date=1639939034000.0,
-                        document_expiration_date=1839939034000.0,
-                        document_issued_country=CountryCode.DE,
-                        tags=[
-                            Tag(
-                                key="customerType",
-                                value="wallet",
-                            ),
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                        ],
-                        name_on_document=ConsumerName(
-                            first_name="Baran",
-                            middle_name="Realblood",
-                            last_name="Ozkan",
-                        ),
-                    ),
-                ],
-                contact_details=ContactDetails(
-                    email_ids=["baran@flagright.com", "emailIds"],
-                    contact_numbers=["+37112345432", "contactNumbers"],
-                    websites=["flagright.com", "websites"],
-                    addresses=[
-                        Address(
-                            address_lines=["Klara-Franke Str 20"],
-                            postcode="10557",
-                            city="Berlin",
-                            state="Berlin",
-                            country="Germany",
-                            tags=[
-                                Tag(
-                                    key="customKey",
-                                    value="customValue",
-                                ),
-                                Tag(
-                                    key="customKey",
-                                    value="customValue",
-                                ),
-                            ],
-                        ),
-                        Address(
-                            address_lines=["Klara-Franke Str 20"],
-                            postcode="10557",
-                            city="Berlin",
-                            state="Berlin",
-                            country="Germany",
-                            tags=[
-                                Tag(
-                                    key="customKey",
-                                    value="customValue",
-                                ),
-                                Tag(
-                                    key="customKey",
-                                    value="customValue",
-                                ),
-                            ],
-                        ),
-                    ],
+                destination_amount_details=TransactionAmountDetails(
+                    transaction_amount=68351.34,
+                    transaction_currency=CurrencyCode.INR,
+                    country=CountryCode.IN,
+                ),
+                promotion_code_used=True,
+                reference="loan repayment",
+                origin_device_data=DeviceData(
+                    battery_level=95.0,
+                    device_latitude=13.0033,
+                    device_longitude=76.1004,
+                    ip_address="10.23.191.2",
+                    device_identifier="3c49f915d04485e34caba",
+                    vpn_used=False,
+                    operating_system="Android 11.2",
+                    device_maker="ASUS",
+                    device_model="Zenphone M2 Pro Max",
+                    device_year="2018",
+                    app_version="1.1.0",
                 ),
-                transaction_limits=TransactionLimits(
-                    maximum_daily_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_weekly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_monthly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_quarterly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_yearly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
+                destination_device_data=DeviceData(
+                    battery_level=95.0,
+                    device_latitude=13.0033,
+                    device_longitude=76.1004,
+                    ip_address="10.23.191.2",
+                    device_identifier="3c49f915d04485e34caba",
+                    vpn_used=False,
+                    operating_system="Android 11.2",
+                    device_maker="ASUS",
+                    device_model="Zenphone M2 Pro Max",
+                    device_year="2018",
+                    app_version="1.1.0",
                 ),
                 tags=[
                     Tag(
                         key="customKey",
                         value="customValue",
-                    ),
-                    Tag(
-                        key="customKey",
-                        value="customValue",
-                    ),
+                    )
                 ],
-                user_id="96647cfd9e8fe66ee0f3362e011e34e8",
-                created_timestamp=1641654664000.0,
+                type=TransactionType.DEPOSIT,
+                transaction_id="7b80a539eea6e78acbd6d458e5971482",
+                timestamp=1641654664000.0,
+                origin_user_id="8650a2611d0771cba03310f74bf6",
+                destination_user_id="9350a2611e0771cba03310f74bf6",
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "consumer/users"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "transactions"),
+            params=remove_none_from_dict(
+                {
+                    "validateOriginUserId": validate_origin_user_id,
+                    "validateDestinationUserId": validate_destination_user_id,
+                }
+            ),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ConsumerUsersCreateResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TransactionsVerifyResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, user_id: str) -> UserWithRulesResult:
+    async def get(self, transaction_id: str) -> TransactionWithRulesResult:
         """
-        ### GET Consumer User
+        ### GET Transactions
 
-        `/consumer/user` endpoint allows you to operate on the Consumer User entity.
+        `/transactions` endpoint allows you to operate on the [Transaction entity](/guides/overview/entities#transaction).
 
-        Calling `GET /consumer/user/{userId}` will return the entire user payload and rule execution results for the user with the corresponding `userId`
+        Calling `GET /transactions/{transactionId}` will return the entire transaction payload and rule execution results for the transaction with the corresponding `transactionId`
 
         Parameters:
-            - user_id: str.
+            - transaction_id: str. Unique Transaction Identifier
         ---
         from flagright.client import AsyncFlagright
 
         client = AsyncFlagright(
             api_key="YOUR_API_KEY",
         )
-        await client.consumer_users.get(
-            user_id="userId",
+        await client.transactions.get(
+            transaction_id="transactionId",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"consumer/users/{user_id}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"transactions/{transaction_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UserWithRulesResult, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TransactionWithRulesResult, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
```

### Comparing `flagright-1.5.2/src/flagright/resources/consumer_users/types/consumer_users_create_response.py` & `flagright-1.5.3/src/flagright/resources/consumer_users/types/consumer_users_create_response.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/resources/transactions/types/transactions_verify_response.py` & `flagright-1.5.3/src/flagright/resources/transactions/types/transactions_verify_response.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/__init__.py` & `flagright-1.5.3/src/flagright/types/__init__.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/ach_details.py` & `flagright-1.5.3/src/flagright/types/ach_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/acquisition_channel.py` & `flagright-1.5.3/src/flagright/types/acquisition_channel.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/address.py` & `flagright-1.5.3/src/flagright/types/address.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/alert_closed_details.py` & `flagright-1.5.3/src/flagright/types/alert_closed_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/amount.py` & `flagright-1.5.3/src/flagright/types/amount.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/business.py` & `flagright-1.5.3/src/flagright/types/business.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/business_base.py` & `flagright-1.5.3/src/flagright/types/business_base.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/business_entity_link.py` & `flagright-1.5.3/src/flagright/types/business_entity_link.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/business_optional.py` & `flagright-1.5.3/src/flagright/types/business_optional.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/business_optional_saved_payment_details_item.py` & `flagright-1.5.3/src/flagright/types/business_optional_saved_payment_details_item.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/business_user_event.py` & `flagright-1.5.3/src/flagright/types/business_user_event.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/business_user_segment.py` & `flagright-1.5.3/src/flagright/types/business_user_segment.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/business_users_response.py` & `flagright-1.5.3/src/flagright/types/business_users_response.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/business_with_rules_result.py` & `flagright-1.5.3/src/flagright/types/business_with_rules_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/card_brand.py` & `flagright-1.5.3/src/flagright/types/card_brand.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/card_details.py` & `flagright-1.5.3/src/flagright/types/card_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/card_expiry.py` & `flagright-1.5.3/src/flagright/types/card_expiry.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/card_funding.py` & `flagright-1.5.3/src/flagright/types/card_funding.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/card_merchant_details.py` & `flagright-1.5.3/src/flagright/types/card_merchant_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/case_closed_details.py` & `flagright-1.5.3/src/flagright/types/case_closed_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/case_management_event.py` & `flagright-1.5.3/src/flagright/types/case_management_event.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/case_management_event_case_status.py` & `flagright-1.5.3/src/flagright/types/case_management_event_case_status.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/case_management_event_case_status_reason.py` & `flagright-1.5.3/src/flagright/types/case_management_event_case_status_reason.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/case_opened_details.py` & `flagright-1.5.3/src/flagright/types/case_opened_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/check_delivery_status.py` & `flagright-1.5.3/src/flagright/types/check_delivery_status.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/check_details.py` & `flagright-1.5.3/src/flagright/types/check_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/company_financial_details.py` & `flagright-1.5.3/src/flagright/types/company_financial_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/company_general_details.py` & `flagright-1.5.3/src/flagright/types/company_general_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/company_registration_details.py` & `flagright-1.5.3/src/flagright/types/company_registration_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/consumer_name.py` & `flagright-1.5.3/src/flagright/types/consumer_name.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/consumer_user_event.py` & `flagright-1.5.3/src/flagright/types/consumer_user_event.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/consumer_users_response.py` & `flagright-1.5.3/src/flagright/types/consumer_users_response.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/contact_details.py` & `flagright-1.5.3/src/flagright/types/contact_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/country_code.py` & `flagright-1.5.3/src/flagright/types/country_code.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/currency_code.py` & `flagright-1.5.3/src/flagright/types/currency_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -479,15 +479,15 @@
         afn: typing.Callable[[], T_Result],
         agld: typing.Callable[[], T_Result],
         aioz: typing.Callable[[], T_Result],
         alcx: typing.Callable[[], T_Result],
         aleph: typing.Callable[[], T_Result],
         algo: typing.Callable[[], T_Result],
         alice: typing.Callable[[], T_Result],
-        all: typing.Callable[[], T_Result],
+        all_: typing.Callable[[], T_Result],
         amd: typing.Callable[[], T_Result],
         amp: typing.Callable[[], T_Result],
         ang: typing.Callable[[], T_Result],
         ankr: typing.Callable[[], T_Result],
         ant: typing.Callable[[], T_Result],
         aoa: typing.Callable[[], T_Result],
         ape: typing.Callable[[], T_Result],
@@ -954,15 +954,15 @@
         if self is CurrencyCode.ALEPH:
             return aleph()
         if self is CurrencyCode.ALGO:
             return algo()
         if self is CurrencyCode.ALICE:
             return alice()
         if self is CurrencyCode.ALL:
-            return all()
+            return all_()
         if self is CurrencyCode.AMD:
             return amd()
         if self is CurrencyCode.AMP:
             return amp()
         if self is CurrencyCode.ANG:
             return ang()
         if self is CurrencyCode.ANKR:
```

### Comparing `flagright-1.5.2/src/flagright/types/date.py` & `flagright-1.5.3/src/flagright/types/date.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/device_data.py` & `flagright-1.5.3/src/flagright/types/device_data.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/employment_status.py` & `flagright-1.5.3/src/flagright/types/employment_status.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/executed_rules_result.py` & `flagright-1.5.3/src/flagright/types/executed_rules_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/failed_rules_result.py` & `flagright-1.5.3/src/flagright/types/failed_rules_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/false_positive_details.py` & `flagright-1.5.3/src/flagright/types/false_positive_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/gender.py` & `flagright-1.5.3/src/flagright/types/gender.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/generic_bank_account_details.py` & `flagright-1.5.3/src/flagright/types/generic_bank_account_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/hit_rules_details.py` & `flagright-1.5.3/src/flagright/types/hit_rules_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/iban_details.py` & `flagright-1.5.3/src/flagright/types/iban_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/kyc_status.py` & `flagright-1.5.3/src/flagright/types/kyc_status.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/kyc_status_details.py` & `flagright-1.5.3/src/flagright/types/kyc_status_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/legal_document.py` & `flagright-1.5.3/src/flagright/types/legal_document.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/legal_entity.py` & `flagright-1.5.3/src/flagright/types/legal_entity.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/list_data.py` & `flagright-1.5.3/src/flagright/types/list_data.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/list_existed.py` & `flagright-1.5.3/src/flagright/types/list_existed.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/list_header.py` & `flagright-1.5.3/src/flagright/types/list_header.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/list_item.py` & `flagright-1.5.3/src/flagright/types/list_item.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/list_metadata.py` & `flagright-1.5.3/src/flagright/types/list_metadata.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/list_subtype.py` & `flagright-1.5.3/src/flagright/types/list_subtype.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/list_type.py` & `flagright-1.5.3/src/flagright/types/list_type.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/mcc_details.py` & `flagright-1.5.3/src/flagright/types/mcc_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/mpesa_details.py` & `flagright-1.5.3/src/flagright/types/mpesa_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/mpesa_transaction_type.py` & `flagright-1.5.3/src/flagright/types/mpesa_transaction_type.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/payment_method.py` & `flagright-1.5.3/src/flagright/types/payment_method.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/pep_status.py` & `flagright-1.5.3/src/flagright/types/pep_status.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/person.py` & `flagright-1.5.3/src/flagright/types/person.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/risk_level.py` & `flagright-1.5.3/src/flagright/types/risk_level.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/rule_action.py` & `flagright-1.5.3/src/flagright/types/rule_action.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/rule_failure_exception.py` & `flagright-1.5.3/src/flagright/types/rule_failure_exception.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/rule_hit_meta.py` & `flagright-1.5.3/src/flagright/types/rule_hit_meta.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/rule_labels.py` & `flagright-1.5.3/src/flagright/types/rule_labels.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/rule_nature.py` & `flagright-1.5.3/src/flagright/types/rule_nature.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/rules_results.py` & `flagright-1.5.3/src/flagright/types/rules_results.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/sanctions_details.py` & `flagright-1.5.3/src/flagright/types/sanctions_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/sanctions_details_entity_type.py` & `flagright-1.5.3/src/flagright/types/sanctions_details_entity_type.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/source_of_funds.py` & `flagright-1.5.3/src/flagright/types/source_of_funds.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/swift_details.py` & `flagright-1.5.3/src/flagright/types/swift_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/tag.py` & `flagright-1.5.3/src/flagright/types/tag.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction.py` & `flagright-1.5.3/src/flagright/types/transaction.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_amount_details.py` & `flagright-1.5.3/src/flagright/types/transaction_amount_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_amount_limit.py` & `flagright-1.5.3/src/flagright/types/transaction_amount_limit.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_base.py` & `flagright-1.5.3/src/flagright/types/transaction_base.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_count_limit.py` & `flagright-1.5.3/src/flagright/types/transaction_count_limit.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_event.py` & `flagright-1.5.3/src/flagright/types/transaction_event.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_event_monitoring_result.py` & `flagright-1.5.3/src/flagright/types/transaction_event_monitoring_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_limit.py` & `flagright-1.5.3/src/flagright/types/transaction_limit.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_limits.py` & `flagright-1.5.3/src/flagright/types/transaction_limits.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_limits_payment_method_limits.py` & `flagright-1.5.3/src/flagright/types/transaction_limits_payment_method_limits.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_monitoring_result.py` & `flagright-1.5.3/src/flagright/types/transaction_monitoring_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_risk_scoring_result.py` & `flagright-1.5.3/src/flagright/types/transaction_risk_scoring_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_state.py` & `flagright-1.5.3/src/flagright/types/transaction_state.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_status_details.py` & `flagright-1.5.3/src/flagright/types/transaction_status_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_type.py` & `flagright-1.5.3/src/flagright/types/transaction_type.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_updatable.py` & `flagright-1.5.3/src/flagright/types/transaction_updatable.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_updatable_destination_payment_details.py` & `flagright-1.5.3/src/flagright/types/transaction_updatable_destination_payment_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_updatable_origin_payment_details.py` & `flagright-1.5.3/src/flagright/types/transaction_updatable_origin_payment_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/transaction_with_rules_result.py` & `flagright-1.5.3/src/flagright/types/transaction_with_rules_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/upi_details.py` & `flagright-1.5.3/src/flagright/types/upi_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/user.py` & `flagright-1.5.3/src/flagright/types/user.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/user_base.py` & `flagright-1.5.3/src/flagright/types/user_base.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/user_details.py` & `flagright-1.5.3/src/flagright/types/user_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/user_optional.py` & `flagright-1.5.3/src/flagright/types/user_optional.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/user_registration_status.py` & `flagright-1.5.3/src/flagright/types/user_registration_status.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/user_risk_score_details.py` & `flagright-1.5.3/src/flagright/types/user_risk_score_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/user_state.py` & `flagright-1.5.3/src/flagright/types/user_state.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/user_state_details.py` & `flagright-1.5.3/src/flagright/types/user_state_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/user_with_rules_result.py` & `flagright-1.5.3/src/flagright/types/user_with_rules_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/wallet_details.py` & `flagright-1.5.3/src/flagright/types/wallet_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/wallet_network.py` & `flagright-1.5.3/src/flagright/types/wallet_network.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/webhook_event.py` & `flagright-1.5.3/src/flagright/types/webhook_event.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/webhook_event_base.py` & `flagright-1.5.3/src/flagright/types/webhook_event_base.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/webhook_event_base_triggered_by.py` & `flagright-1.5.3/src/flagright/types/webhook_event_base_triggered_by.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/webhook_event_data.py` & `flagright-1.5.3/src/flagright/types/webhook_event_data.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/src/flagright/types/webhook_event_type.py` & `flagright-1.5.3/src/flagright/types/webhook_event_type.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.2/PKG-INFO` & `flagright-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flagright
-Version: 1.5.2
+Version: 1.5.3
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

