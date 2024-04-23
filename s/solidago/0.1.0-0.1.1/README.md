# Comparing `tmp/solidago-0.1.0.tar.gz` & `tmp/solidago-0.1.1.tar.gz`

## Comparing `solidago-0.1.0.tar` & `solidago-0.1.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 solidago-0.1.0/experiments/engagement.py
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 solidago-0.1.0/experiments/engagement_bias.json
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 solidago-0.1.0/experiments/hyperparameters.json
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 solidago-0.1.0/experiments/multiplicator.json
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 solidago-0.1.0/experiments/plot.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 solidago-0.1.0/experiments/resilience.json
--rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 solidago-0.1.0/experiments/synthetic.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 solidago-0.1.0/experiments/tournesol.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 solidago-0.1.0/experiments/toy.json
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/__version__.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/judgments.py
--rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/primitives.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/privacy_settings.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/scoring_model.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/aggregation/__init__.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/aggregation/average.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/aggregation/base.py
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/aggregation/entitywise_qr_quantile.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/aggregation/standardized_qr_median.py
--rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/aggregation/standardized_qr_quantile.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/comparisons_to_scores/__init__.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/comparisons_to_scores/base.py
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/comparisons_to_scores/continuous_bradley_terry.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/comparisons_to_scores/hooke_individual_scores.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/generative_model/__init__.py
--rw-r--r--   0        0        0     6993 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/generative_model/comparison_model.py
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/generative_model/engagement_model.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/generative_model/entity_model.py
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/generative_model/generative_model.py
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/generative_model/user_model.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/generative_model/vouch_model.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/pipeline/__init__.py
--rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/pipeline/inputs.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/pipeline/outputs.py
--rw-r--r--   0        0        0    13904 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/pipeline/pipeline.py
--rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/pipeline/legacy2023/criterion_pipeline.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/pipeline/legacy2023/global_scores.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/pipeline/legacy2023/individual_scores.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/pipeline/legacy2023/parameters.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/pipeline/legacy2023/collaborative_scaling/__init__.py
--rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/pipeline/legacy2023/collaborative_scaling/scaling.py
--rw-r--r--   0        0        0    10250 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/pipeline/legacy2023/collaborative_scaling/scaling_step.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/post_process/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/post_process/base.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/post_process/no_post_process.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/post_process/squash.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/preference_learning/__init__.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/preference_learning/base.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/preference_learning/comparison_learning.py
--rw-r--r--   0        0        0    10235 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/preference_learning/generalized_bradley_terry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/preference_learning/hookean_model.py
--rw-r--r--   0        0        0     8264 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/preference_learning/lbfgs_generalized_bradley_terry.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/scaling/__init__.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/scaling/base.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/scaling/compose.py
--rw-r--r--   0        0        0    35006 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/scaling/mehestan.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/scaling/no_scaling.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/scaling/quantile_zero_shift.py
--rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/scaling/standardize.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/solvers/dichotomy.py
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/solvers/optimize.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/trust_propagation/__init__.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/trust_propagation/base.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/trust_propagation/lipschitrust.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/trust_propagation/no_trust_propagation.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/trust_propagation/trust_all.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/utils/date.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/utils/pairs.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/voting_rights/__init__.py
--rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/voting_rights/affine_overtrust.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/voting_rights/base.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/voting_rights/compute_voting_rights.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/voting_rights/is_trust.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 solidago-0.1.0/src/solidago/voting_rights/voting_rights.py
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/test_aggregation.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/test_generative_model.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/test_judgments.py
--rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/test_mehestan.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/test_pipeline.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/test_post_process.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/test_preference_learning.py
--rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/test_primitives.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/test_privacy_settings.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/test_scaling.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/test_solvers.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/test_trust_propagation.py
--rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/test_user_models.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/test_utils.py
--rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/test_voting_rights.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/data/data_0.py
--rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/data/data_1.py
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/data/data_2.py
--rw-r--r--   0        0        0    11197 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/data/data_3.py
--rw-r--r--   0        0        0    22058 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/data/data_4.py
--rw-r--r--   0        0        0   695004 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/data/tiny_tournesol.zip
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 solidago-0.1.0/tests/data/utils.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 solidago-0.1.0/.gitignore
--rw-r--r--   0        0        0    35147 2020-02-02 00:00:00.000000 solidago-0.1.0/LICENSE
--rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 solidago-0.1.0/LICENSE.LESSER
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 solidago-0.1.0/README.md
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 solidago-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 solidago-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 solidago-0.1.1/experiments/engagement.py
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 solidago-0.1.1/experiments/engagement_bias.json
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 solidago-0.1.1/experiments/hyperparameters.json
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 solidago-0.1.1/experiments/multiplicator.json
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 solidago-0.1.1/experiments/plot.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 solidago-0.1.1/experiments/resilience.json
+-rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 solidago-0.1.1/experiments/synthetic.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 solidago-0.1.1/experiments/tournesol.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 solidago-0.1.1/experiments/toy.json
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/__version__.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/judgments.py
+-rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/primitives.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/privacy_settings.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/scoring_model.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/aggregation/__init__.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/aggregation/average.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/aggregation/base.py
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/aggregation/entitywise_qr_quantile.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/aggregation/standardized_qr_median.py
+-rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/aggregation/standardized_qr_quantile.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/comparisons_to_scores/__init__.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/comparisons_to_scores/base.py
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/comparisons_to_scores/continuous_bradley_terry.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/comparisons_to_scores/hooke_individual_scores.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/generative_model/__init__.py
+-rw-r--r--   0        0        0     6993 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/generative_model/comparison_model.py
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/generative_model/engagement_model.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/generative_model/entity_model.py
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/generative_model/generative_model.py
+-rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/generative_model/user_model.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/generative_model/vouch_model.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/pipeline/__init__.py
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/pipeline/inputs.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/pipeline/outputs.py
+-rw-r--r--   0        0        0    13904 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/pipeline/pipeline.py
+-rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/pipeline/legacy2023/criterion_pipeline.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/pipeline/legacy2023/global_scores.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/pipeline/legacy2023/individual_scores.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/pipeline/legacy2023/parameters.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/pipeline/legacy2023/collaborative_scaling/__init__.py
+-rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/pipeline/legacy2023/collaborative_scaling/scaling.py
+-rw-r--r--   0        0        0    10250 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/pipeline/legacy2023/collaborative_scaling/scaling_step.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/post_process/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/post_process/base.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/post_process/no_post_process.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/post_process/squash.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/preference_learning/__init__.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/preference_learning/base.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/preference_learning/comparison_learning.py
+-rw-r--r--   0        0        0    10235 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/preference_learning/generalized_bradley_terry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/preference_learning/hookean_model.py
+-rw-r--r--   0        0        0     8264 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/preference_learning/lbfgs_generalized_bradley_terry.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/scaling/__init__.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/scaling/base.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/scaling/compose.py
+-rw-r--r--   0        0        0    35006 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/scaling/mehestan.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/scaling/no_scaling.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/scaling/quantile_zero_shift.py
+-rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/scaling/standardize.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/solvers/dichotomy.py
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/solvers/optimize.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/trust_propagation/__init__.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/trust_propagation/base.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/trust_propagation/lipschitrust.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/trust_propagation/no_trust_propagation.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/trust_propagation/trust_all.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/utils/date.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/utils/pairs.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/voting_rights/__init__.py
+-rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/voting_rights/affine_overtrust.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/voting_rights/base.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/voting_rights/compute_voting_rights.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/voting_rights/is_trust.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 solidago-0.1.1/src/solidago/voting_rights/voting_rights.py
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/test_aggregation.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/test_generative_model.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/test_judgments.py
+-rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/test_mehestan.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/test_pipeline.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/test_post_process.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/test_preference_learning.py
+-rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/test_primitives.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/test_privacy_settings.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/test_scaling.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/test_solvers.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/test_trust_propagation.py
+-rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/test_user_models.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/test_utils.py
+-rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/test_voting_rights.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/data/data_0.py
+-rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/data/data_1.py
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/data/data_2.py
+-rw-r--r--   0        0        0    11197 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/data/data_3.py
+-rw-r--r--   0        0        0    22058 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/data/data_4.py
+-rw-r--r--   0        0        0   695004 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/data/tiny_tournesol.zip
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 solidago-0.1.1/tests/data/utils.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 solidago-0.1.1/.gitignore
+-rw-r--r--   0        0        0    35147 2020-02-02 00:00:00.000000 solidago-0.1.1/LICENSE
+-rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 solidago-0.1.1/LICENSE.LESSER
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 solidago-0.1.1/README.md
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 solidago-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 solidago-0.1.1/PKG-INFO
```

### Comparing `solidago-0.1.0/experiments/engagement.py` & `solidago-0.1.1/experiments/engagement.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/experiments/engagement_bias.json` & `solidago-0.1.1/experiments/engagement_bias.json`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/experiments/hyperparameters.json` & `solidago-0.1.1/experiments/hyperparameters.json`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/experiments/multiplicator.json` & `solidago-0.1.1/experiments/multiplicator.json`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/experiments/plot.py` & `solidago-0.1.1/experiments/plot.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/experiments/resilience.json` & `solidago-0.1.1/experiments/resilience.json`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/experiments/synthetic.py` & `solidago-0.1.1/experiments/synthetic.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/experiments/tournesol.py` & `solidago-0.1.1/experiments/tournesol.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/experiments/toy.json` & `solidago-0.1.1/experiments/toy.json`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/judgments.py` & `solidago-0.1.1/src/solidago/judgments.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/primitives.py` & `solidago-0.1.1/src/solidago/primitives.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/privacy_settings.py` & `solidago-0.1.1/src/solidago/privacy_settings.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/scoring_model.py` & `solidago-0.1.1/src/solidago/scoring_model.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/aggregation/average.py` & `solidago-0.1.1/src/solidago/aggregation/average.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/aggregation/base.py` & `solidago-0.1.1/src/solidago/aggregation/base.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/aggregation/entitywise_qr_quantile.py` & `solidago-0.1.1/src/solidago/aggregation/entitywise_qr_quantile.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/aggregation/standardized_qr_median.py` & `solidago-0.1.1/src/solidago/aggregation/standardized_qr_median.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/aggregation/standardized_qr_quantile.py` & `solidago-0.1.1/src/solidago/aggregation/standardized_qr_quantile.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/comparisons_to_scores/base.py` & `solidago-0.1.1/src/solidago/comparisons_to_scores/base.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/comparisons_to_scores/continuous_bradley_terry.py` & `solidago-0.1.1/src/solidago/comparisons_to_scores/continuous_bradley_terry.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/comparisons_to_scores/hooke_individual_scores.py` & `solidago-0.1.1/src/solidago/comparisons_to_scores/hooke_individual_scores.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/generative_model/comparison_model.py` & `solidago-0.1.1/src/solidago/generative_model/comparison_model.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/generative_model/engagement_model.py` & `solidago-0.1.1/src/solidago/generative_model/engagement_model.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/generative_model/entity_model.py` & `solidago-0.1.1/src/solidago/generative_model/entity_model.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/generative_model/generative_model.py` & `solidago-0.1.1/src/solidago/generative_model/generative_model.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/generative_model/user_model.py` & `solidago-0.1.1/src/solidago/generative_model/user_model.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/generative_model/vouch_model.py` & `solidago-0.1.1/src/solidago/generative_model/vouch_model.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/pipeline/inputs.py` & `solidago-0.1.1/src/solidago/pipeline/inputs.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/pipeline/outputs.py` & `solidago-0.1.1/src/solidago/pipeline/outputs.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/pipeline/pipeline.py` & `solidago-0.1.1/src/solidago/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/pipeline/legacy2023/criterion_pipeline.py` & `solidago-0.1.1/src/solidago/pipeline/legacy2023/criterion_pipeline.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/pipeline/legacy2023/global_scores.py` & `solidago-0.1.1/src/solidago/pipeline/legacy2023/global_scores.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/pipeline/legacy2023/individual_scores.py` & `solidago-0.1.1/src/solidago/pipeline/legacy2023/individual_scores.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/pipeline/legacy2023/parameters.py` & `solidago-0.1.1/src/solidago/pipeline/legacy2023/parameters.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/pipeline/legacy2023/collaborative_scaling/scaling.py` & `solidago-0.1.1/src/solidago/pipeline/legacy2023/collaborative_scaling/scaling.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/pipeline/legacy2023/collaborative_scaling/scaling_step.py` & `solidago-0.1.1/src/solidago/pipeline/legacy2023/collaborative_scaling/scaling_step.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/post_process/base.py` & `solidago-0.1.1/src/solidago/post_process/base.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/post_process/no_post_process.py` & `solidago-0.1.1/src/solidago/post_process/no_post_process.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/post_process/squash.py` & `solidago-0.1.1/src/solidago/post_process/squash.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/preference_learning/base.py` & `solidago-0.1.1/src/solidago/preference_learning/base.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/preference_learning/comparison_learning.py` & `solidago-0.1.1/src/solidago/preference_learning/comparison_learning.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/preference_learning/generalized_bradley_terry.py` & `solidago-0.1.1/src/solidago/preference_learning/generalized_bradley_terry.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/preference_learning/lbfgs_generalized_bradley_terry.py` & `solidago-0.1.1/src/solidago/preference_learning/lbfgs_generalized_bradley_terry.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/scaling/__init__.py` & `solidago-0.1.1/src/solidago/scaling/__init__.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/scaling/base.py` & `solidago-0.1.1/src/solidago/scaling/base.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/scaling/compose.py` & `solidago-0.1.1/src/solidago/scaling/compose.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/scaling/mehestan.py` & `solidago-0.1.1/src/solidago/scaling/mehestan.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/scaling/no_scaling.py` & `solidago-0.1.1/src/solidago/scaling/no_scaling.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/scaling/quantile_zero_shift.py` & `solidago-0.1.1/src/solidago/scaling/quantile_zero_shift.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/scaling/standardize.py` & `solidago-0.1.1/src/solidago/scaling/standardize.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/solvers/dichotomy.py` & `solidago-0.1.1/src/solidago/solvers/dichotomy.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/solvers/optimize.py` & `solidago-0.1.1/src/solidago/solvers/optimize.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/trust_propagation/base.py` & `solidago-0.1.1/src/solidago/trust_propagation/base.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/trust_propagation/lipschitrust.py` & `solidago-0.1.1/src/solidago/trust_propagation/lipschitrust.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/trust_propagation/no_trust_propagation.py` & `solidago-0.1.1/src/solidago/trust_propagation/no_trust_propagation.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/trust_propagation/trust_all.py` & `solidago-0.1.1/src/solidago/trust_propagation/trust_all.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/utils/date.py` & `solidago-0.1.1/src/solidago/utils/date.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/utils/pairs.py` & `solidago-0.1.1/src/solidago/utils/pairs.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/voting_rights/affine_overtrust.py` & `solidago-0.1.1/src/solidago/voting_rights/affine_overtrust.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pandas as pd
 
-from .base import VotingRights, VotingRightsAssignment
-
 from solidago import PrivacySettings
 from solidago.solvers.dichotomy import solve
+from .base import VotingRights, VotingRightsAssignment
+
 
 class AffineOvertrust(VotingRightsAssignment):
     def __init__(
         self, 
         privacy_penalty: float = 0.5, 
         min_overtrust: float = 2.0,
         overtrust_ratio: float = 0.1,
@@ -27,126 +27,129 @@
     def __call__(
         self,
         users: pd.DataFrame,
         entities: pd.DataFrame,
         vouches: pd.DataFrame,
         privacy: PrivacySettings,
     ) -> tuple[VotingRights, pd.DataFrame]:
-        """ Compute voting rights
-        
+        """Compute voting rights
+
         Parameters
         ----------
         users: DataFrame with columns
             * user_id (int, index)
             * trust_score (float)
         entities: DataFrame with columns
             * entity_id (int, index)
         vouches: DataFrame
             This is not used by VotingRightsWithLimitedOvertrust
         privacy: PrivacySettings
             privacy[user, entity] is the privacy setting of user for entity
             May be True, False or None
-        
+
         Returns
         -------
         voting_rights[user, entity] is the voting right
             of a user on entity for criterion
         entities: DataFrame with columns
             * entity_id (int, index)
             * cumulative_trust (float)
             * min_voting_right (float)
             * overtrust (float)
-        """            
+        """
         voting_rights = VotingRights()
         if len(users) == 0:
             return voting_rights, entities
 
+        trust_scores = users["trust_score"]
         new_records = list()
         for e in entities.index:
             user_ids = privacy.users(e)
             privacy_weights = pd.Series(
-                {u: self.privacy_penalty if privacy[u, e] else 1 for u in user_ids}
+                {u: self.privacy_penalty if privacy[u, e] else 1.0 for u in user_ids}
             )
-
             (voting_rights_series, cumulative_trust, min_voting_right, overtrust) = (
                 self.compute_entity_voting_rights(
-                    trust_scores=users["trust_score"],
+                    trust_scores=trust_scores,
                     privacy_weights=privacy_weights,
                 )
             )
-
             for user_id, voting_right in voting_rights_series.items():
                 voting_rights[user_id, e] = voting_right  # type: ignore
             new_records.append((cumulative_trust, min_voting_right, overtrust))
 
         r = list(zip(*new_records))
         entities = entities.assign(cumulative_trust=r[0], min_voting_right=r[1], overtrust=r[2])
         return voting_rights, entities
 
     def compute_entity_voting_rights(
         self,
         trust_scores: pd.Series,
         privacy_weights: pd.Series,
     ) -> tuple[pd.Series, float, float, float]:
-        cumulative_trust = self.cumulative_trust(trust_scores, privacy_weights)
+        trust_scores_np = trust_scores[privacy_weights.index].fillna(0.0).to_numpy()
+        privacy_weights_np = privacy_weights.to_numpy()
+        cumulative_trust = self.cumulative_trust(trust_scores_np, privacy_weights_np)
         max_overtrust = self.maximal_overtrust(cumulative_trust)
-        min_voting_right = self.min_voting_right(max_overtrust, trust_scores, privacy_weights)
+        min_voting_right = self.min_voting_right(
+            max_overtrust, trust_scores_np, privacy_weights_np
+        )
         voting_rights = pd.Series(
-            privacy_weights * trust_scores.clip(lower=min_voting_right),
+            privacy_weights_np * trust_scores_np.clip(min=min_voting_right),
             index=privacy_weights.index,
         )
         return (
             voting_rights,
             cumulative_trust,
             min_voting_right,
-            voting_rights.sum() - cumulative_trust
+            voting_rights.sum() - cumulative_trust,
         )
 
     def cumulative_trust(
         self,
-        trust_scores: pd.Series,
-        privacy_weights: pd.Series,
+        trust_scores: np.ndarray,
+        privacy_weights: np.ndarray,
     ) -> float:
-        """ Returns the sum of trusts of raters of entity entity_id, 
+        """Returns the sum of trusts of raters of entity entity_id,
         weighted by their privacy setting.
-        
+
         Parameters
         ----------
         trust_scores: Series with
             * index "user_id (int, index)
             * values "trust_score" (float)
         privacy_weights: dict[int, float]
             privacy_weights[u] is the privacy weight of user u
-            
+
         Returns
         -------
         out: float
         """
         return (trust_scores * privacy_weights).sum()
 
     def maximal_overtrust(self, trust: float) -> float:
-        """ Computes the maximal allowed overtrust of an entity,
+        """Computes the maximal allowed overtrust of an entity,
         for a given total trust of the entity's raters.
-        
+
         Parameters
         ----------
         trust: float
             Cumulative trust received by the entity
-            
+
         Returns
         -------
         out: float
         """
         return trust * self.overtrust_ratio + self.min_overtrust 
 
     def overtrust(
         self,
         min_voting_right: float,
-        trust_scores: pd.Series,
-        privacy_weights: pd.Series,
+        trust_scores: np.ndarray,
+        privacy_weights: np.ndarray,
     ) -> float:
         """Returns the overtrust, if min_voting_right is enforced upon all raters.
 
         Parameters
         ----------
         min_voting_right: float
             Overtrust for min_voting_right
@@ -162,34 +165,35 @@
         return (privacy_weights * (min_voting_right - trust_scores))[
             min_voting_right > trust_scores
         ].sum()
 
     def min_voting_right(
         self,
         max_overtrust: float,
-        trust_scores: pd.Series,
-        privacy_weights: pd.Series,
+        trust_scores: np.ndarray,
+        privacy_weights: np.ndarray,
     ) -> float:
-        """ Returns the minimal voting rights that corresponds to max_overtrust.
-        
+        """Returns the minimal voting rights that corresponds to max_overtrust.
+
         Parameters
         ----------
         max_overtrust: float
             Maximal overtrust allowed for entity_id
         users: DataFrame with columns
             * user_id (int, index)
             * trust_score (float)
         privacy_weights: dict[int, float]
             privacy_weights[u] is the privacy weight of user u
-            
+
         Returns
         -------
         out: float
         """
         assert max_overtrust >= 0
+
         def overtrust(min_voting_right):
             return self.overtrust(min_voting_right, trust_scores, privacy_weights)
 
         if overtrust(1) <= max_overtrust:
             return 1.0
 
         return solve(overtrust, max_overtrust, 0, 1)
```

