# Comparing `tmp/policyengine-canada-0.94.0.tar.gz` & `tmp/policyengine-canada-0.95.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "policyengine-canada-0.94.0.tar", last modified: Fri Mar 15 03:17:27 2024, max compression
+gzip compressed data, was "policyengine-canada-0.95.0.tar", last modified: Mon Apr 22 23:29:26 2024, max compression
```

## Comparing `policyengine-canada-0.94.0.tar` & `policyengine-canada-0.95.0.tar`

### file list

```diff
@@ -1,1523 +1,1529 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.397791 policyengine-canada-0.94.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-15 03:17:27.397791 policyengine-canada-0.94.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.261792 policyengine-canada-0.94.0/policyengine_canada/
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.261792 policyengine-canada-0.94.0/policyengine_canada/data/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.261792 policyengine-canada-0.94.0/policyengine_canada/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/data/datasets/country_template_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/model_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/modelled_policies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.233792 policyengine-canada-0.94.0/policyengine_canada/parameters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.213792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.261792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.209792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.261792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/ccb/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/ccb/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/ccb/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/ccb/divisor.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.261792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/four_or_more_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/one_child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/three_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/two_children.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.261792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cdb/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cdb/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cdb/base.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.261792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cdb/reduction/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cdb/reduction/one_child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cdb/reduction/two_or_more_children.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.261792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.265792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/amount/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/amount/disability_supplement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/amount/family.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/amount/single.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/eligible_age.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.265792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.265792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/base/family.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/base/single.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/disability_supplement.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.265792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.265792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/base/family.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/base/single.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.265792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/disability_supplement/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/disability_supplement/family_with_one_spouse_disabled.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/disability_supplement/family_with_two_spouses_disabled.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/disability_supplement/single.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/working_income_sources.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.265792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/dental_benefit/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/dental_benefit/additional_benefit_threshold.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/dental_benefit/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/dental_benefit/ineligible_age.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/dental_benefit/shared_custody_share.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.265792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.265792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/amount/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/amount/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/amount/older_seniors_increase_factor.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.213792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/eligibility/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.265792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/eligibility/age/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/eligibility/age/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/eligibility/age/older_seniors_increase.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.265792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/eligibility/residence/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/eligibility/residence/any.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/eligibility/residence/full_base_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/repayment_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.213792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.265792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.265792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.265792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/age_amount_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/age_amount_credit/age_eligibility.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.265792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/age_amount_credit/amount/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/age_amount_credit/amount/credit_cap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/age_amount_credit/amount/reduction.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.269792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/max_amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.213792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/phase_out/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.269792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/phase_out/threshold/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/phase_out/threshold/end.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/phase_out/threshold/start.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.269792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/canada_employment_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/canada_employment_amount/income_sources.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/canada_employment_amount/max_amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.269792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/climate_action_incentive/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/climate_action_incentive/adult_age.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/climate_action_incentive/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/climate_action_incentive/rural.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.269792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/dtc/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/dtc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/dtc/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/dtc/child_supplement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/dtc/supplement_ineligible_age.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.269792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/adult_age.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/base_amounts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/reduction.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.269792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/singles_boost/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/singles_boost/cap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/singles_boost/phase_in.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/non_refundable.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/refundable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.269792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/school_supply_credit/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/school_supply_credit/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/school_supply_credit/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/school_supply_credit/cap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.269792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.269792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/age_eligibility/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/age_eligibility/max.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/age_eligibility/min.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/income_sources.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/lifetime_cap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/income_tax_schedule.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.229792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.269792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.269792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.273792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/age_eligibility.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.213792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.273792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/base/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/base/four_or_more_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/base/one_child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/base/three_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/base/two_children.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.273792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/four_or_more_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/one_child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/three_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/two_children.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.213792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.273792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/four_or_more_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/one_child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/three_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/two_children.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.273792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_in/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_in/rate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_in/start.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.273792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/four_or_more_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/one_child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/three_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/two_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/benefits.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.213792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.273792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.273792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.273792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/age_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/age_credit/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/age_credit/eligible_age.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/age_credit/phase_out_rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.273792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.273792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/additional_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/additional_amount/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/additional_amount/childcare_expense_threshold.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/cap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/non_refundable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.277792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/pension/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/pension/max_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/refundable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.277792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/spouse_and_common_law_partner_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/spouse_and_common_law_partner_amount/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.277792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.277792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.277792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.277792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/base/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/base/one_child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/base/three_or_more_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/base/two_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/child_ineligible_age_threshold.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.277792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/first_reduction/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.277792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/first_reduction/max_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/first_reduction/max_amount/one_child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/first_reduction/max_amount/three_or_more_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/first_reduction/max_amount/two_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/first_reduction/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.277792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/second_reduction/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/second_reduction/rate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/benefits.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.217792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.277792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.277792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.277792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/age/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/age/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/age/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/age/eligible_age.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.277792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/age/phase_out/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/age/phase_out/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/age/phase_out/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.277792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/basic_personal_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/basic_personal_amount/base.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.277792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/adult_age.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.277792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/reduction_rate/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/reduction_rate/family.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/reduction_rate/single.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.277792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/disability/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.281792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/disability/additional_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/disability/additional_amount/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/disability/additional_amount/childcare_expense_threshold.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/disability/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/non_refundable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.281792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/pension_income_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/pension_income_amount/cap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/refundable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.281792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/tax_reduction/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/tax_reduction/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/tax_reduction/reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.281792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.217792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.281792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/eligible_age.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/max_child_count.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.281792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/five_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/four_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/one_child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/six_or_more_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/three_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/two_children.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.217792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.281792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.281792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.281792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/age_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/age_amount/age_eligibility.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/age_amount/max_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/age_amount/phase_out_rate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/basic_personal_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/non_refundable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.281792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/pension_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/pension_amount/max_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/refundable.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.281792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.281792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/benefits.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.281792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/eligible_age.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.281792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/phase_out/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/phase_out/multiple_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/phase_out/one_child.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.281792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/working_income_supplement/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/working_income_supplement/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/working_income_supplement/phase_in.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/working_income_supplement/phase_out.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.281792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/pension_benefit/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/pension_benefit/cap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.217792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.281792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.217792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.285791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/age_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/age_amount/age_eligibility.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/age_amount/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/age_amount/reduction_rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.285791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.285791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/base/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/base/dependant.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/base/head.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/base/max_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/base/spouse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/child_eligible_age.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/rate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.285791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nl/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nl/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.221792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nl/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.285791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.221792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.285791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/credits/physical_activity/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/credits/physical_activity/age_eligible.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/credits/physical_activity/max_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/credits/physical_activity/rate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.285791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.285791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/benefits/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/benefits/benefits.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.285791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/benefits/child_benefit/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/benefits/child_benefit/age_eligibility.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/benefits/child_benefit/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/benefits/child_benefit/higher_income_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/benefits/child_benefit/lower_threshold.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/benefits/child_benefit/upper_threshold.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.221792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.285791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.285791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.285791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/age/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/age/age_eligibility.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/age/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/age/income_eligibility.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.285791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/disability_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/disability_amount/base.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.285791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/age_eligibility.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.285791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/base.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/dependant/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/dependant/age_eligibility.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/dependant/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/eligible_dependant.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/max_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/spouse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/phase_out.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/non_refundable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/nsaltc/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/nsaltc/child_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/nsaltc/individual_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/nsaltc/reduction.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/pension_income_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/pension_income_amount/cap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/prc/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/prc/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/prc/income_threshold.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/refundable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.221792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.221792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/eligibility/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/eligibility/age/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/eligibility/age/lower.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/eligibility/age/main.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/applicable_assets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/limit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nt/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nt/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.221792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nt/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.221792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/age_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/age_credit/age_eligibility.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/age_credit/max_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/age_credit/reduction.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/basic_personal_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/basic_personal_amount/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.221792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/benefits.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/age_limit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/base/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/base/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/base/phase_out_rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/working/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/working/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/working/phase_in_rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/age_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/age_amount/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/age_amount/eligible_age.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/age_amount/phase_out_rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/cost_of_living/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/cost_of_living/max_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/cost_of_living/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/cost_of_living/supplement_for_single_parents/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/cost_of_living/supplement_for_single_parents/income.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/cost_of_living/supplement_for_single_parents/max_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/cost_of_living/supplement_for_single_parents/rate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/non_refundable.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.289791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/benefits/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/benefits/benefits.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.293791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/benefits/ocb/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/benefits/ocb/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/benefits/ocb/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/benefits/ocb/reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/benefits/ocb/shared_custody_divisor.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.225792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/subsidies/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.293791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/child_age_eligibility.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/full_time_calculation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/part_time_child_care_multiplier.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.293791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/reduction/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/reduction/age.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/reduction/factor.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.225792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.225792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.293791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/age_eligibility.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/max_amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.293791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/reduction/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/reduction/family.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/reduction/single.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.293791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.293791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.293791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/phase_in_rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.293791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/reduction/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/reduction/family.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/reduction/single.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.293791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/age_eligibility.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/child_max_age.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.293791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.293791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/shared_custody/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/shared_custody/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/shared_custody/divisor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/shared_custody/start.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/start.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/non_refundable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.293791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/child_max_age.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.297791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/energy_component/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/energy_component/max_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/energy_component/multiplier.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/energy_component/student_resident_reduction.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.297791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/occupancy_costs/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/occupancy_costs/rent_multiplier.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/occupancy_costs/student_resident_supplement.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.297791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.297791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/shared_custody/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/shared_custody/divisor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/shared_custody/start.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/start.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.297791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/property_tax_component/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/property_tax_component/initial_cap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/property_tax_component/multiplier.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/property_tax_component/supplement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/second_subtraction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/senior_age.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.297791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/ostc/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/ostc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/ostc/amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.297791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/ostc/reduction/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/ostc/reduction/family.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/ostc/reduction/single.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/refundable.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.297791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/pe/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/pe/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.225792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/pe/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.297791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/pe/tax/income/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/pe/tax/income/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.225792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.225792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.297791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.297791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/basic_personal_amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.297791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cce/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cce/age_eligibility.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cce/child_income_limit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cce/disabled_child_expense_limit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cce/nondisabled_child_expense_limit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cce/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.297791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cost_of_living/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cost_of_living/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cost_of_living/reduction.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.297791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/age_eligibility.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.297791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/child_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/child_amount/max.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/child_amount/min.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.297791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/reduction/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/reduction/single_parent_family.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/reduction/two_parent_family.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/shared_custody_multiplier.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.297791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/single_parent_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/single_parent_amount/max.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/single_parent_amount/min.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.229792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/handicapped_child/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/handicapped_child/base_amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/handicapped_child/exceptional_care_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/handicapped_child/exceptional_care_amount/tier1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/handicapped_child/exceptional_care_amount/tier2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/school_supplies/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/school_supplies/handicapped_child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/school_supplies/non_handicapped_child.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/age_eligibility.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/amount/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/amount/married_both_eligible.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/amount/married_one_eligible.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/amount/single.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/reduction/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/reduction/married.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/reduction/single.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/couple/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/couple/amount/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/couple/amount/with_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/couple/amount/without_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/couple/reduction.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/single/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/single/amount/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/single/amount/person_living_alone.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/single/amount/single_parent.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/single/reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/work_income_requirement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/age_eligibility.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.229792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/amount/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/amount/with_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/amount/without_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/work_income_requirement.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/amount/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/amount/person_living_alone.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/amount/single_parent.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/work_income_requirement.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/supplement/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/supplement/amount/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/supplement/amount/couple.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/supplement/amount/single.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/supplement/work_income_eligibility.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.229792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.301792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/amount/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/amount/disabled.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/amount/non_disabled.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.305791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/eligibility/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/eligibility/age.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/eligibility/income.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/benefits/benefits.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.229792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.305791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.229792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.305791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/age_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/age_amount/age_eligibility.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/age_amount/max_amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.305791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/age_amount/reduction/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/age_amount/reduction/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.305791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/disability_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/disability_amount/amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.305791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/age_threshold.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.305791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.305791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/child/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/child/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/child/ineligible_age.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/child/max_number.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/head.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/phase_out.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/spouse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.305791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.233792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.305791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/child_benefit/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/child_benefit/base.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.305791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/child_benefit/multiple_children/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/child_benefit/multiple_children/reduction_rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.305791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/child_benefit/one_child/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/child_benefit/one_child/reduction_rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.233792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.305791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.305791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/amount/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/amount/child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/amount/self.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/amount/spouse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/child_ineligible_age.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.309791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/non_whitehorse_supplement/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/non_whitehorse_supplement/child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/non_whitehorse_supplement/self.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/non_whitehorse_supplement/spouse.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.233792 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.309791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.309791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.309791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_arts_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_arts_credit/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_arts_credit/child_age_eligibility.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.309791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_fitness/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_fitness/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_fitness/child_age_eligibility.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.309791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_fitness/disability_supplement/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_fitness/disability_supplement/age.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_fitness/disability_supplement/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_fitness/disability_supplement/minimum_fees.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_fitness/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.309791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/employment_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/employment_amount/amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.309791 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/first_nations_tax/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/first_nations_tax/rate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/non_refundable.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.309791 policyengine-canada-0.94.0/policyengine_canada/parameters/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/parameters/simulation/marginal_tax_rate_adults.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.309791 policyengine-canada-0.94.0/policyengine_canada/reforms/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/reforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.309791 policyengine-canada-0.94.0/policyengine_canada/situation_examples/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/situation_examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.245792 policyengine-canada-0.94.0/policyengine_canada/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.309791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.233792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.233792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.309791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/ccb/
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/ccb/child_benefit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.309791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cdb/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cdb/child_disability_benefit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cdb/child_disability_benefit_eligible.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cdb/child_disability_benefit_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cdb/integration.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.313791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.313791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/base/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/base/cwb_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/base/cwb_base_max_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/base/cwb_base_phase_in.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/base/cwb_base_phase_out.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/canada_workers_benefit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/cwb_dependant.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/cwb_eligible.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.313791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_category.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_eligible.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_max_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_phase_in.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_phase_out.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/is_cwb_family.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.313791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/dental_benefit/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/dental_benefit/dental_benefit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/dental_benefit/dental_benefit_eligible.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.313791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/oas/
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/oas/integration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/oas/oas_eligibility.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/oas/oas_pre_repayment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/oas/oas_repayment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.233792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.313791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.313791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/age_amount_credit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.313791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/basic_personal_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/basic_personal_amount/basic_personal_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/basic_personal_amount/basic_personal_amount_supplement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/canada_employment_amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.317791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/climate_action_incentive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/climate_action_incentive_dependant_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/climate_action_incentive_person.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/climate_action_incentive_single_parent_household.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/integration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/integration_eldest_child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/is_child_for_climate_action_incentive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/is_eldest_child_for_climate_action_incentive.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.317791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/dtc/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/dtc/dtc_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/dtc/dtc_child_supplement.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.317791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit_category.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit_person.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit_single_parent_household.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit_singles_boost.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/integration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/is_child_for_gst_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/is_eldest_child_in_single_household_for_gst_credit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.317791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/school_supply_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/school_supply_credit/school_supply_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/training_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/income_tax_before_credits.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/income_tax_before_refundable_credits.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/integration.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.233792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.233792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.317791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_base_component.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_base_component_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_base_component_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_eligible_child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_working_component.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_working_component_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_working_component_reduction.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.233792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.321791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.233792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.321791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/ab_spouse_and_common_law_partner_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/ab_spouse_and_common_law_partner_amount/ab_spouse_and_common_law_partner_amount_credit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.321791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/age_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/age_credit/ab_age_credit_eligible.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/age_credit/age_credit_amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.321791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/disability/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit_additional_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit_eligible.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.321791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/pension/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/pension/ab_pension_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/income_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.237792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.237792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.321791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/benefits/bcfb/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/benefits/bcfb/bc_family_benefit_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/benefits/bcfb/bc_family_benefit_first_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/benefits/bcfb/bc_family_benefit_second_reduction.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.237792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.321791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.321791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.321791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/basic_personal_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/basic_personal_amount/bc_basic_personal_amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.321791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_age_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_age_credit/bc_age_credit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.321791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_disability_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit_additional_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit_eligible.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.321791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_pension_income_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_pension_income_amount/bc_pension_income_amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.321791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_tax_reduction_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_tax_reduction_credit/bc_tax_reduction_credit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.325791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_person.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_single_parent_household.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/integration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/is_child_for_bc_climate_action_tax_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/is_eldest_child_for_bc_climate_action_tax_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bx_income_tax_before_refundable_credits.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/income_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.237792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/mb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.237792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/mb/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.325791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/mb/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.325791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/mb/tax/income/benefits/
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/mb/tax/income/benefits/mb_child_benefit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/mb/tax/income/benefits/mb_child_benefit_eligible_child.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.325791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.325791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/age_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/age_amount/mb_age_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/age_amount/mb_age_credit_eligible.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/mb_basic_personal_amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.325791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/pension_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/pension_amount/mb_pension_amount_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/mb/tax/income/income_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.237792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.237792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.325791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/benefits/nbcb/
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/benefits/nbcb/nb_child_benefit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/benefits/nbcb/nb_child_benefit_supplement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/benefits/nbcb/nb_family_benefit_eligible_child.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.325791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/pension_benefits/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/pension_benefits/nb_pension_benefit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.237792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.325791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.325791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.325791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/nb_low_income_tax_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/nb_low_income_tax_reduction_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/tax/income/credits/nb_age_amount_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/tax/income/income_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.237792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.237792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nl/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.325791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nl/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.325791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nl/tax/income/credits/
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nl/tax/income/credits/nl_phyical_activity_tax_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nl/tax/income/income_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.237792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.237792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.325791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/benefits/child_benefit/
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/benefits/child_benefit/ns_child_benefit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/benefits/child_benefit/ns_child_benefit_eligible_child.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.237792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.325791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.325791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.325791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/age/
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/age/ns_age_tax_credit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.329791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_base_children.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_eligible_child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/ns_disability_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/ns_pension_income_amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.329791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/nsaltc/
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/nsaltc/ns_affordable_living_tax_credit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.329791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/prc/
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/prc/ns_poverty_reduction_credit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.237792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_assistance/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.237792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_assistance/eligibility/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.329791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_assistance/eligibility/age/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_assistance/eligibility/age/ns_income_assistance_age_eligibility.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.329791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/ns_income_assistance_asset_eligibility.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.237792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.237792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nt/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.329791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nt/tax/income/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nt/tax/income/income_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nt/tax/income/nt_age_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nt/tax/income/nt_age_credit_eligible.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nt/tax/income/nt_basic_personal_amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.329791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/nu_child_benefit_base_component.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/nu_child_benefit_base_component_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/nu_child_benefit_base_component_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/nu_child_benefit_eligible_child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/nu_child_benefit_working_component.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.329791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.329791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.329791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/age_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/age_amount/nu_age_amount_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/age_amount/nu_age_amount_credit_eligible_person.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/nu_cost_of_living_basic_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/nu_cost_of_living_credit_adjusted_net_income.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/nu_cost_of_living_credit_supplement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/tax/income/income_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.329791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/benefits/ocb/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/benefits/ocb/on_child_benefit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/benefits/ocb/on_child_benefit_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/benefits/ocb/on_child_benefit_reduction.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/grants/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.333791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/grants/oshptg/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant_reduction.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.333791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.333791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.333791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/lift/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit_eligible.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.333791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/noec/
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/noec/northern_ontario_energy_credit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.333791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/integration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/is_senior_for_oeptc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oeptc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oeptc_energy_component.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oeptc_occupancy_costs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oeptc_property_tax_component.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oshptg_adjusted_opetc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/on_income_tax_before_refundable_credits.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.333791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/ostc/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/income_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.333791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/is_child_for_on_child_care_fee_subsidy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/is_child_for_on_child_care_fee_subsidy_reduction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_full_time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_part_time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_reduction.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/pe/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/pe/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.333791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/pe/tax/income/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/pe/tax/income/income_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.333791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.337791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.337791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/cce/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/cce/cce_disabled_child_tax_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/cce/cce_nondisabled_child_tax_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/cce/cce_tax_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/cost_of_living.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.337791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/fa/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/fa/qc_fa_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/fa/qc_fa_eligibility.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/fa/qc_fa_payment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/fa/qc_fa_supplement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/qc_basic_personal_amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.337791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/qc_sa_married_both_eligible.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/qc_sa_married_one_eligible.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/qc_sa_single_eligible.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/qc_sa_spouse_eligible.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/qc_sa_tax_credit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.337791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.337791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/qc_adapted_work_premium_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/qc_adapted_work_premium_eligible.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.337791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/qc_general_work_premium_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/qc_general_work_premium_eligible.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit_supplement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_eligible.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/income_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.337791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/benefits/afb/
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/benefits/afb/sk_active_family_benefit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.337791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.337791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.341791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/age_amount/
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/age_amount/sk_age_amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/age_amount/sk_age_amount_eligible.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/sk_disability_amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.341791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/sk_senior_supplementary_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/sk_senior_supplementary_eligible.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.341791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/slic/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit_eligible_child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/income_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.241792 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.341791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.341791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/benefits/
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/benefits/yt_child_benefit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/benefits/yt_child_benefit_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/benefits/yt_child_benefit_eligible_child.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.341791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/benefits/yt_employment_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/benefits/yt_employment_amount/yt_employment_amount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.341791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.341791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_arts_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit_eligible_child.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.341791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_disabled_child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_eligible_child.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_childrens_fitness_tax_credit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_childrens_fitness_tax_credit_disability_supplement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/yt_first_nations_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/income_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.341791 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/rebates/
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/rebates/yt_government_carbon_price_rebate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.245792 policyengine-canada-0.94.0/policyengine_canada/tests/household/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.341791 policyengine-canada-0.94.0/policyengine_canada/tests/household/person/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/household/person/is_dependant.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/household/person/person_index.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tests/household/person/spouse_income.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.341791 policyengine-canada-0.94.0/policyengine_canada/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/tools/general.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.345791 policyengine-canada-0.94.0/policyengine_canada/variables/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.345791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/benefits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.345791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/adjusted_family_net_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.245792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.345791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/ccb/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit_base_person.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit_eligible.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit_eligible_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/ccb/family_net_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.345791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cdb/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cdb/child_disability_benefit.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cdb/child_disability_benefit_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cdb/child_disability_benefit_eligible.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cdb/child_disability_benefit_reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.345791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.345791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/base/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/base/cwb_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/base/cwb_base_max_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/base/cwb_base_phase_in.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/base/cwb_base_phase_out.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/canada_workers_benefit.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/cwb_dependant.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/cwb_eligible.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.349791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_eligible.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_max_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_phase_in.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_phase_out.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/family_working_income.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/is_cwb_family.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/working_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.349791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/dental_benefit/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/dental_benefit/additional_dental_benefit.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/dental_benefit/dental_benefit.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/dental_benefit/dental_benefit_eligible.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.349791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/old_age_security_pension/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/old_age_security_pension/oas_eligibility.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/old_age_security_pension/oas_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/old_age_security_pension/oas_pre_repayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/old_age_security_pension/oas_repayment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.349791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/deductions/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/deductions/deductions_from_total_to_net_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.245792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.349791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.349791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.349791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/age_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/age_amount/age_amount_credit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.349791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/basic_personal_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/basic_personal_amount/basic_personal_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/basic_personal_amount/basic_personal_amount_supplement.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/canada_employment_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.353791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive_dependant_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive_person.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive_pre_rural.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive_single_parent_household.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/is_child_for_climate_action_incentive.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/is_eldest_child_for_climate_action_incentive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.353791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/dtc/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/dtc/disability_tax_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/dtc/dtc_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/dtc/dtc_child_supplement.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/dtc/dtc_eligible.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.353791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_dependant_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_person.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_single_parent_household.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_singles_boost.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/is_child_for_gst_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/is_eldest_child_in_single_household_for_gst_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/non_refundable_tax_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/refundable_tax_credits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.353791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/school_supply_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/school_supply_credit/school_supply_credit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.353791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/training/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/training/prior_training_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/training/training_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/training/training_credit_income.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/income_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/income_tax_before_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/income_tax_before_refundable_credits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.353791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/uccb/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/uccb/universal_child_care_benefit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.353791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/esdc/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/esdc/maternity_and_parental_benefit.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/esdc/registered_disability_savings_plan_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.257792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.245792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.353791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/benefits/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/benefits/ab_benefits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.357791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_base_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_base_component_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_base_component_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_eligible_child.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_eligible_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_working_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_working_component_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_working_component_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/alberta_child_and_family_benefit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.245792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.357791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/ab_income_tax_before_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/ab_income_tax_before_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/ab_taxable_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.357791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/ab_non_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/ab_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/ab_spouse_and_common_law_partner_amount_credit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.357791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/age_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/age_credit/ab_age_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/age_credit/ab_age_credit_eligible.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.357791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/disability/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit_additional_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit_eligible.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.357791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/pension/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/pension/ab_pension_credit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.245792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.357791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/benefits/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/benefits/bc_benefits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.357791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit_eligible_child.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit_eligible_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit_first_reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.249792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.361791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/bc_income_tax_before_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/bc_income_tax_before_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/bc_taxable_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.361791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.361791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/basic_personal_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/basic_personal_amount/bc_basic_personal_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.361791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_age_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_age_credit/bc_age_credit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.361791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_disability_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit_additional_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit_eligible.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_non_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_refundable_credits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.361791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_tax_reduction_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_tax_reduction_credit/bc_tax_reduction_credit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.361791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_incentive_category.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_dependant_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_person.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_single_parent_household.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/is_child_for_bc_climate_action_tax_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/is_eldest_child_for_bc_climate_action_tax_credit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.361791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/pension_income_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/pension_income_amount/bc_pension_income_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.249792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.249792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.361791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.249792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.361791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/benefits/child_benefit/
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/benefits/child_benefit/mb_child_benefit.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/benefits/child_benefit/mb_child_benefit_eligible_child.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/benefits/child_benefit/mb_child_benefit_eligible_children.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.361791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.361791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/age_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/age_amount/mb_age_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/age_amount/mb_age_credit_eligible.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/mb_basic_personal_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/mb_non_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/mb_refundable_credits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.365791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/pension_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/pension_amount/mb_pension_amount_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/mb_income_tax_before_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/mb_income_tax_before_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/mb_taxable_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.249792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.365791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/benefits/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/benefits/nb_benefits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.365791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/benefits/nbcb/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/benefits/nbcb/nb_child_benefit.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/benefits/nbcb/nb_child_benefit_eligible_child.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/benefits/nbcb/nb_child_benefit_eligible_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/benefits/nbcb/nb_child_benefit_supplement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.365791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/benefits/pension_benefit/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/benefits/pension_benefit/nb_pension_benefit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.249792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.365791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.249792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.365791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/age_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/age_amount/nb_age_amount_credit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.365791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/nb_low_income_tax_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/nb_low_income_tax_reduction_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/tax/income/nb_income_tax_before_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/tax/income/nb_income_tax_before_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/tax/income/nb_taxable_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.249792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.249792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nl/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.365791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nl/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.365791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nl/tax/income/credit/
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nl/tax/income/credit/nl_physical_activity_tax_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nl/tax/income/nl_income_tax_before_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nl/tax/income/nl_income_tax_before_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nl/tax/income/nl_taxable_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.249792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.365791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.365791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/benefits/child_benefit/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/benefits/child_benefit/ns_child_benefit.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/benefits/child_benefit/ns_child_benefit_eligible_child.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/benefits/child_benefit/ns_child_benefit_eligible_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/benefits/ns_benefits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.249792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.365791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.365791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.365791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/age/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/age/ns_age_tax_credit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.369791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_base_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_eligible_child.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_eligible_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/ns_disability_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/ns_non_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/ns_pension_income_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/ns_refundable_credits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.369791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/nsaltc/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/nsaltc/ns_affordable_living_tax_credit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.369791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/prc/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/prc/ns_poverty_reduction_credit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.369791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.249792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.369791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/age/
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/age/ns_income_assistance_age_eligibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.369791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/ns_income_assistance_applicable_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/ns_income_assistance_asset_eligibility.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/ns_income_assistance.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/ns_income_tax_before_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/ns_income_tax_before_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/ns_taxable_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.249792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.253792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nt/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.369791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nt/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.253792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.369791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/age_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/age_credit/nt_age_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/age_credit/nt_age_credit_eligible.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.369791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/basic_personal_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/basic_personal_amount/nt_basic_personal_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nt/tax/income/nt_income_tax_before_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nt/tax/income/nt_income_tax_before_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nt/tax/income/nt_taxable_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.253792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.253792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.369791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.369791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_benefits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.369791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_base_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_base_component_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_base_component_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_eligible_child.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_eligible_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_working_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.373791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.373791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/age_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/age_amount/nu_age_amount_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/age_amount/nu_age_amount_credit_eligible.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/nu_cost_of_living_basic_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/nu_cost_of_living_credit_adjusted_net_income.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/nu_cost_of_living_credit_post_supplement.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/nu_cost_of_living_credit_supplement.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/nu_non_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/nu_income_tax_before_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/nu_income_tax_before_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/nu_taxable_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.253792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.373791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.373791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/benefits/ocb/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/benefits/ocb/on_child_benefit.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/benefits/ocb/on_child_benefit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/benefits/ocb/on_child_benefit_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/benefits/on_benefits.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/benefits/on_trillium_benefit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.253792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/subsidies/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.373791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/is_child_for_on_child_care_fee_subsidy.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/is_child_for_on_child_care_fee_subsidy_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_full_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_part_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_reduction_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/per_child_care_subsidy_costs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.253792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.253792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/grants/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.373791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/grants/oshptg/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant_reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.373791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.373791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.377791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/lift/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit_eligible.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit_eligible_people.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.377791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/noec/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/noec/is_in_northern_ontario.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/noec/noec_child.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/noec/noec_count_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/noec/northern_ontario_energy_credit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.377791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/is_senior_for_oeptc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_child.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_count_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_energy_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_occupancy_cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_property_tax_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oshptg_adjusted_oeptc.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/on_non_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/on_refundable_credits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.377791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/ostc/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/on_income_tax_before_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/on_income_tax_before_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/on_taxable_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.253792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/pe/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.253792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/pe/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.377791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/pe/tax/income/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/pe/tax/income/pe_income_tax_before_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/pe/tax/income/pe_income_tax_before_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/pe/tax/income/pe_taxable_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.253792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.253792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.377791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.377791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.377791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cce/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cce/qc_cce_disabled_child_tax_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cce/qc_cce_nondisabled_child_tax_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cce/qc_cce_tax_credit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.377791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cost_of_living/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cost_of_living/qc_cost_of_living_credit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.381791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_eligibility.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_exceptional_care_tier1_child.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_exceptional_care_tier2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_supplement.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/qc_basic_personal_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.381791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_married_both_eligible.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_married_one_eligible.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_single_eligible.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_spouse_eligible.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_tax_credit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.381791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.381791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/qc_adapted_work_premium_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/qc_adapted_work_premium_eligible.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.381791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/qc_general_work_premium_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/qc_general_work_premium_eligible.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit_supplement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_eligible.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/qc_income_tax_before_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/qc_income_tax_before_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/qc_taxable_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.253792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.381791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.381791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/benefits/afb/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/benefits/afb/childrens_sports_and_culture_participation_costs.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/benefits/afb/sk_active_family_benefit.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/benefits/sk_benefits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.253792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.381791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.257792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.381791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/age_amount/
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/age_amount/sk_age_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/age_amount/sk_age_amount_eligible.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.381791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/disability_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/disability_amount/sk_disability_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.385791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/sk_senior_supplementary_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/sk_senior_supplementary_credit/sk_senior_supplementary_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/sk_senior_supplementary_credit/sk_senior_supplementary_credit_eligible.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.385791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/slic/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit_eligible_child.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit_eligible_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/sk_income_tax_before_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/sk_income_tax_before_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/sk_taxable_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.257792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.257792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.385791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/benefits/yukon_child_benefit/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/benefits/yukon_child_benefit/yt_child_benefit.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/benefits/yukon_child_benefit/yt_child_benefit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/benefits/yukon_child_benefit/yt_child_benefit_eligible_child.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/benefits/yukon_child_benefit/yt_child_benefit_eligible_children.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.257792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.385791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.257792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/benefits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.257792 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/benefits/rebates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.385791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/benefits/rebates/ygcpri/
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/benefits/rebates/ygcpri/yt_government_carbon_price_rebate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.385791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.385791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_arts_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit_eligible_child.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit_eligible_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit_expenses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.385791 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_disabled_child.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_disabled_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_eligible_child.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_eligible_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_childrens_fitness_tax_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_childrens_fitness_tax_credit_disability_supplement.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/yt_employment_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/yt_first_nations_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/yt_non_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/yt_income_tax_before_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/yt_income_tax_before_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/yt_taxable_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.385791 policyengine-canada-0.94.0/policyengine_canada/variables/household/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.257792 policyengine-canada-0.94.0/policyengine_canada/variables/household/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.389791 policyengine-canada-0.94.0/policyengine_canada/variables/household/assets/household/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/assets/household/household_liquid_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/assets/household/real_and_personal_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.257792 policyengine-canada-0.94.0/policyengine_canada/variables/household/demographic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.389791 policyengine-canada-0.94.0/policyengine_canada/variables/household/demographic/geographic/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/demographic/geographic/in_whitehorse.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/demographic/geographic/is_rural.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.389791 policyengine-canada-0.94.0/policyengine_canada/variables/household/demographic/geographic/province/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/demographic/geographic/province/in_province.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/demographic/geographic/province/province.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/demographic/geographic/province/province_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/demographic/geographic/province/province_code_str.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/demographic/geographic/province/province_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/demographic/geographic/province/province_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/demographic/geographic/province/province_str.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.389791 policyengine-canada-0.94.0/policyengine_canada/variables/household/expenses/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.389791 policyengine-canada-0.94.0/policyengine_canada/variables/household/expenses/childcare/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/expenses/childcare/childcare_costs.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/expenses/childcare/childcare_received_days.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/expenses/childcare/childcare_received_hours_per_day.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/expenses/childcare/full_time_childcare.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/expenses/dental_expenses.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/expenses/has_private_dental_insurance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.389791 policyengine-canada-0.94.0/policyengine_canada/variables/household/expenses/housing/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/expenses/housing/home_energy_costs_on_a_reserve.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/expenses/housing/public_or_non_profit_long_term_care_home.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/expenses/housing/rent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.389791 policyengine-canada-0.94.0/policyengine_canada/variables/household/expenses/tax/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/expenses/tax/property_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/household_size.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.389791 policyengine-canada-0.94.0/policyengine_canada/variables/household/ids/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/ids/household_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/ids/person_id.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.257792 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.389791 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/household/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/household/household_benefits.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/household/household_income_tax_before_refundable_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/household/household_market_income.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/household/household_net_income.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/household/household_refundable_tax_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/household/market_income.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/household/resides_on_settlement_land.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.393791 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/individual/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/individual/benefits_income.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/individual/individual_net_income.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/individual/investment_income.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/individual/other_employment_income.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/individual/pension_and_savings_plan_income.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/individual/person_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/individual/self_employment_income.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/income/individual/total_individual_pre_tax_income.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/marginal_tax_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.397791 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/adult_years_in_canada.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/age.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/canadian_armed_forces_and_personnel_deduction.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/care_expenses.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/childcare_expense.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/count_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/count_dependants.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/full_custody.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/in_need_of_protective_services.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/is_ emancipated.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/is_adult.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/is_child.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/is_child_of_filer.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/is_dependant.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/is_disabled.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/is_father.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/is_female.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/is_full_time_student.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/is_head.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/is_head_or_spouse.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/is_male.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/is_married.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/is_mother.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/is_spouse.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/lived_in_a_student_residence.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/own_children_in_household.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/physical_activities_fees.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/spouse_income.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/teaching_supplies_expenses.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/household/person/tuition_expenses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.397791 policyengine-canada-0.94.0/policyengine_canada/variables/input/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/input/employment_income.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/policyengine_canada/variables/input/family_employment_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 03:17:27.261792 policyengine-canada-0.94.0/policyengine_canada.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-15 03:17:27.000000 policyengine-canada-0.94.0/policyengine_canada.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    93262 2024-03-15 03:17:27.000000 policyengine-canada-0.94.0/policyengine_canada.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 03:17:27.000000 policyengine-canada-0.94.0/policyengine_canada.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-15 03:17:27.000000 policyengine-canada-0.94.0/policyengine_canada.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-15 03:17:27.000000 policyengine-canada-0.94.0/policyengine_canada.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 03:17:27.397791 policyengine-canada-0.94.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-03-15 03:16:37.000000 policyengine-canada-0.94.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.268954 policyengine-canada-0.95.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-22 23:29:26.268954 policyengine-canada-0.95.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.136953 policyengine-canada-0.95.0/policyengine_canada/
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.140953 policyengine-canada-0.95.0/policyengine_canada/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.140953 policyengine-canada-0.95.0/policyengine_canada/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/data/datasets/country_template_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/model_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/modelled_policies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.112952 policyengine-canada-0.95.0/policyengine_canada/parameters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.096952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.140953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.092952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.140953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/ccb/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/ccb/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/ccb/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/ccb/divisor.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.140953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/four_or_more_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/one_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/three_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/two_children.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.140953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cdb/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cdb/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cdb/base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.140953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cdb/reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cdb/reduction/one_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cdb/reduction/two_or_more_children.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.140953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.140953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/amount/disability_supplement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/amount/family.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/amount/single.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/eligible_age.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.140953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.140953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/base/family.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/base/single.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/disability_supplement.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.140953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.144953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/base/family.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/base/single.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.144953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/disability_supplement/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/disability_supplement/family_with_one_spouse_disabled.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/disability_supplement/family_with_two_spouses_disabled.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/disability_supplement/single.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/working_income_sources.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.144953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/dental_benefit/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/dental_benefit/additional_benefit_threshold.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/dental_benefit/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/dental_benefit/ineligible_age.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/dental_benefit/shared_custody_share.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.144953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.144953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/amount/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/amount/older_seniors_increase_factor.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.092952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/eligibility/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.144953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/eligibility/age/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/eligibility/age/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/eligibility/age/older_seniors_increase.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.144953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/eligibility/residence/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/eligibility/residence/any.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/eligibility/residence/full_base_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/repayment_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.096952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.144953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.144953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.144953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/age_amount_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/age_amount_credit/age_eligibility.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.144953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/age_amount_credit/amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/age_amount_credit/amount/credit_cap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/age_amount_credit/amount/reduction.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.144953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/max_amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.096952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/phase_out/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.144953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/phase_out/threshold/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/phase_out/threshold/end.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/phase_out/threshold/start.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.144953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/canada_employment_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/canada_employment_amount/income_sources.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/canada_employment_amount/max_amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.148953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/climate_action_incentive/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/climate_action_incentive/adult_age.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/climate_action_incentive/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/climate_action_incentive/rural.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.148953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/dtc/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/dtc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/dtc/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/dtc/child_supplement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/dtc/supplement_ineligible_age.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.148953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/adult_age.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/base_amounts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/reduction.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.148953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/singles_boost/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/singles_boost/cap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/singles_boost/phase_in.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/non_refundable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/refundable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.148953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/school_supply_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/school_supply_credit/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/school_supply_credit/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/school_supply_credit/cap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.148953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.148953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/age_eligibility/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/age_eligibility/max.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/age_eligibility/min.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/income_sources.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/lifetime_cap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/income_tax_schedule.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.112952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.148953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.148953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.148953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/age_eligibility.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.096952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.148953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/base/four_or_more_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/base/one_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/base/three_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/base/two_children.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.148953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/four_or_more_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/one_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/three_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/two_children.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.096952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.152953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/four_or_more_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/one_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/three_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/two_children.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.152953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_in/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_in/rate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_in/start.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.152953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/four_or_more_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/one_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/three_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/two_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/benefits.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.096952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.152953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.152953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.152953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/age_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/age_credit/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/age_credit/eligible_age.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/age_credit/phase_out_rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.152953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/basic_personal_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/basic_personal_amount/amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.152953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.152953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/additional_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/additional_amount/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/additional_amount/childcare_expense_threshold.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/cap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/non_refundable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.152953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/pension/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/pension/max_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/refundable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.152953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/spouse_and_common_law_partner_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/spouse_and_common_law_partner_amount/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.152953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.152953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.152953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.152953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/base/one_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/base/three_or_more_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/base/two_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/child_ineligible_age_threshold.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.156953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/first_reduction/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.156953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/first_reduction/max_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/first_reduction/max_amount/one_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/first_reduction/max_amount/three_or_more_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/first_reduction/max_amount/two_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/first_reduction/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.156953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/second_reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/second_reduction/rate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/benefits.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.096952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.156953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.156953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.156953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/age/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/age/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/age/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/age/eligible_age.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.156953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/age/phase_out/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/age/phase_out/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/age/phase_out/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.156953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/basic_personal_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/basic_personal_amount/base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.156953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/adult_age.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.156953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/reduction_rate/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/reduction_rate/family.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/reduction_rate/single.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.156953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/disability/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.156953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/disability/additional_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/disability/additional_amount/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/disability/additional_amount/childcare_expense_threshold.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/disability/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/non_refundable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.156953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/pension_income_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/pension_income_amount/cap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/refundable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.156953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/tax_reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/tax_reduction/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/tax_reduction/reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.156953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.100952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.156953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/eligible_age.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/max_child_count.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.160953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/five_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/four_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/one_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/six_or_more_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/three_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/two_children.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.100952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.160953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.160953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.160953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/age_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/age_amount/age_eligibility.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/age_amount/max_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/age_amount/phase_out_rate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/basic_personal_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/non_refundable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.160953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/pension_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/pension_amount/max_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/refundable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.160953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.160953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/benefits.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.160953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/eligible_age.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.160953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/phase_out/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/phase_out/multiple_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/phase_out/one_child.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.160953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/working_income_supplement/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/working_income_supplement/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/working_income_supplement/phase_in.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/working_income_supplement/phase_out.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.160953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/pension_benefit/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/pension_benefit/cap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.100952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.160953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.100952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.160953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/age_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/age_amount/age_eligibility.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/age_amount/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/age_amount/reduction_rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.160953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.164953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/base/dependant.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/base/head.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/base/max_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/base/spouse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/child_eligible_age.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/rate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.164953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nl/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nl/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.100952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nl/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.164953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.100952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.164953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/credits/physical_activity/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/credits/physical_activity/age_eligible.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/credits/physical_activity/max_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/credits/physical_activity/rate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.164953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.164953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/benefits/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/benefits/benefits.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.164953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/benefits/child_benefit/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/benefits/child_benefit/age_eligibility.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/benefits/child_benefit/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/benefits/child_benefit/higher_income_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/benefits/child_benefit/lower_threshold.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/benefits/child_benefit/upper_threshold.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.100952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.164953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.164953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.164953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/age/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/age/age_eligibility.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/age/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/age/income_eligibility.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.164953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/disability_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/disability_amount/base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.164953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/age_eligibility.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.164953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.164953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/dependant/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/dependant/age_eligibility.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/dependant/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/eligible_dependant.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/max_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/spouse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/phase_out.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/non_refundable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/nsaltc/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/nsaltc/child_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/nsaltc/individual_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/nsaltc/reduction.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/pension_income_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/pension_income_amount/cap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/prc/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/prc/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/prc/income_threshold.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/refundable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.104952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.104952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/eligibility/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/eligibility/age/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/eligibility/age/lower.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/eligibility/age/main.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/applicable_assets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/limit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nt/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nt/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.104952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nt/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.104952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/age_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/age_credit/age_eligibility.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/age_credit/max_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/age_credit/reduction.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/basic_personal_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/basic_personal_amount/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.104952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/benefits.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/age_limit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/base/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/base/phase_out_rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/working/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/working/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/working/phase_in_rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/age_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/age_amount/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/age_amount/eligible_age.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/age_amount/phase_out_rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/cost_of_living/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/cost_of_living/max_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/cost_of_living/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/cost_of_living/supplement_for_single_parents/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/cost_of_living/supplement_for_single_parents/income.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/cost_of_living/supplement_for_single_parents/max_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/cost_of_living/supplement_for_single_parents/rate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/non_refundable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/benefits/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/benefits/benefits.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.168953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/benefits/ocb/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/benefits/ocb/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/benefits/ocb/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/benefits/ocb/reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/benefits/ocb/shared_custody_divisor.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.104952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/subsidies/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.172953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/child_age_eligibility.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/full_time_calculation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/part_time_child_care_multiplier.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.172953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/reduction/age.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/reduction/factor.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.104952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.104952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.172953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/age_eligibility.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/max_amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.172953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/reduction/family.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/reduction/single.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.172953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.172953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.172953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/phase_in_rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.172953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/reduction/family.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/reduction/single.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.172953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/age_eligibility.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/child_max_age.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.172953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.172953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/shared_custody/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/shared_custody/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/shared_custody/divisor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/shared_custody/start.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/start.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/non_refundable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.172953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/child_max_age.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.172953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/energy_component/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/energy_component/max_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/energy_component/multiplier.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/energy_component/student_resident_reduction.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/occupancy_costs/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/occupancy_costs/rent_multiplier.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/occupancy_costs/student_resident_supplement.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/shared_custody/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/shared_custody/divisor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/shared_custody/start.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/start.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/property_tax_component/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/property_tax_component/initial_cap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/property_tax_component/multiplier.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/property_tax_component/supplement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/second_subtraction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/senior_age.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/ostc/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/ostc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/ostc/amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/ostc/reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/ostc/reduction/family.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/ostc/reduction/single.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/refundable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/pe/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/pe/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.108952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/pe/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/pe/tax/income/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/pe/tax/income/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.108952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.108952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/basic_personal_amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cce/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cce/age_eligibility.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cce/child_income_limit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cce/disabled_child_expense_limit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cce/nondisabled_child_expense_limit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cce/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cost_of_living/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cost_of_living/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cost_of_living/reduction.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/age_eligibility.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/child_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/child_amount/max.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/child_amount/min.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/reduction/single_parent_family.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/reduction/two_parent_family.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/shared_custody_multiplier.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/single_parent_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/single_parent_amount/max.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/single_parent_amount/min.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.108952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/handicapped_child/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/handicapped_child/base_amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.176953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/handicapped_child/exceptional_care_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/handicapped_child/exceptional_care_amount/tier1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/handicapped_child/exceptional_care_amount/tier2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/school_supplies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/school_supplies/handicapped_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/school_supplies/non_handicapped_child.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/age_eligibility.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/amount/married_both_eligible.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/amount/married_one_eligible.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/amount/single.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/reduction/married.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/reduction/single.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/couple/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/couple/amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/couple/amount/with_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/couple/amount/without_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/couple/reduction.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/single/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/single/amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/single/amount/person_living_alone.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/single/amount/single_parent.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/single/reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/work_income_requirement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/age_eligibility.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.108952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/amount/with_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/amount/without_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/work_income_requirement.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/amount/person_living_alone.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/amount/single_parent.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/work_income_requirement.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/supplement/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/supplement/amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/supplement/amount/couple.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/supplement/amount/single.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/supplement/work_income_eligibility.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.108952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/amount/disabled.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/amount/non_disabled.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/eligibility/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/eligibility/age.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/eligibility/income.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/benefits/benefits.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.108952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.112952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.180953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/age_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/age_amount/age_eligibility.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/age_amount/max_amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/age_amount/reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/age_amount/reduction/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/disability_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/disability_amount/amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/age_threshold.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/child/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/child/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/child/ineligible_age.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/child/max_number.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/head.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/phase_out.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/spouse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.112952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/child_benefit/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/child_benefit/base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/child_benefit/multiple_children/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/child_benefit/multiple_children/reduction_rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/child_benefit/one_child/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/child_benefit/one_child/reduction_rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.112952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/amount/child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/amount/self.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/amount/spouse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/child_ineligible_age.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/non_whitehorse_supplement/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/non_whitehorse_supplement/child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/non_whitehorse_supplement/self.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/non_whitehorse_supplement/spouse.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.112952 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_arts_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_arts_credit/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_arts_credit/child_age_eligibility.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_fitness/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_fitness/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_fitness/child_age_eligibility.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_fitness/disability_supplement/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_fitness/disability_supplement/age.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_fitness/disability_supplement/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_fitness/disability_supplement/minimum_fees.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_fitness/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/employment_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/employment_amount/amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.184953 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/first_nations_tax/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/first_nations_tax/rate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/non_refundable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.188953 policyengine-canada-0.95.0/policyengine_canada/parameters/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/parameters/simulation/marginal_tax_rate_adults.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.188953 policyengine-canada-0.95.0/policyengine_canada/reforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/reforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.188953 policyengine-canada-0.95.0/policyengine_canada/situation_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/situation_examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.124953 policyengine-canada-0.95.0/policyengine_canada/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.188953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.112952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.112952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.188953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/ccb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/ccb/child_benefit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.188953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cdb/child_disability_benefit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cdb/child_disability_benefit_eligible.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cdb/child_disability_benefit_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cdb/integration.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.188953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.188953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/base/cwb_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/base/cwb_base_max_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/base/cwb_base_phase_in.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/base/cwb_base_phase_out.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/canada_workers_benefit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/cwb_dependant.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/cwb_eligible.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.188953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_category.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_eligible.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_max_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_phase_in.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_phase_out.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/is_cwb_family.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.192953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/dental_benefit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/dental_benefit/dental_benefit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/dental_benefit/dental_benefit_eligible.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.192953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/oas/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/oas/integration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/oas/oas_eligibility.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/oas/oas_pre_repayment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/oas/oas_repayment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.112952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.192953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.192953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/age_amount_credit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.192953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/basic_personal_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/basic_personal_amount/basic_personal_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/basic_personal_amount/basic_personal_amount_supplement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/canada_employment_amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.192953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/climate_action_incentive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/climate_action_incentive_dependant_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/climate_action_incentive_person.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/climate_action_incentive_single_parent_household.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/integration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/integration_eldest_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/is_child_for_climate_action_incentive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/is_eldest_child_for_climate_action_incentive.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.192953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/dtc/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/dtc/dtc_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/dtc/dtc_child_supplement.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.192953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit_category.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit_person.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit_single_parent_household.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit_singles_boost.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/integration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/is_child_for_gst_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/is_eldest_child_in_single_household_for_gst_credit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.192953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/school_supply_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/school_supply_credit/school_supply_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/training_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/income_tax_before_credits.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/income_tax_before_refundable_credits.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/integration.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.124953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.116953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.116953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_base_component.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_base_component_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_base_component_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_eligible_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_working_component.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_working_component_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_working_component_reduction.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.116953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.116953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/ab_spouse_and_common_law_partner_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/ab_spouse_and_common_law_partner_amount/ab_spouse_and_common_law_partner_amount_credit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/age_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/age_credit/ab_age_credit_eligible.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/age_credit/age_credit_amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/basic_personal_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/basic_personal_amount/ab_basic_personal_amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/disability/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit_additional_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit_eligible.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/pension/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/pension/ab_pension_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/income_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.116953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.116953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/benefits/bcfb/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/benefits/bcfb/bc_family_benefit_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/benefits/bcfb/bc_family_benefit_first_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/benefits/bcfb/bc_family_benefit_second_reduction.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.116953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/basic_personal_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/basic_personal_amount/bc_basic_personal_amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_age_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_age_credit/bc_age_credit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_disability_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit_additional_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit_eligible.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_pension_income_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_pension_income_amount/bc_pension_income_amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_tax_reduction_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_tax_reduction_credit/bc_tax_reduction_credit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_person.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_single_parent_household.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/integration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/is_child_for_bc_climate_action_tax_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/is_eldest_child_for_bc_climate_action_tax_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bx_income_tax_before_refundable_credits.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/income_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.116953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/mb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.116953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/mb/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/mb/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/mb/tax/income/benefits/
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/mb/tax/income/benefits/mb_child_benefit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/mb/tax/income/benefits/mb_child_benefit_eligible_child.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.196953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/age_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/age_amount/mb_age_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/age_amount/mb_age_credit_eligible.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/mb_basic_personal_amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/pension_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/pension_amount/mb_pension_amount_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/mb/tax/income/income_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.116953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.116953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/benefits/nbcb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/benefits/nbcb/nb_child_benefit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/benefits/nbcb/nb_child_benefit_supplement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/benefits/nbcb/nb_family_benefit_eligible_child.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/pension_benefits/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/pension_benefits/nb_pension_benefit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.116953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/nb_low_income_tax_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/nb_low_income_tax_reduction_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/tax/income/credits/nb_age_amount_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/tax/income/income_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.116953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.116953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nl/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nl/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nl/tax/income/credits/
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nl/tax/income/credits/nl_phyical_activity_tax_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nl/tax/income/income_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.116953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.116953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/benefits/child_benefit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/benefits/child_benefit/ns_child_benefit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/benefits/child_benefit/ns_child_benefit_eligible_child.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.116953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/age/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/age/ns_age_tax_credit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_base_children.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_eligible_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/ns_disability_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/ns_pension_income_amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/nsaltc/
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/nsaltc/ns_affordable_living_tax_credit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/prc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/prc/ns_poverty_reduction_credit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_assistance/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_assistance/eligibility/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_assistance/eligibility/age/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_assistance/eligibility/age/ns_income_assistance_age_eligibility.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/ns_income_assistance_asset_eligibility.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nt/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.200953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nt/tax/income/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nt/tax/income/income_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nt/tax/income/nt_age_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nt/tax/income/nt_age_credit_eligible.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nt/tax/income/nt_basic_personal_amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.204953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/nu_child_benefit_base_component.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/nu_child_benefit_base_component_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/nu_child_benefit_base_component_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/nu_child_benefit_eligible_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/nu_child_benefit_working_component.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.204953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.204953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.204953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/age_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/age_amount/nu_age_amount_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/age_amount/nu_age_amount_credit_eligible_person.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/nu_cost_of_living_basic_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/nu_cost_of_living_credit_adjusted_net_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/nu_cost_of_living_credit_supplement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/tax/income/income_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.204953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/benefits/ocb/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/benefits/ocb/on_child_benefit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/benefits/ocb/on_child_benefit_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/benefits/ocb/on_child_benefit_reduction.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/grants/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.204953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/grants/oshptg/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant_reduction.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.204953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.204953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.204953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/lift/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit_eligible.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.204953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/noec/
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/noec/northern_ontario_energy_credit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.204953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/integration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/is_senior_for_oeptc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oeptc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oeptc_energy_component.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oeptc_occupancy_costs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oeptc_property_tax_component.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oshptg_adjusted_opetc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/on_income_tax_before_refundable_credits.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.204953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/ostc/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/income_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.204953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/is_child_for_on_child_care_fee_subsidy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/is_child_for_on_child_care_fee_subsidy_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_full_time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_part_time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_reduction.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/pe/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/pe/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.208953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/pe/tax/income/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/pe/tax/income/income_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.208953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.208953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.208953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/cce/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/cce/cce_disabled_child_tax_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/cce/cce_nondisabled_child_tax_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/cce/cce_tax_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/cost_of_living.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.208953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/fa/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/fa/qc_fa_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/fa/qc_fa_eligibility.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/fa/qc_fa_payment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/fa/qc_fa_supplement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/qc_basic_personal_amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.208953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/qc_sa_married_both_eligible.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/qc_sa_married_one_eligible.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/qc_sa_single_eligible.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/qc_sa_spouse_eligible.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/qc_sa_tax_credit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.208953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.208953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/qc_adapted_work_premium_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/qc_adapted_work_premium_eligible.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.208953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/qc_general_work_premium_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/qc_general_work_premium_eligible.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit_supplement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_eligible.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/income_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.208953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/benefits/afb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/benefits/afb/sk_active_family_benefit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.120952 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.208953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.208953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.208953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/age_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/age_amount/sk_age_amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/age_amount/sk_age_amount_eligible.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/sk_disability_amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.208953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/sk_senior_supplementary_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/sk_senior_supplementary_eligible.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.208953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/slic/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit_eligible_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/income_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.124953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.124953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.208953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.212953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/benefits/
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/benefits/yt_child_benefit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/benefits/yt_child_benefit_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/benefits/yt_child_benefit_eligible_child.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.212953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/benefits/yt_employment_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/benefits/yt_employment_amount/yt_employment_amount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.212953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.212953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_arts_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit_eligible_child.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.212953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_disabled_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_eligible_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_childrens_fitness_tax_credit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_childrens_fitness_tax_credit_disability_supplement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/yt_first_nations_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/income_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.212953 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/rebates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/rebates/yt_government_carbon_price_rebate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.124953 policyengine-canada-0.95.0/policyengine_canada/tests/household/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.212953 policyengine-canada-0.95.0/policyengine_canada/tests/household/person/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/household/person/is_dependant.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/household/person/person_index.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tests/household/person/spouse_income.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.212953 policyengine-canada-0.95.0/policyengine_canada/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/tools/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.212953 policyengine-canada-0.95.0/policyengine_canada/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.212953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/benefits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.212953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/adjusted_family_net_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.124953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.212953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/ccb/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit_base_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit_eligible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit_eligible_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/ccb/family_net_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.212953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cdb/child_disability_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cdb/child_disability_benefit_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cdb/child_disability_benefit_eligible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cdb/child_disability_benefit_reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.212953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.216953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/base/cwb_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/base/cwb_base_max_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/base/cwb_base_phase_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/base/cwb_base_phase_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/canada_workers_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/cwb_dependant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/cwb_eligible.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.216953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_eligible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_max_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_phase_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_phase_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/family_working_income.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/is_cwb_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/working_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.216953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/dental_benefit/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/dental_benefit/additional_dental_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/dental_benefit/dental_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/dental_benefit/dental_benefit_eligible.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.216953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/old_age_security_pension/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/old_age_security_pension/oas_eligibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/old_age_security_pension/oas_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/old_age_security_pension/oas_pre_repayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/old_age_security_pension/oas_repayment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.216953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/deductions/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/deductions/deductions_from_total_to_net_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.124953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.216953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.216953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.216953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/age_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/age_amount/age_amount_credit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.216953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/basic_personal_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/basic_personal_amount/basic_personal_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/basic_personal_amount/basic_personal_amount_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/canada_employment_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.220953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive_dependant_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive_pre_rural.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive_single_parent_household.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/is_child_for_climate_action_incentive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/is_eldest_child_for_climate_action_incentive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.220953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/dtc/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/dtc/disability_tax_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/dtc/dtc_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/dtc/dtc_child_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/dtc/dtc_eligible.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.220953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_dependant_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_single_parent_household.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_singles_boost.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/is_child_for_gst_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/is_eldest_child_in_single_household_for_gst_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/non_refundable_tax_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/refundable_tax_credits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.220953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/school_supply_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/school_supply_credit/school_supply_credit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.220953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/training/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/training/prior_training_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/training/training_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/training/training_credit_income.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/income_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/income_tax_before_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/income_tax_before_refundable_credits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.220953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/uccb/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/uccb/universal_child_care_benefit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.220953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/esdc/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/esdc/maternity_and_parental_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/esdc/registered_disability_savings_plan_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.136953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.124953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.220953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/benefits/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/benefits/ab_benefits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.224954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_base_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_base_component_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_base_component_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_eligible_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_eligible_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_working_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_working_component_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_working_component_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/alberta_child_and_family_benefit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.124953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.224954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/ab_income_tax_before_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/ab_income_tax_before_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/ab_taxable_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.224954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/ab_non_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/ab_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/ab_spouse_and_common_law_partner_amount_credit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.224954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/age_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/age_credit/ab_age_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/age_credit/ab_age_credit_eligible.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.224954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/basic_personal_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/basic_personal_amount/ab_basic_personal_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.224954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/disability/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit_additional_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit_eligible.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.224954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/pension/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/pension/ab_pension_credit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.128953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.224954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/benefits/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/benefits/bc_benefits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.224954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit_eligible_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit_eligible_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit_first_reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.128953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.224954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/bc_income_tax_before_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/bc_income_tax_before_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/bc_taxable_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.224954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.224954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/basic_personal_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/basic_personal_amount/bc_basic_personal_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.224954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_age_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_age_credit/bc_age_credit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.224954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_disability_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit_additional_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit_eligible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_non_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_refundable_credits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.228953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_tax_reduction_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_tax_reduction_credit/bc_tax_reduction_credit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.228953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_incentive_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_dependant_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_single_parent_household.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/is_child_for_bc_climate_action_tax_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/is_eldest_child_for_bc_climate_action_tax_credit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.228953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/pension_income_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/pension_income_amount/bc_pension_income_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.128953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.128953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.228953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.128953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.228953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/benefits/child_benefit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/benefits/child_benefit/mb_child_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/benefits/child_benefit/mb_child_benefit_eligible_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/benefits/child_benefit/mb_child_benefit_eligible_children.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.228953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.228953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/age_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/age_amount/mb_age_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/age_amount/mb_age_credit_eligible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/mb_basic_personal_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/mb_non_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/mb_refundable_credits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.228953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/pension_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/pension_amount/mb_pension_amount_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/mb_income_tax_before_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/mb_income_tax_before_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/mb_taxable_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.128953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.228953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/benefits/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/benefits/nb_benefits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.228953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/benefits/nbcb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/benefits/nbcb/nb_child_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/benefits/nbcb/nb_child_benefit_eligible_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/benefits/nbcb/nb_child_benefit_eligible_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/benefits/nbcb/nb_child_benefit_supplement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.228953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/benefits/pension_benefit/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/benefits/pension_benefit/nb_pension_benefit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.128953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.232953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.128953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.232953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/age_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/age_amount/nb_age_amount_credit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.232953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/nb_low_income_tax_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/nb_low_income_tax_reduction_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/tax/income/nb_income_tax_before_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/tax/income/nb_income_tax_before_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/tax/income/nb_taxable_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.128953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.128953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nl/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.232953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nl/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.232953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nl/tax/income/credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nl/tax/income/credit/nl_physical_activity_tax_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nl/tax/income/nl_income_tax_before_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nl/tax/income/nl_income_tax_before_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nl/tax/income/nl_taxable_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.128953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.232953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.232953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/benefits/child_benefit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/benefits/child_benefit/ns_child_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/benefits/child_benefit/ns_child_benefit_eligible_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/benefits/child_benefit/ns_child_benefit_eligible_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/benefits/ns_benefits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.128953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.232953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.232953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.232953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/age/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/age/ns_age_tax_credit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.236954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_base_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_eligible_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_eligible_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/ns_disability_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/ns_non_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/ns_pension_income_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/ns_refundable_credits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.236954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/nsaltc/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/nsaltc/ns_affordable_living_tax_credit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.236954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/prc/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/prc/ns_poverty_reduction_credit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.236954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.132953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.236954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/age/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/age/ns_income_assistance_age_eligibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.236954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/ns_income_assistance_applicable_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/ns_income_assistance_asset_eligibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/ns_income_assistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/ns_income_tax_before_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/ns_income_tax_before_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/ns_taxable_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.132953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.132953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nt/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.236954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nt/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.132953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.236954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/age_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/age_credit/nt_age_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/age_credit/nt_age_credit_eligible.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.240954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/basic_personal_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/basic_personal_amount/nt_basic_personal_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nt/tax/income/nt_income_tax_before_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nt/tax/income/nt_income_tax_before_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nt/tax/income/nt_taxable_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.132953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.132953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.240954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.240954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_benefits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.240954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_base_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_base_component_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_base_component_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_eligible_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_eligible_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_working_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.240954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.244953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/age_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/age_amount/nu_age_amount_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/age_amount/nu_age_amount_credit_eligible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/nu_cost_of_living_basic_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/nu_cost_of_living_credit_adjusted_net_income.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/nu_cost_of_living_credit_post_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/nu_cost_of_living_credit_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/nu_non_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/nu_income_tax_before_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/nu_income_tax_before_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/nu_taxable_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.132953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.244953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.244953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/benefits/ocb/
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/benefits/ocb/on_child_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/benefits/ocb/on_child_benefit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/benefits/ocb/on_child_benefit_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/benefits/on_benefits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/benefits/on_trillium_benefit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.132953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/subsidies/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.244953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/is_child_for_on_child_care_fee_subsidy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/is_child_for_on_child_care_fee_subsidy_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_full_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_part_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_reduction_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/per_child_care_subsidy_costs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.132953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.132953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/grants/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.248954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/grants/oshptg/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant_reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.248954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.248954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.248954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/lift/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit_eligible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit_eligible_people.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.248954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/noec/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/noec/is_in_northern_ontario.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/noec/noec_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/noec/noec_count_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/noec/northern_ontario_energy_credit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.248954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/is_senior_for_oeptc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_count_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_energy_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_occupancy_cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_property_tax_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oshptg_adjusted_oeptc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/on_non_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/on_refundable_credits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.248954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/ostc/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/on_income_tax_before_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/on_income_tax_before_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/on_taxable_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.132953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/pe/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.132953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/pe/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.252954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/pe/tax/income/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/pe/tax/income/pe_income_tax_before_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/pe/tax/income/pe_income_tax_before_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/pe/tax/income/pe_taxable_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.132953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.132953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.252954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.252954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.252954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cce/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cce/qc_cce_disabled_child_tax_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cce/qc_cce_nondisabled_child_tax_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cce/qc_cce_tax_credit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.252954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cost_of_living/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cost_of_living/qc_cost_of_living_credit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.252954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_eligibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_exceptional_care_tier1_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_exceptional_care_tier2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/qc_basic_personal_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.252954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_married_both_eligible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_married_one_eligible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_single_eligible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_spouse_eligible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_tax_credit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.256954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.256954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/qc_adapted_work_premium_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/qc_adapted_work_premium_eligible.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.256954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/qc_general_work_premium_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/qc_general_work_premium_eligible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_eligible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/qc_income_tax_before_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/qc_income_tax_before_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/qc_taxable_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.132953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.256954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.256954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/benefits/afb/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/benefits/afb/childrens_sports_and_culture_participation_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/benefits/afb/sk_active_family_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/benefits/sk_benefits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.132953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.256954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.136953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.256954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/age_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/age_amount/sk_age_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/age_amount/sk_age_amount_eligible.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.256954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/disability_amount/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/disability_amount/sk_disability_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.256954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/sk_senior_supplementary_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/sk_senior_supplementary_credit/sk_senior_supplementary_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/sk_senior_supplementary_credit/sk_senior_supplementary_credit_eligible.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.256954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/slic/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit_eligible_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit_eligible_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/sk_income_tax_before_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/sk_income_tax_before_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/sk_taxable_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.136953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.136953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.256954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/benefits/yukon_child_benefit/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/benefits/yukon_child_benefit/yt_child_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/benefits/yukon_child_benefit/yt_child_benefit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/benefits/yukon_child_benefit/yt_child_benefit_eligible_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/benefits/yukon_child_benefit/yt_child_benefit_eligible_children.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.136953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.256954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.136953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/benefits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.136953 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/benefits/rebates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.260954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/benefits/rebates/ygcpri/
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/benefits/rebates/ygcpri/yt_government_carbon_price_rebate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.260954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.260954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_arts_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit_eligible_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit_eligible_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit_expenses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.260954 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_disabled_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_disabled_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_eligible_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_eligible_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_childrens_fitness_tax_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_childrens_fitness_tax_credit_disability_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/yt_employment_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/yt_first_nations_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/yt_non_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/yt_income_tax_before_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/yt_income_tax_before_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/yt_taxable_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.260954 policyengine-canada-0.95.0/policyengine_canada/variables/household/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.136953 policyengine-canada-0.95.0/policyengine_canada/variables/household/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.260954 policyengine-canada-0.95.0/policyengine_canada/variables/household/assets/household/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/assets/household/household_liquid_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/assets/household/real_and_personal_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.136953 policyengine-canada-0.95.0/policyengine_canada/variables/household/demographic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.260954 policyengine-canada-0.95.0/policyengine_canada/variables/household/demographic/geographic/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/demographic/geographic/in_whitehorse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/demographic/geographic/is_rural.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.260954 policyengine-canada-0.95.0/policyengine_canada/variables/household/demographic/geographic/province/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/demographic/geographic/province/in_province.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/demographic/geographic/province/province.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/demographic/geographic/province/province_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/demographic/geographic/province/province_code_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/demographic/geographic/province/province_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/demographic/geographic/province/province_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/demographic/geographic/province/province_str.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.260954 policyengine-canada-0.95.0/policyengine_canada/variables/household/expenses/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.264954 policyengine-canada-0.95.0/policyengine_canada/variables/household/expenses/childcare/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/expenses/childcare/childcare_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/expenses/childcare/childcare_received_days.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/expenses/childcare/childcare_received_hours_per_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/expenses/childcare/full_time_childcare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/expenses/dental_expenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/expenses/has_private_dental_insurance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.264954 policyengine-canada-0.95.0/policyengine_canada/variables/household/expenses/housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/expenses/housing/home_energy_costs_on_a_reserve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/expenses/housing/public_or_non_profit_long_term_care_home.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/expenses/housing/rent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.264954 policyengine-canada-0.95.0/policyengine_canada/variables/household/expenses/tax/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/expenses/tax/property_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/household_size.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.264954 policyengine-canada-0.95.0/policyengine_canada/variables/household/ids/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/ids/household_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/ids/person_id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.136953 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.264954 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/household/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/household/household_benefits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/household/household_income_tax_before_refundable_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/household/household_market_income.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/household/household_net_income.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/household/household_refundable_tax_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/household/market_income.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/household/resides_on_settlement_land.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.264954 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/individual/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/individual/benefits_income.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/individual/individual_net_income.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/individual/investment_income.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/individual/other_employment_income.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/individual/pension_and_savings_plan_income.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/individual/person_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/individual/self_employment_income.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/income/individual/total_individual_pre_tax_income.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/marginal_tax_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.268954 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/adult_years_in_canada.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/age.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/canadian_armed_forces_and_personnel_deduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/care_expenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/childcare_expense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/count_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/count_dependants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/full_custody.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/in_need_of_protective_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/is_ emancipated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/is_adult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/is_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/is_child_of_filer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/is_dependant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/is_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/is_father.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/is_female.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/is_full_time_student.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/is_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/is_head_or_spouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/is_male.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/is_married.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/is_mother.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/is_spouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/lived_in_a_student_residence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/own_children_in_household.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/physical_activities_fees.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/spouse_income.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/teaching_supplies_expenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/household/person/tuition_expenses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.268954 policyengine-canada-0.95.0/policyengine_canada/variables/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/input/employment_income.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/policyengine_canada/variables/input/family_employment_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:26.140953 policyengine-canada-0.95.0/policyengine_canada.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-22 23:29:25.000000 policyengine-canada-0.95.0/policyengine_canada.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    93593 2024-04-22 23:29:26.000000 policyengine-canada-0.95.0/policyengine_canada.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:29:25.000000 policyengine-canada-0.95.0/policyengine_canada.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-22 23:29:25.000000 policyengine-canada-0.95.0/policyengine_canada.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-22 23:29:25.000000 policyengine-canada-0.95.0/policyengine_canada.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:29:26.268954 policyengine-canada-0.95.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-22 23:28:34.000000 policyengine-canada-0.95.0/setup.py
```

### Comparing `policyengine-canada-0.94.0/LICENSE` & `policyengine-canada-0.95.0/LICENSE`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/PKG-INFO` & `policyengine-canada-0.95.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyengine-canada
-Version: 0.94.0
+Version: 0.95.0
 Summary: Microsimulation model for Canada's tax-benefit system.
 Home-page: https://github.com/policyengine/policyengine-canada
 Author: PolicyEngine
 Author-email: hello@policyengine.org
 License: https://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit microsimulation framework
 Platform: UNKNOWN
```

