# Comparing `tmp/plaid-python-9.8.0.tar.gz` & `tmp/plaid-python-9.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plaid-python-9.8.0.tar", last modified: Wed Jul 20 16:52:21 2022, max compression
+gzip compressed data, was "dist/plaid-python-9.9.0.tar", last modified: Wed Aug  3 21:27:09 2022, max compression
```

## Comparing `plaid-python-9.8.0.tar` & `plaid-python-9.9.0.tar`

### file list

```diff
@@ -1,920 +1,937 @@
-drwxrwxr-x   0 jenkins   (2222) jenkins   (2222)        0 2022-07-20 16:52:21.000000 plaid-python-9.8.0/
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)      992 2022-07-20 16:52:12.000000 plaid-python-9.8.0/setup.py
-drwxrwxr-x   0 jenkins   (2222) jenkins   (2222)        0 2022-07-20 16:52:21.000000 plaid-python-9.8.0/tests/
-drwxrwxr-x   0 jenkins   (2222) jenkins   (2222)        0 2022-07-20 16:52:21.000000 plaid-python-9.8.0/tests/integration/
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6293 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_assets.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)      793 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_webhooks.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     2549 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_deposit_switch.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     5020 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_investment_transactions.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)      190 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_categories.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     5010 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_income_verification.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7754 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_item.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     2756 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_accounts.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     2365 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_auth.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)      820 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/util.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     3405 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_institutions.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     5331 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_payment_initiation.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     4739 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_transactions.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7500 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_bank_transfer.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     1353 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_processor.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     1499 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_identity.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)        0 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/__init__.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     4979 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_link_token.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     2001 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_liabilities.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     1548 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/integration/test_holdings.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)        0 2022-07-20 16:52:12.000000 plaid-python-9.8.0/tests/__init__.py
-drwxrwxr-x   0 jenkins   (2222) jenkins   (2222)        0 2022-07-20 16:52:21.000000 plaid-python-9.8.0/plaid/
-drwxrwxr-x   0 jenkins   (2222) jenkins   (2222)        0 2022-07-20 16:52:21.000000 plaid-python-9.8.0/plaid/apis/
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)      450 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/apis/__init__.py
-drwxrwxr-x   0 jenkins   (2222) jenkins   (2222)        0 2022-07-20 16:52:21.000000 plaid-python-9.8.0/plaid/model/
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    11813 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_transaction_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8158 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/pay_stub_deductions_total.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7572 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/deposit_switch_state_update_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7244 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_breakdown_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7130 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/employment_verification_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7362 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_account_subtypes.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6619 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/investment_holdings_get_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7788 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/physical_document_extracted_data_analysis.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    13213 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/mortgage_liability.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7010 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paystub_ytd_details.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7817 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_request_account_subtypes.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8970 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_optional_restriction_bacs.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7388 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_migrate_account_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7501 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_payroll_income_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7405 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_sweep.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6534 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_import_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7777 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/screening_hit_analysis.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7029 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_status_last_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9185 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/program_name_sensitivity.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6823 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/numbers_iban.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7880 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_address.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7001 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/pay_stub_taxpayer_id.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7686 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/employer.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6963 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_rule_field.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9005 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/employee_income_summary_field_string.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6896 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_transfer_repayment_simulate_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7121 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_consent_valid_date_time.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10198 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/error.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7082 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/address.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8097 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_initiated_risk_tier.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9178 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/watchlist_screening_hit.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7770 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_sweep_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6918 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_refresh_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7297 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_audit_copy_token_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7353 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_transaction_amount.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7104 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_payment_create_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8132 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_request_auth.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7220 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/get_identity_verification_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8181 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/w2_state_and_local_wages.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7864 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/product_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7779 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/image_quality.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9444 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_transaction.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8484 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_payroll_income_precheck_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7400 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/document_metadata.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7300 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/processor_stripe_bank_account_token_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7833 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_transaction_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7412 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_public_token_exchange_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7729 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/override_account_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7306 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/processor_bank_transfer_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7340 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_event_list_transfer_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7511 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_repayment.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7016 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/risk_signal_document_reference.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7396 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_authorization_decision_rationale.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7612 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7491 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/list_watchlist_screening_entity_history_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8263 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/create_individual_watchlist_screening_review_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7797 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/documentary_verification.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7378 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_event_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6862 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paystub_override_employee.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7327 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/phone_number.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7516 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payroll_income_account_data.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7774 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/auth_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9554 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_summary.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8448 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_verification_user_data.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7510 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_error_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7168 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_pay_stub_employer.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7748 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/standalone_investment_transaction_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7483 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/list_watchlist_screening_entity_hit_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7908 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7360 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/signal_person_name.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8722 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/watchlist_screening_individual_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10896 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/account_base.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6815 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/update_individual_screening_request_resettable_field.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6496 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_screening_hit_urls.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7269 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/institutions_get_by_id_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7398 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/depository_account_subtypes.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7411 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/issuing_country.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7215 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_failure.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7103 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_pay_frequency.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7189 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_public_token_exchange_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6898 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/signal_prepare_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7716 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_documents_download_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6936 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/physical_document_id_number.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8069 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_sweep_list_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7299 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/document_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7360 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_authorization_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7983 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/customer_initiated_risk_tier.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7388 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_warning.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7458 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/signal_scores.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8019 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paystub_details.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9020 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/numbers_international_nullable.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10146 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_event.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7627 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_audit_copy_token_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8926 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sender_bacs_nullable.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8327 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/historical_balance.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7307 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_repayment_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7091 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/list_dashboard_user_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7351 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/address_purpose_label.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8664 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_payment_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8293 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_recipient_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    12771 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/security.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7247 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_remove_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7251 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8391 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_watchlist_screening_search_terms.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7539 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_status_investments.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7051 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/depository_filter.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9011 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/projected_income_summary_field_number.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7867 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_removed_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8086 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/physical_document_images.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9247 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_watchlist_screening_hit.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7773 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paginated_individual_watchlist_program_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6702 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_oauth_select_accounts_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7725 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_create_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7231 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/processor_auth_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9005 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/employer_income_summary_field_string.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7267 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_sweep_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8018 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_sweep_list_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7913 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sync_updates_available_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7512 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/accounts_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7714 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_account_filters.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7198 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_transaction_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8423 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/products.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8249 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transaction_stream_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8404 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/pay_stub_deductions_breakdown.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8128 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_watchlist_screening.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7341 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/employers_search_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7712 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/address_data.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7807 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/loan_account_subtype.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7500 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_transaction_counterparty_numbers.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8092 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paystub_address.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7382 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7960 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_import_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    11363 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/external_payment_schedule_get.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7623 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_payment_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9009 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/ytd_gross_income_summary_field_number.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10276 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_request_income_verification.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7194 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_direction.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7067 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_payroll_flow_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8599 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_income_fire_webhook_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9895 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_request_user.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7883 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/student_loan_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6877 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_screening_hit_documents_items.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6975 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/generic_screening_hit_location_items.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7088 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/webhook_verification_key_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7039 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/institutions_search_payment_initiation_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7686 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/physical_document_extracted_data.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7170 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/account_filter.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7792 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7458 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payroll_income_object.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7295 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8073 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_transaction_idempotency_key.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6496 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_eu_config.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7856 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_consent_periodic_amount.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7573 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_verification_retry_request_steps_object.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7204 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_rule_details.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8669 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6910 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_refresh_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6982 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/customer_initiated_return_risk.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7807 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paginated_entity_watchlist_screening_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7296 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/individual_screening_hit_names.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7543 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/user_permission_revoked_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7405 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_repayment_return_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7912 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/auth_get_numbers.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8413 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/connected_application.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6842 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/document_risk_signal_institution_metadata.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7420 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/account_access.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7332 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/institutions_search_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7667 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/processor_balance_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7942 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_migrate_account_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7208 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_event_list_direction.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7214 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_payment_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6932 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_bank_transfer_fire_webhook_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6992 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/watchlist_screening_hit_locations.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7528 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/processor_auth_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6900 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_cancel_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6938 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/screening_hit_documents_items.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6861 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_refresh_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7167 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_consent_revoke_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7204 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_public_token_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8934 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_consent.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7171 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_profile_remove_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7617 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/pslf_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7398 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/investment_account_subtypes.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7346 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_application_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6924 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_transfer_fire_webhook_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7028 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_authorization_device.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7182 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_rules_list_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8108 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_transactions_list_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8329 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_event_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8332 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/liabilities_default_update_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8925 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/investments_transactions_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7184 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/numbers_international.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8181 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_screening_hit_analysis.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8932 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/recipient_bacs_nullable.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6912 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/signal_decision_report_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7299 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/update_individual_screening_request_search_terms.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8390 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/mfa.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8477 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/match_summary_code.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7629 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/pending_expiration_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8605 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/processor_token_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8932 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/institutions_search_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7247 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_sweep_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7367 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/signal_user.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9742 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_authorization_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7747 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_consent_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6719 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_get_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6485 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/cause_all_of.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8843 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/recaptcha_required_error.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7510 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_employment_item.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6516 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/accounts_get_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7239 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/processor_identity_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7185 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paystub_override_employee_address.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7962 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/deductions_total.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6627 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_recipient_get_response_all_of.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7582 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/accounts_balance_get_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7201 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_audit_copy_remove_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7710 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_user_in_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8086 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_payment_reverse_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9809 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_pay_stub.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8360 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/update_entity_screening_request_search_terms.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10092 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/numbers_ach_nullable.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9532 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/account_product_access_nullable.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7338 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_precheck_employer.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7748 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/client_provided_raw_transaction.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8092 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/watchlist_screening_individual.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6976 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_loan_filter.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9691 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9085 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_consent_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8953 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/distribution_breakdown.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7476 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/automatically_verified_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    16159 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_transaction.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7508 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_payroll_income_refresh_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6816 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/pay_stub_verification_attribute.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6937 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/source_uid.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8327 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_verification_step_summary.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8021 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/individual_watchlist_code.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8311 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/create_entity_watchlist_screening_review_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7058 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/watchlist_screening_audit_trail.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7233 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/webhook_verification_key_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7632 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_precheck_employer_address_data.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7696 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transaction_stream_amount.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7381 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_relay_refresh_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6490 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/removed_transaction.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7288 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7045 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/user_stated_income_source_pay_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7421 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/weak_alias_determination.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7712 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_payment_token_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8838 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_authorization_proposed_transfer.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9741 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/user_custom_password.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7480 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_verification_step_updated_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6860 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_match_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7587 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_filter_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8998 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/inflow_model.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7248 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/get_watchlist_screening_entity_program_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8355 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_authorization_guarantee_decision_rationale_code.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6932 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/watchlist_screening_individual_name.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7250 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/get_entity_watchlist_screening_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6541 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_maximum_payment_amount.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7582 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_refresh_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6912 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_transaction_counterparty_international.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8820 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_metadata.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7196 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_profile_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7133 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_audit_copy_remove_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9398 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/simulated_transfer_sweep.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9405 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/id_number_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7786 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paginated_entity_watchlist_program_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    16060 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/student_loan.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9589 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/doc_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8130 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/client_provided_enhanced_transaction.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8390 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/kyc_check_details.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6947 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/phone_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8195 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_authorization_decision.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7227 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7724 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_precheck_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7532 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/deposit_switch_address_data.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8197 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_verification_retry_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7606 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/employee.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9697 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7781 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_refund_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8382 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/investments_default_update_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7539 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/assets_error_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7865 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paginated_entity_watchlist_screening_hit_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7132 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/get_dashboard_user_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7085 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_network.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7304 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/assets_product_ready_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7422 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/processor_apex_processor_token_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7431 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_pay_stub_verification.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7574 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_payment_reverse_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7214 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    11339 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_consent_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7434 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_paystubs_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7306 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_transaction_counterparty.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7351 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/po_box_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10835 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/investment_transaction_subtype.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7937 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_watchlist_screening_review.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7591 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_payroll_income_risk_signals_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6916 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_precheck_military_info.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7625 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_refresh_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7291 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/document_name_match_code.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6717 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_request_update.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10894 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transaction_stream.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7271 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7454 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payroll_risk_signals_item.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6863 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/watchlist_screening_phone_number.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6977 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/dashboard_user_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6766 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_employer_verification.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7595 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_consent_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8786 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/address_nullable.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7972 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/watchlist_screening_search_terms.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7733 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_event_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7212 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_access_token_invalidate_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7283 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paystub_deduction.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7186 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/deposit_switch_create_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7397 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_user.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6791 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_account_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7806 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_match_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7841 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_warning_code.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7689 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_verification_step_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7133 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_audit_copy_token_remove_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7200 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/get_watchlist_screening_individual_program_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8153 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_document_metadata.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7253 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/application_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8478 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/investments_transactions_override.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    13193 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/deposit_switch_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7287 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_audit_copy_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7810 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/historical_update_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7580 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7863 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/deposit_switch_target_account.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8101 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/standalone_account_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7924 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/product_status_breakdown.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7103 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/source.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7014 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_screening_hit_phone_numbers.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7282 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7235 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_failure.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7574 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_event_sync_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9824 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_card_liability.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7135 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/signal_prepare_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7185 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_item_fire_webhook_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7967 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/watchlist_screening_hit_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7593 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_sweep.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7590 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/watchlist_screening_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7602 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_consent_payment_execute_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10179 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_status_update_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6734 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/employer_verification.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8045 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/verification_attribute.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7119 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_rule_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8250 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_status_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7001 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_recurring_get_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8083 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_rules_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6651 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/kyc_check_id_number_summary.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6991 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/signal_score.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7827 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/account_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7031 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_create_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8603 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/institution_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6920 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_income_fire_webhook_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    11524 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/account_subtype.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7569 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/accounts_balance_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7375 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/user_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7443 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/list_watchlist_screening_individual_reviews_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6926 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_bank_transfer_simulate_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8664 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_sync_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7430 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/processor_stripe_bank_account_token_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7319 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_intent_create_mode.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8256 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/institutions_get_by_id_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7812 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_repayment_return_list_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7685 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transaction_data.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7860 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/dashboard_user_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7565 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/signal_return_report_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7147 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_refresh_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7709 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/warning.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6598 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/liabilities_get_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7163 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/watchlist_screening_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7280 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_sweep_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8354 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_sync_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7521 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7210 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_summary_field_string.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7635 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/watchlist_screening_request_search_terms.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6937 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/screening_hit_names_items.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8957 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_transaction_counterparty_bacs.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7582 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_user_in_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7434 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/institutions_search_account_filter.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7595 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/investments_holdings_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7623 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paginated_dashboard_user_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8079 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_consent_constraints.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7102 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paystub_employer.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6918 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_rules_remove_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7354 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_rules_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7402 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/numbers_eft.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7644 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_processor_token_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8427 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/net_pay.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7307 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/account_subtypes.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7931 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_document_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6854 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_public_token_create_request_options_transactions.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7133 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_consent_periodic_alignment.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7250 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/processor_balance_get_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7125 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_application_list_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7950 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_migrate_account_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7525 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_product_ready_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6603 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_get_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7884 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_item_set_verification_status_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7067 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_update_types.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7201 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_audit_copy_token_remove_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7666 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7445 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_intent_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10309 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/holding.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6892 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_remove_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8232 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_intent_authorization_decision.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6820 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/user_name.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7192 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_audit_copy_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7776 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_pay_stub_employee.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8314 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_user.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9628 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_watchlist_program_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7114 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9820 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/application.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7539 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_watchlist_code.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7170 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/standalone_currency_code_list.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7100 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_request_identity_verification.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    30739 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/signal_evaluate_core_attributes.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7225 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/update_entity_screening_request_resettable_field_list.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7396 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_migrate_account_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7821 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/ach_class.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7479 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_refresh_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7501 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/signal_address_data.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9505 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/address_data_nullable.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7247 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_pdf_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9154 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/pay_stub_earnings_breakdown.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7058 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/client_user_id.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7313 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7641 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/student_repayment_plan.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8552 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/jwk_public_key.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7220 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7321 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_pay_stub_earnings.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7308 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_rules_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    11000 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/override_accounts.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7066 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_watchlist_screening_program_name.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8260 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/assets_relay_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9194 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_get_metadata_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7626 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paystub_override.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6992 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_credit_filter.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8819 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_transaction_execute_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7848 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_paystubs_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8293 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7615 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_pay_stub_address.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7633 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/multi_document_risk_signal.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7819 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payroll_item.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    19046 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transaction.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8392 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_pay_stub_net_pay.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7129 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_item_reset_login_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7487 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_verification_status_updated_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7712 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/account_filters_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7189 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_recipient_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7446 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8990 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_consent_periodic_amount_amount.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6936 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_transfer_repayment_simulate_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7785 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_public_token_create_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7989 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_watchlist_search_terms.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6933 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_screening_hit_emails_items.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6565 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_transaction_all_of.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6925 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_screening_hit_names_items.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7255 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/webhook_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7123 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7159 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_access_token_invalidate_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7941 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/consent_payment_idempotency_key.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7675 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/depository_account_subtype.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7165 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_recipient_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9141 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_authorization_decision_rationale_code.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8330 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_standing_order_metadata.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7470 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/verification_expired_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7267 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/taxpayer_id.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7311 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/pay_frequency.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10154 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paystub.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8206 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/institutions_search_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    19578 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8143 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_item.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9387 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/external_payment_schedule_base.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9264 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_get_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8583 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_meta.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9204 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_transaction.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7259 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/application_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6967 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_request_payment_initiation.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7223 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_numbers.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    13679 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/account_identity.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6912 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_profile_remove_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7310 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_event_sync_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9374 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/enhancements.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7378 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_event_sync_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7156 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/new_accounts_available_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7369 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_rules_remove_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8071 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/deposit_switch_target_user.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7996 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/list_entity_watchlist_screening_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7367 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/expiration_date.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7210 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/processor_token_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8329 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/deposit_switch_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8122 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_scheme.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7372 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/category.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7126 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_amount_currency.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7355 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_public_token_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7097 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6872 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_warning_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7214 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_consent_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8887 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_precheck_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7055 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/external_payment_refund_details.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7315 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_channel.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8589 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/owner.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7297 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/categories_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7672 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_taxforms_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8042 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_repayment_list_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6678 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/jwt_header.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9421 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transaction_all_of.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7504 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/institutions_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7236 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/deposit_switch_alt_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8372 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_public_token_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    12116 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8921 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_screening_hit_data.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7107 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_payroll_income_refresh_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6908 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/signal_return_report_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7162 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_employment_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7269 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/taxform.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7917 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7083 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_sweep_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7659 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_enhance_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8017 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_payment_list_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7702 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/liabilities_object.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7452 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_relay_refresh_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6565 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_metadata.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7368 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_screening_status_updated_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8548 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/watchlist_screening_review_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8758 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_watchlist_screening_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7214 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_summary_field_number.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7151 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_public_token_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8190 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_request_user_stated_income_source.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6989 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_schedule_interval.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6736 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/account_ids_with_updated_identity.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7274 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paystub_pay_frequency.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7003 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/loan_filter.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7435 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/incident_update.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7230 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/dashboard_user.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10608 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_verification.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7580 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_filter_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8754 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/update_entity_screening_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9907 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_intent_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10730 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7325 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_intent_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7644 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_balance_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10085 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/product_access.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7523 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/create_entity_screening_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8440 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/deposit_switch_alt_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7638 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/earnings_breakdown_canonical_description.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6520 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_request_transfer.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7349 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/screening_status_updated_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7521 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paystub_verification.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7051 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/investment_filter.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6972 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/watchlist_screening_document_value.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9332 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_status_nullable.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7929 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/verification_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7697 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_category_rule.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7271 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_account_subtype.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9098 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_verification_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7563 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_transaction_execute_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7699 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/initial_update_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10898 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7404 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_webhook_update_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7159 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/employment_verification_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7134 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/deposit_switch_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7646 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_verification_user_address.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7151 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_item_reset_login_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7234 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_sweep_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7151 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_cancel_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7200 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/scopes.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6573 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_metadata.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6730 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_verification_template_reference.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7154 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_import_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8265 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transaction_override.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6524 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_institution_data.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7194 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_relay_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8395 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_list_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9570 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_precheck_employer_address.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7268 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/processor_identity_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7075 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_sweep_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7473 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7242 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/processor_balance_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10708 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/processor_bank_transfer_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7034 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_balance.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7992 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_cause.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8987 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/numbers_bacs_nullable.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6872 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_profile_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6884 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/w2_box12.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6717 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/date_range.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6888 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_transfer_sweep_simulate_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7818 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paginated_individual_watchlist_screening_review_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6950 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_initiated_return_risk.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7082 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/mortgage_interest_rate.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7848 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/processor_number.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7973 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_profile_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7512 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6832 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/user_id_number.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10063 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/investment_account_subtype.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9216 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/pay_period_details.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7133 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/recipient_bacs.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8175 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_account.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9206 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_summary.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7675 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_create_idempotency_key.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7396 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_payroll_income_risk_signals_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6629 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/match_summary.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7416 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_intent_get_failure_reason.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8034 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/apr.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8314 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/institutions_get_by_id_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8266 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/investments_holdings_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7632 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/servicer_address_data.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7349 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/document_date_of_birth_match_code.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7442 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_recipient_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7227 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_amount.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7423 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/account_product_access.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7123 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7606 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/accounts_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7954 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/documentary_verification_document.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7702 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_match_user.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7922 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_item_fire_webhook_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7620 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/signal_evaluate_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7525 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_category.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7691 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/deposit_switch_token_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7015 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_network.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7145 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7194 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/numbers_international_iban.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9316 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transaction_code.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    11955 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/plaid_error.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7788 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_authorization_guarantee_decision.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8042 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/holdings_override.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6657 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/kyc_check_date_of_birth_summary.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7124 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7565 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_idempotency_key.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7530 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_audit_copy_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7844 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/user_address.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9189 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/numbers_eft_nullable.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7815 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_profile_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7024 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_investment_filter.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7555 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/security_override.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7151 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/user_stated_income_source_frequency.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7983 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/owner_override.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8067 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/investment_transaction_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6715 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_application_list_user_auth.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7257 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_request_income_verification_payroll_income.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7496 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/earnings.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6908 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_cancel_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7033 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfers_events_update_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8392 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/pay_stub_earnings_total.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7331 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_intent_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8981 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/institutions_get_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7349 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_pay_stub_deductions.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7543 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/document_analysis.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8610 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/earnings_total.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7683 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/account_selection_cardinality.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7951 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_transfer_simulate_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7093 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/meta.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7657 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/mortgage_property_address.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7233 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7262 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payroll_item_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7809 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/default_update_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7202 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/get_individual_watchlist_screening_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7088 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/employment_details.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    13362 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_intent_get.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8982 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_consent_max_payment_amount.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    13660 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_payment_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7435 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/list_watchlist_screening_individual_hit_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6930 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_request_income_verification_bank_income.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7314 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_employment_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7948 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/list_individual_watchlist_screening_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6758 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/account_filter_subtypes.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7825 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/liabilities_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8024 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_bank_transfer_simulate_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6982 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_screening_hits_phone_number_items.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6635 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_request_deposit_switch.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8182 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/deductions_breakdown.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8126 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_list_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10150 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_event_list_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8585 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/document_authenticity_match_code.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7268 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_relay_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    11233 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/account_balance.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7723 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/list_identity_verification_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7443 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/list_watchlist_screening_individual_history_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8521 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/location.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7913 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paginated_entity_watchlist_screening_review_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7304 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_transfer_sweep_simulate_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7202 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_enhance_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8254 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/signal_decision_report_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6514 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_match_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7570 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_breakdown.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8792 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_list_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7787 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/webhook_update_acknowledged_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    14522 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/liability_override.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7019 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_filter.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7883 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_recipient.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6741 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_import_request_user_auth.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8075 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_recurring_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8108 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_default_update_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8227 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/employment_verification.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9622 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_authorization.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7001 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_consent_periodic_interval.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8178 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/investments_transactions_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10795 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9005 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/ytd_net_income_summary_field_number.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7277 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/email.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7165 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_profile_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    11425 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7323 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_platform_ids.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6643 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/kyc_check_name_summary.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10293 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_recipient_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8717 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/physical_document_category.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8809 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/account_assets_all_of.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8498 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8334 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/numbers_iban_nullable.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6592 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_oauth_select_accounts_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7259 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/relay_event.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7582 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/total.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6873 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/review_comment.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7950 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/total_canonical_description.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7662 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_transactions_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7071 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)      348 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/__init__.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6929 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/pay.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8517 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/institutions_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8901 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/pay_stub_distribution_breakdown.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7795 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paginated_individual_watchlist_screening_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8295 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_verification_request_user.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7216 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_relay_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7174 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_webhook_update_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7915 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_relay_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7100 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_transfer_fire_webhook_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8418 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/numbers.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7261 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/update_individual_screening_request_resettable_field_list.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7344 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/loan_account_subtypes.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6926 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_application_scopes_update_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7957 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/screening_hit_data.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    11588 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_payment_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7108 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_bank_transfer_fire_webhook_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6916 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_watchlist_screening_name.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8797 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/strategy.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7103 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_cancel_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7038 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/wallet_iso_currency_code.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10360 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_intent_create.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9047 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/individual_watchlist_program.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10489 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_event_list_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    11733 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/w2.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7011 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_events_update_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7355 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_intent_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8481 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/external_payment_initiation_consent_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7230 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/deposit_switch_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7234 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/account_identity_all_of.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7040 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/generic_country_code.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8305 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/numbers_ach.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7129 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/list_watchlist_screening_entity_programs_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8044 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/document_risk_signals_object.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7671 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_user_address_in_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7007 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_document.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7536 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/liabilities_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    11141 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/investment_transaction.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    10445 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/institution.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6722 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_webhook_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9677 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/individual_watchlist_program_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7129 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_remove_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7798 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_sync_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6595 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/auth_get_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7491 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/list_watchlist_screening_entity_reviews_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7727 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paginated_identity_verification_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    11254 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_payment.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    15247 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/account_assets.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7171 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_refresh_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7099 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_payroll_income_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7207 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/kyc_check_address_summary.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8923 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_verification_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7107 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/personal_finance_category.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7297 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/user_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7150 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/deposit_switch_token_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7281 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/scopes_context.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7529 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/single_document_risk_signal.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7395 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/student_loan_repayment_model.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8287 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9477 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/watchlist_screening_document_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8690 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/external_payment_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8004 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_relay_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    13887 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transaction_base.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7125 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/country_code.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8120 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/holdings_default_update_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7278 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7431 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_payroll_income_precheck_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6533 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_screening_hit_emails.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6645 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/kyc_check_phone_summary.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7926 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_consent_payment_execute_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6936 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_item_set_verification_status_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7371 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_consent_scope.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8384 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_application_scopes_update_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6917 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_screening_hit_urls_items.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7283 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/employers_search_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7392 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paystub_verification_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    11238 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_verification_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6985 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_source_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6918 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_transfer_simulate_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7918 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/watchlist_screening_review.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7608 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/deductions.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8485 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6894 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_consent_revoke_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7478 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_user_address_in_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7366 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_event_list_bank_transfer_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8754 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/update_individual_screening_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7947 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_recurring_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6768 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/signal_device.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    12321 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/cause.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8771 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_historical_summary.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    11303 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/external_payment_schedule_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7135 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/pay_frequency_value.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7524 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7218 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/platform_ids.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7098 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/individual_watchlist_screening_program_name.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7045 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_processor_token_create_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7480 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/auth_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8140 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_item.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7310 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_event_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7209 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/investments_transactions_get_request_options.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7598 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_repayment_return.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6996 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payroll_income_rate_of_pay.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8110 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_refresh_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7137 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/list_watchlist_screening_individual_programs_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6555 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/liabilities_account_ids_with_updated_liabilities.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7104 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/watchlist_screening_document.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8074 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transactions_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7397 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/employment_verification_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9371 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_employment_verification.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    13436 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_w2.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8567 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_watchlist_screening_review_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6892 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_recipient_list_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9885 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/pay_stub_pay_period_details.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7595 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/user_stated_income_source_category.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8525 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_error_type.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9195 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/scopes_nullable.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9411 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/credit_bank_income_source.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7263 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_screening_hit_names.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6874 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_verification_user_phone_number.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7132 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_relay_remove_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7230 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_payment_token_create_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7019 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/auth_metadata.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9861 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_event.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7561 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_event_sync_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6451 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paystub_override_employer.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7381 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/auth_supported_methods.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8809 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/document_risk_signal.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7442 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/transfer_authorization_guarantee_decision_rationale.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7167 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_relay_remove_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7926 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/verification_refresh_status.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8175 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/recurring_transaction_frequency.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7264 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_precheck_user.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7468 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/identity_verification_retried_webhook.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7210 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/sandbox_processor_token_create_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6653 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_override.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     8998 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/entity_watchlist_program.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7787 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_precheck_confidence.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7389 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_refresh_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7196 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/numbers_bacs.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7853 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/income_verification_taxforms_get_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7773 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/health_incident.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6807 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/update_entity_screening_request_resettable_field.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7245 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_balance_get_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7117 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/asset_report_remove_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9627 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/signal_evaluate_request.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6837 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/screening_hit_date_of_birth_item.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7543 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/item_status_transactions.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7812 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/payment_initiation_payment_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     9120 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/earnings_breakdown.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     6964 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/report_token.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7791 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/paginated_individual_watchlist_screening_hit_list_response.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7024 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/link_token_create_depository_filter.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     7220 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model/bank_transfer_balance.py
-drwxrwxr-x   0 jenkins   (2222) jenkins   (2222)        0 2022-07-20 16:52:21.000000 plaid-python-9.8.0/plaid/api/
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)   850474 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/api/plaid_api.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)      207 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/api/__init__.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    17962 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/configuration.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)     5015 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/exceptions.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    12439 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/rest.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    72852 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/model_utils.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)      687 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/__init__.py
-drwxrwxr-x   0 jenkins   (2222) jenkins   (2222)        0 2022-07-20 16:52:21.000000 plaid-python-9.8.0/plaid/models/
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    69269 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/models/__init__.py
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    36733 2022-07-20 16:52:12.000000 plaid-python-9.8.0/plaid/api_client.py
-drwxrwxr-x   0 jenkins   (2222) jenkins   (2222)        0 2022-07-20 16:52:21.000000 plaid-python-9.8.0/plaid_python.egg-info/
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)       12 2022-07-20 16:52:21.000000 plaid-python-9.8.0/plaid_python.egg-info/top_level.txt
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)    39476 2022-07-20 16:52:21.000000 plaid-python-9.8.0/plaid_python.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)       41 2022-07-20 16:52:21.000000 plaid-python-9.8.0/plaid_python.egg-info/requires.txt
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)      638 2022-07-20 16:52:21.000000 plaid-python-9.8.0/plaid_python.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)        1 2022-07-20 16:52:21.000000 plaid-python-9.8.0/plaid_python.egg-info/not-zip-safe
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)        1 2022-07-20 16:52:21.000000 plaid-python-9.8.0/plaid_python.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)      638 2022-07-20 16:52:21.000000 plaid-python-9.8.0/PKG-INFO
--rw-rw-r--   0 jenkins   (2222) jenkins   (2222)       38 2022-07-20 16:52:21.000000 plaid-python-9.8.0/setup.cfg
+drwxrwxr-x   0 jenkins   (2166) jenkins   (2166)        0 2022-08-03 21:27:09.000000 plaid-python-9.9.0/
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)      992 2022-08-03 21:26:51.000000 plaid-python-9.9.0/setup.py
+drwxrwxr-x   0 jenkins   (2166) jenkins   (2166)        0 2022-08-03 21:27:09.000000 plaid-python-9.9.0/tests/
+drwxrwxr-x   0 jenkins   (2166) jenkins   (2166)        0 2022-08-03 21:27:09.000000 plaid-python-9.9.0/tests/integration/
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6293 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_assets.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)      793 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_webhooks.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     2549 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_deposit_switch.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     5020 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_investment_transactions.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)      190 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_categories.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     5010 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_income_verification.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7749 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_item.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     2756 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_accounts.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     2365 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_auth.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)      820 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/util.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     3405 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_institutions.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     5331 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_payment_initiation.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     4739 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_transactions.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7500 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_bank_transfer.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     1353 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_processor.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     1499 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_identity.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)        0 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/__init__.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     4979 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_link_token.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     2001 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_liabilities.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     1548 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/integration/test_holdings.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)        0 2022-08-03 21:26:51.000000 plaid-python-9.9.0/tests/__init__.py
+drwxrwxr-x   0 jenkins   (2166) jenkins   (2166)        0 2022-08-03 21:27:09.000000 plaid-python-9.9.0/plaid/
+drwxrwxr-x   0 jenkins   (2166) jenkins   (2166)        0 2022-08-03 21:27:09.000000 plaid-python-9.9.0/plaid/apis/
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)      450 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/apis/__init__.py
+drwxrwxr-x   0 jenkins   (2166) jenkins   (2166)        0 2022-08-03 21:27:09.000000 plaid-python-9.9.0/plaid/model/
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    11813 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_transaction_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8158 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/pay_stub_deductions_total.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7572 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/deposit_switch_state_update_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7244 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_breakdown_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7130 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/employment_verification_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7362 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_account_subtypes.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6619 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/investment_holdings_get_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7788 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/physical_document_extracted_data_analysis.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    13213 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/mortgage_liability.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7010 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paystub_ytd_details.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7817 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_request_account_subtypes.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8970 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_optional_restriction_bacs.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7388 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_migrate_account_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7501 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_payroll_income_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7405 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_sweep.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6534 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_import_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7777 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/screening_hit_analysis.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7029 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_status_last_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9185 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/program_name_sensitivity.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6823 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/numbers_iban.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7880 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_address.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7001 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/pay_stub_taxpayer_id.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7686 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/employer.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6963 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_rule_field.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9005 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/employee_income_summary_field_string.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6896 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_transfer_repayment_simulate_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7121 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_consent_valid_date_time.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10198 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/error.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7082 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/address.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8097 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_initiated_risk_tier.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9178 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/watchlist_screening_hit.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7770 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_sweep_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6918 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_refresh_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7297 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_audit_copy_token_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7353 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_transaction_amount.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7104 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_payment_create_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8132 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_request_auth.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7220 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/get_identity_verification_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8181 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/w2_state_and_local_wages.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7864 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/product_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7779 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/image_quality.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9444 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_transaction.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8484 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_payroll_income_precheck_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7400 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/document_metadata.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7300 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/processor_stripe_bank_account_token_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7833 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_transaction_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7412 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_public_token_exchange_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7729 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/override_account_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7306 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/processor_bank_transfer_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7137 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_pdf_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7340 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_event_list_transfer_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7511 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_repayment.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7016 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/risk_signal_document_reference.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7396 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_authorization_decision_rationale.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7612 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7491 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/list_watchlist_screening_entity_history_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8263 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/create_individual_watchlist_screening_review_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7797 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/documentary_verification.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7378 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_event_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6862 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paystub_override_employee.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7327 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/phone_number.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7516 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payroll_income_account_data.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7774 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/auth_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9554 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_summary.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8448 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_verification_user_data.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7510 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_error_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7168 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_pay_stub_employer.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7748 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/standalone_investment_transaction_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7483 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/list_watchlist_screening_entity_hit_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7908 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7360 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/signal_person_name.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8722 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/watchlist_screening_individual_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10896 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/account_base.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6815 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/update_individual_screening_request_resettable_field.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6496 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_screening_hit_urls.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7269 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/institutions_get_by_id_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7398 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/depository_account_subtypes.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7411 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/issuing_country.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7215 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_failure.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7103 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_pay_frequency.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7189 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_public_token_exchange_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6898 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/signal_prepare_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7716 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_documents_download_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6936 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/physical_document_id_number.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8069 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_sweep_list_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7299 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/document_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7360 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_authorization_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7983 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/customer_initiated_risk_tier.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7388 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_warning.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7458 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/signal_scores.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8019 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paystub_details.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9020 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/numbers_international_nullable.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10146 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_event.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7627 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_audit_copy_token_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8926 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sender_bacs_nullable.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8327 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/historical_balance.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7307 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_repayment_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7091 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/list_dashboard_user_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7351 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/address_purpose_label.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8664 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_payment_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8293 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_recipient_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    12771 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/security.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7247 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_remove_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7251 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8391 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_watchlist_screening_search_terms.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7539 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_status_investments.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7051 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/depository_filter.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9011 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/projected_income_summary_field_number.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7867 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_removed_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8086 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/physical_document_images.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9247 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_watchlist_screening_hit.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7773 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paginated_individual_watchlist_program_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6702 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_oauth_select_accounts_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7725 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_create_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7231 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/processor_auth_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9005 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/employer_income_summary_field_string.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6917 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/report_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7267 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_sweep_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8018 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_sweep_list_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7913 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sync_updates_available_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7512 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/accounts_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7714 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_account_filters.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7016 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/form1099_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7198 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_transaction_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8423 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/products.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8249 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transaction_stream_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8404 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/pay_stub_deductions_breakdown.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8128 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_watchlist_screening.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7545 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/recurring_transactions_update_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7341 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/employers_search_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    20161 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit1099.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8027 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit1099_recipient.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7712 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/address_data.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7807 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/loan_account_subtype.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7500 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_transaction_counterparty_numbers.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8092 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paystub_address.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7382 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7960 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_import_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    11363 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/external_payment_schedule_get.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7623 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_payment_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9009 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/ytd_gross_income_summary_field_number.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10276 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_request_income_verification.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7194 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_direction.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7067 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_payroll_flow_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8599 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_income_fire_webhook_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10628 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_request_user.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7462 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_relay_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7883 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/student_loan_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6877 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_screening_hit_documents_items.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7476 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/partner_customers_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6975 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/generic_screening_hit_location_items.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7088 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/webhook_verification_key_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7039 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/institutions_search_payment_initiation_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7686 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/physical_document_extracted_data.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7170 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/account_filter.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7792 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7762 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payroll_income_object.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7295 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8073 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_transaction_idempotency_key.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6496 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_eu_config.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7856 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_consent_periodic_amount.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7573 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_verification_retry_request_steps_object.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7204 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_rule_details.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8669 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6910 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_refresh_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6982 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/customer_initiated_return_risk.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7807 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paginated_entity_watchlist_screening_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7296 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/individual_screening_hit_names.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7543 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/user_permission_revoked_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7405 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_repayment_return_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7912 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/auth_get_numbers.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8413 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/connected_application.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6842 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/document_risk_signal_institution_metadata.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7420 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/account_access.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7332 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/institutions_search_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7667 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/processor_balance_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7942 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_migrate_account_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7208 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_event_list_direction.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7214 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_payment_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6932 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_bank_transfer_fire_webhook_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6992 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/watchlist_screening_hit_locations.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7528 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/processor_auth_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6900 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_cancel_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6938 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/screening_hit_documents_items.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6861 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_refresh_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7167 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_consent_revoke_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7204 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_public_token_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8934 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_consent.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7171 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_profile_remove_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7617 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/pslf_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7398 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/investment_account_subtypes.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7346 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_application_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6924 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_transfer_fire_webhook_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7106 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_authorization_device.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7182 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_rules_list_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8108 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_transactions_list_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8269 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_event_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8332 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/liabilities_default_update_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8925 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/investments_transactions_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7184 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/numbers_international.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8181 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_screening_hit_analysis.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8932 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/recipient_bacs_nullable.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6912 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/signal_decision_report_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7299 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/update_individual_screening_request_search_terms.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8390 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/mfa.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8477 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/match_summary_code.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7629 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/pending_expiration_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8605 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/processor_token_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8932 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/institutions_search_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7247 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_sweep_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7367 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/signal_user.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10467 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_authorization_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7747 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_consent_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6719 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_get_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6485 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/cause_all_of.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8843 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/recaptcha_required_error.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7510 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_employment_item.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6516 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/accounts_get_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7239 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/processor_identity_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7185 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paystub_override_employee_address.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7962 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/deductions_total.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6627 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_recipient_get_response_all_of.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7582 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/accounts_balance_get_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7201 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_audit_copy_remove_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7710 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_user_in_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8086 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_payment_reverse_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9809 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_pay_stub.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8360 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/update_entity_screening_request_search_terms.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10092 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/numbers_ach_nullable.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9532 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/account_product_access_nullable.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7338 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_precheck_employer.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7748 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/client_provided_raw_transaction.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8092 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/watchlist_screening_individual.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6976 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_loan_filter.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9691 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9085 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_consent_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8953 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/distribution_breakdown.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7476 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/automatically_verified_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    16159 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_transaction.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7508 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_payroll_income_refresh_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6816 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/pay_stub_verification_attribute.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6937 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/source_uid.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8327 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_verification_step_summary.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8021 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/individual_watchlist_code.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8311 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/create_entity_watchlist_screening_review_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7058 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/watchlist_screening_audit_trail.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7233 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/webhook_verification_key_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7632 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_precheck_employer_address_data.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7696 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transaction_stream_amount.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7381 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_relay_refresh_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6490 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/removed_transaction.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7288 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7045 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/user_stated_income_source_pay_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7421 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/weak_alias_determination.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7712 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_payment_token_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8838 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_authorization_proposed_transfer.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9741 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/user_custom_password.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7480 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_verification_step_updated_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6860 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_match_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6753 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/partner_end_customer_client.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7587 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_filter_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8998 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/inflow_model.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7248 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/get_watchlist_screening_entity_program_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8583 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_authorization_guarantee_decision_rationale_code.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6932 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/watchlist_screening_individual_name.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7250 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/get_entity_watchlist_screening_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6541 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_maximum_payment_amount.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7582 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_refresh_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6912 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_transaction_counterparty_international.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8820 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_metadata.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7196 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_profile_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7133 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_audit_copy_remove_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9398 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/simulated_transfer_sweep.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9405 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/id_number_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7786 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paginated_entity_watchlist_program_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    16060 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/student_loan.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9725 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/doc_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8130 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/client_provided_enhanced_transaction.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8390 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/kyc_check_details.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6947 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/phone_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8195 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_authorization_decision.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7227 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7724 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_precheck_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7532 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/deposit_switch_address_data.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8197 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_verification_retry_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7606 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/employee.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9697 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7781 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_refund_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8382 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/investments_default_update_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7539 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/assets_error_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7865 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paginated_entity_watchlist_screening_hit_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7132 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/get_dashboard_user_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7085 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_network.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7304 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/assets_product_ready_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7422 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/processor_apex_processor_token_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7431 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_pay_stub_verification.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7574 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_payment_reverse_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7214 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    11339 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_consent_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7434 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_paystubs_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7306 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_transaction_counterparty.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7351 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/po_box_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10835 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/investment_transaction_subtype.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7937 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_watchlist_screening_review.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7591 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_payroll_income_risk_signals_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6916 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_precheck_military_info.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7625 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_refresh_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7291 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/document_name_match_code.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6717 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_request_update.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10894 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transaction_stream.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7271 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7454 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payroll_risk_signals_item.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6863 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/watchlist_screening_phone_number.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6977 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/dashboard_user_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6766 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_employer_verification.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7595 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_consent_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8786 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/address_nullable.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7972 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/watchlist_screening_search_terms.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7733 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_event_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7212 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_access_token_invalidate_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7283 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paystub_deduction.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7186 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/deposit_switch_create_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7397 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_user.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6791 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_account_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7806 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_match_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7841 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_warning_code.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7689 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_verification_step_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7109 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_relay_remove_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7133 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_audit_copy_token_remove_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7200 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/get_watchlist_screening_individual_program_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8153 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_document_metadata.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7253 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/application_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8478 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/investments_transactions_override.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    13193 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/deposit_switch_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7287 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_audit_copy_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7810 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/historical_update_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7580 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7863 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/deposit_switch_target_account.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8101 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/standalone_account_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7924 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/product_status_breakdown.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7103 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/source.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7362 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_relay_refresh_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7014 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_screening_hit_phone_numbers.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7282 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7235 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_failure.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7574 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_event_sync_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9824 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_card_liability.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7135 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/signal_prepare_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7185 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_item_fire_webhook_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7967 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/watchlist_screening_hit_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7593 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_sweep.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7590 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/watchlist_screening_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7602 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_consent_payment_execute_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10179 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_status_update_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6734 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/employer_verification.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8045 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/verification_attribute.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7119 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_rule_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8250 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_status_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7001 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_recurring_get_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8083 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_rules_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6651 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/kyc_check_id_number_summary.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6991 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/signal_score.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7827 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/account_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7031 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_create_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8603 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/institution_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7838 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_authorization_user_in_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6920 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_income_fire_webhook_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    11524 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/account_subtype.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7569 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/accounts_balance_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7375 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/user_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7443 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/list_watchlist_screening_individual_reviews_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6926 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_bank_transfer_simulate_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8664 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_sync_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7430 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/processor_stripe_bank_account_token_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7319 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_intent_create_mode.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8256 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/institutions_get_by_id_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7812 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_repayment_return_list_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7685 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transaction_data.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7860 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/dashboard_user_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7565 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/signal_return_report_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7147 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_refresh_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7709 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/warning.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6598 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/liabilities_get_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7163 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/watchlist_screening_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7280 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_sweep_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8354 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_sync_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7521 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7210 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_summary_field_string.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8157 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/partner_customers_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7635 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/watchlist_screening_request_search_terms.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6937 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/screening_hit_names_items.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8957 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_transaction_counterparty_bacs.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7582 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_user_in_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7434 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/institutions_search_account_filter.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7595 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/investments_holdings_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7623 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paginated_dashboard_user_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8079 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_consent_constraints.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7102 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paystub_employer.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6918 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_rules_remove_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7354 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_rules_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7402 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/numbers_eft.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7644 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_processor_token_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8427 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/net_pay.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7307 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/account_subtypes.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7931 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_document_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6854 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_public_token_create_request_options_transactions.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7133 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_consent_periodic_alignment.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7250 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/processor_balance_get_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7125 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_application_list_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7950 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_migrate_account_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7525 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_product_ready_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6603 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_get_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7884 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_item_set_verification_status_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7067 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_update_types.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7201 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_audit_copy_token_remove_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7666 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7445 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_intent_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10309 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/holding.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6892 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_remove_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8232 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_intent_authorization_decision.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6820 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/user_name.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7192 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_audit_copy_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7776 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_pay_stub_employee.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8314 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_user.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9628 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_watchlist_program_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7114 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9820 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/application.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7539 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_watchlist_code.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7170 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/standalone_currency_code_list.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7267 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_request_identity_verification.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    30739 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/signal_evaluate_core_attributes.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7225 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/update_entity_screening_request_resettable_field_list.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7396 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_migrate_account_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7821 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/ach_class.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7479 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_refresh_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7501 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/signal_address_data.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9505 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/address_data_nullable.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7247 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_pdf_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9154 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/pay_stub_earnings_breakdown.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7058 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/client_user_id.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7313 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7641 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/student_repayment_plan.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8552 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/jwk_public_key.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7220 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7321 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_pay_stub_earnings.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7308 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_rules_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    11000 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/override_accounts.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7066 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_watchlist_screening_program_name.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8260 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/assets_relay_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9194 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_get_metadata_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7626 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paystub_override.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6992 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_credit_filter.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8819 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_transaction_execute_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7848 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_paystubs_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8293 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7615 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_pay_stub_address.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7633 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/multi_document_risk_signal.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7819 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payroll_item.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    19046 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transaction.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8392 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_pay_stub_net_pay.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7129 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_item_reset_login_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7487 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_verification_status_updated_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7712 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/account_filters_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7189 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_recipient_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7446 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8990 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_consent_periodic_amount_amount.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6936 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_transfer_repayment_simulate_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7785 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_public_token_create_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7989 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_watchlist_search_terms.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6933 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_screening_hit_emails_items.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6565 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_transaction_all_of.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6925 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_screening_hit_names_items.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7255 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/webhook_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7063 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7159 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_access_token_invalidate_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7941 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/consent_payment_idempotency_key.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7675 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/depository_account_subtype.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7165 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_recipient_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9141 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_authorization_decision_rationale_code.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8330 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_standing_order_metadata.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7470 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/verification_expired_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7267 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/taxpayer_id.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7311 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/pay_frequency.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10154 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paystub.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8206 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/institutions_search_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    19578 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8143 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_item.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9387 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/external_payment_schedule_base.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9264 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_get_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8583 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_meta.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9204 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_transaction.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7259 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/application_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6967 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_request_payment_initiation.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7223 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_numbers.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    13679 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/account_identity.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6912 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_profile_remove_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7310 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_event_sync_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9742 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/enhancements.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7378 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_event_sync_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7156 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/new_accounts_available_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7369 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_rules_remove_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8071 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/deposit_switch_target_user.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7996 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/list_entity_watchlist_screening_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7367 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/expiration_date.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7210 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/processor_token_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8329 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/deposit_switch_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8122 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_scheme.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7372 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/category.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7126 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_amount_currency.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7355 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_public_token_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7097 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6872 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_warning_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7214 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_consent_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8887 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_precheck_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7055 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/external_payment_refund_details.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7315 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_channel.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8589 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/owner.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7297 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/categories_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7672 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_taxforms_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8042 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_repayment_list_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6678 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/jwt_header.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9421 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transaction_all_of.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7504 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/institutions_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7236 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/deposit_switch_alt_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8372 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_public_token_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    12116 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8921 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_screening_hit_data.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7107 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_payroll_income_refresh_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6908 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/signal_return_report_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7162 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_employment_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7269 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/taxform.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7917 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7083 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_sweep_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7659 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_enhance_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8017 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_payment_list_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7702 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/liabilities_object.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7452 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_relay_refresh_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6565 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_metadata.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7368 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_screening_status_updated_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8548 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/watchlist_screening_review_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8758 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_watchlist_screening_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7214 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_summary_field_number.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7151 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_public_token_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8190 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_request_user_stated_income_source.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6989 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_schedule_interval.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6736 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/account_ids_with_updated_identity.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7274 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paystub_pay_frequency.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7003 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/loan_filter.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7435 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/incident_update.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7230 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/dashboard_user.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10608 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_verification.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7580 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_filter_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8754 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/update_entity_screening_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9907 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_intent_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10761 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7325 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_intent_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7644 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_balance_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10085 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/product_access.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7523 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/create_entity_screening_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8440 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/deposit_switch_alt_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7638 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/earnings_breakdown_canonical_description.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6783 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_request_transfer.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7349 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/screening_status_updated_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7521 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paystub_verification.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7051 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/investment_filter.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6972 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/watchlist_screening_document_value.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9332 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_status_nullable.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7929 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/verification_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7697 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_category_rule.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7505 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit1099_payer.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7271 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_account_subtype.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9098 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_verification_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7563 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_transaction_execute_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7699 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/initial_update_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10898 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7404 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_webhook_update_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7159 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/employment_verification_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7134 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/deposit_switch_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7646 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_verification_user_address.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7151 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_item_reset_login_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7234 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_sweep_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7151 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_cancel_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7200 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/scopes.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6573 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_metadata.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6730 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_verification_template_reference.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7154 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_import_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8265 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transaction_override.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6524 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_institution_data.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7194 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_relay_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8395 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_list_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9570 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_precheck_employer_address.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7268 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/processor_identity_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7075 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_sweep_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7473 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7242 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/processor_balance_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10708 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/processor_bank_transfer_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7034 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_balance.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7992 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_cause.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8987 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/numbers_bacs_nullable.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6872 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_profile_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6884 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/w2_box12.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6717 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/date_range.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6888 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_transfer_sweep_simulate_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7818 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paginated_individual_watchlist_screening_review_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6950 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_initiated_return_risk.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7082 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/mortgage_interest_rate.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7848 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/processor_number.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7973 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_profile_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7512 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6832 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/user_id_number.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10063 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/investment_account_subtype.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9216 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/pay_period_details.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7133 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/recipient_bacs.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8175 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_account.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9206 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_summary.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7675 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_create_idempotency_key.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7396 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_payroll_income_risk_signals_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6629 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/match_summary.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7416 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_intent_get_failure_reason.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8034 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/apr.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8314 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/institutions_get_by_id_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8266 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/investments_holdings_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7632 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/servicer_address_data.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7349 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/document_date_of_birth_match_code.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7442 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_recipient_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7227 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_amount.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7423 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/account_product_access.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7123 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7606 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/accounts_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7954 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/documentary_verification_document.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7702 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_match_user.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7565 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit1099_filer.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8000 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_item_fire_webhook_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7620 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/signal_evaluate_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7525 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_category.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7691 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/deposit_switch_token_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8101 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_network.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7145 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7194 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/numbers_international_iban.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9316 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transaction_code.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    11954 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/plaid_error.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7788 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_authorization_guarantee_decision.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8042 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/holdings_override.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6657 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/kyc_check_date_of_birth_summary.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7124 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7565 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_idempotency_key.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7530 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_audit_copy_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7844 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/user_address.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9189 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/numbers_eft_nullable.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7815 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_profile_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7024 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_investment_filter.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7555 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/security_override.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7151 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/user_stated_income_source_frequency.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7983 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/owner_override.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8067 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/investment_transaction_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6715 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_application_list_user_auth.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7257 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_request_income_verification_payroll_income.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7496 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/earnings.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6908 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_cancel_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7033 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfers_events_update_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8392 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/pay_stub_earnings_total.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7331 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_intent_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8981 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/institutions_get_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7349 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_pay_stub_deductions.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7543 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/document_analysis.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8610 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/earnings_total.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7683 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/account_selection_cardinality.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7951 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_transfer_simulate_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7093 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/meta.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7657 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/mortgage_property_address.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7233 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7262 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payroll_item_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7809 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/default_update_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7202 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/get_individual_watchlist_screening_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7088 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/employment_details.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    13362 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_intent_get.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8982 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_consent_max_payment_amount.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    13660 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_payment_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7435 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/list_watchlist_screening_individual_hit_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6930 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_request_income_verification_bank_income.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7314 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_employment_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7948 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/list_individual_watchlist_screening_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6758 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/account_filter_subtypes.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7825 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/liabilities_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8024 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_bank_transfer_simulate_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6982 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_screening_hits_phone_number_items.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6635 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_request_deposit_switch.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8182 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/deductions_breakdown.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8126 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_list_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10150 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_event_list_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8585 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/document_authenticity_match_code.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7268 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_relay_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    11233 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/account_balance.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7723 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/list_identity_verification_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7443 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/list_watchlist_screening_individual_history_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8521 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/location.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7913 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paginated_entity_watchlist_screening_review_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7304 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_transfer_sweep_simulate_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7202 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_enhance_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8254 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/signal_decision_report_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6514 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_match_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7570 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_breakdown.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8792 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_list_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7787 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/webhook_update_acknowledged_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    14522 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/liability_override.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7019 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_filter.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7883 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_recipient.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6741 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_import_request_user_auth.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8075 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_recurring_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8108 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_default_update_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8227 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/employment_verification.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9622 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_authorization.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7001 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_consent_periodic_interval.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8178 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/investments_transactions_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10980 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9005 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/ytd_net_income_summary_field_number.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7277 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/email.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7165 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_profile_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    11425 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7323 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_platform_ids.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6643 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/kyc_check_name_summary.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10293 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_recipient_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8717 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/physical_document_category.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8669 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/account_assets_all_of.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8498 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8334 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/numbers_iban_nullable.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6592 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_oauth_select_accounts_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7259 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/relay_event.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7582 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/total.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6873 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/review_comment.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7950 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/total_canonical_description.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7662 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_transactions_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7071 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)      348 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/__init__.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6929 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/pay.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8517 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/institutions_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8901 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/pay_stub_distribution_breakdown.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7795 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paginated_individual_watchlist_screening_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8295 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_verification_request_user.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7216 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_relay_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7174 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_webhook_update_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7915 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_relay_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7100 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_transfer_fire_webhook_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8418 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/numbers.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7261 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/update_individual_screening_request_resettable_field_list.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7344 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/loan_account_subtypes.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6926 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_application_scopes_update_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7957 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/screening_hit_data.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    11588 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_payment_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7108 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_bank_transfer_fire_webhook_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6916 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_watchlist_screening_name.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8797 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/strategy.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7103 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_cancel_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7038 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/wallet_iso_currency_code.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10360 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_intent_create.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9047 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/individual_watchlist_program.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10489 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_event_list_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    11733 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/w2.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7011 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_events_update_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7355 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_intent_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8481 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/external_payment_initiation_consent_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7230 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/deposit_switch_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7234 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/account_identity_all_of.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7040 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/generic_country_code.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8305 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/numbers_ach.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7129 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/list_watchlist_screening_entity_programs_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8044 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/document_risk_signals_object.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7671 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_user_address_in_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7007 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_document.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7536 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/liabilities_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    11141 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/investment_transaction.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    10445 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/institution.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6722 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_webhook_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9677 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/individual_watchlist_program_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7129 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_remove_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7798 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_sync_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6595 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/auth_get_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7491 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/list_watchlist_screening_entity_reviews_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7727 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paginated_identity_verification_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    11254 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_payment.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    15247 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/account_assets.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7171 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_refresh_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7099 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_payroll_income_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7207 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/kyc_check_address_summary.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8923 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_verification_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7107 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/personal_finance_category.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7297 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/user_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7150 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/deposit_switch_token_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7281 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/scopes_context.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7529 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/single_document_risk_signal.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7395 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/student_loan_repayment_model.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8287 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9477 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/watchlist_screening_document_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8690 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/external_payment_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8004 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_relay_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    13887 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transaction_base.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7125 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/country_code.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8120 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/holdings_default_update_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7278 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7431 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_payroll_income_precheck_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6533 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_screening_hit_emails.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6645 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/kyc_check_phone_summary.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7926 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_consent_payment_execute_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6936 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_item_set_verification_status_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7371 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_consent_scope.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8384 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_application_scopes_update_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6917 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_screening_hit_urls_items.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7283 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/employers_search_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7392 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paystub_verification_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    11238 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_verification_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6985 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_source_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6918 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_transfer_simulate_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7918 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/watchlist_screening_review.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7608 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/deductions.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8485 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6894 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_consent_revoke_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7478 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_user_address_in_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7366 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_event_list_bank_transfer_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8754 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/update_individual_screening_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7947 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_recurring_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6768 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/signal_device.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    12321 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/cause.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8771 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_historical_summary.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    11303 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/external_payment_schedule_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7135 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/pay_frequency_value.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7524 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7218 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/platform_ids.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7098 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/individual_watchlist_screening_program_name.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7045 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_processor_token_create_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7480 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/auth_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8140 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_item.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7310 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_event_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7209 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/investments_transactions_get_request_options.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7598 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_repayment_return.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6996 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payroll_income_rate_of_pay.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8110 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_refresh_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7137 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/list_watchlist_screening_individual_programs_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6555 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/liabilities_account_ids_with_updated_liabilities.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7104 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/watchlist_screening_document.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8074 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transactions_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7116 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_relay_remove_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7397 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/employment_verification_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9371 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_employment_verification.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    13436 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_w2.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8567 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_watchlist_screening_review_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6892 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_recipient_list_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9885 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/pay_stub_pay_period_details.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7595 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/user_stated_income_source_category.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8525 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_error_type.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9195 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/scopes_nullable.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9411 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_bank_income_source.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7263 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_screening_hit_names.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6874 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_verification_user_phone_number.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7132 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_relay_remove_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7230 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_payment_token_create_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7019 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/auth_metadata.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9861 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_event.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7561 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_event_sync_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6451 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paystub_override_employer.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7381 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/auth_supported_methods.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8809 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/document_risk_signal.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7442 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/transfer_authorization_guarantee_decision_rationale.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7167 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_relay_remove_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7926 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/verification_refresh_status.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8175 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/recurring_transaction_frequency.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7264 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_precheck_user.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7468 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/identity_verification_retried_webhook.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7210 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/sandbox_processor_token_create_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6653 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_override.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     8998 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/entity_watchlist_program.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7787 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_precheck_confidence.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7389 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_refresh_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7196 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/numbers_bacs.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7730 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/credit_relay_refresh_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7853 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/income_verification_taxforms_get_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7773 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/health_incident.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6807 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/update_entity_screening_request_resettable_field.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7245 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_balance_get_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7117 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/asset_report_remove_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9627 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/signal_evaluate_request.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     6837 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/screening_hit_date_of_birth_item.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7543 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/item_status_transactions.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7812 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/payment_initiation_payment_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     9120 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/earnings_breakdown.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7084 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/report_token.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7791 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/paginated_individual_watchlist_screening_hit_list_response.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7024 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/link_token_create_depository_filter.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     7220 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model/bank_transfer_balance.py
+drwxrwxr-x   0 jenkins   (2166) jenkins   (2166)        0 2022-08-03 21:27:09.000000 plaid-python-9.9.0/plaid/api/
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)   875681 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/api/plaid_api.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)      207 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/api/__init__.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    17962 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/configuration.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)     5015 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/exceptions.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    12439 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/rest.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    72852 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/model_utils.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)      687 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/__init__.py
+drwxrwxr-x   0 jenkins   (2166) jenkins   (2166)        0 2022-08-03 21:27:09.000000 plaid-python-9.9.0/plaid/models/
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    70516 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/models/__init__.py
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    36733 2022-08-03 21:26:51.000000 plaid-python-9.9.0/plaid/api_client.py
+drwxrwxr-x   0 jenkins   (2166) jenkins   (2166)        0 2022-08-03 21:27:09.000000 plaid-python-9.9.0/plaid_python.egg-info/
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)       12 2022-08-03 21:27:08.000000 plaid-python-9.9.0/plaid_python.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)    40171 2022-08-03 21:27:08.000000 plaid-python-9.9.0/plaid_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)       41 2022-08-03 21:27:08.000000 plaid-python-9.9.0/plaid_python.egg-info/requires.txt
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)      638 2022-08-03 21:27:08.000000 plaid-python-9.9.0/plaid_python.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)        1 2022-08-03 21:27:08.000000 plaid-python-9.9.0/plaid_python.egg-info/not-zip-safe
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)        1 2022-08-03 21:27:08.000000 plaid-python-9.9.0/plaid_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)      638 2022-08-03 21:27:09.000000 plaid-python-9.9.0/PKG-INFO
+-rw-rw-r--   0 jenkins   (2166) jenkins   (2166)       38 2022-08-03 21:27:09.000000 plaid-python-9.9.0/setup.cfg
```

### Comparing `plaid-python-9.8.0/setup.py` & `plaid-python-9.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '9.8.0'
+VERSION = '9.9.0'
 url = 'https://github.com/plaid/plaid-python'
 
 REQUIRES = [
   "urllib3 >= 1.25.3",
   "python-dateutil",
   "nulltype",
 ]