### Comparing `solidago-0.1.0/src/solidago/voting_rights/base.py` & `solidago-0.1.1/src/solidago/voting_rights/base.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/voting_rights/compute_voting_rights.py` & `solidago-0.1.1/src/solidago/voting_rights/compute_voting_rights.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/voting_rights/is_trust.py` & `solidago-0.1.1/src/solidago/voting_rights/is_trust.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/src/solidago/voting_rights/voting_rights.py` & `solidago-0.1.1/src/solidago/voting_rights/voting_rights.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/tests/test_aggregation.py` & `solidago-0.1.1/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/tests/test_generative_model.py` & `solidago-0.1.1/tests/test_generative_model.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/tests/test_mehestan.py` & `solidago-0.1.1/tests/test_mehestan.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/tests/test_post_process.py` & `solidago-0.1.1/tests/test_post_process.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/tests/test_preference_learning.py` & `solidago-0.1.1/tests/test_preference_learning.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/tests/test_primitives.py` & `solidago-0.1.1/tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/tests/test_privacy_settings.py` & `solidago-0.1.1/tests/test_privacy_settings.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/tests/test_scaling.py` & `solidago-0.1.1/tests/test_scaling.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/tests/test_trust_propagation.py` & `solidago-0.1.1/tests/test_trust_propagation.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/tests/test_user_models.py` & `solidago-0.1.1/tests/test_user_models.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/tests/test_voting_rights.py` & `solidago-0.1.1/tests/test_voting_rights.py`

 * *Files 5% similar despite different names*