### Comparing `policyengine-canada-0.94.0/policyengine_canada/__init__.py` & `policyengine-canada-0.95.0/policyengine_canada/__init__.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/data/datasets/country_template_dataset.py` & `policyengine-canada-0.95.0/policyengine_canada/data/datasets/country_template_dataset.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/entities.py` & `policyengine-canada-0.95.0/policyengine_canada/entities.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/modelled_policies.yaml` & `policyengine-canada-0.95.0/policyengine_canada/modelled_policies.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/ccb/base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/ccb/base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/four_or_more_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/four_or_more_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/one_child.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/one_child.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/three_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/three_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/two_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/ccb/reduction/two_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cdb/reduction/one_child.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cdb/reduction/one_child.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cdb/reduction/two_or_more_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cdb/reduction/two_or_more_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/amount/disability_supplement.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/amount/disability_supplement.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/amount/family.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/amount/family.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/amount/single.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/amount/single.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/eligible_age.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/eligible_age.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/base/family.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/base/family.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/base/single.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/base/single.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/disability_supplement.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_in/disability_supplement.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/base/family.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/base/family.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/base/single.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/base/single.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/disability_supplement/family_with_one_spouse_disabled.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/disability_supplement/family_with_one_spouse_disabled.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/disability_supplement/family_with_two_spouses_disabled.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/disability_supplement/family_with_two_spouses_disabled.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/disability_supplement/single.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/phase_out/disability_supplement/single.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/cwb/working_income_sources.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/cwb/working_income_sources.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/dental_benefit/additional_benefit_threshold.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/dental_benefit/additional_benefit_threshold.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/dental_benefit/amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/dental_benefit/amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/repayment_tax.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/benefits/old_age_security_pension/repayment_tax.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/age_amount_credit/age_eligibility.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/age_amount_credit/age_eligibility.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/age_amount_credit/amount/credit_cap.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/age_amount_credit/amount/credit_cap.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/age_amount_credit/amount/reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/age_amount_credit/amount/reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/max_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/max_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/phase_out/threshold/end.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/phase_out/threshold/end.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/phase_out/threshold/start.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/basic_personal_amount/phase_out/threshold/start.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/canada_employment_amount/income_sources.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/canada_employment_amount/income_sources.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/canada_employment_amount/max_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/canada_employment_amount/max_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/climate_action_incentive/adult_age.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/climate_action_incentive/adult_age.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/climate_action_incentive/amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/climate_action_incentive/amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/dtc/base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/dtc/base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/dtc/child_supplement.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/dtc/child_supplement.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/dtc/supplement_ineligible_age.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/dtc/supplement_ineligible_age.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/base_amounts.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/base_amounts.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/singles_boost/cap.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/singles_boost/cap.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/singles_boost/phase_in.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/gst_credit/singles_boost/phase_in.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/school_supply_credit/amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/school_supply_credit/amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/school_supply_credit/cap.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/school_supply_credit/cap.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/credits/training/amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/cra/tax/income/income_tax_schedule.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/cra/tax/income/income_tax_schedule.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/four_or_more_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/four_or_more_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/one_child.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/one_child.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/three_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/three_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/two_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/base_component/phase_out/two_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/four_or_more_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/four_or_more_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/one_child.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/one_child.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/three_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/three_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/two_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/base/two_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_in/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_in/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/four_or_more_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/four_or_more_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/one_child.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/one_child.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/three_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/three_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/two_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/two_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/age_credit/base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/age_credit/base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/age_credit/eligible_age.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/age_credit/eligible_age.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/age_credit/phase_out_rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/age_credit/phase_out_rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/additional_amount/base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/additional_amount/base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/additional_amount/childcare_expense_threshold.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/additional_amount/childcare_expense_threshold.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/non_refundable.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/non_refundable.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 description: Alberta provides the following non-refundable tax credits.  
 values:
   2022-01-01:
     - ab_age_credit
     - ab_disability_credit
     - ab_pension_credit
     - ab_spouse_and_common_law_partner_amount_credit