```

### Comparing `plaid-python-9.8.0/tests/integration/test_assets.py` & `plaid-python-9.9.0/tests/integration/test_assets.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/tests/integration/test_webhooks.py` & `plaid-python-9.9.0/tests/integration/test_webhooks.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/tests/integration/test_deposit_switch.py` & `plaid-python-9.9.0/tests/integration/test_deposit_switch.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/tests/integration/test_investment_transactions.py` & `plaid-python-9.9.0/tests/integration/test_investment_transactions.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/tests/integration/test_income_verification.py` & `plaid-python-9.9.0/tests/integration/test_income_verification.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/tests/integration/test_item.py` & `plaid-python-9.9.0/tests/integration/test_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     try:
         ir_request = ItemRemoveRequest(
             access_token=exchange_response['access_token']
         )
         client.item_remove(ir_request)
     except plaid.ApiException as e:
         response = json.loads(e.body)
-        assert response['error_code'] == 'INVALID_ACCESS_TOKEN'
+        assert response['error_code'] == 'ITEM_NOT_FOUND'
 
 
 def test_import():
     client = create_client()
     at_request = ItemImportRequest(
         products=[Products('identity'), Products('auth')],
         user_auth=ItemImportRequestUserAuth(
@@ -225,8 +225,8 @@
     with ensure_item_removed(exchange_response['access_token']):
         webhook_request = ItemWebhookUpdateRequest(
             access_token=exchange_response['access_token'],
             webhook='https://plaid.com/webhook-test'
         )
         webhook_response = client.item_webhook_update(webhook_request)
         assert (webhook_response['item']['webhook'] ==
-                'https://plaid.com/webhook-test')
+                'https://plaid.com/webhook-test')
```

### Comparing `plaid-python-9.8.0/tests/integration/test_accounts.py` & `plaid-python-9.9.0/tests/integration/test_accounts.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/tests/integration/test_auth.py` & `plaid-python-9.9.0/tests/integration/test_auth.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/tests/integration/util.py` & `plaid-python-9.9.0/tests/integration/util.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/tests/integration/test_institutions.py` & `plaid-python-9.9.0/tests/integration/test_institutions.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/tests/integration/test_payment_initiation.py` & `plaid-python-9.9.0/tests/integration/test_payment_initiation.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/tests/integration/test_transactions.py` & `plaid-python-9.9.0/tests/integration/test_transactions.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/tests/integration/test_bank_transfer.py` & `plaid-python-9.9.0/tests/integration/test_bank_transfer.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/tests/integration/test_processor.py` & `plaid-python-9.9.0/tests/integration/test_processor.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/tests/integration/test_identity.py` & `plaid-python-9.9.0/tests/integration/test_identity.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/tests/integration/test_link_token.py` & `plaid-python-9.9.0/tests/integration/test_link_token.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/tests/integration/test_liabilities.py` & `plaid-python-9.9.0/tests/integration/test_liabilities.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/tests/integration/test_holdings.py` & `plaid-python-9.9.0/tests/integration/test_holdings.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_transaction_get_response.py` & `plaid-python-9.9.0/plaid/model/wallet_transaction_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/pay_stub_deductions_total.py` & `plaid-python-9.9.0/plaid/model/pay_stub_deductions_total.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/deposit_switch_state_update_webhook.py` & `plaid-python-9.9.0/plaid/model/deposit_switch_state_update_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_breakdown_type.py` & `plaid-python-9.9.0/plaid/model/income_breakdown_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/employment_verification_status.py` & `plaid-python-9.9.0/plaid/model/employment_verification_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_account_subtypes.py` & `plaid-python-9.9.0/plaid/model/credit_account_subtypes.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/investment_holdings_get_request_options.py` & `plaid-python-9.9.0/plaid/model/investment_holdings_get_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/physical_document_extracted_data_analysis.py` & `plaid-python-9.9.0/plaid/model/physical_document_extracted_data_analysis.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/mortgage_liability.py` & `plaid-python-9.9.0/plaid/model/mortgage_liability.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paystub_ytd_details.py` & `plaid-python-9.9.0/plaid/model/paystub_ytd_details.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_request_account_subtypes.py` & `plaid-python-9.9.0/plaid/model/link_token_create_request_account_subtypes.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_optional_restriction_bacs.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_optional_restriction_bacs.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_migrate_account_response.py` & `plaid-python-9.9.0/plaid/model/transfer_migrate_account_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_payroll_income_get_response.py` & `plaid-python-9.9.0/plaid/model/credit_payroll_income_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_sweep.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_sweep.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_import_request_options.py` & `plaid-python-9.9.0/plaid/model/item_import_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/screening_hit_analysis.py` & `plaid-python-9.9.0/plaid/model/screening_hit_analysis.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_status_last_webhook.py` & `plaid-python-9.9.0/plaid/model/item_status_last_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/program_name_sensitivity.py` & `plaid-python-9.9.0/plaid/model/program_name_sensitivity.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/numbers_iban.py` & `plaid-python-9.9.0/plaid/model/numbers_iban.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_address.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_address.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/pay_stub_taxpayer_id.py` & `plaid-python-9.9.0/plaid/model/pay_stub_taxpayer_id.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/employer.py` & `plaid-python-9.9.0/plaid/model/employer.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_rule_field.py` & `plaid-python-9.9.0/plaid/model/transactions_rule_field.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/employee_income_summary_field_string.py` & `plaid-python-9.9.0/plaid/model/employee_income_summary_field_string.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_transfer_repayment_simulate_request.py` & `plaid-python-9.9.0/plaid/model/sandbox_transfer_repayment_simulate_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_consent_valid_date_time.py` & `plaid-python-9.9.0/plaid/model/payment_consent_valid_date_time.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/error.py` & `plaid-python-9.9.0/plaid/model/error.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/address.py` & `plaid-python-9.9.0/plaid/model/address.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_initiated_risk_tier.py` & `plaid-python-9.9.0/plaid/model/bank_initiated_risk_tier.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/watchlist_screening_hit.py` & `plaid-python-9.9.0/plaid/model/watchlist_screening_hit.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_sweep_status.py` & `plaid-python-9.9.0/plaid/model/transfer_sweep_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_refresh_response.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_refresh_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_audit_copy_token_create_response.py` & `plaid-python-9.9.0/plaid/model/credit_audit_copy_token_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_transaction_amount.py` & `plaid-python-9.9.0/plaid/model/wallet_transaction_amount.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_payment_create_status.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_payment_create_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_request_auth.py` & `plaid-python-9.9.0/plaid/model/link_token_create_request_auth.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/get_identity_verification_request.py` & `plaid-python-9.9.0/plaid/model/get_identity_verification_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/w2_state_and_local_wages.py` & `plaid-python-9.9.0/plaid/model/w2_state_and_local_wages.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/product_status.py` & `plaid-python-9.9.0/plaid/model/product_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/image_quality.py` & `plaid-python-9.9.0/plaid/model/image_quality.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_transaction.py` & `plaid-python-9.9.0/plaid/model/wallet_transaction.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_payroll_income_precheck_request.py` & `plaid-python-9.9.0/plaid/model/credit_payroll_income_precheck_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/document_metadata.py` & `plaid-python-9.9.0/plaid/model/document_metadata.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/processor_stripe_bank_account_token_create_response.py` & `plaid-python-9.9.0/plaid/model/processor_stripe_bank_account_token_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_transaction_status.py` & `plaid-python-9.9.0/plaid/model/wallet_transaction_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_public_token_exchange_response.py` & `plaid-python-9.9.0/plaid/model/item_public_token_exchange_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/override_account_type.py` & `plaid-python-9.9.0/plaid/model/override_account_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/processor_bank_transfer_create_response.py` & `plaid-python-9.9.0/plaid/model/processor_bank_transfer_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_event_list_transfer_type.py` & `plaid-python-9.9.0/plaid/model/transfer_event_list_transfer_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_repayment.py` & `plaid-python-9.9.0/plaid/model/transfer_repayment.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/risk_signal_document_reference.py` & `plaid-python-9.9.0/plaid/model/risk_signal_document_reference.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_authorization_decision_rationale.py` & `plaid-python-9.9.0/plaid/model/transfer_authorization_decision_rationale.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_status.py` & `plaid-python-9.9.0/plaid/model/item_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/list_watchlist_screening_entity_history_request.py` & `plaid-python-9.9.0/plaid/model/list_watchlist_screening_entity_history_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/create_individual_watchlist_screening_review_request.py` & `plaid-python-9.9.0/plaid/model/create_individual_watchlist_screening_review_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/documentary_verification.py` & `plaid-python-9.9.0/plaid/model/documentary_verification.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_event_list_response.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_event_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paystub_override_employee.py` & `plaid-python-9.9.0/plaid/model/paystub_override_employee.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/phone_number.py` & `plaid-python-9.9.0/plaid/model/phone_number.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payroll_income_account_data.py` & `plaid-python-9.9.0/plaid/model/payroll_income_account_data.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/auth_get_response.py` & `plaid-python-9.9.0/plaid/model/auth_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_summary.py` & `plaid-python-9.9.0/plaid/model/income_summary.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_verification_user_data.py` & `plaid-python-9.9.0/plaid/model/identity_verification_user_data.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_error_webhook.py` & `plaid-python-9.9.0/plaid/model/item_error_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_pay_stub_employer.py` & `plaid-python-9.9.0/plaid/model/credit_pay_stub_employer.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/standalone_investment_transaction_type.py` & `plaid-python-9.9.0/plaid/model/standalone_investment_transaction_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/list_watchlist_screening_entity_hit_request.py` & `plaid-python-9.9.0/plaid/model/list_watchlist_screening_entity_hit_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_get_request.py` & `plaid-python-9.9.0/plaid/model/asset_report_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/signal_person_name.py` & `plaid-python-9.9.0/plaid/model/signal_person_name.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/watchlist_screening_individual_response.py` & `plaid-python-9.9.0/plaid/model/watchlist_screening_individual_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/account_base.py` & `plaid-python-9.9.0/plaid/model/account_base.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/update_individual_screening_request_resettable_field.py` & `plaid-python-9.9.0/plaid/model/update_individual_screening_request_resettable_field.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_screening_hit_urls.py` & `plaid-python-9.9.0/plaid/model/entity_screening_hit_urls.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/institutions_get_by_id_response.py` & `plaid-python-9.9.0/plaid/model/institutions_get_by_id_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/depository_account_subtypes.py` & `plaid-python-9.9.0/plaid/model/depository_account_subtypes.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/issuing_country.py` & `plaid-python-9.9.0/plaid/model/issuing_country.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_failure.py` & `plaid-python-9.9.0/plaid/model/transfer_failure.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_pay_frequency.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_pay_frequency.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_public_token_exchange_request.py` & `plaid-python-9.9.0/plaid/model/item_public_token_exchange_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/signal_prepare_response.py` & `plaid-python-9.9.0/plaid/model/signal_prepare_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_documents_download_request.py` & `plaid-python-9.9.0/plaid/model/income_verification_documents_download_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/physical_document_id_number.py` & `plaid-python-9.9.0/plaid/model/physical_document_id_number.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_sweep_list_request.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_sweep_list_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/document_status.py` & `plaid-python-9.9.0/plaid/model/document_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_authorization_create_response.py` & `plaid-python-9.9.0/plaid/model/transfer_authorization_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/customer_initiated_risk_tier.py` & `plaid-python-9.9.0/plaid/model/customer_initiated_risk_tier.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_warning.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_warning.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/signal_scores.py` & `plaid-python-9.9.0/plaid/model/signal_scores.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paystub_details.py` & `plaid-python-9.9.0/plaid/model/paystub_details.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/numbers_international_nullable.py` & `plaid-python-9.9.0/plaid/model/numbers_international_nullable.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_event.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_event.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_audit_copy_token_create_request.py` & `plaid-python-9.9.0/plaid/model/credit_audit_copy_token_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sender_bacs_nullable.py` & `plaid-python-9.9.0/plaid/model/sender_bacs_nullable.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/historical_balance.py` & `plaid-python-9.9.0/plaid/model/historical_balance.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_repayment_list_response.py` & `plaid-python-9.9.0/plaid/model/transfer_repayment_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/list_dashboard_user_request.py` & `plaid-python-9.9.0/plaid/model/list_dashboard_user_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/address_purpose_label.py` & `plaid-python-9.9.0/plaid/model/address_purpose_label.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_payment_create_request.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_payment_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_recipient_create_request.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_recipient_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/security.py` & `plaid-python-9.9.0/plaid/model/security.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_remove_request.py` & `plaid-python-9.9.0/plaid/model/asset_report_remove_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_type.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_watchlist_screening_search_terms.py` & `plaid-python-9.9.0/plaid/model/entity_watchlist_screening_search_terms.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_status_investments.py` & `plaid-python-9.9.0/plaid/model/item_status_investments.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/depository_filter.py` & `plaid-python-9.9.0/plaid/model/depository_filter.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/projected_income_summary_field_number.py` & `plaid-python-9.9.0/plaid/model/projected_income_summary_field_number.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_removed_webhook.py` & `plaid-python-9.9.0/plaid/model/transactions_removed_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/physical_document_images.py` & `plaid-python-9.9.0/plaid/model/physical_document_images.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_watchlist_screening_hit.py` & `plaid-python-9.9.0/plaid/model/entity_watchlist_screening_hit.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paginated_individual_watchlist_program_list_response.py` & `plaid-python-9.9.0/plaid/model/paginated_individual_watchlist_program_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_oauth_select_accounts_request.py` & `plaid-python-9.9.0/plaid/model/sandbox_oauth_select_accounts_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_create_request_options.py` & `plaid-python-9.9.0/plaid/model/asset_report_create_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/processor_auth_get_request.py` & `plaid-python-9.9.0/plaid/model/processor_auth_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/employer_income_summary_field_string.py` & `plaid-python-9.9.0/plaid/model/employer_income_summary_field_string.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_sweep_get_response.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_sweep_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_sweep_list_request.py` & `plaid-python-9.9.0/plaid/model/transfer_sweep_list_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sync_updates_available_webhook.py` & `plaid-python-9.9.0/plaid/model/sync_updates_available_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/accounts_get_request.py` & `plaid-python-9.9.0/plaid/model/accounts_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_account_filters.py` & `plaid-python-9.9.0/plaid/model/link_token_account_filters.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_transaction_get_request.py` & `plaid-python-9.9.0/plaid/model/wallet_transaction_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/products.py` & `plaid-python-9.9.0/plaid/model/products.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transaction_stream_status.py` & `plaid-python-9.9.0/plaid/model/transaction_stream_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/pay_stub_deductions_breakdown.py` & `plaid-python-9.9.0/plaid/model/pay_stub_deductions_breakdown.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_watchlist_screening.py` & `plaid-python-9.9.0/plaid/model/entity_watchlist_screening.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/employers_search_request.py` & `plaid-python-9.9.0/plaid/model/employers_search_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/address_data.py` & `plaid-python-9.9.0/plaid/model/address_data.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/loan_account_subtype.py` & `plaid-python-9.9.0/plaid/model/loan_account_subtype.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_transaction_counterparty_numbers.py` & `plaid-python-9.9.0/plaid/model/wallet_transaction_counterparty_numbers.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paystub_address.py` & `plaid-python-9.9.0/plaid/model/paystub_address.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet.py` & `plaid-python-9.9.0/plaid/model/wallet.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_import_request.py` & `plaid-python-9.9.0/plaid/model/item_import_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/external_payment_schedule_get.py` & `plaid-python-9.9.0/plaid/model/external_payment_schedule_get.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_payment_create_response.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_payment_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/ytd_gross_income_summary_field_number.py` & `plaid-python-9.9.0/plaid/model/ytd_gross_income_summary_field_number.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_request_income_verification.py` & `plaid-python-9.9.0/plaid/model/link_token_create_request_income_verification.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_direction.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_direction.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_payroll_flow_type.py` & `plaid-python-9.9.0/plaid/model/income_verification_payroll_flow_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_income_fire_webhook_request.py` & `plaid-python-9.9.0/plaid/model/sandbox_income_fire_webhook_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_request_user.py` & `plaid-python-9.9.0/plaid/model/link_token_create_request_user.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,20 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
+def lazy_import():
+    from plaid.model.user_address import UserAddress
+    from plaid.model.user_id_number import UserIDNumber
+    globals()['UserAddress'] = UserAddress
+    globals()['UserIDNumber'] = UserIDNumber
+
 
 class LinkTokenCreateRequestUser(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
@@ -65,39 +71,46 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
             'client_user_id': (str,),  # noqa: E501
             'legal_name': (str,),  # noqa: E501
+            'name': (object,),  # noqa: E501
             'phone_number': (str,),  # noqa: E501
             'phone_number_verified_time': (datetime,),  # noqa: E501
             'email_address': (str,),  # noqa: E501
             'email_address_verified_time': (datetime,),  # noqa: E501
             'ssn': (str,),  # noqa: E501
             'date_of_birth': (date,),  # noqa: E501
+            'address': (UserAddress,),  # noqa: E501
+            'id_number': (UserIDNumber,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'client_user_id': 'client_user_id',  # noqa: E501
         'legal_name': 'legal_name',  # noqa: E501
+        'name': 'name',  # noqa: E501
         'phone_number': 'phone_number',  # noqa: E501
         'phone_number_verified_time': 'phone_number_verified_time',  # noqa: E501
         'email_address': 'email_address',  # noqa: E501
         'email_address_verified_time': 'email_address_verified_time',  # noqa: E501
         'ssn': 'ssn',  # noqa: E501
         'date_of_birth': 'date_of_birth',  # noqa: E501
+        'address': 'address',  # noqa: E501
+        'id_number': 'id_number',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
@@ -141,21 +154,24 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            legal_name (str): The user's full legal name. This is an optional field used in the [returning user experience](https://plaid.com/docs/link/returning-user) to associate Items to the user.. [optional]  # noqa: E501
+            legal_name (str): The user's full legal name. Currently used only to support certain legacy flows.. [optional]  # noqa: E501
+            name (object): The user's full name. Optional if using the [Identity Verification](https://plaid.com/docs/api/products/identity-verification) product; if not using Identity Verification, this field is not allowed. Users will not be asked for their name when this field is provided.. [optional]  # noqa: E501
             phone_number (str): The user's phone number in [E.164](https://en.wikipedia.org/wiki/E.164) format. This field is optional, but required to enable the [returning user experience](https://plaid.com/docs/link/returning-user).. [optional]  # noqa: E501
             phone_number_verified_time (datetime): The date and time the phone number was verified in [ISO 8601](https://wikipedia.org/wiki/ISO_8601) format (`YYYY-MM-DDThh:mm:ssZ`). This field is optional, but required to enable any [returning user experience](https://plaid.com/docs/link/returning-user).   Only pass a verification time for a phone number that you have verified. If you have performed verification but don’t have the time, you may supply a signal value of the start of the UNIX epoch.   Example: `2020-01-01T00:00:00Z` . [optional]  # noqa: E501
             email_address (str): The user's email address. This field is optional, but required to enable the [pre-authenticated returning user flow](https://plaid.com/docs/link/returning-user/#enabling-the-returning-user-experience).. [optional]  # noqa: E501
             email_address_verified_time (datetime): The date and time the email address was verified in [ISO 8601](https://wikipedia.org/wiki/ISO_8601) format (`YYYY-MM-DDThh:mm:ssZ`). This is an optional field used in the [returning user experience](https://plaid.com/docs/link/returning-user).   Only pass a verification time for an email address that you have verified. If you have performed verification but don’t have the time, you may supply a signal value of the start of the UNIX epoch.   Example: `2020-01-01T00:00:00Z`. [optional]  # noqa: E501
-            ssn (str): To be provided in the format \"ddd-dd-dddd\". This field is optional and will support not-yet-implemented functionality for new products.. [optional]  # noqa: E501
-            date_of_birth (date): To be provided in the format \"yyyy-mm-dd\". This field is optional and will support not-yet-implemented functionality for new products.. [optional]  # noqa: E501
+            ssn (str): To be provided in the format \"ddd-dd-dddd\". Not currently used.. [optional]  # noqa: E501
+            date_of_birth (date): To be provided in the format \"yyyy-mm-dd\". Not currently used.. [optional]  # noqa: E501
+            address (UserAddress): [optional]  # noqa: E501
+            id_number (UserIDNumber): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `plaid-python-9.8.0/plaid/model/student_loan_status.py` & `plaid-python-9.9.0/plaid/model/student_loan_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_screening_hit_documents_items.py` & `plaid-python-9.9.0/plaid/model/entity_screening_hit_documents_items.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/generic_screening_hit_location_items.py` & `plaid-python-9.9.0/plaid/model/generic_screening_hit_location_items.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/webhook_verification_key_get_request.py` & `plaid-python-9.9.0/plaid/model/webhook_verification_key_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/institutions_search_payment_initiation_options.py` & `plaid-python-9.9.0/plaid/model/institutions_search_payment_initiation_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/physical_document_extracted_data.py` & `plaid-python-9.9.0/plaid/model/physical_document_extracted_data.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/account_filter.py` & `plaid-python-9.9.0/plaid/model/account_filter.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_response.py` & `plaid-python-9.9.0/plaid/model/link_token_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payroll_income_object.py` & `plaid-python-9.9.0/plaid/model/payroll_income_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,18 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 def lazy_import():
+    from plaid.model.credit1099 import Credit1099
     from plaid.model.credit_pay_stub import CreditPayStub
     from plaid.model.credit_w2 import CreditW2
+    globals()['Credit1099'] = Credit1099
     globals()['CreditPayStub'] = CreditPayStub
     globals()['CreditW2'] = CreditW2
 
 
 class PayrollIncomeObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -83,46 +85,49 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'account_id': (str, none_type,),  # noqa: E501
             'pay_stubs': ([CreditPayStub],),  # noqa: E501
             'w2s': ([CreditW2],),  # noqa: E501
+            'form1099s': ([Credit1099],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'account_id': 'account_id',  # noqa: E501
         'pay_stubs': 'pay_stubs',  # noqa: E501
         'w2s': 'w2s',  # noqa: E501
+        'form1099s': 'form1099s',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, account_id, pay_stubs, w2s, *args, **kwargs):  # noqa: E501
+    def __init__(self, account_id, pay_stubs, w2s, form1099s, *args, **kwargs):  # noqa: E501
         """PayrollIncomeObject - a model defined in OpenAPI
 
         Args:
             account_id (str, none_type): ID of the payroll provider account.
             pay_stubs ([CreditPayStub]): Array of pay stubs for the user.
             w2s ([CreditW2]): Array of tax form W-2s.
+            form1099s ([Credit1099]): Array of tax form 1099s.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -175,14 +180,15 @@
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.account_id = account_id
         self.pay_stubs = pay_stubs
         self.w2s = w2s
+        self.form1099s = form1099s
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_list_response.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_transaction_idempotency_key.py` & `plaid-python-9.9.0/plaid/model/wallet_transaction_idempotency_key.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_eu_config.py` & `plaid-python-9.9.0/plaid/model/link_token_eu_config.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_consent_periodic_amount.py` & `plaid-python-9.9.0/plaid/model/payment_consent_periodic_amount.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_verification_retry_request_steps_object.py` & `plaid-python-9.9.0/plaid/model/identity_verification_retry_request_steps_object.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_rule_details.py` & `plaid-python-9.9.0/plaid/model/transactions_rule_details.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_get_response.py` & `plaid-python-9.9.0/plaid/model/transactions_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_refresh_response.py` & `plaid-python-9.9.0/plaid/model/transactions_refresh_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/customer_initiated_return_risk.py` & `plaid-python-9.9.0/plaid/model/customer_initiated_return_risk.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paginated_entity_watchlist_screening_list_response.py` & `plaid-python-9.9.0/plaid/model/paginated_entity_watchlist_screening_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/individual_screening_hit_names.py` & `plaid-python-9.9.0/plaid/model/individual_screening_hit_names.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/user_permission_revoked_webhook.py` & `plaid-python-9.9.0/plaid/model/user_permission_revoked_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_repayment_return_list_response.py` & `plaid-python-9.9.0/plaid/model/transfer_repayment_return_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/auth_get_numbers.py` & `plaid-python-9.9.0/plaid/model/auth_get_numbers.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/connected_application.py` & `plaid-python-9.9.0/plaid/model/connected_application.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/document_risk_signal_institution_metadata.py` & `plaid-python-9.9.0/plaid/model/document_risk_signal_institution_metadata.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/account_access.py` & `plaid-python-9.9.0/plaid/model/account_access.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/institutions_search_response.py` & `plaid-python-9.9.0/plaid/model/institutions_search_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/processor_balance_get_request.py` & `plaid-python-9.9.0/plaid/model/processor_balance_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_migrate_account_request.py` & `plaid-python-9.9.0/plaid/model/transfer_migrate_account_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_event_list_direction.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_event_list_direction.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_payment_get_request.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_payment_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_bank_transfer_fire_webhook_response.py` & `plaid-python-9.9.0/plaid/model/sandbox_bank_transfer_fire_webhook_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/watchlist_screening_hit_locations.py` & `plaid-python-9.9.0/plaid/model/watchlist_screening_hit_locations.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/processor_auth_get_response.py` & `plaid-python-9.9.0/plaid/model/processor_auth_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_cancel_response.py` & `plaid-python-9.9.0/plaid/model/transfer_cancel_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/screening_hit_documents_items.py` & `plaid-python-9.9.0/plaid/model/screening_hit_documents_items.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_refresh_request_options.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_refresh_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_consent_revoke_request.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_consent_revoke_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_public_token_create_response.py` & `plaid-python-9.9.0/plaid/model/sandbox_public_token_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_consent.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_consent.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_profile_remove_request.py` & `plaid-python-9.9.0/plaid/model/payment_profile_remove_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/pslf_status.py` & `plaid-python-9.9.0/plaid/model/pslf_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/investment_account_subtypes.py` & `plaid-python-9.9.0/plaid/model/investment_account_subtypes.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_application_list_response.py` & `plaid-python-9.9.0/plaid/model/item_application_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_transfer_fire_webhook_response.py` & `plaid-python-9.9.0/plaid/model/sandbox_transfer_fire_webhook_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_authorization_device.py` & `plaid-python-9.9.0/plaid/model/transfer_authorization_device.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,16 +132,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            ip_address (str): The IP address of the device being used to initiate the authorization.. [optional]  # noqa: E501
-            user_agent (str): The user agent of the device being used to initiate the authorization.. [optional]  # noqa: E501
+            ip_address (str): The IP address of the device being used to initiate the authorization. Required for guaranteed ACH customers.. [optional]  # noqa: E501
+            user_agent (str): The user agent of the device being used to initiate the authorization. Required for guaranteed ACH customers.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `plaid-python-9.8.0/plaid/model/transactions_rules_list_request.py` & `plaid-python-9.9.0/plaid/model/transactions_rules_list_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_transactions_list_request.py` & `plaid-python-9.9.0/plaid/model/wallet_transactions_list_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_event_type.py` & `plaid-python-9.9.0/plaid/model/transfer_event_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 
     allowed_values = {
         ('value',): {
             'PENDING': "pending",
             'CANCELLED': "cancelled",
             'FAILED': "failed",
             'POSTED': "posted",
-            'REVERSED': "reversed",
             'RETURNED': "returned",
             'SWEPT': "swept",
             'REVERSE_SWEPT': "reverse_swept",
             'RETURN_SWEPT': "return_swept",
         },
     }
 
@@ -101,18 +100,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """TransferEventType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): The type of event that this transfer represents.  `pending`: A new transfer was created; it is in the pending state.  `cancelled`: The transfer was cancelled by the client.  `failed`: The transfer failed, no funds were moved.  `posted`: The transfer has been successfully submitted to the payment network.  `returned`: A posted transfer was returned.  `swept`: The transfer was swept to / from the sweep account.  `return_swept`: Due to the transfer being returned, funds were pulled from or pushed back to the sweep account.., must be one of ["pending", "cancelled", "failed", "posted", "reversed", "returned", "swept", "reverse_swept", "return_swept", ]  # noqa: E501
+            args[0] (str): The type of event that this transfer represents.  `pending`: A new transfer was created; it is in the pending state.  `cancelled`: The transfer was cancelled by the client.  `failed`: The transfer failed, no funds were moved.  `posted`: The transfer has been successfully submitted to the payment network.  `returned`: A posted transfer was returned.  `swept`: The transfer was swept to / from the sweep account.  `return_swept`: Due to the transfer being returned, funds were pulled from or pushed back to the sweep account.., must be one of ["pending", "cancelled", "failed", "posted", "returned", "swept", "reverse_swept", "return_swept", ]  # noqa: E501
 
         Keyword Args:
-            value (str): The type of event that this transfer represents.  `pending`: A new transfer was created; it is in the pending state.  `cancelled`: The transfer was cancelled by the client.  `failed`: The transfer failed, no funds were moved.  `posted`: The transfer has been successfully submitted to the payment network.  `returned`: A posted transfer was returned.  `swept`: The transfer was swept to / from the sweep account.  `return_swept`: Due to the transfer being returned, funds were pulled from or pushed back to the sweep account.., must be one of ["pending", "cancelled", "failed", "posted", "reversed", "returned", "swept", "reverse_swept", "return_swept", ]  # noqa: E501
+            value (str): The type of event that this transfer represents.  `pending`: A new transfer was created; it is in the pending state.  `cancelled`: The transfer was cancelled by the client.  `failed`: The transfer failed, no funds were moved.  `posted`: The transfer has been successfully submitted to the payment network.  `returned`: A posted transfer was returned.  `swept`: The transfer was swept to / from the sweep account.  `return_swept`: Due to the transfer being returned, funds were pulled from or pushed back to the sweep account.., must be one of ["pending", "cancelled", "failed", "posted", "returned", "swept", "reverse_swept", "return_swept", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `plaid-python-9.8.0/plaid/model/liabilities_default_update_webhook.py` & `plaid-python-9.9.0/plaid/model/liabilities_default_update_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/investments_transactions_get_response.py` & `plaid-python-9.9.0/plaid/model/investments_transactions_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/numbers_international.py` & `plaid-python-9.9.0/plaid/model/numbers_international.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_screening_hit_analysis.py` & `plaid-python-9.9.0/plaid/model/entity_screening_hit_analysis.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/recipient_bacs_nullable.py` & `plaid-python-9.9.0/plaid/model/recipient_bacs_nullable.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/signal_decision_report_response.py` & `plaid-python-9.9.0/plaid/model/signal_decision_report_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/update_individual_screening_request_search_terms.py` & `plaid-python-9.9.0/plaid/model/update_individual_screening_request_search_terms.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/mfa.py` & `plaid-python-9.9.0/plaid/model/mfa.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/match_summary_code.py` & `plaid-python-9.9.0/plaid/model/match_summary_code.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/pending_expiration_webhook.py` & `plaid-python-9.9.0/plaid/model/pending_expiration_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/processor_token_create_request.py` & `plaid-python-9.9.0/plaid/model/processor_token_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/institutions_search_request.py` & `plaid-python-9.9.0/plaid/model/institutions_search_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_sweep_list_response.py` & `plaid-python-9.9.0/plaid/model/transfer_sweep_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/signal_user.py` & `plaid-python-9.9.0/plaid/model/signal_user.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_authorization_create_request.py` & `plaid-python-9.9.0/plaid/model/transfer_authorization_create_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,22 +23,22 @@
     none_type,
     validate_get_composed_info,
 )
 
 def lazy_import():
     from plaid.model.ach_class import ACHClass
     from plaid.model.transfer_authorization_device import TransferAuthorizationDevice
+    from plaid.model.transfer_authorization_user_in_request import TransferAuthorizationUserInRequest
     from plaid.model.transfer_network import TransferNetwork
     from plaid.model.transfer_type import TransferType
-    from plaid.model.transfer_user_in_request import TransferUserInRequest
     globals()['ACHClass'] = ACHClass
     globals()['TransferAuthorizationDevice'] = TransferAuthorizationDevice
+    globals()['TransferAuthorizationUserInRequest'] = TransferAuthorizationUserInRequest
     globals()['TransferNetwork'] = TransferNetwork
     globals()['TransferType'] = TransferType
-    globals()['TransferUserInRequest'] = TransferUserInRequest
 
 
 class TransferAuthorizationCreateRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -79,71 +79,73 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'access_token': (str,),  # noqa: E501
-            'account_id': (str,),  # noqa: E501
             'type': (TransferType,),  # noqa: E501
             'network': (TransferNetwork,),  # noqa: E501
             'amount': (str,),  # noqa: E501
             'ach_class': (ACHClass,),  # noqa: E501
-            'user': (TransferUserInRequest,),  # noqa: E501
+            'user': (TransferAuthorizationUserInRequest,),  # noqa: E501
             'client_id': (str,),  # noqa: E501
             'secret': (str,),  # noqa: E501
+            'access_token': (str,),  # noqa: E501
+            'account_id': (str,),  # noqa: E501
             'device': (TransferAuthorizationDevice,),  # noqa: E501
             'origination_account_id': (str,),  # noqa: E501
             'iso_currency_code': (str,),  # noqa: E501
+            'user_present': (bool, none_type,),  # noqa: E501
+            'payment_profile_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'access_token': 'access_token',  # noqa: E501
-        'account_id': 'account_id',  # noqa: E501
         'type': 'type',  # noqa: E501
         'network': 'network',  # noqa: E501
         'amount': 'amount',  # noqa: E501
         'ach_class': 'ach_class',  # noqa: E501
         'user': 'user',  # noqa: E501
         'client_id': 'client_id',  # noqa: E501
         'secret': 'secret',  # noqa: E501
+        'access_token': 'access_token',  # noqa: E501
+        'account_id': 'account_id',  # noqa: E501
         'device': 'device',  # noqa: E501
         'origination_account_id': 'origination_account_id',  # noqa: E501
         'iso_currency_code': 'iso_currency_code',  # noqa: E501
+        'user_present': 'user_present',  # noqa: E501
+        'payment_profile_id': 'payment_profile_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, access_token, account_id, type, network, amount, ach_class, user, *args, **kwargs):  # noqa: E501
+    def __init__(self, type, network, amount, ach_class, user, *args, **kwargs):  # noqa: E501
         """TransferAuthorizationCreateRequest - a model defined in OpenAPI
 
         Args:
-            access_token (str): The Plaid `access_token` for the account that will be debited or credited.
-            account_id (str): The Plaid `account_id` for the account that will be debited or credited.
             type (TransferType):
             network (TransferNetwork):
             amount (str): The amount of the transfer (decimal string with two digits of precision e.g. \"10.00\").
             ach_class (ACHClass):
-            user (TransferUserInRequest):
+            user (TransferAuthorizationUserInRequest):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -170,17 +172,21 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             client_id (str): Your Plaid API `client_id`. The `client_id` is required and may be provided either in the `PLAID-CLIENT-ID` header or as part of a request body.. [optional]  # noqa: E501
             secret (str): Your Plaid API `secret`. The `secret` is required and may be provided either in the `PLAID-SECRET` header or as part of a request body.. [optional]  # noqa: E501
+            access_token (str): The Plaid `access_token` for the account that will be debited or credited.. [optional]  # noqa: E501
+            account_id (str): The Plaid `account_id` for the account that will be debited or credited.. [optional]  # noqa: E501
             device (TransferAuthorizationDevice): [optional]  # noqa: E501
             origination_account_id (str): Plaid's unique identifier for the origination account for this authorization. If not specified, the default account will be used.. [optional]  # noqa: E501
             iso_currency_code (str): The currency of the transfer amount. The default value is \"USD\".. [optional]  # noqa: E501
+            user_present (bool, none_type): Required for guaranteed ACH customers. If the end user is initiating the specific transfer themselves via an interactive UI, this should be `true`; for automatic recurring payments where the end user is not actually initiating each individual transfer, it should be `false`.. [optional]  # noqa: E501
+            payment_profile_id (str): Plaid’s unique identifier for a payment profile.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -198,16 +204,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.access_token = access_token
-        self.account_id = account_id
         self.type = type
         self.network = network
         self.amount = amount
         self.ach_class = ach_class
         self.user = user
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_consent_status.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_consent_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_get_request_options.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_get_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/cause_all_of.py` & `plaid-python-9.9.0/plaid/model/cause_all_of.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/recaptcha_required_error.py` & `plaid-python-9.9.0/plaid/model/recaptcha_required_error.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_employment_item.py` & `plaid-python-9.9.0/plaid/model/credit_employment_item.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/accounts_get_request_options.py` & `plaid-python-9.9.0/plaid/model/accounts_get_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/processor_identity_get_request.py` & `plaid-python-9.9.0/plaid/model/processor_identity_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paystub_override_employee_address.py` & `plaid-python-9.9.0/plaid/model/paystub_override_employee_address.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/deductions_total.py` & `plaid-python-9.9.0/plaid/model/deductions_total.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_recipient_get_response_all_of.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_recipient_get_response_all_of.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/accounts_balance_get_request_options.py` & `plaid-python-9.9.0/plaid/model/accounts_balance_get_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_audit_copy_remove_request.py` & `plaid-python-9.9.0/plaid/model/asset_report_audit_copy_remove_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_user_in_response.py` & `plaid-python-9.9.0/plaid/model/transfer_user_in_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_payment_reverse_request.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_payment_reverse_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_pay_stub.py` & `plaid-python-9.9.0/plaid/model/credit_pay_stub.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/update_entity_screening_request_search_terms.py` & `plaid-python-9.9.0/plaid/model/update_entity_screening_request_search_terms.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/numbers_ach_nullable.py` & `plaid-python-9.9.0/plaid/model/numbers_ach_nullable.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/account_product_access_nullable.py` & `plaid-python-9.9.0/plaid/model/account_product_access_nullable.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_precheck_employer.py` & `plaid-python-9.9.0/plaid/model/income_verification_precheck_employer.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/client_provided_raw_transaction.py` & `plaid-python-9.9.0/plaid/model/client_provided_raw_transaction.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/watchlist_screening_individual.py` & `plaid-python-9.9.0/plaid/model/watchlist_screening_individual.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_loan_filter.py` & `plaid-python-9.9.0/plaid/model/link_token_create_loan_filter.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_get_response.py` & `plaid-python-9.9.0/plaid/model/wallet_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_consent_create_request.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_consent_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/distribution_breakdown.py` & `plaid-python-9.9.0/plaid/model/distribution_breakdown.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/automatically_verified_webhook.py` & `plaid-python-9.9.0/plaid/model/automatically_verified_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_transaction.py` & `plaid-python-9.9.0/plaid/model/asset_report_transaction.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_payroll_income_refresh_response.py` & `plaid-python-9.9.0/plaid/model/credit_payroll_income_refresh_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/pay_stub_verification_attribute.py` & `plaid-python-9.9.0/plaid/model/pay_stub_verification_attribute.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/source_uid.py` & `plaid-python-9.9.0/plaid/model/source_uid.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_verification_step_summary.py` & `plaid-python-9.9.0/plaid/model/identity_verification_step_summary.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/individual_watchlist_code.py` & `plaid-python-9.9.0/plaid/model/individual_watchlist_code.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/create_entity_watchlist_screening_review_request.py` & `plaid-python-9.9.0/plaid/model/create_entity_watchlist_screening_review_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/watchlist_screening_audit_trail.py` & `plaid-python-9.9.0/plaid/model/watchlist_screening_audit_trail.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/webhook_verification_key_get_response.py` & `plaid-python-9.9.0/plaid/model/webhook_verification_key_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_precheck_employer_address_data.py` & `plaid-python-9.9.0/plaid/model/income_verification_precheck_employer_address_data.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transaction_stream_amount.py` & `plaid-python-9.9.0/plaid/model/transaction_stream_amount.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_relay_refresh_request.py` & `plaid-python-9.9.0/plaid/model/asset_report_relay_refresh_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/removed_transaction.py` & `plaid-python-9.9.0/plaid/model/removed_transaction.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_create_response.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/user_stated_income_source_pay_type.py` & `plaid-python-9.9.0/plaid/model/user_stated_income_source_pay_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/weak_alias_determination.py` & `plaid-python-9.9.0/plaid/model/weak_alias_determination.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_payment_token_create_response.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_payment_token_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_authorization_proposed_transfer.py` & `plaid-python-9.9.0/plaid/model/transfer_authorization_proposed_transfer.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/user_custom_password.py` & `plaid-python-9.9.0/plaid/model/user_custom_password.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_verification_step_updated_webhook.py` & `plaid-python-9.9.0/plaid/model/identity_verification_step_updated_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_match_response.py` & `plaid-python-9.9.0/plaid/model/identity_match_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_filter_request.py` & `plaid-python-9.9.0/plaid/model/asset_report_filter_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/inflow_model.py` & `plaid-python-9.9.0/plaid/model/inflow_model.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/get_watchlist_screening_entity_program_request.py` & `plaid-python-9.9.0/plaid/model/get_watchlist_screening_entity_program_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_authorization_guarantee_decision_rationale_code.py` & `plaid-python-9.9.0/plaid/model/transfer_authorization_guarantee_decision_rationale_code.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
     allowed_values = {
         ('value',): {
             'RETURN_BANK': "RETURN_BANK",
             'RETURN_CUSTOMER': "RETURN_CUSTOMER",
             'GUARANTEE_LIMIT_REACHED': "GUARANTEE_LIMIT_REACHED",
             'RISK_ESTIMATE_UNAVAILABLE': "RISK_ESTIMATE_UNAVAILABLE",
+            'REQUIRED_PARAM_MISSING': "REQUIRED_PARAM_MISSING",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,18 +97,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """TransferAuthorizationGuaranteeDecisionRationaleCode - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): A code representing the reason Plaid declined to guarantee this transfer:  `RETURN_BANK`: The risk of a bank-initiated return (for example, an R01/NSF) is too high to guarantee this transfer.  `RETURN_CUSTOMER`: The risk of a customer-initiated return (for example, a R10/Unauthorized) is too high to guarantee this transfer.  `GUARANTEE_LIMIT_REACHED`: This transfer is low-risk, but Guaranteed ACH has exhausted an internal limit on the number or rate of guarantees that applies to this transfer.  `RISK_ESTIMATE_UNAVAILABLE`: A risk estimate is unavailable for this Item.., must be one of ["RETURN_BANK", "RETURN_CUSTOMER", "GUARANTEE_LIMIT_REACHED", "RISK_ESTIMATE_UNAVAILABLE", ]  # noqa: E501
+            args[0] (str): A code representing the reason Plaid declined to guarantee this transfer:  `RETURN_BANK`: The risk of a bank-initiated return (for example, an R01/NSF) is too high to guarantee this transfer.  `RETURN_CUSTOMER`: The risk of a customer-initiated return (for example, a R10/Unauthorized) is too high to guarantee this transfer.  `GUARANTEE_LIMIT_REACHED`: This transfer is low-risk, but Guaranteed ACH has exhausted an internal limit on the number or rate of guarantees that applies to this transfer.  `RISK_ESTIMATE_UNAVAILABLE`: A risk estimate is unavailable for this Item.  `REQUIRED_PARAM_MISSING`: Required fields are missing.., must be one of ["RETURN_BANK", "RETURN_CUSTOMER", "GUARANTEE_LIMIT_REACHED", "RISK_ESTIMATE_UNAVAILABLE", "REQUIRED_PARAM_MISSING", ]  # noqa: E501
 
         Keyword Args:
-            value (str): A code representing the reason Plaid declined to guarantee this transfer:  `RETURN_BANK`: The risk of a bank-initiated return (for example, an R01/NSF) is too high to guarantee this transfer.  `RETURN_CUSTOMER`: The risk of a customer-initiated return (for example, a R10/Unauthorized) is too high to guarantee this transfer.  `GUARANTEE_LIMIT_REACHED`: This transfer is low-risk, but Guaranteed ACH has exhausted an internal limit on the number or rate of guarantees that applies to this transfer.  `RISK_ESTIMATE_UNAVAILABLE`: A risk estimate is unavailable for this Item.., must be one of ["RETURN_BANK", "RETURN_CUSTOMER", "GUARANTEE_LIMIT_REACHED", "RISK_ESTIMATE_UNAVAILABLE", ]  # noqa: E501
+            value (str): A code representing the reason Plaid declined to guarantee this transfer:  `RETURN_BANK`: The risk of a bank-initiated return (for example, an R01/NSF) is too high to guarantee this transfer.  `RETURN_CUSTOMER`: The risk of a customer-initiated return (for example, a R10/Unauthorized) is too high to guarantee this transfer.  `GUARANTEE_LIMIT_REACHED`: This transfer is low-risk, but Guaranteed ACH has exhausted an internal limit on the number or rate of guarantees that applies to this transfer.  `RISK_ESTIMATE_UNAVAILABLE`: A risk estimate is unavailable for this Item.  `REQUIRED_PARAM_MISSING`: Required fields are missing.., must be one of ["RETURN_BANK", "RETURN_CUSTOMER", "GUARANTEE_LIMIT_REACHED", "RISK_ESTIMATE_UNAVAILABLE", "REQUIRED_PARAM_MISSING", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `plaid-python-9.8.0/plaid/model/watchlist_screening_individual_name.py` & `plaid-python-9.9.0/plaid/model/watchlist_screening_individual_name.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/get_entity_watchlist_screening_request.py` & `plaid-python-9.9.0/plaid/model/get_entity_watchlist_screening_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_maximum_payment_amount.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_maximum_payment_amount.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_refresh_response.py` & `plaid-python-9.9.0/plaid/model/asset_report_refresh_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_transaction_counterparty_international.py` & `plaid-python-9.9.0/plaid/model/wallet_transaction_counterparty_international.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_metadata.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_metadata.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_profile_create_response.py` & `plaid-python-9.9.0/plaid/model/payment_profile_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_audit_copy_remove_response.py` & `plaid-python-9.9.0/plaid/model/asset_report_audit_copy_remove_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/simulated_transfer_sweep.py` & `plaid-python-9.9.0/plaid/model/simulated_transfer_sweep.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/id_number_type.py` & `plaid-python-9.9.0/plaid/model/id_number_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paginated_entity_watchlist_program_list_response.py` & `plaid-python-9.9.0/plaid/model/paginated_entity_watchlist_program_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/student_loan.py` & `plaid-python-9.9.0/plaid/model/student_loan.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/doc_type.py` & `plaid-python-9.9.0/plaid/model/doc_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             'DOCUMENT_TYPE_US_TAX_W2': "DOCUMENT_TYPE_US_TAX_W2",
             'DOCUMENT_TYPE_US_MILITARY_ERAS': "DOCUMENT_TYPE_US_MILITARY_ERAS",
             'DOCUMENT_TYPE_US_MILITARY_LES': "DOCUMENT_TYPE_US_MILITARY_LES",
             'DOCUMENT_TYPE_US_MILITARY_CLES': "DOCUMENT_TYPE_US_MILITARY_CLES",
             'DOCUMENT_TYPE_GIG': "DOCUMENT_TYPE_GIG",
             'DOCUMENT_TYPE_NONE': "DOCUMENT_TYPE_NONE",
             'DOCUMENT_TYPE_US_TAX_1099_MISC': "DOCUMENT_TYPE_US_TAX_1099_MISC",
+            'DOCUMENT_TYPE_US_TAX_1099_K': "DOCUMENT_TYPE_US_TAX_1099_K",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -102,18 +103,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """DocType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): The type of document.  `DOCUMENT_TYPE_PAYSTUB`: A paystub.  `DOCUMENT_TYPE_BANK_STATEMENT`: A bank statement.  `DOCUMENT_TYPE_US_TAX_W2`: A W-2 wage and tax statement provided by a US employer reflecting wages earned by the employee.  `DOCUMENT_TYPE_US_MILITARY_ERAS`: An electronic Retirement Account Statement (eRAS) issued by the US military.  `DOCUMENT_TYPE_US_MILITARY_LES`: A Leave and Earnings Statement (LES) issued by the US military.  `DOCUMENT_TYPE_US_MILITARY_CLES`: A Civilian Leave and Earnings Statment (CLES) issued by the US military.  `DOCUMENT_TYPE_GIG`: Used to indicate that the income is related to gig work. Does not necessarily correspond to a specific document type.  `DOCUMENT_TYPE_NONE`: Used to indicate that there is no underlying document for the data.  `UNKNOWN`: Document type could not be determined.., must be one of ["UNKNOWN", "DOCUMENT_TYPE_PAYSTUB", "DOCUMENT_TYPE_BANK_STATEMENT", "DOCUMENT_TYPE_US_TAX_W2", "DOCUMENT_TYPE_US_MILITARY_ERAS", "DOCUMENT_TYPE_US_MILITARY_LES", "DOCUMENT_TYPE_US_MILITARY_CLES", "DOCUMENT_TYPE_GIG", "DOCUMENT_TYPE_NONE", "DOCUMENT_TYPE_US_TAX_1099_MISC", ]  # noqa: E501
+            args[0] (str): The type of document.  `DOCUMENT_TYPE_PAYSTUB`: A paystub.  `DOCUMENT_TYPE_BANK_STATEMENT`: A bank statement.  `DOCUMENT_TYPE_US_TAX_W2`: A W-2 wage and tax statement provided by a US employer reflecting wages earned by the employee.  `DOCUMENT_TYPE_US_MILITARY_ERAS`: An electronic Retirement Account Statement (eRAS) issued by the US military.  `DOCUMENT_TYPE_US_MILITARY_LES`: A Leave and Earnings Statement (LES) issued by the US military.  `DOCUMENT_TYPE_US_MILITARY_CLES`: A Civilian Leave and Earnings Statment (CLES) issued by the US military.  `DOCUMENT_TYPE_GIG`: Used to indicate that the income is related to gig work. Does not necessarily correspond to a specific document type.  `DOCUMENT_TYPE_NONE`: Used to indicate that there is no underlying document for the data.  `UNKNOWN`: Document type could not be determined.., must be one of ["UNKNOWN", "DOCUMENT_TYPE_PAYSTUB", "DOCUMENT_TYPE_BANK_STATEMENT", "DOCUMENT_TYPE_US_TAX_W2", "DOCUMENT_TYPE_US_MILITARY_ERAS", "DOCUMENT_TYPE_US_MILITARY_LES", "DOCUMENT_TYPE_US_MILITARY_CLES", "DOCUMENT_TYPE_GIG", "DOCUMENT_TYPE_NONE", "DOCUMENT_TYPE_US_TAX_1099_MISC", "DOCUMENT_TYPE_US_TAX_1099_K", ]  # noqa: E501
 
         Keyword Args:
-            value (str): The type of document.  `DOCUMENT_TYPE_PAYSTUB`: A paystub.  `DOCUMENT_TYPE_BANK_STATEMENT`: A bank statement.  `DOCUMENT_TYPE_US_TAX_W2`: A W-2 wage and tax statement provided by a US employer reflecting wages earned by the employee.  `DOCUMENT_TYPE_US_MILITARY_ERAS`: An electronic Retirement Account Statement (eRAS) issued by the US military.  `DOCUMENT_TYPE_US_MILITARY_LES`: A Leave and Earnings Statement (LES) issued by the US military.  `DOCUMENT_TYPE_US_MILITARY_CLES`: A Civilian Leave and Earnings Statment (CLES) issued by the US military.  `DOCUMENT_TYPE_GIG`: Used to indicate that the income is related to gig work. Does not necessarily correspond to a specific document type.  `DOCUMENT_TYPE_NONE`: Used to indicate that there is no underlying document for the data.  `UNKNOWN`: Document type could not be determined.., must be one of ["UNKNOWN", "DOCUMENT_TYPE_PAYSTUB", "DOCUMENT_TYPE_BANK_STATEMENT", "DOCUMENT_TYPE_US_TAX_W2", "DOCUMENT_TYPE_US_MILITARY_ERAS", "DOCUMENT_TYPE_US_MILITARY_LES", "DOCUMENT_TYPE_US_MILITARY_CLES", "DOCUMENT_TYPE_GIG", "DOCUMENT_TYPE_NONE", "DOCUMENT_TYPE_US_TAX_1099_MISC", ]  # noqa: E501
+            value (str): The type of document.  `DOCUMENT_TYPE_PAYSTUB`: A paystub.  `DOCUMENT_TYPE_BANK_STATEMENT`: A bank statement.  `DOCUMENT_TYPE_US_TAX_W2`: A W-2 wage and tax statement provided by a US employer reflecting wages earned by the employee.  `DOCUMENT_TYPE_US_MILITARY_ERAS`: An electronic Retirement Account Statement (eRAS) issued by the US military.  `DOCUMENT_TYPE_US_MILITARY_LES`: A Leave and Earnings Statement (LES) issued by the US military.  `DOCUMENT_TYPE_US_MILITARY_CLES`: A Civilian Leave and Earnings Statment (CLES) issued by the US military.  `DOCUMENT_TYPE_GIG`: Used to indicate that the income is related to gig work. Does not necessarily correspond to a specific document type.  `DOCUMENT_TYPE_NONE`: Used to indicate that there is no underlying document for the data.  `UNKNOWN`: Document type could not be determined.., must be one of ["UNKNOWN", "DOCUMENT_TYPE_PAYSTUB", "DOCUMENT_TYPE_BANK_STATEMENT", "DOCUMENT_TYPE_US_TAX_W2", "DOCUMENT_TYPE_US_MILITARY_ERAS", "DOCUMENT_TYPE_US_MILITARY_LES", "DOCUMENT_TYPE_US_MILITARY_CLES", "DOCUMENT_TYPE_GIG", "DOCUMENT_TYPE_NONE", "DOCUMENT_TYPE_US_TAX_1099_MISC", "DOCUMENT_TYPE_US_TAX_1099_K", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `plaid-python-9.8.0/plaid/model/client_provided_enhanced_transaction.py` & `plaid-python-9.9.0/plaid/model/client_provided_enhanced_transaction.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/kyc_check_details.py` & `plaid-python-9.9.0/plaid/model/kyc_check_details.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/phone_type.py` & `plaid-python-9.9.0/plaid/model/phone_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_authorization_decision.py` & `plaid-python-9.9.0/plaid/model/transfer_authorization_decision.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_list_response.py` & `plaid-python-9.9.0/plaid/model/transfer_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_precheck_response.py` & `plaid-python-9.9.0/plaid/model/income_verification_precheck_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/deposit_switch_address_data.py` & `plaid-python-9.9.0/plaid/model/deposit_switch_address_data.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_verification_retry_request.py` & `plaid-python-9.9.0/plaid/model/identity_verification_retry_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/employee.py` & `plaid-python-9.9.0/plaid/model/employee.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_create_response.py` & `plaid-python-9.9.0/plaid/model/wallet_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_refund_status.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_refund_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/investments_default_update_webhook.py` & `plaid-python-9.9.0/plaid/model/investments_default_update_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/assets_error_webhook.py` & `plaid-python-9.9.0/plaid/model/assets_error_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paginated_entity_watchlist_screening_hit_list_response.py` & `plaid-python-9.9.0/plaid/model/paginated_entity_watchlist_screening_hit_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/get_dashboard_user_request.py` & `plaid-python-9.9.0/plaid/model/get_dashboard_user_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_network.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_network.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/assets_product_ready_webhook.py` & `plaid-python-9.9.0/plaid/model/assets_product_ready_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/processor_apex_processor_token_create_request.py` & `plaid-python-9.9.0/plaid/model/processor_apex_processor_token_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_pay_stub_verification.py` & `plaid-python-9.9.0/plaid/model/credit_pay_stub_verification.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_payment_reverse_response.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_payment_reverse_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_get_response.py` & `plaid-python-9.9.0/plaid/model/transfer_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_consent_get_response.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_consent_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_paystubs_get_request.py` & `plaid-python-9.9.0/plaid/model/income_verification_paystubs_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_transaction_counterparty.py` & `plaid-python-9.9.0/plaid/model/wallet_transaction_counterparty.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/po_box_status.py` & `plaid-python-9.9.0/plaid/model/po_box_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/investment_transaction_subtype.py` & `plaid-python-9.9.0/plaid/model/investment_transaction_subtype.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_watchlist_screening_review.py` & `plaid-python-9.9.0/plaid/model/entity_watchlist_screening_review.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_payroll_income_risk_signals_get_response.py` & `plaid-python-9.9.0/plaid/model/credit_payroll_income_risk_signals_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_precheck_military_info.py` & `plaid-python-9.9.0/plaid/model/income_verification_precheck_military_info.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_refresh_request.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_refresh_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/document_name_match_code.py` & `plaid-python-9.9.0/plaid/model/document_name_match_code.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_request_update.py` & `plaid-python-9.9.0/plaid/model/link_token_create_request_update.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transaction_stream.py` & `plaid-python-9.9.0/plaid/model/transaction_stream.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_create_response.py` & `plaid-python-9.9.0/plaid/model/income_verification_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payroll_risk_signals_item.py` & `plaid-python-9.9.0/plaid/model/payroll_risk_signals_item.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/watchlist_screening_phone_number.py` & `plaid-python-9.9.0/plaid/model/watchlist_screening_phone_number.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/dashboard_user_status.py` & `plaid-python-9.9.0/plaid/model/dashboard_user_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_employer_verification.py` & `plaid-python-9.9.0/plaid/model/credit_employer_verification.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_consent_create_response.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_consent_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/address_nullable.py` & `plaid-python-9.9.0/plaid/model/address_nullable.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/watchlist_screening_search_terms.py` & `plaid-python-9.9.0/plaid/model/watchlist_screening_search_terms.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_event_type.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_event_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_access_token_invalidate_response.py` & `plaid-python-9.9.0/plaid/model/item_access_token_invalidate_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paystub_deduction.py` & `plaid-python-9.9.0/plaid/model/paystub_deduction.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/deposit_switch_create_request_options.py` & `plaid-python-9.9.0/plaid/model/deposit_switch_create_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_user.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_user.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_account_type.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_account_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_match_request.py` & `plaid-python-9.9.0/plaid/model/identity_match_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_warning_code.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_warning_code.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_verification_step_status.py` & `plaid-python-9.9.0/plaid/model/identity_verification_step_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_audit_copy_token_remove_response.py` & `plaid-python-9.9.0/plaid/model/credit_audit_copy_token_remove_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/get_watchlist_screening_individual_program_request.py` & `plaid-python-9.9.0/plaid/model/get_watchlist_screening_individual_program_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_document_metadata.py` & `plaid-python-9.9.0/plaid/model/credit_document_metadata.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/application_get_request.py` & `plaid-python-9.9.0/plaid/model/application_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/investments_transactions_override.py` & `plaid-python-9.9.0/plaid/model/investments_transactions_override.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/deposit_switch_get_response.py` & `plaid-python-9.9.0/plaid/model/deposit_switch_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_audit_copy_create_response.py` & `plaid-python-9.9.0/plaid/model/asset_report_audit_copy_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/historical_update_webhook.py` & `plaid-python-9.9.0/plaid/model/historical_update_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_create_response.py` & `plaid-python-9.9.0/plaid/model/asset_report_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/deposit_switch_target_account.py` & `plaid-python-9.9.0/plaid/model/deposit_switch_target_account.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/standalone_account_type.py` & `plaid-python-9.9.0/plaid/model/standalone_account_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/product_status_breakdown.py` & `plaid-python-9.9.0/plaid/model/product_status_breakdown.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/source.py` & `plaid-python-9.9.0/plaid/model/source.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_screening_hit_phone_numbers.py` & `plaid-python-9.9.0/plaid/model/entity_screening_hit_phone_numbers.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_get_response.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_failure.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_failure.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_event_sync_request.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_event_sync_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_card_liability.py` & `plaid-python-9.9.0/plaid/model/credit_card_liability.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/signal_prepare_request.py` & `plaid-python-9.9.0/plaid/model/signal_prepare_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_item_fire_webhook_response.py` & `plaid-python-9.9.0/plaid/model/sandbox_item_fire_webhook_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/watchlist_screening_hit_status.py` & `plaid-python-9.9.0/plaid/model/watchlist_screening_hit_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_sweep.py` & `plaid-python-9.9.0/plaid/model/transfer_sweep.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/watchlist_screening_create_request.py` & `plaid-python-9.9.0/plaid/model/watchlist_screening_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_consent_payment_execute_response.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_consent_payment_execute_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_status_update_webhook.py` & `plaid-python-9.9.0/plaid/model/payment_status_update_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/employer_verification.py` & `plaid-python-9.9.0/plaid/model/employer_verification.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/verification_attribute.py` & `plaid-python-9.9.0/plaid/model/verification_attribute.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_rule_type.py` & `plaid-python-9.9.0/plaid/model/transactions_rule_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_status_webhook.py` & `plaid-python-9.9.0/plaid/model/income_verification_status_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_recurring_get_request_options.py` & `plaid-python-9.9.0/plaid/model/transactions_recurring_get_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_rules_create_request.py` & `plaid-python-9.9.0/plaid/model/transactions_rules_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/kyc_check_id_number_summary.py` & `plaid-python-9.9.0/plaid/model/kyc_check_id_number_summary.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/signal_score.py` & `plaid-python-9.9.0/plaid/model/signal_score.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/account_type.py` & `plaid-python-9.9.0/plaid/model/account_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_create_request_options.py` & `plaid-python-9.9.0/plaid/model/income_verification_create_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/institution_status.py` & `plaid-python-9.9.0/plaid/model/institution_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_income_fire_webhook_response.py` & `plaid-python-9.9.0/plaid/model/sandbox_income_fire_webhook_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/account_subtype.py` & `plaid-python-9.9.0/plaid/model/account_subtype.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/accounts_balance_get_request.py` & `plaid-python-9.9.0/plaid/model/accounts_balance_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/user_create_response.py` & `plaid-python-9.9.0/plaid/model/user_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/list_watchlist_screening_individual_reviews_request.py` & `plaid-python-9.9.0/plaid/model/list_watchlist_screening_individual_reviews_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_bank_transfer_simulate_response.py` & `plaid-python-9.9.0/plaid/model/sandbox_bank_transfer_simulate_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_sync_response.py` & `plaid-python-9.9.0/plaid/model/transactions_sync_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/processor_stripe_bank_account_token_create_request.py` & `plaid-python-9.9.0/plaid/model/processor_stripe_bank_account_token_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_intent_create_mode.py` & `plaid-python-9.9.0/plaid/model/transfer_intent_create_mode.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/institutions_get_by_id_request.py` & `plaid-python-9.9.0/plaid/model/institutions_get_by_id_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_repayment_return_list_request.py` & `plaid-python-9.9.0/plaid/model/transfer_repayment_return_list_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transaction_data.py` & `plaid-python-9.9.0/plaid/model/transaction_data.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/dashboard_user_response.py` & `plaid-python-9.9.0/plaid/model/dashboard_user_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/signal_return_report_request.py` & `plaid-python-9.9.0/plaid/model/signal_return_report_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_refresh_request.py` & `plaid-python-9.9.0/plaid/model/transactions_refresh_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/warning.py` & `plaid-python-9.9.0/plaid/model/warning.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/liabilities_get_request_options.py` & `plaid-python-9.9.0/plaid/model/liabilities_get_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/watchlist_screening_status.py` & `plaid-python-9.9.0/plaid/model/watchlist_screening_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_sweep_list_response.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_sweep_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_sync_request.py` & `plaid-python-9.9.0/plaid/model/transactions_sync_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_get_response.py` & `plaid-python-9.9.0/plaid/model/identity_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_summary_field_string.py` & `plaid-python-9.9.0/plaid/model/income_summary_field_string.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/watchlist_screening_request_search_terms.py` & `plaid-python-9.9.0/plaid/model/watchlist_screening_request_search_terms.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/screening_hit_names_items.py` & `plaid-python-9.9.0/plaid/model/screening_hit_names_items.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_transaction_counterparty_bacs.py` & `plaid-python-9.9.0/plaid/model/wallet_transaction_counterparty_bacs.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_user_in_request.py` & `plaid-python-9.9.0/plaid/model/transfer_user_in_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/institutions_search_account_filter.py` & `plaid-python-9.9.0/plaid/model/institutions_search_account_filter.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/investments_holdings_get_request.py` & `plaid-python-9.9.0/plaid/model/investments_holdings_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paginated_dashboard_user_list_response.py` & `plaid-python-9.9.0/plaid/model/paginated_dashboard_user_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_consent_constraints.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_consent_constraints.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paystub_employer.py` & `plaid-python-9.9.0/plaid/model/paystub_employer.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_rules_remove_response.py` & `plaid-python-9.9.0/plaid/model/transactions_rules_remove_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_rules_list_response.py` & `plaid-python-9.9.0/plaid/model/transactions_rules_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/numbers_eft.py` & `plaid-python-9.9.0/plaid/model/numbers_eft.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_processor_token_create_request.py` & `plaid-python-9.9.0/plaid/model/sandbox_processor_token_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/net_pay.py` & `plaid-python-9.9.0/plaid/model/net_pay.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/account_subtypes.py` & `plaid-python-9.9.0/plaid/model/account_subtypes.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_document_type.py` & `plaid-python-9.9.0/plaid/model/entity_document_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_public_token_create_request_options_transactions.py` & `plaid-python-9.9.0/plaid/model/sandbox_public_token_create_request_options_transactions.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_consent_periodic_alignment.py` & `plaid-python-9.9.0/plaid/model/payment_consent_periodic_alignment.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/processor_balance_get_request_options.py` & `plaid-python-9.9.0/plaid/model/processor_balance_get_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_application_list_request.py` & `plaid-python-9.9.0/plaid/model/item_application_list_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_migrate_account_request.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_migrate_account_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_product_ready_webhook.py` & `plaid-python-9.9.0/plaid/model/item_product_ready_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_get_request_options.py` & `plaid-python-9.9.0/plaid/model/identity_get_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_item_set_verification_status_request.py` & `plaid-python-9.9.0/plaid/model/sandbox_item_set_verification_status_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_update_types.py` & `plaid-python-9.9.0/plaid/model/identity_update_types.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_audit_copy_token_remove_request.py` & `plaid-python-9.9.0/plaid/model/credit_audit_copy_token_remove_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_get_response.py` & `plaid-python-9.9.0/plaid/model/asset_report_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_intent_get_request.py` & `plaid-python-9.9.0/plaid/model/transfer_intent_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/holding.py` & `plaid-python-9.9.0/plaid/model/holding.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_remove_response.py` & `plaid-python-9.9.0/plaid/model/item_remove_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_intent_authorization_decision.py` & `plaid-python-9.9.0/plaid/model/transfer_intent_authorization_decision.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/user_name.py` & `plaid-python-9.9.0/plaid/model/user_name.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_audit_copy_get_request.py` & `plaid-python-9.9.0/plaid/model/asset_report_audit_copy_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_pay_stub_employee.py` & `plaid-python-9.9.0/plaid/model/credit_pay_stub_employee.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_user.py` & `plaid-python-9.9.0/plaid/model/asset_report_user.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_watchlist_program_response.py` & `plaid-python-9.9.0/plaid/model/entity_watchlist_program_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_get_request.py` & `plaid-python-9.9.0/plaid/model/link_token_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/application.py` & `plaid-python-9.9.0/plaid/model/application.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_watchlist_code.py` & `plaid-python-9.9.0/plaid/model/entity_watchlist_code.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/standalone_currency_code_list.py` & `plaid-python-9.9.0/plaid/model/standalone_currency_code_list.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_request_identity_verification.py` & `plaid-python-9.9.0/plaid/model/link_token_create_request_identity_verification.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,25 +67,27 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'template_id': (str,),  # noqa: E501
-            'consent': (bool,),  # noqa: E501
+            'consent': (object,),  # noqa: E501
+            'gave_consent': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'template_id': 'template_id',  # noqa: E501
         'consent': 'consent',  # noqa: E501
+        'gave_consent': 'gave_consent',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
@@ -129,15 +131,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            consent (bool): A flag specifying whether the end user has already agreed to a privacy policy specifying that their data will be shared with Plaid for verification purposes.  If `gave_consent` is set to `true`, the `accept_tos` step will be marked as `skipped` and the end user's session will start at the next step requirement.. [optional] if omitted the server will use the default value of False  # noqa: E501
+            consent (object): [optional]  # noqa: E501
+            gave_consent (bool): A flag specifying whether the end user has already agreed to a privacy policy specifying that their data will be shared with Plaid for verification purposes.  If `gave_consent` is set to `true`, the `accept_tos` step will be marked as `skipped` and the end user's session will start at the next step requirement.. [optional] if omitted the server will use the default value of False  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `plaid-python-9.8.0/plaid/model/signal_evaluate_core_attributes.py` & `plaid-python-9.9.0/plaid/model/signal_evaluate_core_attributes.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/update_entity_screening_request_resettable_field_list.py` & `plaid-python-9.9.0/plaid/model/update_entity_screening_request_resettable_field_list.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_migrate_account_response.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_migrate_account_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/ach_class.py` & `plaid-python-9.9.0/plaid/model/ach_class.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_refresh_response.py` & `plaid-python-9.9.0/plaid/model/income_verification_refresh_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/signal_address_data.py` & `plaid-python-9.9.0/plaid/model/signal_address_data.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/address_data_nullable.py` & `plaid-python-9.9.0/plaid/model/address_data_nullable.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_pdf_get_request.py` & `plaid-python-9.9.0/plaid/model/asset_report_pdf_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/pay_stub_earnings_breakdown.py` & `plaid-python-9.9.0/plaid/model/pay_stub_earnings_breakdown.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/client_user_id.py` & `plaid-python-9.9.0/plaid/model/client_user_id.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_create_request.py` & `plaid-python-9.9.0/plaid/model/wallet_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/student_repayment_plan.py` & `plaid-python-9.9.0/plaid/model/student_repayment_plan.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/jwk_public_key.py` & `plaid-python-9.9.0/plaid/model/jwk_public_key.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_create_response.py` & `plaid-python-9.9.0/plaid/model/transfer_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_pay_stub_earnings.py` & `plaid-python-9.9.0/plaid/model/credit_pay_stub_earnings.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_rules_create_response.py` & `plaid-python-9.9.0/plaid/model/transactions_rules_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/override_accounts.py` & `plaid-python-9.9.0/plaid/model/override_accounts.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_watchlist_screening_program_name.py` & `plaid-python-9.9.0/plaid/model/entity_watchlist_screening_program_name.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/assets_relay_webhook.py` & `plaid-python-9.9.0/plaid/model/assets_relay_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_get_metadata_response.py` & `plaid-python-9.9.0/plaid/model/link_token_get_metadata_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paystub_override.py` & `plaid-python-9.9.0/plaid/model/paystub_override.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_credit_filter.py` & `plaid-python-9.9.0/plaid/model/link_token_create_credit_filter.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_transaction_execute_request.py` & `plaid-python-9.9.0/plaid/model/wallet_transaction_execute_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_paystubs_get_response.py` & `plaid-python-9.9.0/plaid/model/income_verification_paystubs_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_get_response.py` & `plaid-python-9.9.0/plaid/model/link_token_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_pay_stub_address.py` & `plaid-python-9.9.0/plaid/model/credit_pay_stub_address.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/multi_document_risk_signal.py` & `plaid-python-9.9.0/plaid/model/multi_document_risk_signal.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payroll_item.py` & `plaid-python-9.9.0/plaid/model/payroll_item.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transaction.py` & `plaid-python-9.9.0/plaid/model/transaction.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_pay_stub_net_pay.py` & `plaid-python-9.9.0/plaid/model/credit_pay_stub_net_pay.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_item_reset_login_response.py` & `plaid-python-9.9.0/plaid/model/sandbox_item_reset_login_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_verification_status_updated_webhook.py` & `plaid-python-9.9.0/plaid/model/identity_verification_status_updated_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/account_filters_response.py` & `plaid-python-9.9.0/plaid/model/account_filters_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_recipient_get_request.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_recipient_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_get_response.py` & `plaid-python-9.9.0/plaid/model/item_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_consent_periodic_amount_amount.py` & `plaid-python-9.9.0/plaid/model/payment_consent_periodic_amount_amount.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_transfer_repayment_simulate_response.py` & `plaid-python-9.9.0/plaid/model/sandbox_transfer_repayment_simulate_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_public_token_create_request_options.py` & `plaid-python-9.9.0/plaid/model/sandbox_public_token_create_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_watchlist_search_terms.py` & `plaid-python-9.9.0/plaid/model/entity_watchlist_search_terms.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_screening_hit_emails_items.py` & `plaid-python-9.9.0/plaid/model/entity_screening_hit_emails_items.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_transaction_all_of.py` & `plaid-python-9.9.0/plaid/model/asset_report_transaction_all_of.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_screening_hit_names_items.py` & `plaid-python-9.9.0/plaid/model/entity_screening_hit_names_items.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/webhook_type.py` & `plaid-python-9.9.0/plaid/model/webhook_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_status.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class TransferStatus(ModelSimple):
+class BankTransferStatus(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -48,15 +48,14 @@
     allowed_values = {
         ('value',): {
             'PENDING': "pending",
             'POSTED': "posted",
             'CANCELLED': "cancelled",
             'FAILED': "failed",
             'REVERSED': "reversed",
-            'RETURNED': "returned",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -93,23 +92,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """TransferStatus - a model defined in OpenAPI
+        """BankTransferStatus - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): The status of the transfer.., must be one of ["pending", "posted", "cancelled", "failed", "reversed", "returned", ]  # noqa: E501
+            args[0] (str): The status of the transfer.., must be one of ["pending", "posted", "cancelled", "failed", "reversed", ]  # noqa: E501
 
         Keyword Args:
-            value (str): The status of the transfer.., must be one of ["pending", "posted", "cancelled", "failed", "reversed", "returned", ]  # noqa: E501
+            value (str): The status of the transfer.., must be one of ["pending", "posted", "cancelled", "failed", "reversed", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `plaid-python-9.8.0/plaid/model/item_access_token_invalidate_request.py` & `plaid-python-9.9.0/plaid/model/item_access_token_invalidate_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/consent_payment_idempotency_key.py` & `plaid-python-9.9.0/plaid/model/consent_payment_idempotency_key.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/depository_account_subtype.py` & `plaid-python-9.9.0/plaid/model/depository_account_subtype.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_recipient_create_response.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_recipient_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_authorization_decision_rationale_code.py` & `plaid-python-9.9.0/plaid/model/transfer_authorization_decision_rationale_code.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_standing_order_metadata.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_standing_order_metadata.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/verification_expired_webhook.py` & `plaid-python-9.9.0/plaid/model/verification_expired_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/taxpayer_id.py` & `plaid-python-9.9.0/plaid/model/taxpayer_id.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/pay_frequency.py` & `plaid-python-9.9.0/plaid/model/pay_frequency.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paystub.py` & `plaid-python-9.9.0/plaid/model/paystub.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/institutions_search_request_options.py` & `plaid-python-9.9.0/plaid/model/institutions_search_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_request.py` & `plaid-python-9.9.0/plaid/model/link_token_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_item.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_item.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/external_payment_schedule_base.py` & `plaid-python-9.9.0/plaid/model/external_payment_schedule_base.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_get_request_options.py` & `plaid-python-9.9.0/plaid/model/transactions_get_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_meta.py` & `plaid-python-9.9.0/plaid/model/payment_meta.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_transaction.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_transaction.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/application_get_response.py` & `plaid-python-9.9.0/plaid/model/application_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_request_payment_initiation.py` & `plaid-python-9.9.0/plaid/model/link_token_create_request_payment_initiation.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_numbers.py` & `plaid-python-9.9.0/plaid/model/wallet_numbers.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/account_identity.py` & `plaid-python-9.9.0/plaid/model/account_identity.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_profile_remove_response.py` & `plaid-python-9.9.0/plaid/model/payment_profile_remove_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_event_sync_response.py` & `plaid-python-9.9.0/plaid/model/transfer_event_sync_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/enhancements.py` & `plaid-python-9.9.0/plaid/model/enhancements.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
             'category': ([str],),  # noqa: E501
             'location': (Location,),  # noqa: E501
             'merchant_name': (str, none_type,),  # noqa: E501
             'website': (str, none_type,),  # noqa: E501
             'logo_url': (str, none_type,),  # noqa: E501
             'check_number': (str, none_type,),  # noqa: E501
             'personal_finance_category': (PersonalFinanceCategory,),  # noqa: E501
+            'personal_finance_category_icon_url': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -108,14 +109,15 @@
         'category': 'category',  # noqa: E501
         'location': 'location',  # noqa: E501
         'merchant_name': 'merchant_name',  # noqa: E501
         'website': 'website',  # noqa: E501
         'logo_url': 'logo_url',  # noqa: E501
         'check_number': 'check_number',  # noqa: E501
         'personal_finance_category': 'personal_finance_category',  # noqa: E501
+        'personal_finance_category_icon_url': 'personal_finance_category_icon_url',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
@@ -167,14 +169,15 @@
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             merchant_name (str, none_type): The merchant name, as extracted by Plaid from the raw description.. [optional]  # noqa: E501
             website (str, none_type): The website associated with this transaction.. [optional]  # noqa: E501
             logo_url (str, none_type): A link to the logo associated with this transaction. The logo will always be 100x100 resolution.. [optional]  # noqa: E501
             check_number (str, none_type): The check number of the transaction. This field is only populated for check transactions.. [optional]  # noqa: E501
             personal_finance_category (PersonalFinanceCategory): [optional]  # noqa: E501
+            personal_finance_category_icon_url (str): A link to the icon associated with the primary personal finance category. The logo will always be 100x100 resolution.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_event_sync_response.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_event_sync_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/new_accounts_available_webhook.py` & `plaid-python-9.9.0/plaid/model/new_accounts_available_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_rules_remove_request.py` & `plaid-python-9.9.0/plaid/model/transactions_rules_remove_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/deposit_switch_target_user.py` & `plaid-python-9.9.0/plaid/model/deposit_switch_target_user.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/list_entity_watchlist_screening_request.py` & `plaid-python-9.9.0/plaid/model/list_entity_watchlist_screening_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/expiration_date.py` & `plaid-python-9.9.0/plaid/model/expiration_date.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/processor_token_create_response.py` & `plaid-python-9.9.0/plaid/model/processor_token_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/deposit_switch_create_request.py` & `plaid-python-9.9.0/plaid/model/deposit_switch_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_scheme.py` & `plaid-python-9.9.0/plaid/model/payment_scheme.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/category.py` & `plaid-python-9.9.0/plaid/model/category.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_amount_currency.py` & `plaid-python-9.9.0/plaid/model/payment_amount_currency.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_public_token_create_response.py` & `plaid-python-9.9.0/plaid/model/item_public_token_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_get_request.py` & `plaid-python-9.9.0/plaid/model/transfer_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_warning_type.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_warning_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_consent_get_request.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_consent_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_precheck_request.py` & `plaid-python-9.9.0/plaid/model/income_verification_precheck_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/external_payment_refund_details.py` & `plaid-python-9.9.0/plaid/model/external_payment_refund_details.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_channel.py` & `plaid-python-9.9.0/plaid/model/payment_channel.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/owner.py` & `plaid-python-9.9.0/plaid/model/owner.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/categories_get_response.py` & `plaid-python-9.9.0/plaid/model/categories_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_taxforms_get_request.py` & `plaid-python-9.9.0/plaid/model/income_verification_taxforms_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_repayment_list_request.py` & `plaid-python-9.9.0/plaid/model/transfer_repayment_list_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/jwt_header.py` & `plaid-python-9.9.0/plaid/model/jwt_header.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transaction_all_of.py` & `plaid-python-9.9.0/plaid/model/transaction_all_of.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/institutions_get_response.py` & `plaid-python-9.9.0/plaid/model/institutions_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/deposit_switch_alt_create_response.py` & `plaid-python-9.9.0/plaid/model/deposit_switch_alt_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_public_token_create_request.py` & `plaid-python-9.9.0/plaid/model/sandbox_public_token_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer.py` & `plaid-python-9.9.0/plaid/model/transfer.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_screening_hit_data.py` & `plaid-python-9.9.0/plaid/model/entity_screening_hit_data.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_payroll_income_refresh_request.py` & `plaid-python-9.9.0/plaid/model/credit_payroll_income_refresh_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/signal_return_report_response.py` & `plaid-python-9.9.0/plaid/model/signal_return_report_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_employment_get_request.py` & `plaid-python-9.9.0/plaid/model/credit_employment_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/taxform.py` & `plaid-python-9.9.0/plaid/model/taxform.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_create_request.py` & `plaid-python-9.9.0/plaid/model/income_verification_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_sweep_get_request.py` & `plaid-python-9.9.0/plaid/model/transfer_sweep_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_enhance_get_request.py` & `plaid-python-9.9.0/plaid/model/transactions_enhance_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_payment_list_request.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_payment_list_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/liabilities_object.py` & `plaid-python-9.9.0/plaid/model/liabilities_object.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_relay_refresh_response.py` & `plaid-python-9.9.0/plaid/model/asset_report_relay_refresh_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_metadata.py` & `plaid-python-9.9.0/plaid/model/transfer_metadata.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_screening_status_updated_webhook.py` & `plaid-python-9.9.0/plaid/model/entity_screening_status_updated_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/watchlist_screening_review_response.py` & `plaid-python-9.9.0/plaid/model/watchlist_screening_review_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_watchlist_screening_response.py` & `plaid-python-9.9.0/plaid/model/entity_watchlist_screening_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_summary_field_number.py` & `plaid-python-9.9.0/plaid/model/income_summary_field_number.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_public_token_create_request.py` & `plaid-python-9.9.0/plaid/model/item_public_token_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_request_user_stated_income_source.py` & `plaid-python-9.9.0/plaid/model/link_token_create_request_user_stated_income_source.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_schedule_interval.py` & `plaid-python-9.9.0/plaid/model/payment_schedule_interval.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/account_ids_with_updated_identity.py` & `plaid-python-9.9.0/plaid/model/account_ids_with_updated_identity.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paystub_pay_frequency.py` & `plaid-python-9.9.0/plaid/model/paystub_pay_frequency.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/loan_filter.py` & `plaid-python-9.9.0/plaid/model/loan_filter.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/incident_update.py` & `plaid-python-9.9.0/plaid/model/incident_update.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/dashboard_user.py` & `plaid-python-9.9.0/plaid/model/dashboard_user.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_verification.py` & `plaid-python-9.9.0/plaid/model/identity_verification.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_filter_response.py` & `plaid-python-9.9.0/plaid/model/asset_report_filter_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/update_entity_screening_request.py` & `plaid-python-9.9.0/plaid/model/update_entity_screening_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_intent_create_request.py` & `plaid-python-9.9.0/plaid/model/transfer_intent_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item.py` & `plaid-python-9.9.0/plaid/model/item.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 def lazy_import():
-    from plaid.model.error import Error
+    from plaid.model.plaid_error import PlaidError
     from plaid.model.products import Products
-    globals()['Error'] = Error
+    globals()['PlaidError'] = PlaidError
     globals()['Products'] = Products
 
 
 class Item(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -86,15 +86,15 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'item_id': (str,),  # noqa: E501
             'webhook': (str, none_type,),  # noqa: E501
-            'error': (Error,),  # noqa: E501
+            'error': (PlaidError,),  # noqa: E501
             'available_products': ([Products],),  # noqa: E501
             'billed_products': ([Products],),  # noqa: E501
             'consent_expiration_time': (datetime, none_type,),  # noqa: E501
             'update_type': (str,),  # noqa: E501
             'institution_id': (str, none_type,),  # noqa: E501
             'products': ([Products],),  # noqa: E501
             'consented_products': ([Products],),  # noqa: E501
@@ -132,15 +132,15 @@
     @convert_js_args_to_python_args
     def __init__(self, item_id, webhook, error, available_products, billed_products, consent_expiration_time, update_type, *args, **kwargs):  # noqa: E501
         """Item - a model defined in OpenAPI
 
         Args:
             item_id (str): The Plaid Item ID. The `item_id` is always unique; linking the same account at the same institution twice will result in two Items with different `item_id` values. Like all Plaid identifiers, the `item_id` is case-sensitive.
             webhook (str, none_type): The URL registered to receive webhooks for the Item.
-            error (Error):
+            error (PlaidError):
             available_products ([Products]): A list of products available for the Item that have not yet been accessed. The contents of this array will be mutually exclusive with `billed_products`.
             billed_products ([Products]): A list of products that have been billed for the Item. The contents of this array will be mutually exclusive with `available_products`. Note - `billed_products` is populated in all environments but only requests in Production are billed. Also note that products that are billed on a pay-per-call basis rather than a pay-per-Item basis, such as `balance`, will not appear here. 
             consent_expiration_time (datetime, none_type): The RFC 3339 timestamp after which the consent provided by the end user will expire. Upon consent expiration, the item will enter the `ITEM_LOGIN_REQUIRED` error state. To circumvent the `ITEM_LOGIN_REQUIRED` error and maintain continuous consent, the end user can reauthenticate via Link’s update mode in advance of the consent expiration time.  Note - This is only relevant for certain OAuth-based institutions. For all other institutions, this field will be null. 
             update_type (str): Indicates whether an Item requires user interaction to be updated, which can be the case for Items with some forms of two-factor authentication.  `background` - Item can be updated in the background  `user_present_required` - Item requires user interaction to be updated
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
```

### Comparing `plaid-python-9.8.0/plaid/model/transfer_intent_status.py` & `plaid-python-9.9.0/plaid/model/transfer_intent_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_balance_get_response.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_balance_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/product_access.py` & `plaid-python-9.9.0/plaid/model/product_access.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/create_entity_screening_request.py` & `plaid-python-9.9.0/plaid/model/create_entity_screening_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/deposit_switch_alt_create_request.py` & `plaid-python-9.9.0/plaid/model/deposit_switch_alt_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/earnings_breakdown_canonical_description.py` & `plaid-python-9.9.0/plaid/model/earnings_breakdown_canonical_description.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_request_transfer.py` & `plaid-python-9.9.0/plaid/model/liabilities_account_ids_with_updated_liabilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class LinkTokenCreateRequestTransfer(ModelNormal):
+class LiabilitiesAccountIdsWithUpdatedLiabilities(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,39 +51,43 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    additional_properties_type = None
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return ([str],)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'intent_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'intent_id': 'intent_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
@@ -91,15 +95,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """LinkTokenCreateRequestTransfer - a model defined in OpenAPI
+        """LiabilitiesAccountIdsWithUpdatedLiabilities - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -124,15 +128,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            intent_id (str): The `id` returned by the `/transfer/intent/create` endpoint.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `plaid-python-9.8.0/plaid/model/screening_status_updated_webhook.py` & `plaid-python-9.9.0/plaid/model/screening_status_updated_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paystub_verification.py` & `plaid-python-9.9.0/plaid/model/paystub_verification.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/investment_filter.py` & `plaid-python-9.9.0/plaid/model/investment_filter.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/watchlist_screening_document_value.py` & `plaid-python-9.9.0/plaid/model/watchlist_screening_document_value.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_status_nullable.py` & `plaid-python-9.9.0/plaid/model/item_status_nullable.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/verification_status.py` & `plaid-python-9.9.0/plaid/model/verification_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_category_rule.py` & `plaid-python-9.9.0/plaid/model/transactions_category_rule.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_account_subtype.py` & `plaid-python-9.9.0/plaid/model/credit_account_subtype.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_verification_create_request.py` & `plaid-python-9.9.0/plaid/model/identity_verification_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_transaction_execute_response.py` & `plaid-python-9.9.0/plaid/model/wallet_transaction_execute_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/initial_update_webhook.py` & `plaid-python-9.9.0/plaid/model/initial_update_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_create_request.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_webhook_update_request.py` & `plaid-python-9.9.0/plaid/model/item_webhook_update_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/employment_verification_get_request.py` & `plaid-python-9.9.0/plaid/model/employment_verification_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/deposit_switch_get_request.py` & `plaid-python-9.9.0/plaid/model/deposit_switch_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_verification_user_address.py` & `plaid-python-9.9.0/plaid/model/identity_verification_user_address.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_item_reset_login_request.py` & `plaid-python-9.9.0/plaid/model/sandbox_item_reset_login_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_sweep_get_response.py` & `plaid-python-9.9.0/plaid/model/transfer_sweep_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_cancel_request.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_cancel_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/scopes.py` & `plaid-python-9.9.0/plaid/model/scopes.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_metadata.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_metadata.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_verification_template_reference.py` & `plaid-python-9.9.0/plaid/model/identity_verification_template_reference.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_import_response.py` & `plaid-python-9.9.0/plaid/model/item_import_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transaction_override.py` & `plaid-python-9.9.0/plaid/model/transaction_override.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_institution_data.py` & `plaid-python-9.9.0/plaid/model/link_token_create_institution_data.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_relay_get_request.py` & `plaid-python-9.9.0/plaid/model/asset_report_relay_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_list_request.py` & `plaid-python-9.9.0/plaid/model/transfer_list_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_precheck_employer_address.py` & `plaid-python-9.9.0/plaid/model/income_verification_precheck_employer_address.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/processor_identity_get_response.py` & `plaid-python-9.9.0/plaid/model/processor_identity_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_sweep_get_request.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_sweep_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_list_response.py` & `plaid-python-9.9.0/plaid/model/wallet_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/processor_balance_get_response.py` & `plaid-python-9.9.0/plaid/model/processor_balance_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/processor_bank_transfer_create_request.py` & `plaid-python-9.9.0/plaid/model/processor_bank_transfer_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_balance.py` & `plaid-python-9.9.0/plaid/model/wallet_balance.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_cause.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_cause.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/numbers_bacs_nullable.py` & `plaid-python-9.9.0/plaid/model/numbers_bacs_nullable.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_profile_create_request.py` & `plaid-python-9.9.0/plaid/model/payment_profile_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/w2_box12.py` & `plaid-python-9.9.0/plaid/model/w2_box12.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/date_range.py` & `plaid-python-9.9.0/plaid/model/date_range.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_transfer_sweep_simulate_request.py` & `plaid-python-9.9.0/plaid/model/sandbox_transfer_sweep_simulate_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paginated_individual_watchlist_screening_review_list_response.py` & `plaid-python-9.9.0/plaid/model/paginated_individual_watchlist_screening_review_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_initiated_return_risk.py` & `plaid-python-9.9.0/plaid/model/bank_initiated_return_risk.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/mortgage_interest_rate.py` & `plaid-python-9.9.0/plaid/model/mortgage_interest_rate.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/processor_number.py` & `plaid-python-9.9.0/plaid/model/processor_number.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_profile_get_response.py` & `plaid-python-9.9.0/plaid/model/payment_profile_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_get_request.py` & `plaid-python-9.9.0/plaid/model/identity_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/user_id_number.py` & `plaid-python-9.9.0/plaid/model/user_id_number.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/investment_account_subtype.py` & `plaid-python-9.9.0/plaid/model/investment_account_subtype.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/pay_period_details.py` & `plaid-python-9.9.0/plaid/model/pay_period_details.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/recipient_bacs.py` & `plaid-python-9.9.0/plaid/model/recipient_bacs.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_account.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_account.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_summary.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_summary.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_create_idempotency_key.py` & `plaid-python-9.9.0/plaid/model/transfer_create_idempotency_key.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_payroll_income_risk_signals_get_request.py` & `plaid-python-9.9.0/plaid/model/credit_payroll_income_risk_signals_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/match_summary.py` & `plaid-python-9.9.0/plaid/model/match_summary.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_intent_get_failure_reason.py` & `plaid-python-9.9.0/plaid/model/transfer_intent_get_failure_reason.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/apr.py` & `plaid-python-9.9.0/plaid/model/apr.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/institutions_get_by_id_request_options.py` & `plaid-python-9.9.0/plaid/model/institutions_get_by_id_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/investments_holdings_get_response.py` & `plaid-python-9.9.0/plaid/model/investments_holdings_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/servicer_address_data.py` & `plaid-python-9.9.0/plaid/model/servicer_address_data.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/document_date_of_birth_match_code.py` & `plaid-python-9.9.0/plaid/model/document_date_of_birth_match_code.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_recipient_list_response.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_recipient_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_amount.py` & `plaid-python-9.9.0/plaid/model/payment_amount.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/account_product_access.py` & `plaid-python-9.9.0/plaid/model/account_product_access.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_get_request.py` & `plaid-python-9.9.0/plaid/model/item_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/accounts_get_response.py` & `plaid-python-9.9.0/plaid/model/accounts_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/documentary_verification_document.py` & `plaid-python-9.9.0/plaid/model/documentary_verification_document.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_match_user.py` & `plaid-python-9.9.0/plaid/model/identity_match_user.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_item_fire_webhook_request.py` & `plaid-python-9.9.0/plaid/model/sandbox_item_fire_webhook_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     """
 
     allowed_values = {
         ('webhook_code',): {
             'DEFAULT_UPDATE': "DEFAULT_UPDATE",
             'NEW_ACCOUNTS_AVAILABLE': "NEW_ACCOUNTS_AVAILABLE",
             'AUTH_DATA_UPDATE': "AUTH_DATA_UPDATE",
+            'RECURRING_TRANSACTIONS_UPDATE': "RECURRING_TRANSACTIONS_UPDATE",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
```

### Comparing `plaid-python-9.8.0/plaid/model/signal_evaluate_response.py` & `plaid-python-9.9.0/plaid/model/signal_evaluate_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_category.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_category.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/deposit_switch_token_create_response.py` & `plaid-python-9.9.0/plaid/model/deposit_switch_token_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_network.py` & `plaid-python-9.9.0/plaid/model/report_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class TransferNetwork(ModelSimple):
+class ReportType(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -43,16 +43,16 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'ACH': "ach",
-            'SAME-DAY-ACH': "same-day-ach",
+            'ASSETS': "assets",
+            'INCOME': "income",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -89,23 +89,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """TransferNetwork - a model defined in OpenAPI
+        """ReportType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): The network or rails used for the transfer. Valid options are `ach` or `same-day-ach`.., must be one of ["ach", "same-day-ach", ]  # noqa: E501
+            args[0] (str): The report type. It can be `assets` or `income`.., must be one of ["assets", "income", ]  # noqa: E501
 
         Keyword Args:
-            value (str): The network or rails used for the transfer. Valid options are `ach` or `same-day-ach`.., must be one of ["ach", "same-day-ach", ]  # noqa: E501
+            value (str): The report type. It can be `assets` or `income`.., must be one of ["assets", "income", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_get_request.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/numbers_international_iban.py` & `plaid-python-9.9.0/plaid/model/numbers_international_iban.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transaction_code.py` & `plaid-python-9.9.0/plaid/model/transaction_code.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/plaid_error.py` & `plaid-python-9.9.0/plaid/model/plaid_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
         lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
-    _nullable = False
+    _nullable = True
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
```

### Comparing `plaid-python-9.8.0/plaid/model/transfer_authorization_guarantee_decision.py` & `plaid-python-9.9.0/plaid/model/transfer_authorization_guarantee_decision.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/holdings_override.py` & `plaid-python-9.9.0/plaid/model/holdings_override.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/kyc_check_date_of_birth_summary.py` & `plaid-python-9.9.0/plaid/model/kyc_check_date_of_birth_summary.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_get_request.py` & `plaid-python-9.9.0/plaid/model/wallet_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_idempotency_key.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_idempotency_key.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_audit_copy_create_request.py` & `plaid-python-9.9.0/plaid/model/asset_report_audit_copy_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/user_address.py` & `plaid-python-9.9.0/plaid/model/user_address.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/numbers_eft_nullable.py` & `plaid-python-9.9.0/plaid/model/numbers_eft_nullable.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_profile_status.py` & `plaid-python-9.9.0/plaid/model/payment_profile_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_investment_filter.py` & `plaid-python-9.9.0/plaid/model/link_token_create_investment_filter.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/security_override.py` & `plaid-python-9.9.0/plaid/model/security_override.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/user_stated_income_source_frequency.py` & `plaid-python-9.9.0/plaid/model/user_stated_income_source_frequency.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/owner_override.py` & `plaid-python-9.9.0/plaid/model/owner_override.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/investment_transaction_type.py` & `plaid-python-9.9.0/plaid/model/investment_transaction_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_application_list_user_auth.py` & `plaid-python-9.9.0/plaid/model/item_application_list_user_auth.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_request_income_verification_payroll_income.py` & `plaid-python-9.9.0/plaid/model/link_token_create_request_income_verification_payroll_income.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/earnings.py` & `plaid-python-9.9.0/plaid/model/earnings.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_cancel_response.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_cancel_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfers_events_update_webhook.py` & `plaid-python-9.9.0/plaid/model/bank_transfers_events_update_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/pay_stub_earnings_total.py` & `plaid-python-9.9.0/plaid/model/pay_stub_earnings_total.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_intent_get_response.py` & `plaid-python-9.9.0/plaid/model/transfer_intent_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/institutions_get_request_options.py` & `plaid-python-9.9.0/plaid/model/institutions_get_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_pay_stub_deductions.py` & `plaid-python-9.9.0/plaid/model/credit_pay_stub_deductions.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/document_analysis.py` & `plaid-python-9.9.0/plaid/model/document_analysis.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/earnings_total.py` & `plaid-python-9.9.0/plaid/model/earnings_total.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/account_selection_cardinality.py` & `plaid-python-9.9.0/plaid/model/account_selection_cardinality.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_transfer_simulate_request.py` & `plaid-python-9.9.0/plaid/model/sandbox_transfer_simulate_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/meta.py` & `plaid-python-9.9.0/plaid/model/meta.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/mortgage_property_address.py` & `plaid-python-9.9.0/plaid/model/mortgage_property_address.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_type.py` & `plaid-python-9.9.0/plaid/model/transfer_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payroll_item_status.py` & `plaid-python-9.9.0/plaid/model/payroll_item_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/default_update_webhook.py` & `plaid-python-9.9.0/plaid/model/default_update_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/get_individual_watchlist_screening_request.py` & `plaid-python-9.9.0/plaid/model/get_individual_watchlist_screening_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/employment_details.py` & `plaid-python-9.9.0/plaid/model/employment_details.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_intent_get.py` & `plaid-python-9.9.0/plaid/model/transfer_intent_get.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_consent_max_payment_amount.py` & `plaid-python-9.9.0/plaid/model/payment_consent_max_payment_amount.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_payment_get_response.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_payment_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/list_watchlist_screening_individual_hit_request.py` & `plaid-python-9.9.0/plaid/model/list_watchlist_screening_individual_hit_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_request_income_verification_bank_income.py` & `plaid-python-9.9.0/plaid/model/link_token_create_request_income_verification_bank_income.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_employment_get_response.py` & `plaid-python-9.9.0/plaid/model/credit_employment_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/list_individual_watchlist_screening_request.py` & `plaid-python-9.9.0/plaid/model/list_individual_watchlist_screening_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/account_filter_subtypes.py` & `plaid-python-9.9.0/plaid/model/account_filter_subtypes.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/liabilities_get_response.py` & `plaid-python-9.9.0/plaid/model/liabilities_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_bank_transfer_simulate_request.py` & `plaid-python-9.9.0/plaid/model/sandbox_bank_transfer_simulate_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_screening_hits_phone_number_items.py` & `plaid-python-9.9.0/plaid/model/entity_screening_hits_phone_number_items.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_request_deposit_switch.py` & `plaid-python-9.9.0/plaid/model/link_token_create_request_deposit_switch.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/deductions_breakdown.py` & `plaid-python-9.9.0/plaid/model/deductions_breakdown.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_list_request.py` & `plaid-python-9.9.0/plaid/model/wallet_list_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_event_list_request.py` & `plaid-python-9.9.0/plaid/model/transfer_event_list_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/document_authenticity_match_code.py` & `plaid-python-9.9.0/plaid/model/document_authenticity_match_code.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_relay_create_response.py` & `plaid-python-9.9.0/plaid/model/asset_report_relay_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/account_balance.py` & `plaid-python-9.9.0/plaid/model/account_balance.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/list_identity_verification_request.py` & `plaid-python-9.9.0/plaid/model/list_identity_verification_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/list_watchlist_screening_individual_history_request.py` & `plaid-python-9.9.0/plaid/model/list_watchlist_screening_individual_history_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/location.py` & `plaid-python-9.9.0/plaid/model/location.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paginated_entity_watchlist_screening_review_list_response.py` & `plaid-python-9.9.0/plaid/model/paginated_entity_watchlist_screening_review_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_transfer_sweep_simulate_response.py` & `plaid-python-9.9.0/plaid/model/sandbox_transfer_sweep_simulate_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_enhance_get_response.py` & `plaid-python-9.9.0/plaid/model/transactions_enhance_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/signal_decision_report_request.py` & `plaid-python-9.9.0/plaid/model/signal_decision_report_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_match_request_options.py` & `plaid-python-9.9.0/plaid/model/identity_match_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_breakdown.py` & `plaid-python-9.9.0/plaid/model/income_breakdown.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_list_request.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_list_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/webhook_update_acknowledged_webhook.py` & `plaid-python-9.9.0/plaid/model/webhook_update_acknowledged_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/liability_override.py` & `plaid-python-9.9.0/plaid/model/liability_override.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_filter.py` & `plaid-python-9.9.0/plaid/model/credit_filter.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_recipient.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_recipient.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_import_request_user_auth.py` & `plaid-python-9.9.0/plaid/model/item_import_request_user_auth.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_recurring_get_response.py` & `plaid-python-9.9.0/plaid/model/transactions_recurring_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_default_update_webhook.py` & `plaid-python-9.9.0/plaid/model/identity_default_update_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/employment_verification.py` & `plaid-python-9.9.0/plaid/model/employment_verification.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_authorization.py` & `plaid-python-9.9.0/plaid/model/transfer_authorization.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_consent_periodic_interval.py` & `plaid-python-9.9.0/plaid/model/payment_consent_periodic_interval.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/investments_transactions_get_request.py` & `plaid-python-9.9.0/plaid/model/investments_transactions_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_create_request.py` & `plaid-python-9.9.0/plaid/model/transfer_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,72 +84,72 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'access_token': (str,),  # noqa: E501
-            'account_id': (str,),  # noqa: E501
             'authorization_id': (str,),  # noqa: E501
             'type': (TransferType,),  # noqa: E501
             'network': (TransferNetwork,),  # noqa: E501
             'amount': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'ach_class': (ACHClass,),  # noqa: E501
             'user': (TransferUserInRequest,),  # noqa: E501
             'client_id': (str,),  # noqa: E501
             'secret': (str,),  # noqa: E501
             'idempotency_key': (TransferCreateIdempotencyKey,),  # noqa: E501
+            'access_token': (str,),  # noqa: E501
+            'account_id': (str,),  # noqa: E501
             'metadata': (TransferMetadata,),  # noqa: E501
             'origination_account_id': (str, none_type,),  # noqa: E501
             'iso_currency_code': (str,),  # noqa: E501
+            'payment_profile_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'access_token': 'access_token',  # noqa: E501
-        'account_id': 'account_id',  # noqa: E501
         'authorization_id': 'authorization_id',  # noqa: E501
         'type': 'type',  # noqa: E501
         'network': 'network',  # noqa: E501
         'amount': 'amount',  # noqa: E501
         'description': 'description',  # noqa: E501
         'ach_class': 'ach_class',  # noqa: E501
         'user': 'user',  # noqa: E501
         'client_id': 'client_id',  # noqa: E501
         'secret': 'secret',  # noqa: E501
         'idempotency_key': 'idempotency_key',  # noqa: E501
+        'access_token': 'access_token',  # noqa: E501
+        'account_id': 'account_id',  # noqa: E501
         'metadata': 'metadata',  # noqa: E501
         'origination_account_id': 'origination_account_id',  # noqa: E501
         'iso_currency_code': 'iso_currency_code',  # noqa: E501
+        'payment_profile_id': 'payment_profile_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, access_token, account_id, authorization_id, type, network, amount, description, ach_class, user, *args, **kwargs):  # noqa: E501
+    def __init__(self, authorization_id, type, network, amount, description, ach_class, user, *args, **kwargs):  # noqa: E501
         """TransferCreateRequest - a model defined in OpenAPI
 
         Args:
-            access_token (str): The Plaid `access_token` for the account that will be debited or credited.
-            account_id (str): The Plaid `account_id` for the account that will be debited or credited.
             authorization_id (str): Plaid’s unique identifier for a transfer authorization. This parameter also serves the purpose of acting as an idempotency identifier.
             type (TransferType):
             network (TransferNetwork):
             amount (str): The amount of the transfer (decimal string with two digits of precision e.g. \"10.00\").
             description (str): The transfer description. Maximum of 10 characters.
             ach_class (ACHClass):
             user (TransferUserInRequest):
@@ -184,17 +184,20 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             client_id (str): Your Plaid API `client_id`. The `client_id` is required and may be provided either in the `PLAID-CLIENT-ID` header or as part of a request body.. [optional]  # noqa: E501
             secret (str): Your Plaid API `secret`. The `secret` is required and may be provided either in the `PLAID-SECRET` header or as part of a request body.. [optional]  # noqa: E501
             idempotency_key (TransferCreateIdempotencyKey): [optional]  # noqa: E501
+            access_token (str): The Plaid `access_token` for the account that will be debited or credited.. [optional]  # noqa: E501
+            account_id (str): The Plaid `account_id` for the account that will be debited or credited.. [optional]  # noqa: E501
             metadata (TransferMetadata): [optional]  # noqa: E501
             origination_account_id (str, none_type): Plaid’s unique identifier for the origination account for this transfer. If you have more than one origination account, this value must be specified. Otherwise, this field should be left blank.. [optional]  # noqa: E501
             iso_currency_code (str): The currency of the transfer amount. The default value is \"USD\".. [optional]  # noqa: E501
+            payment_profile_id (str): Plaid’s unique identifier for a payment profile.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -212,16 +215,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.access_token = access_token
-        self.account_id = account_id
         self.authorization_id = authorization_id
         self.type = type
         self.network = network
         self.amount = amount
         self.description = description
         self.ach_class = ach_class
         self.user = user
```

### Comparing `plaid-python-9.8.0/plaid/model/ytd_net_income_summary_field_number.py` & `plaid-python-9.9.0/plaid/model/ytd_net_income_summary_field_number.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/email.py` & `plaid-python-9.9.0/plaid/model/email.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_profile_get_request.py` & `plaid-python-9.9.0/plaid/model/payment_profile_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer.py` & `plaid-python-9.9.0/plaid/model/bank_transfer.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_platform_ids.py` & `plaid-python-9.9.0/plaid/model/credit_platform_ids.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/kyc_check_name_summary.py` & `plaid-python-9.9.0/plaid/model/kyc_check_name_summary.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_recipient_get_response.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_recipient_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/physical_document_category.py` & `plaid-python-9.9.0/plaid/model/physical_document_category.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/account_assets_all_of.py` & `plaid-python-9.9.0/plaid/model/account_assets_all_of.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,23 +105,17 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, days_available, transactions, owners, historical_balances, *args, **kwargs):  # noqa: E501
+    def __init__(self, *args, **kwargs):  # noqa: E501
         """AccountAssetsAllOf - a model defined in OpenAPI
 
-        Args:
-            days_available (float): The duration of transaction history available for this Item, typically defined as the time since the date of the earliest transaction in that account. Only returned by Assets endpoints.
-            transactions ([AssetReportTransaction]): Transaction history associated with the account. Only returned by Assets endpoints. Transaction history returned by endpoints such as `/transactions/get` or `/investments/transactions/get` will be returned in the top-level `transactions` field instead.
-            owners ([Owner]): Data returned by the financial institution about the account owner or owners. Only returned by Identity or Assets endpoints. For business accounts, the name reported may be either the name of the individual or the name of the business, depending on the institution. Multiple owners on a single account will be represented in the same `owner` object, not in multiple owner objects within the array. In API versions 2018-05-22 and earlier, the `owners` object is not returned, and instead identity information is returned in the top level `identity` object. For more details, see [Plaid API versioning](https://plaid.com/docs/api/versioning/#version-2019-05-29)
-            historical_balances ([HistoricalBalance]): Calculated data about the historical balances on the account. Only returned by Assets endpoints and currently not supported by `brokerage` or `investment` accounts.
-
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -145,14 +139,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            days_available (float): The duration of transaction history available for this Item, typically defined as the time since the date of the earliest transaction in that account. Only returned by Assets endpoints.. [optional]  # noqa: E501
+            transactions ([AssetReportTransaction]): Transaction history associated with the account. Only returned by Assets endpoints. Transaction history returned by endpoints such as `/transactions/get` or `/investments/transactions/get` will be returned in the top-level `transactions` field instead.. [optional]  # noqa: E501
+            owners ([Owner]): Data returned by the financial institution about the account owner or owners. Only returned by Identity or Assets endpoints. For business accounts, the name reported may be either the name of the individual or the name of the business, depending on the institution. Multiple owners on a single account will be represented in the same `owner` object, not in multiple owner objects within the array. In API versions 2018-05-22 and earlier, the `owners` object is not returned, and instead identity information is returned in the top level `identity` object. For more details, see [Plaid API versioning](https://plaid.com/docs/api/versioning/#version-2019-05-29). [optional]  # noqa: E501
+            historical_balances ([HistoricalBalance]): Calculated data about the historical balances on the account. Only returned by Assets endpoints and currently not supported by `brokerage` or `investment` accounts.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -170,18 +168,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.days_available = days_available
-        self.transactions = transactions
-        self.owners = owners
-        self.historical_balances = historical_balances
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_create_request.py` & `plaid-python-9.9.0/plaid/model/asset_report_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/numbers_iban_nullable.py` & `plaid-python-9.9.0/plaid/model/numbers_iban_nullable.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_oauth_select_accounts_response.py` & `plaid-python-9.9.0/plaid/model/sandbox_oauth_select_accounts_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/relay_event.py` & `plaid-python-9.9.0/plaid/model/relay_event.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/total.py` & `plaid-python-9.9.0/plaid/model/total.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/review_comment.py` & `plaid-python-9.9.0/plaid/model/review_comment.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/total_canonical_description.py` & `plaid-python-9.9.0/plaid/model/total_canonical_description.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_transactions_list_response.py` & `plaid-python-9.9.0/plaid/model/wallet_transactions_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_status.py` & `plaid-python-9.9.0/plaid/model/transfer_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class BankTransferStatus(ModelSimple):
+class TransferStatus(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -47,15 +47,15 @@
 
     allowed_values = {
         ('value',): {
             'PENDING': "pending",
             'POSTED': "posted",
             'CANCELLED': "cancelled",
             'FAILED': "failed",
-            'REVERSED': "reversed",
+            'RETURNED': "returned",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -92,23 +92,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """BankTransferStatus - a model defined in OpenAPI
+        """TransferStatus - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): The status of the transfer.., must be one of ["pending", "posted", "cancelled", "failed", "reversed", ]  # noqa: E501
+            args[0] (str): The status of the transfer.., must be one of ["pending", "posted", "cancelled", "failed", "returned", ]  # noqa: E501
 
         Keyword Args:
-            value (str): The status of the transfer.., must be one of ["pending", "posted", "cancelled", "failed", "reversed", ]  # noqa: E501
+            value (str): The status of the transfer.., must be one of ["pending", "posted", "cancelled", "failed", "returned", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `plaid-python-9.8.0/plaid/model/pay.py` & `plaid-python-9.9.0/plaid/model/pay.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/institutions_get_request.py` & `plaid-python-9.9.0/plaid/model/institutions_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/pay_stub_distribution_breakdown.py` & `plaid-python-9.9.0/plaid/model/pay_stub_distribution_breakdown.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paginated_individual_watchlist_screening_list_response.py` & `plaid-python-9.9.0/plaid/model/paginated_individual_watchlist_screening_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_verification_request_user.py` & `plaid-python-9.9.0/plaid/model/identity_verification_request_user.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_relay_create_response.py` & `plaid-python-9.9.0/plaid/model/credit_relay_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_webhook_update_response.py` & `plaid-python-9.9.0/plaid/model/item_webhook_update_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_relay_create_request.py` & `plaid-python-9.9.0/plaid/model/asset_report_relay_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_transfer_fire_webhook_request.py` & `plaid-python-9.9.0/plaid/model/sandbox_transfer_fire_webhook_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/numbers.py` & `plaid-python-9.9.0/plaid/model/numbers.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/update_individual_screening_request_resettable_field_list.py` & `plaid-python-9.9.0/plaid/model/update_individual_screening_request_resettable_field_list.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/loan_account_subtypes.py` & `plaid-python-9.9.0/plaid/model/loan_account_subtypes.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_application_scopes_update_response.py` & `plaid-python-9.9.0/plaid/model/item_application_scopes_update_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/screening_hit_data.py` & `plaid-python-9.9.0/plaid/model/screening_hit_data.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_payment_status.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_payment_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_bank_transfer_fire_webhook_request.py` & `plaid-python-9.9.0/plaid/model/sandbox_bank_transfer_fire_webhook_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_watchlist_screening_name.py` & `plaid-python-9.9.0/plaid/model/entity_watchlist_screening_name.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/strategy.py` & `plaid-python-9.9.0/plaid/model/strategy.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_cancel_request.py` & `plaid-python-9.9.0/plaid/model/transfer_cancel_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/wallet_iso_currency_code.py` & `plaid-python-9.9.0/plaid/model/wallet_iso_currency_code.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_intent_create.py` & `plaid-python-9.9.0/plaid/model/transfer_intent_create.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/individual_watchlist_program.py` & `plaid-python-9.9.0/plaid/model/individual_watchlist_program.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_event_list_request.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_event_list_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/w2.py` & `plaid-python-9.9.0/plaid/model/w2.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_events_update_webhook.py` & `plaid-python-9.9.0/plaid/model/transfer_events_update_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_intent_create_response.py` & `plaid-python-9.9.0/plaid/model/transfer_intent_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/external_payment_initiation_consent_options.py` & `plaid-python-9.9.0/plaid/model/external_payment_initiation_consent_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/deposit_switch_create_response.py` & `plaid-python-9.9.0/plaid/model/deposit_switch_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/account_identity_all_of.py` & `plaid-python-9.9.0/plaid/model/account_identity_all_of.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/generic_country_code.py` & `plaid-python-9.9.0/plaid/model/generic_country_code.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/numbers_ach.py` & `plaid-python-9.9.0/plaid/model/numbers_ach.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/list_watchlist_screening_entity_programs_request.py` & `plaid-python-9.9.0/plaid/model/list_watchlist_screening_entity_programs_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/document_risk_signals_object.py` & `plaid-python-9.9.0/plaid/model/document_risk_signals_object.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_user_address_in_response.py` & `plaid-python-9.9.0/plaid/model/transfer_user_address_in_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_document.py` & `plaid-python-9.9.0/plaid/model/entity_document.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/liabilities_get_request.py` & `plaid-python-9.9.0/plaid/model/liabilities_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/investment_transaction.py` & `plaid-python-9.9.0/plaid/model/investment_transaction.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/institution.py` & `plaid-python-9.9.0/plaid/model/institution.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_webhook_status.py` & `plaid-python-9.9.0/plaid/model/income_verification_webhook_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/individual_watchlist_program_response.py` & `plaid-python-9.9.0/plaid/model/individual_watchlist_program_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_remove_request.py` & `plaid-python-9.9.0/plaid/model/item_remove_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_sync_request_options.py` & `plaid-python-9.9.0/plaid/model/transactions_sync_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/auth_get_request_options.py` & `plaid-python-9.9.0/plaid/model/auth_get_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/list_watchlist_screening_entity_reviews_request.py` & `plaid-python-9.9.0/plaid/model/list_watchlist_screening_entity_reviews_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paginated_identity_verification_list_response.py` & `plaid-python-9.9.0/plaid/model/paginated_identity_verification_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_payment.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_payment.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/account_assets.py` & `plaid-python-9.9.0/plaid/model/account_assets.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_refresh_request_options.py` & `plaid-python-9.9.0/plaid/model/asset_report_refresh_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_payroll_income_get_request.py` & `plaid-python-9.9.0/plaid/model/credit_payroll_income_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/kyc_check_address_summary.py` & `plaid-python-9.9.0/plaid/model/kyc_check_address_summary.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_verification_status.py` & `plaid-python-9.9.0/plaid/model/identity_verification_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/personal_finance_category.py` & `plaid-python-9.9.0/plaid/model/personal_finance_category.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/user_create_request.py` & `plaid-python-9.9.0/plaid/model/user_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/deposit_switch_token_create_request.py` & `plaid-python-9.9.0/plaid/model/deposit_switch_token_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/scopes_context.py` & `plaid-python-9.9.0/plaid/model/scopes_context.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/single_document_risk_signal.py` & `plaid-python-9.9.0/plaid/model/single_document_risk_signal.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/student_loan_repayment_model.py` & `plaid-python-9.9.0/plaid/model/student_loan_repayment_model.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/watchlist_screening_document_type.py` & `plaid-python-9.9.0/plaid/model/watchlist_screening_document_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/external_payment_options.py` & `plaid-python-9.9.0/plaid/model/external_payment_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_relay_create_request.py` & `plaid-python-9.9.0/plaid/model/credit_relay_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transaction_base.py` & `plaid-python-9.9.0/plaid/model/transaction_base.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/country_code.py` & `plaid-python-9.9.0/plaid/model/country_code.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/holdings_default_update_webhook.py` & `plaid-python-9.9.0/plaid/model/holdings_default_update_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_get_response.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_payroll_income_precheck_response.py` & `plaid-python-9.9.0/plaid/model/credit_payroll_income_precheck_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_screening_hit_emails.py` & `plaid-python-9.9.0/plaid/model/entity_screening_hit_emails.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/kyc_check_phone_summary.py` & `plaid-python-9.9.0/plaid/model/kyc_check_phone_summary.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_consent_payment_execute_request.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_consent_payment_execute_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_item_set_verification_status_response.py` & `plaid-python-9.9.0/plaid/model/sandbox_item_set_verification_status_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_consent_scope.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_consent_scope.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_application_scopes_update_request.py` & `plaid-python-9.9.0/plaid/model/item_application_scopes_update_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_screening_hit_urls_items.py` & `plaid-python-9.9.0/plaid/model/entity_screening_hit_urls_items.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/employers_search_response.py` & `plaid-python-9.9.0/plaid/model/employers_search_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paystub_verification_status.py` & `plaid-python-9.9.0/plaid/model/paystub_verification_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_verification_response.py` & `plaid-python-9.9.0/plaid/model/identity_verification_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_source_type.py` & `plaid-python-9.9.0/plaid/model/income_verification_source_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_transfer_simulate_response.py` & `plaid-python-9.9.0/plaid/model/sandbox_transfer_simulate_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/watchlist_screening_review.py` & `plaid-python-9.9.0/plaid/model/watchlist_screening_review.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/deductions.py` & `plaid-python-9.9.0/plaid/model/deductions.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report.py` & `plaid-python-9.9.0/plaid/model/asset_report.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_consent_revoke_response.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_consent_revoke_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_user_address_in_request.py` & `plaid-python-9.9.0/plaid/model/transfer_user_address_in_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_event_list_bank_transfer_type.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_event_list_bank_transfer_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/update_individual_screening_request.py` & `plaid-python-9.9.0/plaid/model/update_individual_screening_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_recurring_get_request.py` & `plaid-python-9.9.0/plaid/model/transactions_recurring_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/signal_device.py` & `plaid-python-9.9.0/plaid/model/signal_device.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/cause.py` & `plaid-python-9.9.0/plaid/model/cause.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_historical_summary.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_historical_summary.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/external_payment_schedule_request.py` & `plaid-python-9.9.0/plaid/model/external_payment_schedule_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/pay_frequency_value.py` & `plaid-python-9.9.0/plaid/model/pay_frequency_value.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_get_request.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/platform_ids.py` & `plaid-python-9.9.0/plaid/model/platform_ids.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/individual_watchlist_screening_program_name.py` & `plaid-python-9.9.0/plaid/model/individual_watchlist_screening_program_name.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_processor_token_create_request_options.py` & `plaid-python-9.9.0/plaid/model/sandbox_processor_token_create_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/auth_get_request.py` & `plaid-python-9.9.0/plaid/model/auth_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_item.py` & `plaid-python-9.9.0/plaid/model/asset_report_item.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_event_list_response.py` & `plaid-python-9.9.0/plaid/model/transfer_event_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/investments_transactions_get_request_options.py` & `plaid-python-9.9.0/plaid/model/investments_transactions_get_request_options.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_repayment_return.py` & `plaid-python-9.9.0/plaid/model/transfer_repayment_return.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payroll_income_rate_of_pay.py` & `plaid-python-9.9.0/plaid/model/payroll_income_rate_of_pay.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_refresh_request.py` & `plaid-python-9.9.0/plaid/model/asset_report_refresh_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/list_watchlist_screening_individual_programs_request.py` & `plaid-python-9.9.0/plaid/model/list_watchlist_screening_individual_programs_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/liabilities_account_ids_with_updated_liabilities.py` & `plaid-python-9.9.0/plaid/model/paystub_override_employer.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class LiabilitiesAccountIdsWithUpdatedLiabilities(ModelNormal):
+class PaystubOverrideEmployer(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,43 +51,39 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return ([str],)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
+            'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'name': 'name',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
@@ -95,15 +91,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """LiabilitiesAccountIdsWithUpdatedLiabilities - a model defined in OpenAPI
+        """PaystubOverrideEmployer - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -128,14 +124,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            name (str): The name of the employer.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `plaid-python-9.8.0/plaid/model/watchlist_screening_document.py` & `plaid-python-9.9.0/plaid/model/watchlist_screening_document.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transactions_get_request.py` & `plaid-python-9.9.0/plaid/model/transactions_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/employment_verification_get_response.py` & `plaid-python-9.9.0/plaid/model/employment_verification_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_employment_verification.py` & `plaid-python-9.9.0/plaid/model/credit_employment_verification.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_w2.py` & `plaid-python-9.9.0/plaid/model/credit_w2.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_watchlist_screening_review_response.py` & `plaid-python-9.9.0/plaid/model/entity_watchlist_screening_review_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_recipient_list_request.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_recipient_list_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/pay_stub_pay_period_details.py` & `plaid-python-9.9.0/plaid/model/pay_stub_pay_period_details.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/user_stated_income_source_category.py` & `plaid-python-9.9.0/plaid/model/user_stated_income_source_category.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_error_type.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_error_type.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/scopes_nullable.py` & `plaid-python-9.9.0/plaid/model/scopes_nullable.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/credit_bank_income_source.py` & `plaid-python-9.9.0/plaid/model/credit_bank_income_source.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_screening_hit_names.py` & `plaid-python-9.9.0/plaid/model/entity_screening_hit_names.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_verification_user_phone_number.py` & `plaid-python-9.9.0/plaid/model/identity_verification_user_phone_number.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_relay_remove_response.py` & `plaid-python-9.9.0/plaid/model/asset_report_relay_remove_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_payment_token_create_request.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_payment_token_create_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/auth_metadata.py` & `plaid-python-9.9.0/plaid/model/auth_metadata.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_event.py` & `plaid-python-9.9.0/plaid/model/transfer_event.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_event_sync_request.py` & `plaid-python-9.9.0/plaid/model/transfer_event_sync_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/paystub_override_employer.py` & `plaid-python-9.9.0/plaid/model/asset_report_remove_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class PaystubOverrideEmployer(ModelNormal):
+class AssetReportRemoveResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,55 +51,67 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    additional_properties_type = None
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'name': (str,),  # noqa: E501
+            'removed': (bool,),  # noqa: E501
+            'request_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
+        'removed': 'removed',  # noqa: E501
+        'request_id': 'request_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """PaystubOverrideEmployer - a model defined in OpenAPI
+    def __init__(self, removed, request_id, *args, **kwargs):  # noqa: E501
+        """AssetReportRemoveResponse - a model defined in OpenAPI
+
+        Args:
+            removed (bool): `true` if the Asset Report was successfully removed.
+            request_id (str): A unique identifier for the request, which can be used for troubleshooting. This identifier, like all Plaid identifiers, is case sensitive.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -124,15 +136,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): The name of the employer.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -150,14 +161,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.removed = removed
+        self.request_id = request_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `plaid-python-9.8.0/plaid/model/auth_supported_methods.py` & `plaid-python-9.9.0/plaid/model/auth_supported_methods.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/document_risk_signal.py` & `plaid-python-9.9.0/plaid/model/document_risk_signal.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/transfer_authorization_guarantee_decision_rationale.py` & `plaid-python-9.9.0/plaid/model/transfer_authorization_guarantee_decision_rationale.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_relay_remove_request.py` & `plaid-python-9.9.0/plaid/model/asset_report_relay_remove_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/verification_refresh_status.py` & `plaid-python-9.9.0/plaid/model/verification_refresh_status.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/recurring_transaction_frequency.py` & `plaid-python-9.9.0/plaid/model/recurring_transaction_frequency.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_precheck_user.py` & `plaid-python-9.9.0/plaid/model/income_verification_precheck_user.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/identity_verification_retried_webhook.py` & `plaid-python-9.9.0/plaid/model/identity_verification_retried_webhook.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/sandbox_processor_token_create_response.py` & `plaid-python-9.9.0/plaid/model/sandbox_processor_token_create_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_override.py` & `plaid-python-9.9.0/plaid/model/income_override.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/entity_watchlist_program.py` & `plaid-python-9.9.0/plaid/model/entity_watchlist_program.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_precheck_confidence.py` & `plaid-python-9.9.0/plaid/model/income_verification_precheck_confidence.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_refresh_request.py` & `plaid-python-9.9.0/plaid/model/income_verification_refresh_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/numbers_bacs.py` & `plaid-python-9.9.0/plaid/model/numbers_bacs.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/income_verification_taxforms_get_response.py` & `plaid-python-9.9.0/plaid/model/income_verification_taxforms_get_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/health_incident.py` & `plaid-python-9.9.0/plaid/model/health_incident.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/update_entity_screening_request_resettable_field.py` & `plaid-python-9.9.0/plaid/model/update_entity_screening_request_resettable_field.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_balance_get_request.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_balance_get_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/asset_report_remove_response.py` & `plaid-python-9.9.0/plaid/model/credit_relay_refresh_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class AssetReportRemoveResponse(ModelNormal):
+class CreditRelayRefreshResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -72,45 +72,47 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'removed': (bool,),  # noqa: E501
+            'relay_token': (str,),  # noqa: E501
             'request_id': (str,),  # noqa: E501
+            'asset_report_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'removed': 'removed',  # noqa: E501
+        'relay_token': 'relay_token',  # noqa: E501
         'request_id': 'request_id',  # noqa: E501
+        'asset_report_id': 'asset_report_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, removed, request_id, *args, **kwargs):  # noqa: E501
-        """AssetReportRemoveResponse - a model defined in OpenAPI
+    def __init__(self, relay_token, request_id, *args, **kwargs):  # noqa: E501
+        """CreditRelayRefreshResponse - a model defined in OpenAPI
 
         Args:
-            removed (bool): `true` if the Asset Report was successfully removed.
+            relay_token (str):
             request_id (str): A unique identifier for the request, which can be used for troubleshooting. This identifier, like all Plaid identifiers, is case sensitive.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -136,14 +138,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            asset_report_id (str): A unique ID identifying an Asset Report. Like all Plaid identifiers, this ID is case sensitive.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -161,15 +164,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.removed = removed
+        self.relay_token = relay_token
         self.request_id = request_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
```

### Comparing `plaid-python-9.8.0/plaid/model/signal_evaluate_request.py` & `plaid-python-9.9.0/plaid/model/signal_evaluate_request.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/screening_hit_date_of_birth_item.py` & `plaid-python-9.9.0/plaid/model/screening_hit_date_of_birth_item.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/item_status_transactions.py` & `plaid-python-9.9.0/plaid/model/item_status_transactions.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/payment_initiation_payment_list_response.py` & `plaid-python-9.9.0/plaid/model/payment_initiation_payment_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/earnings_breakdown.py` & `plaid-python-9.9.0/plaid/model/earnings_breakdown.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/report_token.py` & `plaid-python-9.9.0/plaid/model/report_token.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,18 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
+def lazy_import():
+    from plaid.model.report_type import ReportType
+    globals()['ReportType'] = ReportType
+
 
 class ReportToken(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
@@ -57,30 +61,32 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'report_type': (str,),  # noqa: E501
+            'report_type': (ReportType,),  # noqa: E501
             'token': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -132,15 +138,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            report_type (str): The report type. It can be `assets` or `income`.. [optional]  # noqa: E501
+            report_type (ReportType): [optional]  # noqa: E501
             token (str): The report token. It can be an asset report token or an income report token.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `plaid-python-9.8.0/plaid/model/paginated_individual_watchlist_screening_hit_list_response.py` & `plaid-python-9.9.0/plaid/model/paginated_individual_watchlist_screening_hit_list_response.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/link_token_create_depository_filter.py` & `plaid-python-9.9.0/plaid/model/link_token_create_depository_filter.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model/bank_transfer_balance.py` & `plaid-python-9.9.0/plaid/model/bank_transfer_balance.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/api/plaid_api.py` & `plaid-python-9.9.0/plaid/api/plaid_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,26 +75,32 @@
 from plaid.model.create_individual_watchlist_screening_review_request import CreateIndividualWatchlistScreeningReviewRequest
 from plaid.model.credit_audit_copy_token_create_request import CreditAuditCopyTokenCreateRequest
 from plaid.model.credit_audit_copy_token_create_response import CreditAuditCopyTokenCreateResponse
 from plaid.model.credit_audit_copy_token_remove_request import CreditAuditCopyTokenRemoveRequest
 from plaid.model.credit_audit_copy_token_remove_response import CreditAuditCopyTokenRemoveResponse
 from plaid.model.credit_bank_income_get_request import CreditBankIncomeGetRequest
 from plaid.model.credit_bank_income_get_response import CreditBankIncomeGetResponse
+from plaid.model.credit_bank_income_pdf_get_request import CreditBankIncomePDFGetRequest
 from plaid.model.credit_bank_income_refresh_request import CreditBankIncomeRefreshRequest
 from plaid.model.credit_bank_income_refresh_response import CreditBankIncomeRefreshResponse
 from plaid.model.credit_employment_get_request import CreditEmploymentGetRequest
 from plaid.model.credit_employment_get_response import CreditEmploymentGetResponse
 from plaid.model.credit_payroll_income_get_request import CreditPayrollIncomeGetRequest
 from plaid.model.credit_payroll_income_get_response import CreditPayrollIncomeGetResponse
 from plaid.model.credit_payroll_income_precheck_request import CreditPayrollIncomePrecheckRequest
 from plaid.model.credit_payroll_income_precheck_response import CreditPayrollIncomePrecheckResponse
 from plaid.model.credit_payroll_income_refresh_request import CreditPayrollIncomeRefreshRequest
 from plaid.model.credit_payroll_income_refresh_response import CreditPayrollIncomeRefreshResponse
 from plaid.model.credit_relay_create_request import CreditRelayCreateRequest
 from plaid.model.credit_relay_create_response import CreditRelayCreateResponse
+from plaid.model.credit_relay_get_request import CreditRelayGetRequest
+from plaid.model.credit_relay_refresh_request import CreditRelayRefreshRequest
+from plaid.model.credit_relay_refresh_response import CreditRelayRefreshResponse
+from plaid.model.credit_relay_remove_request import CreditRelayRemoveRequest
+from plaid.model.credit_relay_remove_response import CreditRelayRemoveResponse
 from plaid.model.dashboard_user_response import DashboardUserResponse
 from plaid.model.deposit_switch_alt_create_request import DepositSwitchAltCreateRequest
 from plaid.model.deposit_switch_alt_create_response import DepositSwitchAltCreateResponse
 from plaid.model.deposit_switch_create_request import DepositSwitchCreateRequest
 from plaid.model.deposit_switch_create_response import DepositSwitchCreateResponse
 from plaid.model.deposit_switch_get_request import DepositSwitchGetRequest
 from plaid.model.deposit_switch_get_response import DepositSwitchGetResponse
@@ -185,14 +191,16 @@
 from plaid.model.paginated_entity_watchlist_screening_list_response import PaginatedEntityWatchlistScreeningListResponse
 from plaid.model.paginated_entity_watchlist_screening_review_list_response import PaginatedEntityWatchlistScreeningReviewListResponse
 from plaid.model.paginated_identity_verification_list_response import PaginatedIdentityVerificationListResponse
 from plaid.model.paginated_individual_watchlist_program_list_response import PaginatedIndividualWatchlistProgramListResponse
 from plaid.model.paginated_individual_watchlist_screening_hit_list_response import PaginatedIndividualWatchlistScreeningHitListResponse
 from plaid.model.paginated_individual_watchlist_screening_list_response import PaginatedIndividualWatchlistScreeningListResponse
 from plaid.model.paginated_individual_watchlist_screening_review_list_response import PaginatedIndividualWatchlistScreeningReviewListResponse
+from plaid.model.partner_customers_create_request import PartnerCustomersCreateRequest
+from plaid.model.partner_customers_create_response import PartnerCustomersCreateResponse
 from plaid.model.payment_initiation_consent_create_request import PaymentInitiationConsentCreateRequest
 from plaid.model.payment_initiation_consent_create_response import PaymentInitiationConsentCreateResponse
 from plaid.model.payment_initiation_consent_get_request import PaymentInitiationConsentGetRequest
 from plaid.model.payment_initiation_consent_get_response import PaymentInitiationConsentGetResponse
 from plaid.model.payment_initiation_consent_payment_execute_request import PaymentInitiationConsentPaymentExecuteRequest
 from plaid.model.payment_initiation_consent_payment_execute_response import PaymentInitiationConsentPaymentExecuteResponse
 from plaid.model.payment_initiation_consent_revoke_request import PaymentInitiationConsentRevokeRequest
@@ -4119,14 +4127,136 @@
                     'application/json'
                 ]
             },
             api_client=api_client,
             callable=__credit_bank_income_get
         )
 
+        def __credit_bank_income_pdf_get(
+            self,
+            credit_bank_income_pdf_get_request,
+            **kwargs
+        ):
+            """Retrieve information from the bank accounts used for income verification in PDF format  # noqa: E501
+
+            `/credit/bank_income/pdf/get` returns the most recent bank income report for a specified user in PDF format.  # noqa: E501
+            This method makes a synchronous HTTP request by default. To make an
+            asynchronous HTTP request, please pass async_req=True
+
+            >>> thread = api.credit_bank_income_pdf_get(credit_bank_income_pdf_get_request, async_req=True)
+            >>> result = thread.get()
+
+            Args:
+                credit_bank_income_pdf_get_request (CreditBankIncomePDFGetRequest):
+
+            Keyword Args:
+                _return_http_data_only (bool): response data without head status
+                    code and headers. Default is True.
+                _preload_content (bool): if False, the urllib3.HTTPResponse object
+                    will be returned without reading/decoding response data.
+                    Default is True.
+                _request_timeout (float/tuple): timeout setting for this request. If one
+                    number provided, it will be total request timeout. It can also
+                    be a pair (tuple) of (connection, read) timeouts.
+                    Default is None.
+                _check_input_type (bool): specifies if type checking
+                    should be done one the data sent to the server.
+                    Default is True.
+                _check_return_type (bool): specifies if type checking
+                    should be done one the data received from the server.
+                    Default is True.
+                _host_index (int/None): specifies the index of the server
+                    that we want to use.
+                    Default is read from the configuration.
+                async_req (bool): execute request asynchronously
+
+            Returns:
+                file_type
+                    If the method is called asynchronously, returns the request
+                    thread.
+            """
+            kwargs['async_req'] = kwargs.get(
+                'async_req', False
+            )
+            kwargs['_return_http_data_only'] = kwargs.get(
+                '_return_http_data_only', True
+            )
+            kwargs['_preload_content'] = kwargs.get(
+                '_preload_content', True
+            )
+            kwargs['_request_timeout'] = kwargs.get(
+                '_request_timeout', None
+            )
+            kwargs['_check_input_type'] = kwargs.get(
+                '_check_input_type', True
+            )
+            kwargs['_check_return_type'] = kwargs.get(
+                '_check_return_type', True
+            )
+            kwargs['_host_index'] = kwargs.get('_host_index')
+            kwargs['credit_bank_income_pdf_get_request'] = \
+                credit_bank_income_pdf_get_request
+            return self.call_with_http_info(**kwargs)
+
+        self.credit_bank_income_pdf_get = _Endpoint(
+            settings={
+                'response_type': (file_type,),
+                'auth': [
+                    'clientId',
+                    'plaidVersion',
+                    'secret'
+                ],
+                'endpoint_path': '/credit/bank_income/pdf/get',
+                'operation_id': 'credit_bank_income_pdf_get',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'credit_bank_income_pdf_get_request',
+                ],
+                'required': [
+                    'credit_bank_income_pdf_get_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'credit_bank_income_pdf_get_request':
+                        (CreditBankIncomePDFGetRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'credit_bank_income_pdf_get_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/pdf'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client,
+            callable=__credit_bank_income_pdf_get
+        )
+
         def __credit_bank_income_refresh(
             self,
             credit_bank_income_refresh_request,
             **kwargs
         ):
             """Refresh a user's bank income information  # noqa: E501
 
@@ -4851,14 +4981,380 @@
                     'application/json'
                 ]
             },
             api_client=api_client,
             callable=__credit_relay_create
         )
 
+        def __credit_relay_get(
+            self,
+            credit_relay_get_request,
+            **kwargs
+        ):
+            """Retrieve the reports associated with a Relay token that was shared with you  # noqa: E501
+
+            `/credit/relay/get` allows third parties to get a report that was shared with them, using an `relay_token` that was created by the report owner.  # noqa: E501
+            This method makes a synchronous HTTP request by default. To make an
+            asynchronous HTTP request, please pass async_req=True
+
+            >>> thread = api.credit_relay_get(credit_relay_get_request, async_req=True)
+            >>> result = thread.get()
+
+            Args:
+                credit_relay_get_request (CreditRelayGetRequest):
+
+            Keyword Args:
+                _return_http_data_only (bool): response data without head status
+                    code and headers. Default is True.
+                _preload_content (bool): if False, the urllib3.HTTPResponse object
+                    will be returned without reading/decoding response data.
+                    Default is True.
+                _request_timeout (float/tuple): timeout setting for this request. If one
+                    number provided, it will be total request timeout. It can also
+                    be a pair (tuple) of (connection, read) timeouts.
+                    Default is None.
+                _check_input_type (bool): specifies if type checking
+                    should be done one the data sent to the server.
+                    Default is True.
+                _check_return_type (bool): specifies if type checking
+                    should be done one the data received from the server.
+                    Default is True.
+                _host_index (int/None): specifies the index of the server
+                    that we want to use.
+                    Default is read from the configuration.
+                async_req (bool): execute request asynchronously
+
+            Returns:
+                AssetReportGetResponse
+                    If the method is called asynchronously, returns the request
+                    thread.
+            """
+            kwargs['async_req'] = kwargs.get(
+                'async_req', False
+            )
+            kwargs['_return_http_data_only'] = kwargs.get(
+                '_return_http_data_only', True
+            )
+            kwargs['_preload_content'] = kwargs.get(
+                '_preload_content', True
+            )
+            kwargs['_request_timeout'] = kwargs.get(
+                '_request_timeout', None
+            )
+            kwargs['_check_input_type'] = kwargs.get(
+                '_check_input_type', True
+            )
+            kwargs['_check_return_type'] = kwargs.get(
+                '_check_return_type', True
+            )
+            kwargs['_host_index'] = kwargs.get('_host_index')
+            kwargs['credit_relay_get_request'] = \
+                credit_relay_get_request
+            return self.call_with_http_info(**kwargs)
+
+        self.credit_relay_get = _Endpoint(
+            settings={
+                'response_type': (AssetReportGetResponse,),
+                'auth': [
+                    'clientId',
+                    'plaidVersion',
+                    'secret'
+                ],
+                'endpoint_path': '/credit/relay/get',
+                'operation_id': 'credit_relay_get',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'credit_relay_get_request',
+                ],
+                'required': [
+                    'credit_relay_get_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'credit_relay_get_request':
+                        (CreditRelayGetRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'credit_relay_get_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client,
+            callable=__credit_relay_get
+        )
+
+        def __credit_relay_refresh(
+            self,
+            credit_relay_refresh_request,
+            **kwargs
+        ):
+            """Refresh a report of a Relay Token  # noqa: E501
+
+            The `/credit/relay/refresh` endpoint allows third parties to refresh an report that was relayed to them, using a `relay_token` that was created by the report owner. A new report will be created based on the old one, but with the most recent data available.  # noqa: E501
+            This method makes a synchronous HTTP request by default. To make an
+            asynchronous HTTP request, please pass async_req=True
+
+            >>> thread = api.credit_relay_refresh(credit_relay_refresh_request, async_req=True)
+            >>> result = thread.get()
+
+            Args:
+                credit_relay_refresh_request (CreditRelayRefreshRequest):
+
+            Keyword Args:
+                _return_http_data_only (bool): response data without head status
+                    code and headers. Default is True.
+                _preload_content (bool): if False, the urllib3.HTTPResponse object
+                    will be returned without reading/decoding response data.
+                    Default is True.
+                _request_timeout (float/tuple): timeout setting for this request. If one
+                    number provided, it will be total request timeout. It can also
+                    be a pair (tuple) of (connection, read) timeouts.
+                    Default is None.
+                _check_input_type (bool): specifies if type checking
+                    should be done one the data sent to the server.
+                    Default is True.
+                _check_return_type (bool): specifies if type checking
+                    should be done one the data received from the server.
+                    Default is True.
+                _host_index (int/None): specifies the index of the server
+                    that we want to use.
+                    Default is read from the configuration.
+                async_req (bool): execute request asynchronously
+
+            Returns:
+                CreditRelayRefreshResponse
+                    If the method is called asynchronously, returns the request
+                    thread.
+            """
+            kwargs['async_req'] = kwargs.get(
+                'async_req', False
+            )
+            kwargs['_return_http_data_only'] = kwargs.get(
+                '_return_http_data_only', True
+            )
+            kwargs['_preload_content'] = kwargs.get(
+                '_preload_content', True
+            )
+            kwargs['_request_timeout'] = kwargs.get(
+                '_request_timeout', None
+            )
+            kwargs['_check_input_type'] = kwargs.get(
+                '_check_input_type', True
+            )
+            kwargs['_check_return_type'] = kwargs.get(
+                '_check_return_type', True
+            )
+            kwargs['_host_index'] = kwargs.get('_host_index')
+            kwargs['credit_relay_refresh_request'] = \
+                credit_relay_refresh_request
+            return self.call_with_http_info(**kwargs)
+
+        self.credit_relay_refresh = _Endpoint(
+            settings={
+                'response_type': (CreditRelayRefreshResponse,),
+                'auth': [
+                    'clientId',
+                    'plaidVersion',
+                    'secret'
+                ],
+                'endpoint_path': '/credit/relay/refresh',
+                'operation_id': 'credit_relay_refresh',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'credit_relay_refresh_request',
+                ],
+                'required': [
+                    'credit_relay_refresh_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'credit_relay_refresh_request':
+                        (CreditRelayRefreshRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'credit_relay_refresh_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client,
+            callable=__credit_relay_refresh
+        )
+
+        def __credit_relay_remove(
+            self,
+            credit_relay_remove_request,
+            **kwargs
+        ):
+            """Remove Credit Relay Token  # noqa: E501
+
+            The `/credit/relay/remove` endpoint allows you to invalidate a `relay_token`, meaning the third party holding the token will no longer be able to use it to access the reports to which the `relay_token` gives access to. The report, items associated with it, and other Relay tokens that provide access to the same report are not affected and will remain accessible after removing the given `relay_token.  # noqa: E501
+            This method makes a synchronous HTTP request by default. To make an
+            asynchronous HTTP request, please pass async_req=True
+
+            >>> thread = api.credit_relay_remove(credit_relay_remove_request, async_req=True)
+            >>> result = thread.get()
+
+            Args:
+                credit_relay_remove_request (CreditRelayRemoveRequest):
+
+            Keyword Args:
+                _return_http_data_only (bool): response data without head status
+                    code and headers. Default is True.
+                _preload_content (bool): if False, the urllib3.HTTPResponse object
+                    will be returned without reading/decoding response data.
+                    Default is True.
+                _request_timeout (float/tuple): timeout setting for this request. If one
+                    number provided, it will be total request timeout. It can also
+                    be a pair (tuple) of (connection, read) timeouts.
+                    Default is None.
+                _check_input_type (bool): specifies if type checking
+                    should be done one the data sent to the server.
+                    Default is True.
+                _check_return_type (bool): specifies if type checking
+                    should be done one the data received from the server.
+                    Default is True.
+                _host_index (int/None): specifies the index of the server
+                    that we want to use.
+                    Default is read from the configuration.
+                async_req (bool): execute request asynchronously
+
+            Returns:
+                CreditRelayRemoveResponse
+                    If the method is called asynchronously, returns the request
+                    thread.
+            """
+            kwargs['async_req'] = kwargs.get(
+                'async_req', False
+            )
+            kwargs['_return_http_data_only'] = kwargs.get(
+                '_return_http_data_only', True
+            )
+            kwargs['_preload_content'] = kwargs.get(
+                '_preload_content', True
+            )
+            kwargs['_request_timeout'] = kwargs.get(
+                '_request_timeout', None
+            )
+            kwargs['_check_input_type'] = kwargs.get(
+                '_check_input_type', True
+            )
+            kwargs['_check_return_type'] = kwargs.get(
+                '_check_return_type', True
+            )
+            kwargs['_host_index'] = kwargs.get('_host_index')
+            kwargs['credit_relay_remove_request'] = \
+                credit_relay_remove_request
+            return self.call_with_http_info(**kwargs)
+
+        self.credit_relay_remove = _Endpoint(
+            settings={
+                'response_type': (CreditRelayRemoveResponse,),
+                'auth': [
+                    'clientId',
+                    'plaidVersion',
+                    'secret'
+                ],
+                'endpoint_path': '/credit/relay/remove',
+                'operation_id': 'credit_relay_remove',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'credit_relay_remove_request',
+                ],
+                'required': [
+                    'credit_relay_remove_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'credit_relay_remove_request':
+                        (CreditRelayRemoveRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'credit_relay_remove_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client,
+            callable=__credit_relay_remove
+        )
+
         def __credit_report_audit_copy_remove(
             self,
             credit_audit_copy_token_remove_request,
             **kwargs
         ):
             """Remove an Audit Copy token  # noqa: E501
 
@@ -9487,14 +9983,136 @@
                     'application/json'
                 ]
             },
             api_client=api_client,
             callable=__link_token_get
         )
 
+        def __partner_customers_create(
+            self,
+            partner_customers_create_request,
+            **kwargs
+        ):
+            """Creates a new client for a reseller partner end customer.  # noqa: E501
+
+            The `/partner/v1/customers/create` endpoint is used by reseller partners to create an end customer client.  # noqa: E501
+            This method makes a synchronous HTTP request by default. To make an
+            asynchronous HTTP request, please pass async_req=True
+
+            >>> thread = api.partner_customers_create(partner_customers_create_request, async_req=True)
+            >>> result = thread.get()
+
+            Args:
+                partner_customers_create_request (PartnerCustomersCreateRequest):
+
+            Keyword Args:
+                _return_http_data_only (bool): response data without head status
+                    code and headers. Default is True.
+                _preload_content (bool): if False, the urllib3.HTTPResponse object
+                    will be returned without reading/decoding response data.
+                    Default is True.
+                _request_timeout (float/tuple): timeout setting for this request. If one
+                    number provided, it will be total request timeout. It can also
+                    be a pair (tuple) of (connection, read) timeouts.
+                    Default is None.
+                _check_input_type (bool): specifies if type checking
+                    should be done one the data sent to the server.
+                    Default is True.
+                _check_return_type (bool): specifies if type checking
+                    should be done one the data received from the server.
+                    Default is True.
+                _host_index (int/None): specifies the index of the server
+                    that we want to use.
+                    Default is read from the configuration.
+                async_req (bool): execute request asynchronously
+
+            Returns:
+                PartnerCustomersCreateResponse
+                    If the method is called asynchronously, returns the request
+                    thread.
+            """
+            kwargs['async_req'] = kwargs.get(
+                'async_req', False
+            )
+            kwargs['_return_http_data_only'] = kwargs.get(
+                '_return_http_data_only', True
+            )
+            kwargs['_preload_content'] = kwargs.get(
+                '_preload_content', True
+            )
+            kwargs['_request_timeout'] = kwargs.get(
+                '_request_timeout', None
+            )
+            kwargs['_check_input_type'] = kwargs.get(
+                '_check_input_type', True
+            )
+            kwargs['_check_return_type'] = kwargs.get(
+                '_check_return_type', True
+            )
+            kwargs['_host_index'] = kwargs.get('_host_index')
+            kwargs['partner_customers_create_request'] = \
+                partner_customers_create_request
+            return self.call_with_http_info(**kwargs)
+
+        self.partner_customers_create = _Endpoint(
+            settings={
+                'response_type': (PartnerCustomersCreateResponse,),
+                'auth': [
+                    'clientId',
+                    'plaidVersion',
+                    'secret'
+                ],
+                'endpoint_path': '/beta/partner/v1/customers/create',
+                'operation_id': 'partner_customers_create',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'partner_customers_create_request',
+                ],
+                'required': [
+                    'partner_customers_create_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'partner_customers_create_request':
+                        (PartnerCustomersCreateRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'partner_customers_create_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client,
+            callable=__partner_customers_create
+        )
+
         def __payment_initiation_consent_create(
             self,
             payment_initiation_consent_create_request,
             **kwargs
         ):
             """Create payment consent  # noqa: E501
 
@@ -12422,15 +13040,15 @@
         def __sandbox_item_fire_webhook(
             self,
             sandbox_item_fire_webhook_request,
             **kwargs
         ):
             """Fire a test webhook  # noqa: E501
 
-            The `/sandbox/item/fire_webhook` endpoint is used to test that code correctly handles webhooks. This endpoint can trigger the following webhooks:  `DEFAULT_UPDATE`: Transactions update webhook to be fired for a given Sandbox Item. If the Item does not support Transactions, a `SANDBOX_PRODUCT_NOT_ENABLED` error will result.  `NEW_ACCOUNTS_AVAILABLE`: Webhook to be fired for a given Sandbox Item created with Account Select v2.  `AUTH_DATA_UPDATE`: Webhook to be fired for a given Sandbox Item created with Auth as an enabled product.  Note that this endpoint is provided for developer ease-of-use and is not required for testing webhooks; webhooks will also fire in Sandbox under the same conditions that they would in Production or Development'  # noqa: E501
+            The `/sandbox/item/fire_webhook` endpoint is used to test that code correctly handles webhooks. This endpoint can trigger the following webhooks:  `DEFAULT_UPDATE`: Transactions update webhook to be fired for a given Sandbox Item. If the Item does not support Transactions, a `SANDBOX_PRODUCT_NOT_ENABLED` error will result.  `NEW_ACCOUNTS_AVAILABLE`: Webhook to be fired for a given Sandbox Item created with Account Select v2.  `AUTH_DATA_UPDATE`: Webhook to be fired for a given Sandbox Item created with Auth as an enabled product.  `RECURRING_TRANSACTIONS_UPDATE`: Recurring Transactions webhook to be fired for a given Sandbox Item. If the Item does not support Recurring Transactions, a `SANDBOX_PRODUCT_NOT_ENABLED` error will result.  Note that this endpoint is provided for developer ease-of-use and is not required for testing webhooks; webhooks will also fire in Sandbox under the same conditions that they would in Production or Development.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
             >>> thread = api.sandbox_item_fire_webhook(sandbox_item_fire_webhook_request, async_req=True)
             >>> result = thread.get()
 
             Args:
@@ -14984,15 +15602,15 @@
         def __transactions_sync(
             self,
             transactions_sync_request,
             **kwargs
         ):
             """Get incremental transaction updates on an Item  # noqa: E501
 
-            This endpoint replaces `/transactions/get` and its associated webhooks for most common use-cases.  The `/transactions/sync` endpoint allows developers to subscribe to all transactions associated with an Item and get updates synchronously in a stream-like manner, using a cursor to track which updates have already been seen. `/transactions/sync` provides the same functionality as `/transactions/get` and can be used instead of `/transactions/get` to simplify the process of tracking transactions updates.  This endpoint provides user-authorized transaction data for `credit`, `depository`, and some loan-type accounts (only those with account subtype `student`; coverage may be limited). For transaction history from `investments` accounts, use `/investments/transactions/get` instead.  Returned transactions data is grouped into three types of update, indicating whether the transaction was added, removed, or modified since the last call to the API.  In the first call to `/transactions/sync` for an Item, the endpoint will return all historical transactions data associated with that Item up until the time of the API call (as \"adds\"), which then generates a `latest_cursor` for that Item. In subsequent calls, send the `latest_cursor` to receive only the changes that have occurred since the previous call.  Due to the potentially large number of transactions associated with an Item, results are paginated. The `has_more` field specifies if additional calls are necessary to fetch all available transaction updates.  Whenever new or updated transaction data becomes available, `/transactions/sync` will provide these updates. Plaid typically checks for new data multiple times a day, but these checks may occur less frequently, such as once a day, depending on the institution. An Item's `status.transactions.last_successful_update` field will show the timestamp of the most recent successful update. To force Plaid to check for new transactions, use the `/transactions/refresh` endpoint.  Note that for newly created Items, data may not be immediately available to `/transactions/sync`. Plaid begins preparing transactions data when the Item is created, but the process can take anywhere from a few seconds to several minutes to complete, depending on the number of transactions available.  To be alerted when new data is available, listen for the [`SYNC_UPDATES_AVAILABLE`](https://plaid.com/docs/api/products/transactions/#sync_updates_available) webhook.  # noqa: E501
+            This endpoint replaces `/transactions/get` and its associated webhooks for most common use-cases.  The `/transactions/sync` endpoint allows developers to subscribe to all transactions associated with an Item and get updates synchronously in a stream-like manner, using a cursor to track which updates have already been seen. `/transactions/sync` provides the same functionality as `/transactions/get` and can be used instead of `/transactions/get` to simplify the process of tracking transactions updates.  This endpoint provides user-authorized transaction data for `credit`, `depository`, and some loan-type accounts (only those with account subtype `student`; coverage may be limited). For transaction history from `investments` accounts, use `/investments/transactions/get` instead.  Returned transactions data is grouped into three types of update, indicating whether the transaction was added, removed, or modified since the last call to the API.  In the first call to `/transactions/sync` for an Item, the endpoint will return all historical transactions data associated with that Item up until the time of the API call (as \"adds\"), which then generates a `next_cursor` for that Item. In subsequent calls, send the `next_cursor` to receive only the changes that have occurred since the previous call.  Due to the potentially large number of transactions associated with an Item, results are paginated. The `has_more` field specifies if additional calls are necessary to fetch all available transaction updates.  Whenever new or updated transaction data becomes available, `/transactions/sync` will provide these updates. Plaid typically checks for new data multiple times a day, but these checks may occur less frequently, such as once a day, depending on the institution. An Item's `status.transactions.last_successful_update` field will show the timestamp of the most recent successful update. To force Plaid to check for new transactions, use the `/transactions/refresh` endpoint.  Note that for newly created Items, data may not be immediately available to `/transactions/sync`. Plaid begins preparing transactions data when the Item is created, but the process can take anywhere from a few seconds to several minutes to complete, depending on the number of transactions available.  To be alerted when new data is available, listen for the [`SYNC_UPDATES_AVAILABLE`](https://plaid.com/docs/api/products/transactions/#sync_updates_available) webhook.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
             >>> thread = api.transactions_sync(transactions_sync_request, async_req=True)
             >>> result = thread.get()
 
             Args:
@@ -15106,15 +15724,15 @@
         def __transfer_authorization_create(
             self,
             transfer_authorization_create_request,
             **kwargs
         ):
             """Create a transfer authorization  # noqa: E501
 
-            Use the `/transfer/authorization/create` endpoint to determine transfer failure risk.  In Plaid's sandbox environment the decisions will be returned as follows:    - To approve a transfer with null rationale code, make an authorization request with an `amount` less than the available balance in the account.    - To approve a transfer with the rationale code `MANUALLY_VERIFIED_ITEM`, create an Item in Link through the [Same Day Micro-deposits flow](https://plaid.com/docs/auth/coverage/testing/#testing-same-day-micro-deposits).    - To approve a transfer with the rationale code `LOGIN_REQUIRED`, [reset the login for an Item](https://plaid.com/docs/sandbox/#item_login_required).    - To decline a transfer with the rationale code `NSF`, the available balance on the account must be less than the authorization `amount`. See [Create Sandbox test data](https://plaid.com/docs/sandbox/user-custom/) for details on how to customize data in Sandbox.    - To decline a transfer with the rationale code `RISK`, the available balance on the account must be exactly $0. See [Create Sandbox test data](https://plaid.com/docs/sandbox/user-custom/) for details on how to customize data in Sandbox.  # noqa: E501
+            Use the `/transfer/authorization/create` endpoint to determine transfer failure risk.  In Plaid's sandbox environment the decisions will be returned as follows:    - To approve a transfer with null rationale code, make an authorization request with an `amount` less than the available balance in the account.    - To approve a transfer with the rationale code `MANUALLY_VERIFIED_ITEM`, create an Item in Link through the [Same Day Micro-deposits flow](https://plaid.com/docs/auth/coverage/testing/#testing-same-day-micro-deposits).    - To approve a transfer with the rationale code `LOGIN_REQUIRED`, [reset the login for an Item](https://plaid.com/docs/sandbox/#item_login_required).    - To decline a transfer with the rationale code `NSF`, the available balance on the account must be less than the authorization `amount`. See [Create Sandbox test data](https://plaid.com/docs/sandbox/user-custom/) for details on how to customize data in Sandbox.    - To decline a transfer with the rationale code `RISK`, the available balance on the account must be exactly $0. See [Create Sandbox test data](https://plaid.com/docs/sandbox/user-custom/) for details on how to customize data in Sandbox.  For guaranteed ACH customers, the following fields are required : `user.phone_number` (optional if `email_address` provided), `user.email_address` (optional if `phone_number` provided), `device.ip_address`, `device.user_agent`, and `user_present`.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
             >>> thread = api.transfer_authorization_create(transfer_authorization_create_request, async_req=True)
             >>> result = thread.get()
 
             Args:
```

### Comparing `plaid-python-9.8.0/plaid/configuration.py` & `plaid-python-9.9.0/plaid/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,16 +423,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2020-09-14_1.146.0\n"\
-               "SDK Package Version: 9.8.0".\
+               "Version of the API: 2020-09-14_1.161.5\n"\
+               "SDK Package Version: 9.9.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `plaid-python-9.8.0/plaid/exceptions.py` & `plaid-python-9.9.0/plaid/exceptions.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/rest.py` & `plaid-python-9.9.0/plaid/rest.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/model_utils.py` & `plaid-python-9.9.0/plaid/model_utils.py`

 * *Files identical despite different names*

### Comparing `plaid-python-9.8.0/plaid/__init__.py` & `plaid-python-9.9.0/plaid/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     The Plaid API
 
     The Plaid REST API. Please see https://plaid.com/docs/api for more details.  # noqa: E501
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "9.8.0"
+__version__ = "9.9.0"
 
 # import ApiClient
 from plaid.api_client import ApiClient
 
 # import Configuration
 from plaid.configuration import Configuration
 # import Environments
```

### Comparing `plaid-python-9.8.0/plaid/models/__init__.py` & `plaid-python-9.9.0/plaid/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,14 +128,18 @@
 from plaid.model.client_user_id import ClientUserID
 from plaid.model.connected_application import ConnectedApplication
 from plaid.model.consent_payment_idempotency_key import ConsentPaymentIdempotencyKey
 from plaid.model.country_code import CountryCode
 from plaid.model.create_entity_screening_request import CreateEntityScreeningRequest
 from plaid.model.create_entity_watchlist_screening_review_request import CreateEntityWatchlistScreeningReviewRequest
 from plaid.model.create_individual_watchlist_screening_review_request import CreateIndividualWatchlistScreeningReviewRequest
+from plaid.model.credit1099 import Credit1099
+from plaid.model.credit1099_filer import Credit1099Filer
+from plaid.model.credit1099_payer import Credit1099Payer
+from plaid.model.credit1099_recipient import Credit1099Recipient
 from plaid.model.credit_account_subtype import CreditAccountSubtype
 from plaid.model.credit_account_subtypes import CreditAccountSubtypes
 from plaid.model.credit_audit_copy_token_create_request import CreditAuditCopyTokenCreateRequest
 from plaid.model.credit_audit_copy_token_create_response import CreditAuditCopyTokenCreateResponse
 from plaid.model.credit_audit_copy_token_remove_request import CreditAuditCopyTokenRemoveRequest
 from plaid.model.credit_audit_copy_token_remove_response import CreditAuditCopyTokenRemoveResponse
 from plaid.model.credit_bank_income import CreditBankIncome
@@ -145,14 +149,15 @@
 from plaid.model.credit_bank_income_cause import CreditBankIncomeCause
 from plaid.model.credit_bank_income_error_type import CreditBankIncomeErrorType
 from plaid.model.credit_bank_income_get_request import CreditBankIncomeGetRequest
 from plaid.model.credit_bank_income_get_request_options import CreditBankIncomeGetRequestOptions
 from plaid.model.credit_bank_income_get_response import CreditBankIncomeGetResponse
 from plaid.model.credit_bank_income_historical_summary import CreditBankIncomeHistoricalSummary
 from plaid.model.credit_bank_income_item import CreditBankIncomeItem
+from plaid.model.credit_bank_income_pdf_get_request import CreditBankIncomePDFGetRequest
 from plaid.model.credit_bank_income_pay_frequency import CreditBankIncomePayFrequency
 from plaid.model.credit_bank_income_refresh_request import CreditBankIncomeRefreshRequest
 from plaid.model.credit_bank_income_refresh_request_options import CreditBankIncomeRefreshRequestOptions
 from plaid.model.credit_bank_income_refresh_response import CreditBankIncomeRefreshResponse
 from plaid.model.credit_bank_income_source import CreditBankIncomeSource
 from plaid.model.credit_bank_income_summary import CreditBankIncomeSummary
 from plaid.model.credit_bank_income_transaction import CreditBankIncomeTransaction
@@ -182,14 +187,19 @@
 from plaid.model.credit_payroll_income_refresh_request import CreditPayrollIncomeRefreshRequest
 from plaid.model.credit_payroll_income_refresh_response import CreditPayrollIncomeRefreshResponse
 from plaid.model.credit_payroll_income_risk_signals_get_request import CreditPayrollIncomeRiskSignalsGetRequest
 from plaid.model.credit_payroll_income_risk_signals_get_response import CreditPayrollIncomeRiskSignalsGetResponse
 from plaid.model.credit_platform_ids import CreditPlatformIds
 from plaid.model.credit_relay_create_request import CreditRelayCreateRequest
 from plaid.model.credit_relay_create_response import CreditRelayCreateResponse
+from plaid.model.credit_relay_get_request import CreditRelayGetRequest
+from plaid.model.credit_relay_refresh_request import CreditRelayRefreshRequest
+from plaid.model.credit_relay_refresh_response import CreditRelayRefreshResponse
+from plaid.model.credit_relay_remove_request import CreditRelayRemoveRequest
+from plaid.model.credit_relay_remove_response import CreditRelayRemoveResponse
 from plaid.model.credit_w2 import CreditW2
 from plaid.model.customer_initiated_return_risk import CustomerInitiatedReturnRisk
 from plaid.model.customer_initiated_risk_tier import CustomerInitiatedRiskTier
 from plaid.model.dashboard_user import DashboardUser
 from plaid.model.dashboard_user_response import DashboardUserResponse
 from plaid.model.dashboard_user_status import DashboardUserStatus
 from plaid.model.date_range import DateRange
@@ -274,14 +284,15 @@
 from plaid.model.expiration_date import ExpirationDate
 from plaid.model.external_payment_initiation_consent_options import ExternalPaymentInitiationConsentOptions
 from plaid.model.external_payment_options import ExternalPaymentOptions
 from plaid.model.external_payment_refund_details import ExternalPaymentRefundDetails
 from plaid.model.external_payment_schedule_base import ExternalPaymentScheduleBase
 from plaid.model.external_payment_schedule_get import ExternalPaymentScheduleGet
 from plaid.model.external_payment_schedule_request import ExternalPaymentScheduleRequest
+from plaid.model.form1099_type import Form1099Type
 from plaid.model.generic_country_code import GenericCountryCode
 from plaid.model.generic_screening_hit_location_items import GenericScreeningHitLocationItems
 from plaid.model.get_dashboard_user_request import GetDashboardUserRequest
 from plaid.model.get_entity_watchlist_screening_request import GetEntityWatchlistScreeningRequest
 from plaid.model.get_identity_verification_request import GetIdentityVerificationRequest
 from plaid.model.get_individual_watchlist_screening_request import GetIndividualWatchlistScreeningRequest
 from plaid.model.get_watchlist_screening_entity_program_request import GetWatchlistScreeningEntityProgramRequest
@@ -501,14 +512,17 @@
 from plaid.model.paginated_entity_watchlist_screening_list_response import PaginatedEntityWatchlistScreeningListResponse
 from plaid.model.paginated_entity_watchlist_screening_review_list_response import PaginatedEntityWatchlistScreeningReviewListResponse
 from plaid.model.paginated_identity_verification_list_response import PaginatedIdentityVerificationListResponse
 from plaid.model.paginated_individual_watchlist_program_list_response import PaginatedIndividualWatchlistProgramListResponse
 from plaid.model.paginated_individual_watchlist_screening_hit_list_response import PaginatedIndividualWatchlistScreeningHitListResponse
 from plaid.model.paginated_individual_watchlist_screening_list_response import PaginatedIndividualWatchlistScreeningListResponse
 from plaid.model.paginated_individual_watchlist_screening_review_list_response import PaginatedIndividualWatchlistScreeningReviewListResponse
+from plaid.model.partner_customers_create_request import PartnerCustomersCreateRequest
+from plaid.model.partner_customers_create_response import PartnerCustomersCreateResponse
+from plaid.model.partner_end_customer_client import PartnerEndCustomerClient
 from plaid.model.pay import Pay
 from plaid.model.pay_frequency import PayFrequency
 from plaid.model.pay_frequency_value import PayFrequencyValue
 from plaid.model.pay_period_details import PayPeriodDetails
 from plaid.model.pay_stub_deductions_breakdown import PayStubDeductionsBreakdown
 from plaid.model.pay_stub_deductions_total import PayStubDeductionsTotal
 from plaid.model.pay_stub_distribution_breakdown import PayStubDistributionBreakdown
@@ -627,17 +641,19 @@
 from plaid.model.products import Products
 from plaid.model.program_name_sensitivity import ProgramNameSensitivity
 from plaid.model.projected_income_summary_field_number import ProjectedIncomeSummaryFieldNumber
 from plaid.model.recaptcha_required_error import RecaptchaRequiredError
 from plaid.model.recipient_bacs import RecipientBACS
 from plaid.model.recipient_bacs_nullable import RecipientBACSNullable
 from plaid.model.recurring_transaction_frequency import RecurringTransactionFrequency
+from plaid.model.recurring_transactions_update_webhook import RecurringTransactionsUpdateWebhook
 from plaid.model.relay_event import RelayEvent
 from plaid.model.removed_transaction import RemovedTransaction
 from plaid.model.report_token import ReportToken
+from plaid.model.report_type import ReportType
 from plaid.model.review_comment import ReviewComment
 from plaid.model.risk_signal_document_reference import RiskSignalDocumentReference
 from plaid.model.sandbox_bank_transfer_fire_webhook_request import SandboxBankTransferFireWebhookRequest
 from plaid.model.sandbox_bank_transfer_fire_webhook_response import SandboxBankTransferFireWebhookResponse
 from plaid.model.sandbox_bank_transfer_simulate_request import SandboxBankTransferSimulateRequest
 from plaid.model.sandbox_bank_transfer_simulate_response import SandboxBankTransferSimulateResponse
 from plaid.model.sandbox_income_fire_webhook_request import SandboxIncomeFireWebhookRequest
@@ -751,14 +767,15 @@
 from plaid.model.transfer_authorization_decision_rationale import TransferAuthorizationDecisionRationale
 from plaid.model.transfer_authorization_decision_rationale_code import TransferAuthorizationDecisionRationaleCode
 from plaid.model.transfer_authorization_device import TransferAuthorizationDevice
 from plaid.model.transfer_authorization_guarantee_decision import TransferAuthorizationGuaranteeDecision
 from plaid.model.transfer_authorization_guarantee_decision_rationale import TransferAuthorizationGuaranteeDecisionRationale
 from plaid.model.transfer_authorization_guarantee_decision_rationale_code import TransferAuthorizationGuaranteeDecisionRationaleCode
 from plaid.model.transfer_authorization_proposed_transfer import TransferAuthorizationProposedTransfer
+from plaid.model.transfer_authorization_user_in_request import TransferAuthorizationUserInRequest
 from plaid.model.transfer_cancel_request import TransferCancelRequest
 from plaid.model.transfer_cancel_response import TransferCancelResponse
 from plaid.model.transfer_create_idempotency_key import TransferCreateIdempotencyKey
 from plaid.model.transfer_create_request import TransferCreateRequest
 from plaid.model.transfer_create_response import TransferCreateResponse
 from plaid.model.transfer_event import TransferEvent
 from plaid.model.transfer_event_list_request import TransferEventListRequest
```

### Comparing `plaid-python-9.8.0/plaid/api_client.py` & `plaid-python-9.9.0/plaid/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = { 'Plaid-Version': '2020-09-14' }
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Plaid Python v9.8.0'
+        self.user_agent = 'Plaid Python v9.9.0'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `plaid-python-9.8.0/plaid_python.egg-info/SOURCES.txt` & `plaid-python-9.9.0/plaid_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,18 @@
 plaid/model/client_user_id.py
 plaid/model/connected_application.py
 plaid/model/consent_payment_idempotency_key.py
 plaid/model/country_code.py
 plaid/model/create_entity_screening_request.py
 plaid/model/create_entity_watchlist_screening_review_request.py
 plaid/model/create_individual_watchlist_screening_review_request.py
+plaid/model/credit1099.py
+plaid/model/credit1099_filer.py
+plaid/model/credit1099_payer.py
+plaid/model/credit1099_recipient.py
 plaid/model/credit_account_subtype.py
 plaid/model/credit_account_subtypes.py
 plaid/model/credit_audit_copy_token_create_request.py
 plaid/model/credit_audit_copy_token_create_response.py
 plaid/model/credit_audit_copy_token_remove_request.py
 plaid/model/credit_audit_copy_token_remove_response.py
 plaid/model/credit_bank_income.py
@@ -146,14 +150,15 @@
 plaid/model/credit_bank_income_error_type.py
 plaid/model/credit_bank_income_get_request.py
 plaid/model/credit_bank_income_get_request_options.py
 plaid/model/credit_bank_income_get_response.py
 plaid/model/credit_bank_income_historical_summary.py
 plaid/model/credit_bank_income_item.py
 plaid/model/credit_bank_income_pay_frequency.py
+plaid/model/credit_bank_income_pdf_get_request.py
 plaid/model/credit_bank_income_refresh_request.py
 plaid/model/credit_bank_income_refresh_request_options.py
 plaid/model/credit_bank_income_refresh_response.py
 plaid/model/credit_bank_income_source.py
 plaid/model/credit_bank_income_summary.py
 plaid/model/credit_bank_income_transaction.py
 plaid/model/credit_bank_income_warning.py
@@ -182,14 +187,19 @@
 plaid/model/credit_payroll_income_refresh_request.py
 plaid/model/credit_payroll_income_refresh_response.py
 plaid/model/credit_payroll_income_risk_signals_get_request.py
 plaid/model/credit_payroll_income_risk_signals_get_response.py
 plaid/model/credit_platform_ids.py
 plaid/model/credit_relay_create_request.py
 plaid/model/credit_relay_create_response.py
+plaid/model/credit_relay_get_request.py
+plaid/model/credit_relay_refresh_request.py
+plaid/model/credit_relay_refresh_response.py
+plaid/model/credit_relay_remove_request.py
+plaid/model/credit_relay_remove_response.py
 plaid/model/credit_w2.py
 plaid/model/customer_initiated_return_risk.py
 plaid/model/customer_initiated_risk_tier.py
 plaid/model/dashboard_user.py
 plaid/model/dashboard_user_response.py
 plaid/model/dashboard_user_status.py
 plaid/model/date_range.py
@@ -274,14 +284,15 @@
 plaid/model/expiration_date.py
 plaid/model/external_payment_initiation_consent_options.py
 plaid/model/external_payment_options.py
 plaid/model/external_payment_refund_details.py
 plaid/model/external_payment_schedule_base.py
 plaid/model/external_payment_schedule_get.py
 plaid/model/external_payment_schedule_request.py
+plaid/model/form1099_type.py
 plaid/model/generic_country_code.py
 plaid/model/generic_screening_hit_location_items.py
 plaid/model/get_dashboard_user_request.py
 plaid/model/get_entity_watchlist_screening_request.py
 plaid/model/get_identity_verification_request.py
 plaid/model/get_individual_watchlist_screening_request.py
 plaid/model/get_watchlist_screening_entity_program_request.py
@@ -499,14 +510,17 @@
 plaid/model/paginated_entity_watchlist_screening_list_response.py
 plaid/model/paginated_entity_watchlist_screening_review_list_response.py
 plaid/model/paginated_identity_verification_list_response.py
 plaid/model/paginated_individual_watchlist_program_list_response.py
 plaid/model/paginated_individual_watchlist_screening_hit_list_response.py
 plaid/model/paginated_individual_watchlist_screening_list_response.py
 plaid/model/paginated_individual_watchlist_screening_review_list_response.py
+plaid/model/partner_customers_create_request.py
+plaid/model/partner_customers_create_response.py
+plaid/model/partner_end_customer_client.py
 plaid/model/pay.py
 plaid/model/pay_frequency.py
 plaid/model/pay_frequency_value.py
 plaid/model/pay_period_details.py
 plaid/model/pay_stub_deductions_breakdown.py
 plaid/model/pay_stub_deductions_total.py
 plaid/model/pay_stub_distribution_breakdown.py
@@ -627,17 +641,19 @@
 plaid/model/program_name_sensitivity.py
 plaid/model/projected_income_summary_field_number.py
 plaid/model/pslf_status.py
 plaid/model/recaptcha_required_error.py
 plaid/model/recipient_bacs.py
 plaid/model/recipient_bacs_nullable.py
 plaid/model/recurring_transaction_frequency.py
+plaid/model/recurring_transactions_update_webhook.py
 plaid/model/relay_event.py
 plaid/model/removed_transaction.py
 plaid/model/report_token.py
+plaid/model/report_type.py
 plaid/model/review_comment.py
 plaid/model/risk_signal_document_reference.py
 plaid/model/sandbox_bank_transfer_fire_webhook_request.py
 plaid/model/sandbox_bank_transfer_fire_webhook_response.py
 plaid/model/sandbox_bank_transfer_simulate_request.py
 plaid/model/sandbox_bank_transfer_simulate_response.py
 plaid/model/sandbox_income_fire_webhook_request.py
@@ -751,14 +767,15 @@
 plaid/model/transfer_authorization_decision_rationale.py
 plaid/model/transfer_authorization_decision_rationale_code.py
 plaid/model/transfer_authorization_device.py
 plaid/model/transfer_authorization_guarantee_decision.py
 plaid/model/transfer_authorization_guarantee_decision_rationale.py
 plaid/model/transfer_authorization_guarantee_decision_rationale_code.py
 plaid/model/transfer_authorization_proposed_transfer.py
+plaid/model/transfer_authorization_user_in_request.py
 plaid/model/transfer_cancel_request.py
 plaid/model/transfer_cancel_response.py
 plaid/model/transfer_create_idempotency_key.py
 plaid/model/transfer_create_request.py
 plaid/model/transfer_create_response.py
 plaid/model/transfer_event.py
 plaid/model/transfer_event_list_request.py
```

### Comparing `plaid-python-9.8.0/plaid_python.egg-info/PKG-INFO` & `plaid-python-9.9.0/plaid_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: plaid-python
-Version: 9.8.0
+Version: 9.9.0
 Summary: Python client library for the Plaid API and Link
 Home-page: https://github.com/plaid/plaid-python
 Author: Plaid Inc.
 Author-email: developers@plaid.com
 License: MIT
-Download-URL: https://github.com/plaid/plaid-python/tarball/v9.8.0
+Download-URL: https://github.com/plaid/plaid-python/tarball/v9.9.0
 Description: UNKNOWN
 Keywords: api,client,plaid
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `plaid-python-9.8.0/PKG-INFO` & `plaid-python-9.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: plaid-python
-Version: 9.8.0
+Version: 9.9.0
 Summary: Python client library for the Plaid API and Link
 Home-page: https://github.com/plaid/plaid-python
 Author: Plaid Inc.
 Author-email: developers@plaid.com
 License: MIT
-Download-URL: https://github.com/plaid/plaid-python/tarball/v9.8.0
+Download-URL: https://github.com/plaid/plaid-python/tarball/v9.9.0
 Description: UNKNOWN
 Keywords: api,client,plaid
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