```diff
@@ -161,42 +161,55 @@
     trust_scores = np.random.random(size=(n_random_users,))
     min_voting_right = compute_voting_rights_with_params(
         trust_scores, np.ones(shape=n_random_users)
     ).min()
     min_trust_score = trust_scores.min()
     assert min_voting_right > min_trust_score
 
+
 def test_voting_rights_abstraction():
     voting_rights = VotingRights()
     voting_rights[3, 46] = 0.4
     voting_rights[3, 46] *= 2
     assert voting_rights[3, 46] == 0.8
 
 
 def test_affine_overtrust():
     users = pd.DataFrame(dict(trust_score=[0.5, 0.6, 0.0, 0.4, 1]))
     users.index.name = "user_id"
-    vouches = None
+    vouches = pd.DataFrame()
     entities = pd.DataFrame(dict(entity_id=range(6)))
     entities.set_index("entity_id")
-    privacy = PrivacySettings({
-        0: { 0: True, 2: False, 3: False },
-        1: { 1: False, 2: True, 3: False },
-        3: { 0: True, 4: True },
-        5: { 0: False, 1: True }
-    })
-    
+    privacy = PrivacySettings(
+        {
+            0: {0: True, 2: False, 3: False},
+            1: {1: False, 2: True, 3: False},
+            3: {0: True, 4: True},
+            5: {0: False, 1: True},
+        }
+    )
     voting_rights_assignment = AffineOvertrust(
-        privacy_penalty=0.5, 
-        min_overtrust=2.0,
-        overtrust_ratio=0.1
+        privacy_penalty=0.5, min_overtrust=2.0, overtrust_ratio=0.1
     )
     voting_rights, entities = voting_rights_assignment(users, entities, vouches, privacy)
 
+    assert len(entities) == 6  # 6 entities
+    assert list(entities.columns) == [
+        "entity_id",
+        "cumulative_trust",
+        "min_voting_right",
+        "overtrust",
+    ]
+
+    # Voting rights are assigned only on entities where privacy settings are defined.
+    assert voting_rights.entities() == {0, 1, 3, 5}
+
+
 @pytest.mark.parametrize("test", range(4))
 def test_affine_overtrust_test_data(test):
     td = importlib.import_module(f"data.data_{test}")
     voting_rights, entities = td.pipeline.voting_rights(
-        td.users, td.entities, td.vouches, td.privacy)
+        td.users, td.entities, td.vouches, td.privacy
+    )
     for entity in td.voting_rights.entities():
-        for user in td.voting_rights.on_entity(entity):            
+        for user in td.voting_rights.on_entity(entity):
             assert td.voting_rights[user, entity] == voting_rights[user, entity]
```