+    - ab_basic_personal_amount
 
 metadata:
   unit: list  
   period: year 
   label: Alberta non-refundable credits  
   reference:
   - title: Alberta Disablitiy Credit worksheet 2022 - Page 2
```

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/spouse_and_common_law_partner_amount/base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/spouse_and_common_law_partner_amount/base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ab/tax/income/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/first_reduction/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/first_reduction/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/second_reduction/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/benefits/bcfb/second_reduction/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/age/phase_out/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/age/phase_out/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/basic_personal_amount/base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/basic_personal_amount/base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/adult_age.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/adult_age.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/reduction_rate/family.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/reduction_rate/family.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/reduction_rate/single.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/bccatc/reduction_rate/single.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/disability/additional_amount/base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/disability/additional_amount/base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/disability/additional_amount/childcare_expense_threshold.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/disability/additional_amount/childcare_expense_threshold.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/disability/base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/disability/base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/non_refundable.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/non_refundable.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/pension_income_amount/cap.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/pension_income_amount/cap.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/tax_reduction/reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/credits/tax_reduction/reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/bc/tax/income/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/five_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/five_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/four_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/four_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/one_child.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/one_child.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/six_or_more_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/six_or_more_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/three_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/three_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/two_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/benefits/mbcb/reduction/two_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/age_amount/age_eligibility.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/age_amount/age_eligibility.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/age_amount/max_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/age_amount/max_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/age_amount/phase_out_rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/age_amount/phase_out_rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/basic_personal_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/credits/basic_personal_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/mb/tax/income/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/eligible_age.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/eligible_age.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/phase_out/multiple_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/phase_out/multiple_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/phase_out/one_child.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/phase_out/one_child.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/working_income_supplement/base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/working_income_supplement/base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/working_income_supplement/phase_in.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/working_income_supplement/phase_in.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/working_income_supplement/phase_out.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/nbcb/working_income_supplement/phase_out.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/benefits/pension_benefit/cap.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/benefits/pension_benefit/cap.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/age_amount/reduction_rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/age_amount/reduction_rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nb/tax/income/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/credits/physical_activity/age_eligible.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/credits/physical_activity/age_eligible.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nl/tax/income/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/disability_amount/base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/disability_amount/base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/dependant/base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/base/dependant/base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/phase_out.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/phase_out.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/nsaltc/reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/nsaltc/reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/pension_income_amount/cap.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/credits/pension_income_amount/cap.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/limit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/limit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/ns/tax/income/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/age_credit/age_eligibility.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/age_credit/age_eligibility.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/age_credit/max_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/age_credit/max_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/age_credit/reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/age_credit/reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/basic_personal_amount/base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/credits/basic_personal_amount/base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nt/tax/income/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/base/amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/base/amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/base/phase_out_rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/base/phase_out_rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/working/amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/working/amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/working/phase_in_rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/benefits/nucb/working/phase_in_rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/age_amount/phase_out_rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/credits/age_amount/phase_out_rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/nu/tax/income/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/benefits/ocb/reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/benefits/ocb/reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/full_time_calculation.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/subsidies/on_child_care_fee_subsidy/full_time_calculation.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/age_eligibility.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/age_eligibility.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/max_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/max_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/reduction/family.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/reduction/family.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/reduction/single.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/grants/oshptg/reduction/single.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/reduction/family.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/reduction/family.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/reduction/single.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/lift/reduction/single.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/shared_custody/base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/shared_custody/base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/shared_custody/divisor.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/shared_custody/divisor.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/shared_custody/start.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/shared_custody/start.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/start.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/noec/phase_out/start.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/energy_component/max_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/energy_component/max_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/energy_component/multiplier.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/energy_component/multiplier.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/energy_component/student_resident_reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/energy_component/student_resident_reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/occupancy_costs/rent_multiplier.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/occupancy_costs/rent_multiplier.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/occupancy_costs/student_resident_supplement.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/occupancy_costs/student_resident_supplement.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/shared_custody/divisor.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/shared_custody/divisor.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/shared_custody/start.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/shared_custody/start.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/start.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/phase_out/start.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/property_tax_component/initial_cap.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/property_tax_component/initial_cap.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/property_tax_component/multiplier.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/property_tax_component/multiplier.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/property_tax_component/supplement.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/property_tax_component/supplement.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/second_subtraction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/oeptc/second_subtraction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/ostc/reduction/family.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/ostc/reduction/family.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/ostc/reduction/single.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/credits/ostc/reduction/single.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/on/tax/income/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/on/tax/income/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/pe/tax/income/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/pe/tax/income/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/basic_personal_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/basic_personal_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cce/nondisabled_child_expense_limit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cce/nondisabled_child_expense_limit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cce/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cce/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cost_of_living/reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/cost_of_living/reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/age_eligibility.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/age_eligibility.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/child_amount/max.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/child_amount/max.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/child_amount/min.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/child_amount/min.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/reduction/single_parent_family.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/reduction/single_parent_family.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/reduction/two_parent_family.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/reduction/two_parent_family.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/shared_custody_multiplier.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/shared_custody_multiplier.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/single_parent_amount/max.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/single_parent_amount/max.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/single_parent_amount/min.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/single_parent_amount/min.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/handicapped_child/base_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/handicapped_child/base_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/handicapped_child/exceptional_care_amount/tier1.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/handicapped_child/exceptional_care_amount/tier1.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/handicapped_child/exceptional_care_amount/tier2.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/handicapped_child/exceptional_care_amount/tier2.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/school_supplies/handicapped_child.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/school_supplies/handicapped_child.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/school_supplies/non_handicapped_child.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/fa/supplement/school_supplies/non_handicapped_child.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/reduction/married.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/reduction/married.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/reduction/single.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/sa/reduction/single.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/couple/amount/with_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/couple/amount/with_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/couple/amount/without_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/couple/amount/without_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/couple/reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/couple/reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/single/amount/person_living_alone.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/single/amount/person_living_alone.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/single/amount/single_parent.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/single/amount/single_parent.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/single/reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/single/reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/work_income_requirement.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/work_income_requirement.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/age_eligibility.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/age_eligibility.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/amount/with_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/amount/with_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/amount/without_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/amount/without_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/work_income_requirement.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/couple/work_income_requirement.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/amount/person_living_alone.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/amount/person_living_alone.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/amount/single_parent.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/amount/single_parent.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/work_income_requirement.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/single/work_income_requirement.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/supplement/amount/couple.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/supplement/amount/couple.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/supplement/amount/single.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/supplement/amount/single.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/supplement/work_income_eligibility.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/credits/work_premium/supplement/work_income_eligibility.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/qc/tax/income/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/amount/disabled.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/amount/disabled.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/amount/non_disabled.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/amount/non_disabled.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/eligibility/age.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/eligibility/age.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/eligibility/income.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/benefits/afb/eligibility/income.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/age_amount/age_eligibility.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/age_amount/age_eligibility.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/age_amount/max_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/age_amount/max_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/age_amount/reduction/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/age_amount/reduction/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/disability_amount/amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/disability_amount/amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/age_threshold.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/age_threshold.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/child/amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/child/amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/head.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/head.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/phase_out.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/phase_out.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/spouse.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/credits/slic/spouse.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/sk/tax/income/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/amount/child.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/amount/child.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/amount/self.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/amount/self.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/amount/spouse.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/benefits/rebates/ygcpri/amount/spouse.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_arts_credit/amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_arts_credit/amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_arts_credit/child_age_eligibility.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/childrens_arts_credit/child_age_eligibility.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/employment_amount/amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/credits/employment_amount/amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/rate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/parameters/gov/provinces/yt/tax/income/rate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/ccb/child_benefit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/ccb/child_benefit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cdb/child_disability_benefit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cdb/child_disability_benefit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cdb/child_disability_benefit_eligible.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cdb/child_disability_benefit_eligible.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cdb/child_disability_benefit_reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cdb/child_disability_benefit_reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cdb/integration.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cdb/integration.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/base/cwb_base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/base/cwb_base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/base/cwb_base_phase_in.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/base/cwb_base_phase_in.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/canada_workers_benefit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/canada_workers_benefit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_category.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_category.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_eligible.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_eligible.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_max_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_max_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_phase_out.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_phase_out.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/cwb/is_cwb_family.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/cwb/is_cwb_family.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/dental_benefit/dental_benefit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/dental_benefit/dental_benefit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/dental_benefit/dental_benefit_eligible.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/dental_benefit/dental_benefit_eligible.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/benefits/oas/integration.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/benefits/oas/integration.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/age_amount_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/age_amount_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/basic_personal_amount/basic_personal_amount_supplement.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/basic_personal_amount/basic_personal_amount_supplement.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/climate_action_incentive_person.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/climate_action_incentive_person.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/climate_action_incentive_single_parent_household.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/climate_action_incentive_single_parent_household.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/integration.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/integration.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/integration_eldest_child.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/integration_eldest_child.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/is_eldest_child_for_climate_action_incentive.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/climate_action/is_eldest_child_for_climate_action_incentive.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit_category.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit_category.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit_single_parent_household.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit_single_parent_household.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit_singles_boost.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/gst_credit_singles_boost.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/integration.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/gst_credit/integration.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/cra/tax/income/credits/training_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/cra/tax/income/credits/training_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/integration.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/integration.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_base_component.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_base_component.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_base_component_base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_base_component_base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_base_component_reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_base_component_reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_working_component.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_working_component.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_working_component_base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_working_component_base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_working_component_reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_working_component_reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/ab_spouse_and_common_law_partner_amount/ab_spouse_and_common_law_partner_amount_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/ab_spouse_and_common_law_partner_amount/ab_spouse_and_common_law_partner_amount_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/age_credit/age_credit_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/age_credit/age_credit_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit_additional_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit_additional_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/benefits/bcfb/bc_family_benefit_base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/benefits/bcfb/bc_family_benefit_base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/benefits/bcfb/bc_family_benefit_first_reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/benefits/bcfb/bc_family_benefit_first_reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/benefits/bcfb/bc_family_benefit_second_reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/benefits/bcfb/bc_family_benefit_second_reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_age_credit/bc_age_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_age_credit/bc_age_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit_additional_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit_additional_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit_eligible.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit_eligible.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_single_parent_household.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_single_parent_household.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/is_eldest_child_for_bc_climate_action_tax_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/credits/bccatc/is_eldest_child_for_bc_climate_action_tax_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/bc/tax/income/income_tax.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/bc/tax/income/income_tax.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/mb/tax/income/benefits/mb_child_benefit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/mb/tax/income/benefits/mb_child_benefit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/age_amount/mb_age_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/age_amount/mb_age_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/pension_amount/mb_pension_amount_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/mb/tax/income/credits/pension_amount/mb_pension_amount_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/benefits/nbcb/nb_child_benefit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/benefits/nbcb/nb_child_benefit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/benefits/nbcb/nb_child_benefit_supplement.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/benefits/nbcb/nb_child_benefit_supplement.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/nb_low_income_tax_reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/nb_low_income_tax_reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/nb_low_income_tax_reduction_base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/nb_low_income_tax_reduction_base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/tax/income/credits/nb_age_amount_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/tax/income/credits/nb_age_amount_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nb/tax/income/income_tax.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nb/tax/income/income_tax.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nl/tax/income/credits/nl_phyical_activity_tax_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nl/tax/income/credits/nl_phyical_activity_tax_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nl/tax/income/income_tax.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nl/tax/income/income_tax.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/benefits/child_benefit/ns_child_benefit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/benefits/child_benefit/ns_child_benefit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/age/ns_age_tax_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/age/ns_age_tax_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_base_children.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_base_children.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/ns_pension_income_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/ns_pension_income_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/nsaltc/ns_affordable_living_tax_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/nsaltc/ns_affordable_living_tax_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/prc/ns_poverty_reduction_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/credits/prc/ns_poverty_reduction_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_assistance/eligibility/age/ns_income_assistance_age_eligibility.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_assistance/eligibility/age/ns_income_assistance_age_eligibility.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/ns_income_assistance_asset_eligibility.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/ns_income_assistance_asset_eligibility.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nt/tax/income/income_tax.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nt/tax/income/income_tax.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nt/tax/income/nt_age_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nt/tax/income/nt_age_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nt/tax/income/nt_age_credit_eligible.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nt/tax/income/nt_age_credit_eligible.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nt/tax/income/nt_basic_personal_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nt/tax/income/nt_basic_personal_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/nu_child_benefit_base_component_base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/nu_child_benefit_base_component_base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/nu_child_benefit_base_component_reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/nu_child_benefit_base_component_reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/nu_child_benefit_working_component.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/benefits/child_benefit/nu_child_benefit_working_component.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/age_amount/nu_age_amount_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/age_amount/nu_age_amount_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/nu_cost_of_living_basic_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/nu_cost_of_living_basic_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/nu_cost_of_living_credit_supplement.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/nu/tax/income/credits/nu_cost_of_living_credit_supplement.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/benefits/ocb/on_child_benefit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/benefits/ocb/on_child_benefit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/benefits/ocb/on_child_benefit_base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/benefits/ocb/on_child_benefit_base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant_base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant_base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant_reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant_reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit_base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit_base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/noec/northern_ontario_energy_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/noec/northern_ontario_energy_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/integration.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/integration.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oeptc.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oeptc.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oeptc_energy_component.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oeptc_energy_component.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oeptc_property_tax_component.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oeptc_property_tax_component.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oshptg_adjusted_opetc.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/oeptc/oshptg_adjusted_opetc.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit_base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit_base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit_reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit_reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_part_time.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_part_time.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_reduction.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/on/tax/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_reduction.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/pe/tax/income/income_tax.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/pe/tax/income/income_tax.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/cce/cce_disabled_child_tax_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/cce/cce_disabled_child_tax_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/cost_of_living.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/cost_of_living.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/fa/qc_fa_payment.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/fa/qc_fa_payment.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/fa/qc_fa_supplement.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/fa/qc_fa_supplement.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/qc_sa_married_both_eligible.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/qc_sa_married_both_eligible.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/qc_sa_married_one_eligible.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/qc_sa_married_one_eligible.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/qc_sa_tax_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/sa/qc_sa_tax_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/qc_adapted_work_premium_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/qc_adapted_work_premium_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/qc_adapted_work_premium_eligible.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/qc_adapted_work_premium_eligible.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/qc_general_work_premium_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/qc_general_work_premium_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/qc_general_work_premium_eligible.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/qc_general_work_premium_eligible.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit_base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit_base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit_supplement.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit_supplement.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_eligible.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_eligible.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/qc/tax/income/income_tax.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/qc/tax/income/income_tax.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/benefits/afb/sk_active_family_benefit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/benefits/afb/sk_active_family_benefit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/age_amount/sk_age_amount.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/age_amount/sk_age_amount.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/age_amount/sk_age_amount_eligible.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/age_amount/sk_age_amount_eligible.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/sk_senior_supplementary_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/sk_senior_supplementary_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/sk_senior_supplementary_eligible.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/sk_senior_supplementary/sk_senior_supplementary_eligible.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit_base.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit_base.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/sk/tax/income/income_tax.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/sk/tax/income/income_tax.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/benefits/yt_child_benefit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/benefits/yt_child_benefit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_disabled_child.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_disabled_child.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_eligible_child.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_eligible_child.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_childrens_fitness_tax_credit.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_childrens_fitness_tax_credit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_childrens_fitness_tax_credit_disability_supplement.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_childrens_fitness_tax_credit_disability_supplement.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/yt_first_nations_tax.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/credits/yt_first_nations_tax.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/gov/provinces/yt/tax/income/rebates/yt_government_carbon_price_rebate.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/gov/provinces/yt/tax/income/rebates/yt_government_carbon_price_rebate.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/tests/household/person/spouse_income.yaml` & `policyengine-canada-0.95.0/policyengine_canada/tests/household/person/spouse_income.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/benefits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/benefits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit_base_person.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit_base_person.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit_reduction.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/ccb/child_benefit_reduction.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cdb/child_disability_benefit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cdb/child_disability_benefit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cdb/child_disability_benefit_eligible.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cdb/child_disability_benefit_eligible.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cdb/child_disability_benefit_reduction.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cdb/child_disability_benefit_reduction.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/base/cwb_base.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/base/cwb_base.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/base/cwb_base_phase_in.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/base/cwb_base_phase_in.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/base/cwb_base_phase_out.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/base/cwb_base_phase_out.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/cwb_eligible.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/cwb_eligible.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_category.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_category.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_eligible.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_eligible.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_max_amount.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_max_amount.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_phase_out.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/cwb/disability_supplement/cwb_disability_supplement_phase_out.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/dental_benefit/dental_benefit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/dental_benefit/dental_benefit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/dental_benefit/dental_benefit_eligible.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/dental_benefit/dental_benefit_eligible.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/old_age_security_pension/oas_eligibility.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/old_age_security_pension/oas_eligibility.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/old_age_security_pension/oas_pre_repayment.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/old_age_security_pension/oas_pre_repayment.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/benefits/old_age_security_pension/oas_repayment.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/benefits/old_age_security_pension/oas_repayment.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/age_amount/age_amount_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/age_amount/age_amount_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/basic_personal_amount/basic_personal_amount_supplement.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/basic_personal_amount/basic_personal_amount_supplement.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/canada_employment_amount.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/canada_employment_amount.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive_category.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive_category.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive_person.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive_person.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive_single_parent_household.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/climate_action_incentive_single_parent_household.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/is_child_for_climate_action_incentive.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/is_child_for_climate_action_incentive.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/is_eldest_child_for_climate_action_incentive.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/climate_action/is_eldest_child_for_climate_action_incentive.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/dtc/dtc_child_supplement.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/dtc/dtc_child_supplement.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_category.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_category.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_person.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_person.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_reduction.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_reduction.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_single_parent_household.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_single_parent_household.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_singles_boost.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/gst_credit_singles_boost.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/is_child_for_gst_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/is_child_for_gst_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/is_eldest_child_in_single_household_for_gst_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/gst_credit/is_eldest_child_in_single_household_for_gst_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/credits/training/training_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/credits/training/training_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/cra/tax/income/income_tax_before_refundable_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/cra/tax/income/income_tax_before_refundable_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_base_component_base.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_base_component_base.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_base_component_reduction.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_base_component_reduction.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_working_component_base.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_working_component_base.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_working_component_reduction.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/benefits/acfb/acfb_working_component_reduction.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/ab_income_tax_before_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/ab_income_tax_before_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/ab_income_tax_before_refundable_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/ab_income_tax_before_refundable_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/ab_spouse_and_common_law_partner_amount_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/ab_spouse_and_common_law_partner_amount_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit_additional_amount.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit_additional_amount.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit_base.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit_base.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit_first_reduction.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit_first_reduction.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/bc_income_tax_before_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/bc_income_tax_before_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/bc_income_tax_before_refundable_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/bc_income_tax_before_refundable_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/basic_personal_amount/bc_basic_personal_amount.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/basic_personal_amount/bc_basic_personal_amount.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_age_credit/bc_age_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_age_credit/bc_age_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit_additional_amount.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_disability_credit/bc_disability_credit_additional_amount.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_tax_reduction_credit/bc_tax_reduction_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bc_tax_reduction_credit/bc_tax_reduction_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_incentive_category.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_incentive_category.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_person.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_person.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_single_parent_household.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/bc_climate_action_tax_credit_single_parent_household.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/is_child_for_bc_climate_action_tax_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/is_child_for_bc_climate_action_tax_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/is_eldest_child_for_bc_climate_action_tax_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/bccatc/is_eldest_child_for_bc_climate_action_tax_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/pension_income_amount/bc_pension_income_amount.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/bc/tax/income/credits/pension_income_amount/bc_pension_income_amount.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/benefits/child_benefit/mb_child_benefit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/benefits/child_benefit/mb_child_benefit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/age_amount/mb_age_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/age_amount/mb_age_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/age_amount/mb_age_credit_eligible.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/age_amount/mb_age_credit_eligible.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/pension_amount/mb_pension_amount_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/credits/pension_amount/mb_pension_amount_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/mb_income_tax_before_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/mb_income_tax_before_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/mb/tax/income/mb_income_tax_before_refundable_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/mb/tax/income/mb_income_tax_before_refundable_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/benefits/nbcb/nb_child_benefit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/benefits/nbcb/nb_child_benefit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/benefits/nbcb/nb_child_benefit_supplement.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/benefits/nbcb/nb_child_benefit_supplement.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/benefits/pension_benefit/nb_pension_benefit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/benefits/pension_benefit/nb_pension_benefit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/age_amount/nb_age_amount_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/age_amount/nb_age_amount_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/nb_low_income_tax_reduction.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/nb_low_income_tax_reduction.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/nb_low_income_tax_reduction_base.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/tax/income/credits/low_income_tax_reduction/nb_low_income_tax_reduction_base.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/tax/income/nb_income_tax_before_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/tax/income/nb_income_tax_before_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nb/tax/income/nb_income_tax_before_refundable_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nb/tax/income/nb_income_tax_before_refundable_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nl/tax/income/credit/nl_physical_activity_tax_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nl/tax/income/credit/nl_physical_activity_tax_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nl/tax/income/nl_income_tax_before_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nl/tax/income/nl_income_tax_before_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nl/tax/income/nl_income_tax_before_refundable_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nl/tax/income/nl_income_tax_before_refundable_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/benefits/child_benefit/ns_child_benefit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/benefits/child_benefit/ns_child_benefit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/age/ns_age_tax_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/age/ns_age_tax_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_base.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_base.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_base_children.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_base_children.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_eligible_child.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_eligible_child.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_reduction.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/low_income_tax_reduction/ns_low_income_tax_reduction_reduction.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/ns_disability_amount.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/ns_disability_amount.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/ns_pension_income_amount.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/ns_pension_income_amount.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/nsaltc/ns_affordable_living_tax_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/nsaltc/ns_affordable_living_tax_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/prc/ns_poverty_reduction_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/credits/prc/ns_poverty_reduction_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/age/ns_income_assistance_age_eligibility.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/age/ns_income_assistance_age_eligibility.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/ns_income_assistance_applicable_assets.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/ns_income_assistance_applicable_assets.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/ns_income_assistance_asset_eligibility.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/income_assistance/eligibility/assets/ns_income_assistance_asset_eligibility.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/ns_income_tax_before_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/ns_income_tax_before_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/ns/tax/income/ns_income_tax_before_refundable_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/ns/tax/income/ns_income_tax_before_refundable_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/age_credit/nt_age_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/age_credit/nt_age_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/age_credit/nt_age_credit_eligible.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/age_credit/nt_age_credit_eligible.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/basic_personal_amount/nt_basic_personal_amount.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nt/tax/income/credits/basic_personal_amount/nt_basic_personal_amount.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nt/tax/income/nt_income_tax_before_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nt/tax/income/nt_income_tax_before_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nt/tax/income/nt_income_tax_before_refundable_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nt/tax/income/nt_income_tax_before_refundable_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_base_component.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_base_component.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_base_component_base.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_base_component_base.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_working_component.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/benefits/nu_child_benefit/nu_child_benefit_working_component.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/age_amount/nu_age_amount_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/age_amount/nu_age_amount_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/nu_cost_of_living_basic_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/nu_cost_of_living_basic_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/nu_cost_of_living_credit_adjusted_net_income.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/nu_cost_of_living_credit_adjusted_net_income.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/nu_cost_of_living_credit_supplement.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/credits/nu_cost_of_living_credit_supplement.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/nu_income_tax_before_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/nu_income_tax_before_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/nu/tax/income/nu_income_tax_before_refundable_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/nu/tax/income/nu_income_tax_before_refundable_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/benefits/ocb/on_child_benefit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/benefits/ocb/on_child_benefit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/benefits/ocb/on_child_benefit_base.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/benefits/ocb/on_child_benefit_base.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_full_time.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_full_time.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_part_time.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_part_time.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_reduction.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/subsidies/on_child_care_fee_subsidy/on_child_care_fee_subsidy_reduction.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant_base.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant_base.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant_reduction.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/grants/oshptg/on_senior_homeowners_property_tax_grant_reduction.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit_base.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/lift/on_low_income_workers_tax_credit_base.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/noec/northern_ontario_energy_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/noec/northern_ontario_energy_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/is_senior_for_oeptc.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/is_senior_for_oeptc.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_category.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_category.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_energy_component.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_energy_component.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_occupancy_cost.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_occupancy_cost.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_property_tax_component.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oeptc_property_tax_component.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oshptg_adjusted_oeptc.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/oeptc/oshptg_adjusted_oeptc.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit_base.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit_base.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit_reduction.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/credits/ostc/on_sales_tax_credit_reduction.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/on_income_tax_before_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/on_income_tax_before_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/on/tax/income/on_income_tax_before_refundable_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/on/tax/income/on_income_tax_before_refundable_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/pe/tax/income/pe_income_tax_before_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/pe/tax/income/pe_income_tax_before_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/pe/tax/income/pe_income_tax_before_refundable_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/pe/tax/income/pe_income_tax_before_refundable_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cce/qc_cce_disabled_child_tax_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cce/qc_cce_disabled_child_tax_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cce/qc_cce_nondisabled_child_tax_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cce/qc_cce_nondisabled_child_tax_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cost_of_living/qc_cost_of_living_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/cost_of_living/qc_cost_of_living_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_eligibility.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_eligibility.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_payment.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_payment.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_supplement.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/fa/qc_fa_supplement.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/qc_basic_personal_amount.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/qc_basic_personal_amount.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_married_both_eligible.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_married_both_eligible.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_married_one_eligible.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_married_one_eligible.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_single_eligible.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_single_eligible.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_spouse_eligible.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_spouse_eligible.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_tax_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/sa/qc_sa_tax_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/qc_adapted_work_premium_amount.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/qc_adapted_work_premium_amount.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/qc_adapted_work_premium_eligible.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/adapted_work_premium/qc_adapted_work_premium_eligible.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/qc_general_work_premium_amount.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/qc_general_work_premium_amount.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/qc_general_work_premium_eligible.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/general_work_premium/qc_general_work_premium_eligible.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit_base.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit_base.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit_supplement.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_credit_supplement.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_eligible.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/credits/work_premium/qc_work_premium_eligible.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/qc/tax/income/qc_income_tax_before_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/qc/tax/income/qc_income_tax_before_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/benefits/afb/sk_active_family_benefit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/benefits/afb/sk_active_family_benefit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/age_amount/sk_age_amount.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/age_amount/sk_age_amount.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/age_amount/sk_age_amount_eligible.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/age_amount/sk_age_amount_eligible.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/sk_senior_supplementary_credit/sk_senior_supplementary_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/sk_senior_supplementary_credit/sk_senior_supplementary_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/sk_senior_supplementary_credit/sk_senior_supplementary_credit_eligible.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/sk_senior_supplementary_credit/sk_senior_supplementary_credit_eligible.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit_base.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit_base.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit_eligible_child.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/credits/slic/sk_low_income_credit_eligible_child.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/sk/tax/income/sk_income_tax_before_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/sk/tax/income/sk_income_tax_before_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/benefits/yukon_child_benefit/yt_child_benefit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/benefits/yukon_child_benefit/yt_child_benefit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/benefits/rebates/ygcpri/yt_government_carbon_price_rebate.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/benefits/rebates/ygcpri/yt_government_carbon_price_rebate.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit_eligible_child.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_arts_credit/yt_childrens_arts_credit_eligible_child.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_disabled_child.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_disabled_child.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_eligible_child.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_cftc_eligible_child.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_childrens_fitness_tax_credit.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_childrens_fitness_tax_credit.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_childrens_fitness_tax_credit_disability_supplement.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/childrens_fitness_tax_credit/yt_childrens_fitness_tax_credit_disability_supplement.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/yt_employment_amount.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/yt_employment_amount.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/yt_first_nations_tax.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/credits/yt_first_nations_tax.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/gov/provinces/yt/tax/income/yt_income_tax_before_credits.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/gov/provinces/yt/tax/income/yt_income_tax_before_credits.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/household/demographic/geographic/province/in_province.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/household/demographic/geographic/province/in_province.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/household/demographic/geographic/province/province.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/household/demographic/geographic/province/province.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/household/demographic/geographic/province/province_code.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/household/demographic/geographic/province/province_code.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/household/demographic/geographic/province/province_enum.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/household/demographic/geographic/province/province_enum.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/household/demographic/geographic/province/province_name.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/household/demographic/geographic/province/province_name.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/household/income/individual/individual_net_income.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/household/income/individual/individual_net_income.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/household/income/individual/investment_income.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/household/income/individual/investment_income.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/household/income/individual/other_employment_income.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/household/income/individual/other_employment_income.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/household/income/individual/self_employment_income.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/household/income/individual/self_employment_income.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/household/income/individual/total_individual_pre_tax_income.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/household/income/individual/total_individual_pre_tax_income.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/household/marginal_tax_rate.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/household/marginal_tax_rate.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada/variables/household/person/is_father.py` & `policyengine-canada-0.95.0/policyengine_canada/variables/household/person/is_father.py`

 * *Files identical despite different names*