### Comparing `solidago-0.1.0/tests/data/data_0.py` & `solidago-0.1.1/tests/data/data_0.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/tests/data/data_1.py` & `solidago-0.1.1/tests/data/data_1.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/tests/data/data_2.py` & `solidago-0.1.1/tests/data/data_2.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/tests/data/data_3.py` & `solidago-0.1.1/tests/data/data_3.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/tests/data/data_4.py` & `solidago-0.1.1/tests/data/data_4.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/tests/data/tiny_tournesol.zip` & `solidago-0.1.1/tests/data/tiny_tournesol.zip`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/tests/data/utils.py` & `solidago-0.1.1/tests/data/utils.py`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/LICENSE` & `solidago-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/LICENSE.LESSER` & `solidago-0.1.1/LICENSE.LESSER`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/README.md` & `solidago-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/pyproject.toml` & `solidago-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `solidago-0.1.0/PKG-INFO` & `solidago-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: solidago
-Version: 0.1.0
+Version: 0.1.1
 Summary: Algorithms for Secure Algorithmic Governance
 Project-URL: Homepage, https://github.com/tournesol-app/tournesol/tree/main/solidago
 Project-URL: Bug Tracker, https://github.com/tournesol-app/tournesol/issues
 Author-email: Tournesol Association <hello@tournesol.app>
 License-Expression: LGPL-3.0-or-later
 License-File: LICENSE
 License-File: LICENSE.LESSER
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: solidago Version: 0.1.0 Summary: Algorithms for
+Metadata-Version: 2.3 Name: solidago Version: 0.1.1 Summary: Algorithms for
 Secure Algorithmic Governance Project-URL: Homepage, https://github.com/
 tournesol-app/tournesol/tree/main/solidago Project-URL: Bug Tracker, https://
 github.com/tournesol-app/tournesol/issues Author-email: Tournesol Association
 tournesol.app> License-Expression: LGPL-3.0-or-later License-File: LICENSE
 License-File: LICENSE.LESSER Keywords: collaborative recommendations,comparison
 based,judgement aggregation,mehestan,tournesol Classifier: License :: OSI
 Approved :: GNU Lesser General Public License v3 or later (LGPLv3+) Classifier:
```