### Comparing `policyengine-canada-0.94.0/policyengine_canada.egg-info/PKG-INFO` & `policyengine-canada-0.95.0/policyengine_canada.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyengine-canada
-Version: 0.94.0
+Version: 0.95.0
 Summary: Microsimulation model for Canada's tax-benefit system.
 Home-page: https://github.com/policyengine/policyengine-canada
 Author: PolicyEngine
 Author-email: hello@policyengine.org
 License: https://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit microsimulation framework
 Platform: UNKNOWN
```

### Comparing `policyengine-canada-0.94.0/policyengine_canada.egg-info/SOURCES.txt` & `policyengine-canada-0.95.0/policyengine_canada.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 policyengine_canada/parameters/gov/provinces/ab/benefits/acfb/working_component/phase_out/two_children.yaml
 policyengine_canada/parameters/gov/provinces/ab/tax/income/rate.yaml
 policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/non_refundable.yaml
 policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/refundable.yaml
 policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/age_credit/base.yaml
 policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/age_credit/eligible_age.yaml
 policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/age_credit/phase_out_rate.yaml
+policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/basic_personal_amount/amount.yaml
 policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/base.yaml
 policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/cap.yaml
 policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/additional_amount/base.yaml
 policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/disability/additional_amount/childcare_expense_threshold.yaml
 policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/pension/max_amount.yaml
 policyengine_canada/parameters/gov/provinces/ab/tax/income/credits/spouse_and_common_law_partner_amount/base.yaml
 policyengine_canada/parameters/gov/provinces/bc/README.md
@@ -462,14 +463,15 @@
 policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_working_component.yaml
 policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_working_component_base.yaml
 policyengine_canada/tests/gov/provinces/ab/benefits/acbf/acfb_working_component_reduction.yaml
 policyengine_canada/tests/gov/provinces/ab/tax/income/income_tax.yaml
 policyengine_canada/tests/gov/provinces/ab/tax/income/credits/ab_spouse_and_common_law_partner_amount/ab_spouse_and_common_law_partner_amount_credit.yaml
 policyengine_canada/tests/gov/provinces/ab/tax/income/credits/age_credit/ab_age_credit_eligible.yaml
 policyengine_canada/tests/gov/provinces/ab/tax/income/credits/age_credit/age_credit_amount.yaml
+policyengine_canada/tests/gov/provinces/ab/tax/income/credits/basic_personal_amount/ab_basic_personal_amount.yaml
 policyengine_canada/tests/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit.yaml
 policyengine_canada/tests/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit_additional_amount.yaml
 policyengine_canada/tests/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit_eligible.yaml
 policyengine_canada/tests/gov/provinces/ab/tax/income/credits/pension/ab_pension_credit.yaml
 policyengine_canada/tests/gov/provinces/bc/benefits/bcfb/bc_family_benefit_base.yaml
 policyengine_canada/tests/gov/provinces/bc/benefits/bcfb/bc_family_benefit_first_reduction.yaml
 policyengine_canada/tests/gov/provinces/bc/benefits/bcfb/bc_family_benefit_second_reduction.yaml
@@ -704,14 +706,15 @@
 policyengine_canada/variables/gov/provinces/ab/tax/income/ab_income_tax_before_refundable_credits.py
 policyengine_canada/variables/gov/provinces/ab/tax/income/ab_taxable_income.py
 policyengine_canada/variables/gov/provinces/ab/tax/income/credits/ab_non_refundable_credits.py
 policyengine_canada/variables/gov/provinces/ab/tax/income/credits/ab_refundable_credits.py
 policyengine_canada/variables/gov/provinces/ab/tax/income/credits/ab_spouse_and_common_law_partner_amount_credit.py
 policyengine_canada/variables/gov/provinces/ab/tax/income/credits/age_credit/ab_age_credit.py
 policyengine_canada/variables/gov/provinces/ab/tax/income/credits/age_credit/ab_age_credit_eligible.py
+policyengine_canada/variables/gov/provinces/ab/tax/income/credits/basic_personal_amount/ab_basic_personal_amount.py
 policyengine_canada/variables/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit.py
 policyengine_canada/variables/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit_additional_amount.py
 policyengine_canada/variables/gov/provinces/ab/tax/income/credits/disability/ab_disability_credit_eligible.py
 policyengine_canada/variables/gov/provinces/ab/tax/income/credits/pension/ab_pension_credit.py
 policyengine_canada/variables/gov/provinces/bc/benefits/bc_benefits.py
 policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit.py
 policyengine_canada/variables/gov/provinces/bc/benefits/bcfb/bc_family_benefit_base.py
```

### Comparing `policyengine-canada-0.94.0/setup.py` & `policyengine-canada-0.95.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "sphinx",
     "sphinx-argparse",
     "sphinx-math-dollar",
 ]
 
 setup(
     name="policyengine-canada",
-    version="0.94.0",
+    version="0.95.0",
     author="PolicyEngine",
     author_email="hello@policyengine.org",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: POSIX",
         "Programming Language :: Python",
```

