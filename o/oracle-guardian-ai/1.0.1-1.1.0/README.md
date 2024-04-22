# Comparing `tmp/oracle_guardian_ai-1.0.1.tar.gz` & `tmp/oracle_guardian_ai-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oracle_guardian_ai-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "oracle_guardian_ai-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `oracle_guardian_ai-1.0.1.tar` & `oracle_guardian_ai-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1859 2023-12-09 00:14:09.157496 oracle_guardian_ai-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     3841 2023-12-09 00:14:09.157496 oracle_guardian_ai-1.0.1/README.md
--rw-r--r--   0        0        0      385 2023-12-09 00:14:09.161496 oracle_guardian_ai-1.0.1/guardian_ai/__init__.py
--rw-r--r--   0        0        0      204 2023-12-09 00:14:09.161496 oracle_guardian_ai-1.0.1/guardian_ai/fairness/__init__.py
--rw-r--r--   0        0        0      331 2023-12-09 00:14:09.161496 oracle_guardian_ai-1.0.1/guardian_ai/fairness/bias_mitigation/__init__.py
--rw-r--r--   0        0        0    51361 2023-12-09 00:14:09.161496 oracle_guardian_ai-1.0.1/guardian_ai/fairness/bias_mitigation/sklearn.py
--rw-r--r--   0        0        0     1958 2023-12-09 00:14:09.161496 oracle_guardian_ai-1.0.1/guardian_ai/fairness/metrics/__init__.py
--rw-r--r--   0        0        0     2225 2023-12-09 00:14:09.161496 oracle_guardian_ai-1.0.1/guardian_ai/fairness/metrics/core.py
--rw-r--r--   0        0        0    20789 2023-12-09 00:14:09.161496 oracle_guardian_ai-1.0.1/guardian_ai/fairness/metrics/dataset.py
--rw-r--r--   0        0        0    57702 2023-12-09 00:14:09.161496 oracle_guardian_ai-1.0.1/guardian_ai/fairness/metrics/model.py
--rw-r--r--   0        0        0    14872 2023-12-09 00:14:09.161496 oracle_guardian_ai-1.0.1/guardian_ai/fairness/metrics/utils.py
--rw-r--r--   0        0        0      262 2023-12-09 00:14:09.161496 oracle_guardian_ai-1.0.1/guardian_ai/fairness/utils/__init__.py
--rw-r--r--   0        0        0     7320 2023-12-09 00:14:09.161496 oracle_guardian_ai-1.0.1/guardian_ai/fairness/utils/lazy_loader.py
--rw-r--r--   0        0        0     2428 2023-12-09 00:14:09.161496 oracle_guardian_ai-1.0.1/guardian_ai/fairness/utils/util.py
--rw-r--r--   0        0        0      204 2023-12-09 00:14:09.161496 oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/__init__.py
--rw-r--r--   0        0        0    25348 2023-12-09 00:14:09.161496 oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/attack.py
--rw-r--r--   0        0        0    12287 2023-12-09 00:14:09.165496 oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/attack_runner.py
--rw-r--r--   0        0        0     7715 2023-12-09 00:14:09.165496 oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/attack_tuner.py
--rw-r--r--   0        0        0     7373 2023-12-09 00:14:09.165496 oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/combined_attacks.py
--rw-r--r--   0        0        0    24848 2023-12-09 00:14:09.165496 oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/dataset.py
--rw-r--r--   0        0        0     6649 2023-12-09 00:14:09.165496 oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/merlin_attack.py
--rw-r--r--   0        0        0     5995 2023-12-09 00:14:09.165496 oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/model.py
--rw-r--r--   0        0        0     7256 2023-12-09 00:14:09.165496 oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/morgan_attack.py
--rw-r--r--   0        0        0     3266 2023-12-09 00:14:09.165496 oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/plot_results.py
--rw-r--r--   0        0        0     2379 2023-12-09 00:14:09.165496 oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/utils.py
--rw-r--r--   0        0        0      114 2023-12-09 00:14:09.165496 oracle_guardian_ai-1.0.1/guardian_ai/requirements-fairness.txt
--rw-r--r--   0        0        0       79 2023-12-09 00:14:09.165496 oracle_guardian_ai-1.0.1/guardian_ai/requirements-privacy.txt
--rw-r--r--   0        0        0      262 2023-12-09 00:14:09.165496 oracle_guardian_ai-1.0.1/guardian_ai/utils/__init__.py
--rw-r--r--   0        0        0     1209 2023-12-09 00:14:09.165496 oracle_guardian_ai-1.0.1/guardian_ai/utils/exception.py
--rw-r--r--   0        0        0     1379 2023-12-09 00:14:09.165496 oracle_guardian_ai-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5205 1970-01-01 00:00:00.000000 oracle_guardian_ai-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1866 2024-04-22 22:02:30.959659 oracle_guardian_ai-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     3839 2024-04-22 22:02:30.959659 oracle_guardian_ai-1.1.0/README.md
+-rw-r--r--   0        0        0      391 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/__init__.py
+-rw-r--r--   0        0        0      333 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/fairness/__init__.py
+-rw-r--r--   0        0        0      337 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/fairness/bias_mitigation/__init__.py
+-rw-r--r--   0        0        0    67479 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/fairness/bias_mitigation/sklearn.py
+-rw-r--r--   0        0        0     2022 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/fairness/metrics/__init__.py
+-rw-r--r--   0        0        0     2231 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/fairness/metrics/core.py
+-rw-r--r--   0        0        0    20733 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/fairness/metrics/dataset.py
+-rw-r--r--   0        0        0    60384 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/fairness/metrics/model.py
+-rw-r--r--   0        0        0    18550 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/fairness/metrics/utils.py
+-rw-r--r--   0        0        0      268 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/fairness/utils/__init__.py
+-rw-r--r--   0        0        0     7326 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/fairness/utils/lazy_loader.py
+-rw-r--r--   0        0        0     1222 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/fairness/utils/util.py
+-rw-r--r--   0        0        0      210 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/__init__.py
+-rw-r--r--   0        0        0    25354 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/attack.py
+-rw-r--r--   0        0        0    12291 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/attack_runner.py
+-rw-r--r--   0        0        0     7721 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/attack_tuner.py
+-rw-r--r--   0        0        0     7379 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/combined_attacks.py
+-rw-r--r--   0        0        0    24854 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/dataset.py
+-rw-r--r--   0        0        0     6655 2024-04-22 22:02:30.963659 oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/merlin_attack.py
+-rw-r--r--   0        0        0     6001 2024-04-22 22:02:30.967659 oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/model.py
+-rw-r--r--   0        0        0     7262 2024-04-22 22:02:30.967659 oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/morgan_attack.py
+-rw-r--r--   0        0        0     3272 2024-04-22 22:02:30.967659 oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/plot_results.py
+-rw-r--r--   0        0        0     2421 2024-04-22 22:02:30.967659 oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/utils.py
+-rw-r--r--   0        0        0      111 2024-04-22 22:02:30.967659 oracle_guardian_ai-1.1.0/guardian_ai/requirements-fairness.txt
+-rw-r--r--   0        0        0       58 2024-04-22 22:02:30.967659 oracle_guardian_ai-1.1.0/guardian_ai/requirements-privacy.txt
+-rw-r--r--   0        0        0      268 2024-04-22 22:02:30.967659 oracle_guardian_ai-1.1.0/guardian_ai/utils/__init__.py
+-rw-r--r--   0        0        0     1215 2024-04-22 22:02:30.967659 oracle_guardian_ai-1.1.0/guardian_ai/utils/exception.py
+-rw-r--r--   0        0        0     1390 2024-04-22 22:02:30.967659 oracle_guardian_ai-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 oracle_guardian_ai-1.1.0/PKG-INFO
```

### Comparing `oracle_guardian_ai-1.0.1/LICENSE.txt` & `oracle_guardian_ai-1.1.0/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023 Oracle and/or its affiliates. All rights reserved.
+Copyright (c) 2023, 2024 Oracle and/or its affiliates. All rights reserved.
 
 The Universal Permissive License (UPL), Version 1.0
 
 Subject to the condition set forth below, permission is hereby granted to any
 person obtaining a copy of this software, associated documentation and/or data
 (collectively the "Software"), free of charge and under any and all copyright
 rights in the Software, and any and all patent rights owned or freely
@@ -28,8 +28,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `oracle_guardian_ai-1.0.1/README.md` & `oracle_guardian_ai-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -77,9 +77,7 @@
 ## Security
 
 Consult the security guide [SECURITY.md](https://github.com/oracle/guardian-ai/blob/main/SECURITY.md) for our responsible security vulnerability disclosure process.
 
 ## License
 
 Copyright (c) 2023 Oracle and/or its affiliates. Licensed under the [Universal Permissive License v1.0](https://oss.oracle.com/licenses/upl/).
-
-
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/fairness/bias_mitigation/sklearn.py` & `oracle_guardian_ai-1.1.0/guardian_ai/fairness/bias_mitigation/sklearn.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 """Sklearn API for bias mitigation"""
 from __future__ import annotations
+import copy
 
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     List,
@@ -19,14 +20,27 @@
     cast,
 )
 
 from guardian_ai.fairness.utils.lazy_loader import LazyLoader
 from guardian_ai.fairness.metrics import _get_fairness_metric, fairness_metrics_dict
 from guardian_ai.utils.exception import GuardianAITypeError, GuardianAIValueError
 from guardian_ai.fairness.utils.util import dyn_docstring, _supported_score_metric
+from guardian_ai.fairness.metrics.utils import (
+    _positive_fairness_names,
+    _automl_to_fairlearn_metric_names,
+)
+from guardian_ai.fairness.metrics.model import (
+    _valid_regression_metrics,
+)
+from guardian_ai.fairness.metrics.utils import (
+    _get_rate_scorer,
+    _inhouse_metrics,
+)
+
+from fairlearn.postprocessing import ThresholdOptimizer
 
 if TYPE_CHECKING:
     import numpy as np
     import optuna
     import pandas as pd
     import plotly.graph_objects as go
     import sklearn.metrics as skl_metrics
@@ -130,15 +144,16 @@
     constraint_value: float, default=0.05
         What value to apply the constraint with when selecting the default
         model. Look at ``constraint_type``'s documentation for more
         details.
     base_estimator_uses_protected_attributes: bool, default=True
         Whether or not ``base_estimator`` uses the protected attributes for
         inference. If set to ``False``, protected attributes will be removed
-        from any input dataset before being collecting predictions from ``base_estimator``.
+        from any input dataset before being collecting predictions from
+        ``base_estimator``.
     n_trials_per_group: int, default=100
         Number of different multiplying scalars to consider. Scales
         linearly with the number of groups in the data, i.e.
         ``n_trials = n_trials_per_group * n_groups``.
         When both ``n_trials_per_group`` and ``time_limit`` are specified,
         the first occurrence will stop the search procedure.
     time_limit: float or None, default=None
@@ -245,14 +260,16 @@
         )
         self._n_trials_per_group = n_trials_per_group
         self._time_limit = time_limit
         self._subsampling = subsampling
         self._regularization_factor = regularization_factor
         self._favorable_label_idx = favorable_label_idx
         self._random_seed = random_seed
+        self._warmstart_grid_resolution = 100
+        self._warmstart = True
 
         self._set_metric_names_and_callables(fairness_metric, accuracy_metric)
 
         # Public attributes to be set by `fit`
         self.tradeoff_summary_: Optional[pd.DataFrame] = None
         self.selected_multipliers_idx_: Optional[int] = None
         self.constrained_metric_: Optional[str] = None
@@ -263,17 +280,98 @@
         self._best_trials_detailed: Optional[pd.DataFrame] = None
         self._accuracy_base_: Optional[float] = None
         self._fairness_base_: Optional[float] = None
         self._unique_groups_: Optional[np.ndarray] = None
         self._unique_group_names_: Optional[list] = None
         self._multiplier_names_: Optional[List[str]] = None
         self._admissible_trials_mask_: Optional[pd.DataFrame] = None
+        self._third_objective = True
+        self._third_objective_name = "levelling_down"
 
         self._validate_current_state()
 
+        # Setup the objective function
+        def objective_fn(trial):
+            probas = self._probas_predicted.copy()
+
+            multipliers = {}
+            for group_name, multiplier_name in zip(
+                self._unique_group_names_, self._multiplier_names_
+            ):
+                min_val, max_val = self._group_ranges[group_name]
+                multipliers[multiplier_name] = trial.suggest_float(
+                    multiplier_name, min_val, max_val, log=True
+                )
+
+            penalty_acc, penalty_fairness = self._get_multiplier_penalty(
+                multipliers, self._group_ranges, self._unique_group_names_
+            )
+
+            probas = _apply_multiplier(
+                probas,
+                self._groups,
+                self._unique_groups_,
+                self._unique_group_names_,
+                multipliers,
+                self._favorable_label_idx,
+            )
+
+            perf = self._get_accuracy_score(self._y, probas)
+            fairness = self._get_fairness_score(self._y, probas, self._groups)
+            if self.fairness_metric_name in _valid_regression_metrics:
+                adjusted_fairness_regressions = []
+                base_fairness_trial = self._regression_metric_trials_["base"]
+                adjusted_fairness_trial = self._get_outcome_rates(
+                    self._y, probas, self._groups
+                )
+                self._regression_metric_trials_[
+                    trial._trial_id
+                ] = adjusted_fairness_trial
+                for (
+                    group_fairness_name,
+                    group_fairness_value,
+                ) in adjusted_fairness_trial.items():
+                    # Cur version: maximize avg_{groups} (min(TPR_group_adjusted - TPR_group_original, 0))
+                    if self.fairness_metric_name in _positive_fairness_names:
+                        adjusted_fairness_regressions.append(
+                            min(
+                                0,
+                                group_fairness_value
+                                - base_fairness_trial[group_fairness_name],
+                            )
+                        )
+                    else:
+                        adjusted_fairness_regressions.append(
+                            min(
+                                0,
+                                base_fairness_trial[group_fairness_name]
+                                - group_fairness_value,
+                            )
+                        )
+
+                avg_adjusted_fairness_regression = sum(
+                    adjusted_fairness_regressions
+                ) / len(adjusted_fairness_regressions)
+                self._avg_fairness_regression_[
+                    trial._trial_id
+                ] = avg_adjusted_fairness_regression
+            if (
+                self.fairness_metric_name in _valid_regression_metrics
+                and self._third_objective
+            ):
+                return (
+                    perf + penalty_acc,
+                    fairness + penalty_fairness,
+                    avg_adjusted_fairness_regression,
+                )
+            else:
+                return perf + penalty_acc, fairness + penalty_fairness
+
+        self._objective_fn = objective_fn
+
     def _validate_current_state(self):
         """
         Validate current attributes have valid values.
 
         Raises
         ------
         GuardianAITypeError
@@ -558,14 +656,46 @@
         if self._accuracy_metric_uses_probas:
             y_pred = y_probas
         else:
             y_pred = y_probas.argmax(-1)
 
         return self.accuracy_metric_callable(y_true, y_pred)
 
+    def _get_outcome_rates(
+        self, y_true: np.ndarray, y_probas: np.ndarray, groups: pd.DataFrame
+    ) -> Dict:
+        """
+        Get raw outcome rate scores.
+
+        Arguments
+        ---------
+        y_true: np.ndarray
+            True labels
+        y_probas: np.ndarray
+            Label probabilities
+        groups: pd.DataFrame
+            Protected attribute(s) value(s) for every sample.
+
+        Returns
+        -------
+        Dict: score
+            The fairness score
+        """
+        if self._fairness_metric_uses_probas:
+            y_pred = y_probas[:, self._favorable_label_idx]
+        else:
+            y_pred = y_probas.argmax(-1)
+
+        outcome_rates = {}
+        for group_name in self._group_masks:
+            mask = self._group_masks[group_name]
+            outcome_rates[group_name] = self._rate_scorer(y_true[mask], y_pred[mask])
+
+        return outcome_rates
+
     def fit(self, X: pd.DataFrame, y: Union[pd.DataFrame, pd.Series, np.ndarray]):
         """
         Apply bias mitigation to the base estimator given a dataset and labels.
 
         Note that it is highly recommended you use a validation set for this
         method, so as to have a more representative range of probabilities
         for the model instead of the potentially skewed probabilities on
@@ -588,86 +718,81 @@
         GuardianAIValueError
             Raised when an invalid value is encountered.
         """
         groups, group_names = self._prepare_subgroups(X)
 
         X, y, group_names, groups = self._apply_subsampling(X, y, group_names, groups)
 
-        probas_predicted = self._get_base_probas(X)
-
-        group_ranges = self._get_group_ranges(
-            probas_predicted, groups, self._unique_groups_, self._unique_group_names_
+        self._probas_predicted = self._get_base_probas(X)
+        self._groups = groups
+        self._X = X
+        self._y = y
+
+        # Includes the original model and, depending on the fairness metrics, additional solutions
+        # obtained by leveling up all groups and from the EO paper.
+        default_multipliers, max_multiplier = self._warmstart_multipliers(
+            X,
+            y,
+            groups,
         )
+        self._default_multipliers = default_multipliers
+        self._max_multiplier = max_multiplier
 
-        self._accuracy_base_ = self._get_accuracy_score(y, probas_predicted)
-        self._fairness_base_ = self._get_fairness_score(y, probas_predicted, groups)
-
-        def objective_fn(trial):
-            probas = probas_predicted.copy()
-
-            multipliers = {}
-            for group_name, multiplier_name in zip(
-                self._unique_group_names_, self._multiplier_names_
-            ):
-                min_val, max_val = group_ranges[group_name]
-                multipliers[multiplier_name] = trial.suggest_float(
-                    multiplier_name, min_val, max_val, log=True
-                )
+        self._group_ranges = self._get_group_ranges(
+            self._probas_predicted,
+            groups,
+            max_multiplier,
+        )
 
-            penalty_acc, penalty_fairness = self._get_multiplier_penalty(
-                multipliers, group_ranges, self._unique_group_names_
-            )
+        self._regression_metric_trials_ = {}
+        self._avg_fairness_regression_ = {}
+        self._accuracy_base_ = self._get_accuracy_score(y, self._probas_predicted)
+        self._fairness_base_ = self._get_fairness_score(
+            y, self._probas_predicted, groups
+        )
 
-            probas = _apply_multiplier(
-                probas,
-                groups,
-                self._unique_groups_,
-                self._unique_group_names_,
-                multipliers,
-                self._favorable_label_idx,
+        if self.fairness_metric_name in _valid_regression_metrics:
+            self._regression_metric_trials_["base"] = self._get_outcome_rates(
+                y, self._probas_predicted, groups
             )
 
-            perf = self._get_accuracy_score(y, probas)
-            fairness = self._get_fairness_score(y, probas, groups)
-
-            return perf + penalty_acc, fairness + penalty_fairness
-
         sampler = optuna.samplers.NSGAIISampler(seed=self._random_seed)
         study = optuna.create_study(
             directions=self._get_optimization_directions(), sampler=sampler
         )
 
         if self._unique_group_names_ is None:
             raise GuardianAIValueError("_unique_group_names cannot be None!")
 
-        study.enqueue_trial(
-            {
-                f"multiplier_{group_name}": 1.0
-                for group_name in self._unique_group_names_
-            }
-        )
+        for multipliers in default_multipliers:
+            study.enqueue_trial(multipliers)
 
+        # Finally, we allow Optuna to use these starting points to search for solutions
+        # that trade-off between these three solutions/objectives.
         study.optimize(
-            objective_fn,
+            self._objective_fn,
             n_trials=self._n_trials_per_group * len(self._unique_group_names_),
             timeout=self._time_limit,
             show_progress_bar=True,
         )
 
-        self._produce_best_trials_frame(study, group_ranges)
+        self._produce_best_trials_frame(study, self._group_ranges)
 
         self._select_best_model_from_constraints()
 
+        # Otherwise the object cannot be pickled
+        self._objective_fn = None
+
         return self
 
     def _prepare_subgroups(self, X: pd.DataFrame) -> Tuple[pd.DataFrame, pd.Series]:
         """
         Handle protected subgroups logic.
 
-        Sets the `_unique_groups`, `_unique_group_names` and `_multiplier_names`
+        Sets the `_unique_groups_`, `_unique_group_names_` and `_multiplier_names_`
         attributes.
 
         Arguments
         ---------
         X: pd.DataFrame
             Dataset to prepare subgroups for.
 
@@ -774,18 +899,17 @@
                 iter(sss.split(np.arange(0, len(X)).reshape(-1, 1), y=stratas))
             )
 
             return X.iloc[idxs], y.iloc[idxs], group_names.iloc[idxs], groups.iloc[idxs]
 
     def _get_group_ranges(
         self,
-        probas: np.ndarray,
+        probas,
         groups: pd.DataFrame,
-        unique_groups: Optional[np.ndarray],
-        unique_group_names: Optional[List],
+        max_multiplier,
     ) -> Dict:
         """
         Return the range for which to search multipliers for each sensitive
         group.
 
         The logic is that if probabilities are constrained to [0.45, 0.55]
         range, we should be looking at multipliers much closer to 1 than if
@@ -804,45 +928,36 @@
 
         Arguments
         ---------
         probas: pd.DataFrame
             The probabilities used to collect group-specific probability ranges.
         groups: pd.DataFrame
             The groups used to separate samples.
-        unique_groups: np.ndarray or None
-            Array of all possible unique groups.
-        unique_group_names: List or None
-            Array of all unique group names.
 
         Returns
         -------
         Dict: group_ranges
             Dictionary mapping every group name to its (min, max) range
             to consider for multipliers.
 
         Raises
         ------
         GuardianAIValueError
             Raised when an invalid value is encountered.
         """
-        if unique_groups is None:
-            raise GuardianAIValueError("unique_groups cannot be None!")
-        if unique_group_names is None:
-            raise GuardianAIValueError("unique_group_names cannot be None!")
-
         group_ranges = {}
 
-        for group, group_name in zip(unique_groups, unique_group_names):
+        for group, group_name in zip(self._unique_groups_, self._unique_group_names_):
             mask = (groups == group).all(1).to_numpy().squeeze()
 
             min_proba = probas[mask].min()
             max_proba = probas[mask].max()
             ratio = max_proba / (min_proba + 1e-6)
 
-            ratio = min(ratio, 10)
+            ratio = min(ratio, max_multiplier)
 
             group_ranges[group_name] = (1 / ratio, ratio)
 
         return group_ranges
 
     def _get_multiplier_penalty(
         self, multipliers: Dict, group_ranges: Dict, unique_group_names: Optional[List]
@@ -890,14 +1005,29 @@
         penalty = self._regularization_factor * np.mean(multiplier_reg_penalty)
 
         penalty_direction_acc = -1 if self._higher_accuracy_is_better else 1
         penalty_direction_fairness = -1 if self._higher_fairness_is_better else 1
 
         return penalty * penalty_direction_acc, penalty * penalty_direction_fairness
 
+    def _get_pareto_efficient_points(self, metrics):
+        """
+        Find the pareto-efficient points
+        :param cometricssts: An (n_points, n_costs) array
+        :return: A (n_points, ) boolean array, indicating whether each point is Pareto efficient
+        """
+        is_efficient = np.ones(metrics.shape[0], dtype=bool)
+        for i, m in enumerate(metrics):
+            if is_efficient[i]:
+                is_efficient[is_efficient] = np.any(
+                    metrics[is_efficient] > m, axis=1
+                )  # Keep any point with a higher cost
+                is_efficient[i] = True  # And keep self
+        return is_efficient
+
     def _produce_best_trials_frame(self, study: optuna.Study, group_ranges: Dict):
         """
         Produce _best_trials_detailed dataframe from optuna Study object.
 
         Arguments
         ---------
         study: optuna.Study
@@ -906,26 +1036,76 @@
             Mapping from group name to group range (min_val, max_val).
 
         Raises
         ------
         GuardianAIValueError
             Raised when an invalid value is encountered.
         """
+        if self._multiplier_names_ is None:
+            raise GuardianAIValueError("_multiplier_names_ cannot be None!")
         regularized_metric_names = [
             f"{metric}_regularized"
             for metric in [self.accuracy_metric_name, self.fairness_metric_name]
         ]
+        metric_names = copy.deepcopy(regularized_metric_names)
+        if (
+            self.fairness_metric_name in _valid_regression_metrics
+            and self._third_objective
+        ):
+            metric_names.append("Third Objective: " + self._third_objective_name)
 
-        if self._multiplier_names_ is None:
-            raise GuardianAIValueError("_multiplier_names_ cannot be None!")
+        if self.fairness_metric_name in _valid_regression_metrics:
+            fairness_trial_names = list(
+                list(self._regression_metric_trials_.items())[0][1].keys()
+            )
+            _prefix = (
+                "PPR"
+                if self.fairness_metric_name == "statistical_parity"
+                else self.fairness_metric_name
+            )
+            fairness_trial_names = [
+                f"{_prefix}_{name}" for name in fairness_trial_names
+            ]
 
-        df = pd.DataFrame(
-            [(*trial.values, *trial.params.values()) for trial in study.best_trials],
-            columns=regularized_metric_names + self._multiplier_names_,
-        )
+            df = pd.DataFrame(
+                [
+                    (
+                        *trial.values,
+                        *trial.params.values(),
+                        *self._regression_metric_trials_[trial._trial_id].values(),
+                    )
+                    for trial in study.best_trials
+                ],
+                columns=metric_names + self._multiplier_names_ + fairness_trial_names,
+            )
+        else:
+            df = pd.DataFrame(
+                [
+                    (*trial.values, *trial.params.values())
+                    for trial in study.best_trials
+                ],
+                columns=regularized_metric_names + self._multiplier_names_,
+            )
+
+        # This is calculated for when objective_fn considers only two metrics:
+        if self.fairness_metric_name in _valid_regression_metrics:
+            avg_fairness_regression_best_trials = []
+            for trial in study.best_trials:
+                avg_fairness_regression_best_trials.append(
+                    self._avg_fairness_regression_[trial._trial_id]
+                )
+            df[self._third_objective_name] = pd.Series(
+                avg_fairness_regression_best_trials
+            ).values
+            df[self._third_objective_name] = (
+                np.sign(df[self._third_objective_name]) * df[self._third_objective_name]
+            )
+            df["Third Objective: " + self._third_objective_name] = df[
+                self._third_objective_name
+            ]
 
         # Unwrap regularization factors
         regularization_factors = np.array(
             [
                 self._get_multiplier_penalty(
                     multipliers, group_ranges, self._unique_group_names_
                 )
@@ -944,28 +1124,64 @@
             df[f"{self.fairness_metric_name}_regularized"]
             - df["regularization_fairness"]
         )
 
         # Remove possible multipliers duplicates
         df = df.drop_duplicates(self._multiplier_names_)
 
+        # Filter pareto front solutions
+        if (
+            self.fairness_metric_name in _valid_regression_metrics
+            and self._third_objective
+        ):
+            pareto_columns = [
+                self.accuracy_metric_name,
+                self.fairness_metric_name,
+                self._third_objective_name,
+            ]
+        else:
+            pareto_columns = [self.accuracy_metric_name, self.fairness_metric_name]
+
+        datapoints = df[pareto_columns].copy()
+        datapoints[self.fairness_metric_name] = -datapoints[self.fairness_metric_name]
+        datapoints = datapoints.to_numpy()
+        df = df.iloc[np.where(self._get_pareto_efficient_points(datapoints))]
+
         # Sort best trials by fairness
         df = df.sort_values(by=self.fairness_metric_name)
 
         # Need to reset index so that it's ordered by fairness
         df = df.reset_index(drop=True)
 
         self._best_trials_detailed = df
         self.tradeoff_summary_ = df.drop(
-            [col for col in df.columns if "regulariz" in col], axis=1
+            [col for col in df.columns if self._should_drop_column(col)],
+            axis=1,
         )
         self.tradeoff_summary_ = self.tradeoff_summary_[
             self.tradeoff_summary_.columns[::-1]
         ]
 
+    def _should_drop_column(self, column: str) -> bool:
+        """Determines if the specified column should be dropped from
+        tradeoff_summary_.
+
+        Arguments
+        ---------
+        column : str
+            The name of the column to check.
+
+        Returns
+        -------
+        bool:
+            True if the column should be dropped, False otherwise.
+        """
+        unwanted_col_keys = ["regulariz", "Third Objective"]
+        return any(unwanted_key in column for unwanted_key in unwanted_col_keys)
+
     def _get_optimization_directions(self) -> List[str]:
         """
         Return optimization direction list used by Optuna to optimize
         fairness-accuracy trade-off.
 
         Returns
         -------
@@ -973,18 +1189,30 @@
             List of str corresponding to optimization directions for the
             two metrics.
         """
 
         def _get_optimization_direction(higher_is_better: Union[bool, str]):
             return "maximize" if higher_is_better else "minimize"
 
-        return [
-            _get_optimization_direction(self._higher_accuracy_is_better),
-            _get_optimization_direction(self._higher_fairness_is_better),
-        ]
+        if (
+            self.fairness_metric_name in _valid_regression_metrics
+            and self._third_objective
+        ):
+            return [
+                _get_optimization_direction(self._higher_accuracy_is_better),
+                _get_optimization_direction(self._higher_fairness_is_better),
+                _get_optimization_direction(
+                    True
+                ),  # higher outcome regression is better
+            ]
+        else:
+            return [
+                _get_optimization_direction(self._higher_accuracy_is_better),
+                _get_optimization_direction(self._higher_fairness_is_better),
+            ]
 
     def _get_base_probas(self, X: pd.DataFrame) -> np.ndarray:
         """
         Get the probabilities from the base estimator on a dataset.
 
         Is in charge of removing the protected attributes if needed.
 
@@ -1137,39 +1365,78 @@
 
         Arguments
         ---------
         hide_inadmissible: bool, default=False
             Whether or not to hide the models that don't satisfy the
             constraint.
         """
+        metric_is_valid = self.fairness_metric_name in _valid_regression_metrics
+        level_down = "levelling_down: %{customdata:.4f}</br>" if metric_is_valid else ""
+
         df = self._best_trials_detailed
 
         if hide_inadmissible:
             df = df[self._admissible_trials_mask_]  # type: ignore
 
         df = df.reset_index()  # type: ignore
 
-        fig = go.Figure()
+        marker = None
+        if metric_is_valid:
+            marker = dict(
+                color=df[self._third_objective_name],
+                symbol=[
+                    "star" if val == 0.0 else "circle"
+                    for val in df[self._third_objective_name]
+                ],
+                colorscale="bluered",
+                colorbar=dict(title="Levelling Down"),
+                showscale=True,
+                cmin=0,
+                cmax=max(
+                    max(df[self._third_objective_name]),
+                    max(df[self.fairness_metric_name]),
+                ),
+            )
 
+        fig = go.Figure()
         fig.add_trace(
             go.Scatter(
                 x=df[self.fairness_metric_name],
                 y=df[self.accuracy_metric_name],
+                customdata=df[self._third_objective_name] if metric_is_valid else None,
                 text=df["index"],
                 line_shape="vh" if self._higher_fairness_is_better else "hv",
-                mode="markers+lines",
+                mode="markers" if metric_is_valid else "markers+lines",
+                marker=marker,
                 hovertemplate=f"{self.fairness_metric_name}"
                 + ": %{x:.4f}"
                 + f"<br>{self.accuracy_metric_name}"
                 + ": %{y:.4f}</br>"
-                + "Index: %{text}",
+                + level_down
+                + "Index: %{text}</br>",
                 name="Multiplier Tuning (Best Models)",
             )
         )
 
+        # dummy traces to show leveling down legend
+        if metric_is_valid:
+            fig.add_trace(
+                go.Scatter(
+                    x=[None],
+                    y=[None],
+                    mode="markers",
+                    marker=dict(
+                        size=10,
+                        color="blue",
+                        symbol="star",
+                    ),
+                    name="No Levelling Down",
+                )
+            )
+
         fig.add_trace(
             go.Scatter(
                 x=[self._fairness_base_],
                 y=[self._accuracy_base_],
                 mode="markers",
                 marker_symbol="cross",
                 marker_color="green",
@@ -1211,14 +1478,15 @@
         fig.update_yaxes(gridwidth=1, gridcolor="LightGrey", zerolinecolor="LightGrey")
 
         fig.update_layout(
             title="Bias Mitigation Best Models Found",
             xaxis_title=self.fairness_metric_name,
             yaxis_title=self.accuracy_metric_name,
             legend_title="Models",
+            legend_orientation="h" if metric_is_valid else "v",
             plot_bgcolor="rgba(0,0,0,0)",
             width=None,
             height=600,
             margin={"t": 50, "b": 50},
         )
 
         fig.show()
@@ -1290,14 +1558,161 @@
         if self._best_trials_detailed is None or self.selected_multipliers_idx_ is None:
             return None
         else:
             return self._best_trials_detailed[self._multiplier_names_].iloc[
                 self.selected_multipliers_idx_
             ]
 
+    def _warmstart_multipliers(self, X, y, groups):
+        default_multipliers = []
+
+        # ----- Multipliers that re-create the original model -----
+        # good accuracy, bad disparity, good regression
+        default_multipliers.append(
+            {
+                f"multiplier_{group_name}": 1.0
+                for group_name in self._unique_group_names_
+            }
+        )
+
+        # Unless we calculate a better bound below, assume that multipliers should
+        # never be larger than 10
+        max_multiplier = 10
+
+        # Get masks for filtering data by each group
+        group_masks = {}
+        for group, group_name in zip(self._unique_groups_, self._unique_group_names_):
+            mask = (groups == group).all(1).to_numpy().squeeze()
+            group_masks[group_name] = mask
+
+        self._group_masks = group_masks
+
+        if self.fairness_metric_name in _inhouse_metrics:
+            # Get a rate calculator/scorer for the given constraint
+            rate_scorer = _get_rate_scorer(self.fairness_metric_name)
+            self._rate_scorer = rate_scorer
+
+        # For some metrics, we can calculate additional defaults
+        if self.fairness_metric_name in _inhouse_metrics and self._warmstart:
+            # Check if metric is supported by fairlearn
+            if self.fairness_metric_name in _automl_to_fairlearn_metric_names:
+                # Fit the EO method as implemented in fairlearn
+                adjusted_model = ThresholdOptimizer(
+                    estimator=self._base_estimator,
+                    constraints=_automl_to_fairlearn_metric_names[
+                        self.fairness_metric_name
+                    ],
+                    objective=(
+                        "accuracy_score"
+                        if self.accuracy_metric_name == "accuracy"
+                        else "balanced_accuracy_score"
+                    ),
+                    prefit=True,
+                )
+                adjusted_model.fit(X, y, sensitive_features=groups)
+
+                # Estimate the target rate value for the given rate
+                adjusted_predictions = adjusted_model.predict(
+                    X, sensitive_features=groups
+                )
+                target_rate = rate_scorer(y, adjusted_predictions)
+
+                # Find multipliers that produce the corresponding target rate as closely as possible for each group
+                multipliers_eo = self._find_multipliers_for_rate(
+                    y,
+                    target_rate,
+                    rate_scorer,
+                    group_masks,
+                )
+
+                default_multipliers.append(multipliers_eo)
+
+            # Do we want to minimize or maximize the given outcome rate?
+            if self.fairness_metric_name in _positive_fairness_names:
+                best = np.max
+            else:
+                best = np.min
+
+            # Calculate the outcome rates for each group
+            predictions = self._probas_predicted.argmax(-1)
+            rates_by_group = []
+            for group_name in self._unique_group_names_:
+                mask = group_masks[group_name]
+                rates_by_group.append(rate_scorer(y[mask], predictions[mask]))
+
+            # Find the group with the best outcome rate
+            target_rate = best(rates_by_group)
+
+            # Find multipliers that produce the corresponding target rate as closely as possible for each group
+            multipliers_or = self._find_multipliers_for_rate(
+                y,
+                target_rate,
+                rate_scorer,
+                group_masks,
+            )
+
+            default_multipliers.append(multipliers_or)
+
+            max_multiplier = max(
+                [m if m > 1 else 1 / m for m in multipliers_or.values()]
+            )
+
+        # Allow to increase/decrease probabilities by a factor of at most 10,
+        # unless larger is required to allow the trivial solution above.
+        max_multiplier = max(max_multiplier, 10)
+
+        return default_multipliers, max_multiplier
+
+    def _find_multipliers_for_rate(self, y, target_rate, rate_scorer, group_masks):
+        multipliers = {}
+
+        for group, group_name, multiplier_name in zip(
+            self._unique_groups_, self._unique_group_names_, self._multiplier_names_
+        ):
+            # Get only the data for this group
+            mask = group_masks[group_name]
+
+            # Unique values of up to grid_resolution quantiles
+            # Always include 0.5 -- the default threshold
+            thresholds = np.unique(
+                list(
+                    np.quantile(
+                        self._probas_predicted[mask],
+                        np.linspace(0, 1, self._warmstart_grid_resolution + 1),
+                        method="nearest",
+                    )
+                )
+                + [0.5]
+            )
+
+            # Ensure the thresholds are in (0, 1) (exclusive)
+            thresholds = thresholds[np.logical_and(thresholds > 0, thresholds < 1)]
+
+            # Calcuate rate for each threshold
+            rates = [
+                rate_scorer(
+                    y[mask],
+                    self._probas_predicted[mask][:, self._favorable_label_idx]
+                    > threshold,
+                )
+                for threshold in thresholds
+            ]
+
+            # Find threshold with closest rate to target rate, break ties towards
+            # thresholds of 0.5 -- i.e., doing nothing
+            ideal_index = np.argmin(
+                (rates - target_rate) ** 2 + np.abs(thresholds - 0.5) * 10**-5
+            )
+            ideal_threshold = thresholds[ideal_index]
+
+            # Closed form solution to convert thresholds to multipliers
+            multipliers[multiplier_name] = (1 - ideal_threshold) / ideal_threshold
+
+        return multipliers
+
 
 def _apply_multiplier(
     probas: np.ndarray,
     groups: pd.DataFrame,
     unique_groups: np.ndarray,
     unique_group_names: pd.DataFrame,
     multipliers: pd.DataFrame,
@@ -1334,14 +1749,17 @@
         multiplier = multipliers[f"multiplier_{group_name}"]
         probas[:, majority_class_idx][mask] *= multiplier
 
     return probas / probas.sum(-1, keepdims=True)
 
 
 class _PredictionReturner:
+    _estimator_type = "classifier"
+    classes_ = np.array([0, 1])
+
     def predict(self, y_pred):
         self.classes_ = np.unique(y_pred)
         return y_pred
 
     def predict_proba(self, y_pred):
         self.classes_ = np.arange(y_pred.shape[1])
         return y_pred
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/fairness/metrics/__init__.py` & `oracle_guardian_ai-1.1.0/guardian_ai/fairness/metrics/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 from guardian_ai.fairness.metrics.core import (
     _get_fairness_metric,
     _get_fairness_scorer,
     fairness_metrics_dict,
     fairness_scorers_dict,
@@ -34,21 +34,22 @@
     false_negative_rate,
     false_omission_rate,
     false_positive_rate,
     model_statistical_parity,
     theil_index,
     true_positive_rate,
 )
-from guardian_ai.fairness.metrics.utils import _FairnessScorer
+from guardian_ai.fairness.metrics.utils import _FairnessScorer, _positive_fairness_names
 
 __all__ = [
     "_get_fairness_scorer",
     "fairness_scorers_dict",
     "_get_fairness_metric",
     "fairness_metrics_dict",
+    "_positive_fairness_names",
     "FairnessMetric",
     "_FairnessScorer",
     "DatasetStatisticalParityScorer",
     "dataset_statistical_parity",
     "ConsistencyScorer",
     "consistency",
     "SmoothedEDFScorer",
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/fairness/metrics/core.py` & `oracle_guardian_ai-1.1.0/guardian_ai/fairness/metrics/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 """Core for fairness metrics"""
 
 from guardian_ai.fairness.metrics.model import (
     EqualizedOddsScorer,
     ErrorRateScorer,
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/fairness/metrics/dataset.py` & `oracle_guardian_ai-1.1.0/guardian_ai/fairness/metrics/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 """Evaluating the compliance of a dataset with specific fairness metrics"""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Callable, List, Optional, Union
 
@@ -33,18 +33,14 @@
 else:
     pd = LazyLoader("pandas")
     np = LazyLoader("numpy")
     BinaryLabelDatasetMetric = LazyLoader(
         "aif360.metrics", "BinaryLabelDatasetMetric", suppress_import_warnings=True
     )
 
-BinaryLabelDatasetMetric = LazyLoader(
-    "aif360.metrics", "BinaryLabelDatasetMetric", suppress_import_warnings=True
-)
-
 
 def _dataset_metric(
     y_true: Union[pd.Series, np.ndarray, List],
     subgroups: pd.DataFrame,
     metric: str,
     distance_measure: Optional[str],
     reduction: Optional[str],
@@ -105,21 +101,25 @@
     visited_subgroup_pairs = set()
     # subgroup_divisions is a list of all subgroup pairs,
     # e.g. [([{'sex': 0, 'race': 0}], [{'sex': 0, 'race': 1}]), ...]
     for unpriv_group, priv_group in subgroup_divisions:
         subgroup_metrics = BinaryLabelDatasetMetric(ds_true, unpriv_group, priv_group)
 
         score, group_repr = _get_score_group_from_metrics(
-            subgroup_metrics, distance, metric, unpriv_group, priv_group, attr_idx_to_vals
+            subgroup_metrics,
+            distance,
+            metric,
+            unpriv_group,
+            priv_group,
+            attr_idx_to_vals,
         )
         if (group_repr[1], group_repr[0]) not in visited_subgroup_pairs:
             scores.append(score)
             groups.append(group_repr)
             visited_subgroup_pairs.add(group_repr)
-
     return reduction(groups, scores)
 
 
 class _DatasetFairnessScorer(_FairnessScorer):
     """
     Common base object for all dataset metrics.
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/fairness/metrics/model.py` & `oracle_guardian_ai-1.1.0/guardian_ai/fairness/metrics/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 """Fairness metrics for evaluating a model"""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable, List, Optional, Union
 
@@ -15,155 +15,214 @@
     DEFAULT_REDUCTION,
     _DistanceMetric,
     _FairnessScorer,
     _get_check_arrays,
     _get_check_distance,
     _get_check_inputs,
     _get_check_reduction,
+    _get_check_reduction_distance_subgroups,
     _get_score_group_from_metrics,
     _place_space_before_capital_letters,
     _y_to_aifm_ds,
+    _get_rate_scorer,
+    _inhouse_metrics,
+    _aif360_to_automl_metric_names,
 )
 from guardian_ai.utils.exception import GuardianAIValueError
 
 if TYPE_CHECKING:
     import numpy as np
     import pandas as pd
     from aif360.metrics import ClassificationMetric
 else:
     np = LazyLoader("numpy")
     pd = LazyLoader("pandas")
     ClassificationMetric = LazyLoader(
         "aif360.metrics", "ClassificationMetric", suppress_import_warnings=True
     )
 
+_valid_regression_metrics = [
+    "TPR",
+    "statistical_parity",
+    "FPR",
+    "FNR",
+    "FOR",
+    "FDR",
+    "error_rate",
+]
+
 
 def _model_metric(
     y_true: Optional[Union[pd.Series, np.ndarray, List]],
     y_pred: Union[pd.Series, np.ndarray, List],
     subgroups: pd.DataFrame,
     metric: str,
     distance_measure: Optional[str],
     reduction: Optional[str],
     allow_y_true_none: bool,
     allow_distance_measure_none: bool,
 ):
     """
-    Compute engine for all model metrics.
+    Compute engine for all group pairs model metrics.
 
-    This computes a given metric on all subgroup pairs for a specified ``subgroups`` input.
+    This computes a given metric on all group pairs for a specified ``subgroups`` input.
 
     Parameters
     ----------
     y_true : pandas.Series, numpy.ndarray, list or None
         Array of groundtruth labels.
     y_pred : pandas.Series, numpy.ndarray, list
         Array of model predictions.
     subgroups : pandas.DataFrame
         Dataframe containing protected attributes for each instance.
     metric : str
         Name of the base metric to be called.
     distance_measure : str or None
         Determines the distance used to compare a subgroup's metric
-        against the rest of the subgroups. Possible values are:
+        against the rest of the population. Possible values are:
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
             Only allowed if `allow_distance_measure_none` is set to True
     reduction : str or None
         Determines how to reduce scores on all subgroups to
         a single output. Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
     allow_y_true_none : bool
         Whether or not to allow `y_true` to be set to ``None``.
     allow_distance_measure_none : bool
         Whether or not to allow ``distance_measure`` to be set
         to ``None``.
 
 
     Returns
     -------
     float, dict
         The computed metric value, with format according to `reduction`.
 
     """
     y_true, y_pred = _get_check_arrays(y_true, y_pred, allow_y_true_none)
-    (
-        reduction,
-        distance,
-        attr_vals_to_idx,
-        attr_idx_to_vals,
-        subgroup_divisions,
-    ) = _get_check_inputs(
-        reduction, distance_measure, subgroups, allow_distance_measure_none
-    )
 
-    ds_pred = _y_to_aifm_ds(y_pred, subgroups, attr_vals_to_idx)
+    if _aif360_to_automl_metric_names[metric] in _inhouse_metrics:
+        # We can calcualte the simple rate-based metrics 1-2 orders of
+        # magnitude faster than AIF360 does for some reason
+        reduction, distance = _get_check_reduction_distance_subgroups(
+            reduction, distance_measure, subgroups, allow_distance_measure_none
+        )
 
-    # Certain metrics like statistical disparity don't use ground truth labels.
-    # AIF360 still needs a labels dataset, so we copy the predicted dataset.
-    if y_true is None:
-        ds_true = ds_pred.copy()
-    else:
-        ds_true = _y_to_aifm_ds(y_true, subgroups, attr_vals_to_idx)
+        rate_scorer = _get_rate_scorer(_aif360_to_automl_metric_names[metric])
 
-    groups = []
-    scores = []
-    visited_subgroup_pairs = set()
-    # subgroup_divisions is a list of all subgroup pairs,
-    # e.g. [([{'sex': 0, 'race': 0}], [{'sex': 0, 'race': 1}]), ...]
-    for unpriv_group, priv_group in subgroup_divisions:
-        subgroup_metrics = ClassificationMetric(
-            ds_true, ds_pred, unpriv_group, priv_group
-        )
+        rates = {}
+        for group, _ in subgroups.groupby(list(subgroups.columns)):
+            mask = (subgroups == group).all(1).to_numpy().squeeze()
+            group = group if len(group) > 1 else group[0]
+            rates[group] = rate_scorer(
+                y_true[mask] if y_true is not None else None,
+                y_pred[mask],
+            )
+
+        groups = []
+        scores = []
+        visited_subgroup_pairs = set()
+        for group1 in sorted(rates):
+            for group2 in sorted(rates):
+                if group1 == group2:
+                    continue
+
+                group_repr = (group1, group2)
+
+                if (group_repr[1], group_repr[0]) not in visited_subgroup_pairs:
+                    score = distance.from_raw_scores(rates[group1], rates[group2])
+                    scores.append(score)
+                    groups.append(group_repr)
+                    visited_subgroup_pairs.add(group_repr)
 
-        score, group_repr = _get_score_group_from_metrics(
-            subgroup_metrics, distance, metric, unpriv_group, priv_group, attr_idx_to_vals
+    else:
+        # We don't support the more complicated metrics to implement
+        # so we rely on AIF360 for them.
+        (
+            reduction,
+            distance,
+            attr_vals_to_idx,
+            attr_idx_to_vals,
+            subgroup_divisions,
+        ) = _get_check_inputs(
+            reduction, distance_measure, subgroups, allow_distance_measure_none
         )
-        if (group_repr[1], group_repr[0]) not in visited_subgroup_pairs:
-            scores.append(score)
-            groups.append(group_repr)
-            visited_subgroup_pairs.add(group_repr)
+
+        ds_pred = _y_to_aifm_ds(y_pred, subgroups, attr_vals_to_idx)
+
+        # Certain metrics like statistical disparity don't use ground truth labels.
+        # AIF360 still needs a labels dataset, so we copy the predicted dataset.
+        if y_true is None:
+            ds_true = ds_pred.copy()
+        else:
+            ds_true = _y_to_aifm_ds(y_true, subgroups, attr_vals_to_idx)
+
+        groups = []
+        scores = []
+        visited_subgroup_pairs = set()
+        # subgroup_divisions is a list of all subgroup pairs,
+        # e.g. [([{'sex': 0, 'race': 0}], [{'sex': 0, 'race': 1}]), ...]
+        for unpriv_group, priv_group in subgroup_divisions:
+            subgroup_metrics = ClassificationMetric(
+                ds_true, ds_pred, unpriv_group, priv_group
+            )
+
+            score, group_repr = _get_score_group_from_metrics(
+                subgroup_metrics,
+                distance,
+                metric,
+                unpriv_group,
+                priv_group,
+                attr_idx_to_vals,
+            )
+            if (group_repr[1], group_repr[0]) not in visited_subgroup_pairs:
+                scores.append(score)
+                groups.append(group_repr)
+                visited_subgroup_pairs.add(group_repr)
 
     return reduction(groups, scores)
 
 
-class _ModelFairnessScorer(_FairnessScorer):
+class _AllGroupPairsModelFairnessScorer(_FairnessScorer):
     """
-    Common base object for all model metrics.
+    Common base object for all group pairs model metrics.
 
-    This stores settings to pass on to the ``_model_metric`` compute
+    This stores settings to pass on to the ``_all_group_pairs_model_metric`` compute
     engine and does subgroups generation from a `protected_attributes` array on
     an input array of instances ``X``.
 
     Parameters
     ----------
     protected_attributes: pandas.Series, numpy.ndarray, list, str
         Array of attributes or single attribute that should be treated as
         protected. If an attribute is protected, then all of its unique
         values are considered as subgroups.
     metric : str or Callable
         Name of the base metric to be called.
     distance_measure : str or None, default='diff'
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
     reduction : str or None, default='mean'
-        Determines how to reduce scores on all subgroup pairs to a single output.
+        Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
     allow_distance_measure_none : bool, default=True
         Whether or not to allow ``distance_measure`` to be set to ``None``.
     """
 
     def __init__(
         self,
@@ -240,29 +299,30 @@
         )
 
         fullname = " ".join(fullname.split())
 
         return _place_space_before_capital_letters(fullname)
 
 
-class ModelStatisticalParityScorer(_ModelFairnessScorer):  # noqa: D412
+class ModelStatisticalParityScorer(_AllGroupPairsModelFairnessScorer):  # noqa: D412
     """
-    Measure the statistical parity [1] of a model's output between all subgroup pairs.
+    Measure the statistical parity [1] of a model's output between subgroups
+    and the rest of the population.
 
     Statistical parity (also known as Base Rate or Disparate Impact) states that
     a predictor is unbiased if the prediction is independent of the protected
     attribute.
 
     Statistical Parity is calculated as PP / N, where PP and N are the number of
     Positive Predictions and total Number of predictions made, respectively.
 
     Perfect score
         A perfect score for this metric means that the model does not predict
         positively any of the subgroups at a different rate than it does for the
-        rest of the subgroups. For example, if the protected attributes are race
+        rest of the population. For example, if the protected attributes are race
         and sex, then a perfect statistical parity would mean that all combinations
         of values for race and sex have identical ratios of positive predictions.
         Perfect values are:
 
         - 1 if using ``'ratio'`` as ``distance_measure``.
         - 0 if using ``'diff'`` as ``distance_measure``.
 
@@ -270,26 +330,28 @@
     ----------
     protected_attributes: pandas.Series, numpy.ndarray, list, str
         Array of attributes or single attribute that should be treated as
         protected. If an attribute is protected, then all of its unique
         values are considered as subgroups.
     distance_measure : str, default='diff'
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
+
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
     reduction : str, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
 
     References
     ----------
     [1] `Cynthia Dwork et al. "Fairness Through Awareness". Innovations in
     Theoretical Computer Science. 2012. <https://arxiv.org/abs/1104.3913>`_
 
@@ -382,40 +444,43 @@
     y_true: Optional[Union[pd.Series, np.ndarray, List]] = None,
     y_pred: Optional[Union[pd.Series, np.ndarray, List]] = None,
     subgroups: Optional[pd.DataFrame] = None,
     distance_measure: str = DEFAULT_DISTANCE,
     reduction: Optional[str] = DEFAULT_REDUCTION,
 ):
     """
-    Measure the statistical parity of a model's output between all subgroup pairs.
+    Measure the statistical parity of a model's output between subgroups
+    and the rest of the population.
 
     For more details, refer to :class:`.ModelStatisticalParityScorer`.
 
     Parameters
     ----------
     y_true : pandas.Series, numpy.ndarray, list or None, default=None
         Array of groundtruth labels.
     y_pred : pandas.Series, numpy.ndarray, list or None, default=None
         Array of model predictions.
     subgroups : pandas.DataFrame or None, default=None
         Dataframe containing protected attributes for each instance.
     distance_measure : str, default='diff'
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
+
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
     reduction : str or None, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
     Returns
     -------
     float, dict
         The computed metric value, with format according to `reduction`.
 
     Raises
@@ -457,31 +522,31 @@
         distance_measure=distance_measure,
         reduction=reduction,
         allow_y_true_none=True,
         allow_distance_measure_none=False,
     )
 
 
-class TruePositiveRateScorer(_ModelFairnessScorer):
+class TruePositiveRateScorer(_AllGroupPairsModelFairnessScorer):
     """
-    Measures the disparity of a model's true positive rate between
-    all subgroup pairs (also known as equal opportunity).
+    Measures the disparity of a model's true positive rate between subgroups
+    and the rest of the population (also known as equal opportunity).
 
     For each subgroup, the disparity is measured by comparing the true positive
-    rate on instances of a subgroup against the rest of the subgroups.
+    rate on instances of a subgroup against the rest of the population.
 
     True Positive Rate [1] (also known as TPR, recall, or sensitivity) is
     calculated as TP / (TP + FN), where TP and FN are the number of true
     positives and false negatives, respectively.
 
 
     Perfect score
         A perfect score for this metric means that the model does not correctly
         predict the positive class for any of the subgroups more often than it
-        does for the rest of the subgroups. For example, if the protected
+        does for the rest of the population. For example, if the protected
         attributes are race and sex, then a perfect true positive rate disparity
         would mean that all combinations of values for race and sex have
         identical true positive rates. Perfect values are:
 
         - 1 if using ``'ratio'`` as ``distance_measure``.
         - 0 if using ``'diff'`` as ``distance_measure``.
 
@@ -489,26 +554,28 @@
     ----------
     protected_attributes: pandas.Series, numpy.ndarray, list, str
         Array of attributes or single attribute that should be treated as
         protected. If an attribute is protected, then all of its unique
         values are considered as subgroups.
     distance_measure : str, default='diff'
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
+
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
     reduction : str or None, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
     References
     ----------
     [1] `Moritz Hardt et al. "Equality of Opportunity in Supervised Learning".
     Advances in Neural Information Processing Systems. 2016.
     <https://arxiv.org/pdf/1610.02413.pdf>`_
 
@@ -540,39 +607,43 @@
     y_true: Union[pd.Series, np.ndarray, List],
     y_pred: Union[pd.Series, np.ndarray, List],
     subgroups: pd.DataFrame,
     distance_measure: str = DEFAULT_DISTANCE,
     reduction: Optional[str] = DEFAULT_REDUCTION,
 ):
     """
-    Measures the disparity of a model's true positive rate between all subgroup pairs.
+    Measures the disparity of a model's true positive rate between subgroups
+    and the rest of the population.
 
     For more details, refer to :class:`.TruePositiveRateScorer`.
 
     Parameters
     ----------
     y_true : pandas.Series, numpy.ndarray, list
         Array of groundtruth labels.
     y_pred : pandas.Series, numpy.ndarray, list
         Array of model predictions.
     subgroups : pandas.DataFrame
         Dataframe containing protected attributes for each instance.
     distance_measure : str, default='diff'
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
+
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
+
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
     reduction : str or None, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
     Returns
     -------
     float, dict
         The computed metric value, with format according to `reduction`.
 
 
@@ -592,29 +663,30 @@
         distance_measure=distance_measure,
         reduction=reduction,
         allow_y_true_none=False,
         allow_distance_measure_none=False,
     )
 
 
-class FalsePositiveRateScorer(_ModelFairnessScorer):
+class FalsePositiveRateScorer(_AllGroupPairsModelFairnessScorer):
     """
-    Measures the disparity of a model's false positive rate between all subgroup pairs.
+    Measures the disparity of a model's false positive rate between subgroups
+    and the rest of the population.
 
     For each subgroup, the disparity is measured by comparing the false
-    positive rate on instances of a subgroup against the rest of the subgroups.
+    positive rate on instances of a subgroup against the rest of the population.
 
     False Positive Rate [1] (also known as FPR or fall-out) is calculated as
     FP / (FP + TN), where FP and TN are the number of false positives and
     true negatives, respectively.
 
     Perfect score
         A perfect score for this metric means that the model does not incorrectly
         predict the positive class for any of the subgroups more often than it
-        does for the rest of the subgroups. For example, if the protected
+        does for the rest of the population. For example, if the protected
         attributes are race and sex, then a perfect false positive rate disparity
         would mean that all combinations of values for race and sex have identical
         false positive rates. Perfect values are:
 
         - 1 if using ``'ratio'`` as ``distance_measure``.
         - 0 if using ``'diff'`` as ``distance_measure``.
 
@@ -622,26 +694,29 @@
     ----------
     protected_attributes: pandas.Series, numpy.ndarray, list, str
         Array of attributes or single attribute that should be treated as
         protected. If an attribute is protected, then all of its unique
         values are considered as subgroups.
     distance_measure : str, default='diff'
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
+
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
     reduction : str or None, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
+
 
     References
     ----------
     [1] `Alexandra Chouldechova. "Fair Prediction with Disparate Impact: A Study
     of Bias in Recidivism Prediction Instruments". Big Data (2016).
     <https://www.liebertpub.com/doi/10.1089/big.2016.0047>`_
 
@@ -673,40 +748,43 @@
     y_true: Union[pd.Series, np.ndarray, List],
     y_pred: Union[pd.Series, np.ndarray, List],
     subgroups: pd.DataFrame,
     distance_measure: str = DEFAULT_DISTANCE,
     reduction: Optional[str] = DEFAULT_REDUCTION,
 ):
     """
-    Measures the disparity of a model's false positive rate between all subgroup pairs.
+    Measures the disparity of a model's false positive rate between subgroups
+    and the rest of the population.
 
     For more details, refer to :class:`.FalsePositiveRateScorer`.
 
     Parameters
     ----------
     y_true : pandas.Series, numpy.ndarray, list
         Array of groundtruth labels.
     y_pred : pandas.Series, numpy.ndarray, list
         Array of model predictions.
     subgroups : pandas.DataFrame
         Dataframe containing protected attributes for each instance.
     distance_measure : str, default='diff'
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
+
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
     reduction : str or None, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
     Returns
     -------
     float, dict
         The computed metric value, with format according to `reduction`.
 
 
@@ -726,29 +804,30 @@
         distance_measure=distance_measure,
         reduction=reduction,
         allow_y_true_none=False,
         allow_distance_measure_none=False,
     )
 
 
-class FalseNegativeRateScorer(_ModelFairnessScorer):
+class FalseNegativeRateScorer(_AllGroupPairsModelFairnessScorer):
     """
-    Measures the disparity of a model's false negative rate between all subgroup pairs.
+    Measures the disparity of a model's false negative rate between subgroups
+    and the rest of the population.
 
     For each subgroup, the disparity is measured by comparing the false
-    negative rate on instances of a subgroup against the rest of the subgroups.
+    negative rate on instances of a subgroup against the rest of the population.
 
     False Negative Rate [1] (also known as FNR or miss rate) is calculated as
     FN / (FN + TP), where FN and TP are the number of false negatives and
     true positives, respectively.
 
     Perfect score
         A perfect score for this metric means that the model does not incorrectly
         predict the negative class for any of the subgroups more often than it
-        does for the rest of the subgroups. For example, if the protected
+        does for the rest of the population. For example, if the protected
         attributes are race and sex, then a perfect false negative rate disparity
         would mean that all combinations of values for race and sex have identical
         false negative rates. Perfect values are:
 
         - 1 if using ``'ratio'`` as ``distance_measure``.
         - 0 if using ``'diff'`` as ``distance_measure``.
 
@@ -756,26 +835,28 @@
     ----------
     protected_attributes: pandas.Series, numpy.ndarray, list, str
         Array of attributes or single attribute that should be treated as
         protected. If an attribute is protected, then all of its unique
         values are considered as subgroups.
     distance_measure : str, default='diff'
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
+
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
     reduction : str or None, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
     References
     ----------
     [1] `Alexandra Chouldechova. "Fair Prediction with Disparate Impact: A Study
     of Bias in Recidivism Prediction Instruments". Big Data (2016).
     <https://www.liebertpub.com/doi/10.1089/big.2016.0047>`_
 
@@ -807,40 +888,43 @@
     y_true: Union[pd.Series, np.ndarray, List],
     y_pred: Union[pd.Series, np.ndarray, List],
     subgroups: pd.DataFrame,
     distance_measure: str = DEFAULT_DISTANCE,
     reduction: Optional[str] = DEFAULT_REDUCTION,
 ):
     """
-    Measures the disparity of a model's false negative rate between all subgroup pairs.
+    Measures the disparity of a model's false negative rate between subgroups
+    and the rest of the population.
 
     For more details, refer to :class:`.FalseNegativeRateScorer`.
 
     Parameters
     ----------
     y_true : pandas.Series, numpy.ndarray, list
         Array of groundtruth labels.
     y_pred : pandas.Series, numpy.ndarray, list
         Array of model predictions.
     subgroups : pandas.DataFrame
         Dataframe containing protected attributes for each instance.
     distance_measure : str, default='diff'
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
+
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
     reduction : str or None, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
     Returns
     -------
     float, dict
         The computed metric value, with format according to `reduction`.
 
 
@@ -860,29 +944,30 @@
         distance_measure=distance_measure,
         reduction=reduction,
         allow_y_true_none=False,
         allow_distance_measure_none=False,
     )
 
 
-class FalseOmissionRateScorer(_ModelFairnessScorer):
+class FalseOmissionRateScorer(_AllGroupPairsModelFairnessScorer):
     """
-    Measures the disparity of a model's false omission rate between all subgroup pairs.
+    Measures the disparity of a model's false omission rate between subgroups
+    and the rest of the population.
 
     For each subgroup, the disparity is measured by comparing the false
-    omission rate on instances of a subgroup against the rest of the subgroups.
+    omission rate on instances of a subgroup against the rest of the population.
 
     False Omission Rate (also known as FOR) is calculated as
     FN / (FN + TN), where FN and TN are the number of false negatives and
     true negatives, respectively.
 
     Perfect score
         A perfect score for this metric means that the model does not make more
         mistakes on the negative class for any of the subgroups more often than it
-        does for the rest of the subgroups. For example, if the protected
+        does for the rest of the population. For example, if the protected
         attributes are race and sex, then a perfect false omission rate disparity
         would mean that all combinations of values for race and sex have identical
         false omission rates. Perfect values are:
 
         - 1 if using ``'ratio'`` as ``distance_measure``.
         - 0 if using ``'diff'`` as ``distance_measure``.
 
@@ -890,26 +975,28 @@
     ----------
     protected_attributes: pandas.Series, numpy.ndarray, list, str
         Array of attributes or single attribute that should be treated as
         protected. If an attribute is protected, then all of its unique
         values are considered as subgroups.
     distance_measure : str, default='diff'
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
+
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
     reduction : str or None, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
     Examples
     --------
     .. code-block:: python
 
         from guardian_ai.fairness.metrics import FalseOmissionRateScorer
         scorer = FalseOmissionRateScorer(['race', 'sex'])
@@ -935,40 +1022,43 @@
     y_true: Union[pd.Series, np.ndarray, List],
     y_pred: Union[pd.Series, np.ndarray, List],
     subgroups: pd.DataFrame,
     distance_measure: str = DEFAULT_DISTANCE,
     reduction: Optional[str] = DEFAULT_REDUCTION,
 ):
     """
-    Measures the disparity of a model's false omission rate between all subgroup pairs.
+    Measures the disparity of a model's false omission rate between subgroups
+    and the rest of the population.
 
     For more details, refer to :class:`.FalseOmissionRateScorer`.
 
     Parameters
     ----------
     y_true : pandas.Series, numpy.ndarray, list
         Array of groundtruth labels.
     y_pred : pandas.Series, numpy.ndarray, list
         Array of model predictions.
     subgroups : pandas.DataFrame
         Dataframe containing protected attributes for each instance.
     distance_measure : str, default='diff'
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
+
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
     reduction : str or None, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
     Returns
     -------
     float, dict
         The computed metric value, with format according to `reduction`.
 
 
@@ -988,30 +1078,31 @@
         distance_measure=distance_measure,
         reduction=reduction,
         allow_y_true_none=False,
         allow_distance_measure_none=False,
     )
 
 
-class FalseDiscoveryRateScorer(_ModelFairnessScorer):
+class FalseDiscoveryRateScorer(_AllGroupPairsModelFairnessScorer):
     """
-    Measures the disparity of a model's false discovery rate between all subgroup pairs.
+    Measures the disparity of a model's false discovery rate between subgroups
+    and the rest of the population.
 
     For each subgroup, the disparity is measured by comparing the false
     discovery rate on instances of a subgroup against the rest of the
-    subgroups.
+    population.
 
     False Discovery Rate (also known as FDR) is calculated as
     FP / (FP + TP), where FP and TP are the number of false positives and
     true positives, respectively.
 
     Perfect score
         A perfect score for this metric means that the model does not make more
         mistakes on the positive class for any of the subgroups more often than it
-        does for the rest of the subgroups. For example, if the protected
+        does for the rest of the population. For example, if the protected
         attributes are race and sex, then a perfect false discovery rate disparity
         would mean that all combinations of values for race and sex have identical
         false discovery rates. Perfect values are:
 
         - 1 if using ``'ratio'`` as ``distance_measure``.
         - 0 if using ``'diff'`` as ``distance_measure``.
 
@@ -1019,26 +1110,28 @@
     ----------
     protected_attributes: pandas.Series, numpy.ndarray, list, str
         Array of attributes or single attribute that should be treated as
         protected. If an attribute is protected, then all of its unique
         values are considered as subgroups.
     distance_measure : str, default='diff'
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
+
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
     reduction : str, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
     Examples
     --------
     .. code-block:: python
 
         from guardian_ai.fairness.metrics import FalseDiscoveryRateScorer
         scorer = FalseDiscoveryRateScorer(['race', 'sex'])
@@ -1064,40 +1157,43 @@
     y_true: Union[pd.Series, np.ndarray, List],
     y_pred: Union[pd.Series, np.ndarray, List],
     subgroups: pd.DataFrame,
     distance_measure: str = DEFAULT_DISTANCE,
     reduction: Optional[str] = DEFAULT_REDUCTION,
 ):
     """
-    Measures the disparity of a model's false discovery rate between all subgroup pairs.
+    Measures the disparity of a model's false discovery rate between subgroups
+    and the rest of the population.
 
     For more details, refer to :class:`.FalseDiscoveryRateScorer`.
 
     Parameters
     ----------
     y_true : pandas.Series, numpy.ndarray, list
         Array of groundtruth labels.
     y_pred : pandas.Series, numpy.ndarray, list
         Array of model predictions.
     subgroups : pandas.DataFrame
         Dataframe containing protected attributes for each instance.
     distance_measure : str, default='diff'
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
+
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
     reduction : str or None, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
     Returns
     -------
     float, dict
         The computed metric value, with format according to `reduction`.
 
 
@@ -1117,30 +1213,31 @@
         distance_measure=distance_measure,
         reduction=reduction,
         allow_y_true_none=False,
         allow_distance_measure_none=False,
     )
 
 
-class ErrorRateScorer(_ModelFairnessScorer):
+class ErrorRateScorer(_AllGroupPairsModelFairnessScorer):
     """
-    Measures the disparity of a model's error rate between all subgroup pairs.
+    Measures the disparity of a model's error rate between subgroups
+    and the rest of the population.
 
     For each subgroup, the disparity is measured by comparing the error rate on
-    instances of a subgroup against the rest of the subgroups.
+    instances of a subgroup against the rest of the population.
 
     Error Rate (also known as inaccuracy) is calculated as
     (FP + FN) / N, where FP and FN are the number of false positives and
     false negatives, respectively, while N is the total Number of
     instances.
 
     Perfect score
         A perfect score for this metric means that the model does not make more
         mistakes for any of the subgroups more often than it
-        does for the rest of the subgroups. For example, if the protected
+        does for the rest of the population. For example, if the protected
         attributes are race and sex, then a perfect error rate disparity would
         mean that all combinations of values for race and sex have identical
         error rates. Perfect values are:
 
         - 1 if using ``'ratio'`` as ``distance_measure``.
         - 0 if using ``'diff'`` as ``distance_measure``.
 
@@ -1148,26 +1245,28 @@
     ----------
     protected_attributes: pandas.Series, numpy.ndarray, list, str
         Array of attributes or single attribute that should be treated as
         protected. If an attribute is protected, then all of its unique
         values are considered as subgroups.
     distance_measure : str, default='diff'
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
+
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
     reduction : str or None, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
     Examples
     --------
     .. code-block:: python
 
         from guardian_ai.fairness.metrics import ErrorRateScorer
         scorer = ErrorRateScorer(['race', 'sex'])
@@ -1193,40 +1292,43 @@
     y_true: Union[pd.Series, np.ndarray, List],
     y_pred: Union[pd.Series, np.ndarray, List],
     subgroups: pd.DataFrame,
     distance_measure: str = DEFAULT_DISTANCE,
     reduction: Optional[str] = DEFAULT_REDUCTION,
 ):
     """
-    Measures the disparity of a model's error rate between all subgroup pairs.
+    Measures the disparity of a model's error rate between subgroups
+    and the rest of the population.
 
     For more details, refer to :class:`.ErrorRateScorer`.
 
     Parameters
     ----------
     y_true : pandas.Series, numpy.ndarray, list
         Array of groundtruth labels.
     y_pred : pandas.Series, numpy.ndarray, list
         Array of model predictions.
     subgroups : pandas.DataFrame
         Dataframe containing protected attributes for each instance.
     distance_measure : str, default='diff'
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
+
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
     reduction : str or None, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
     Returns
     -------
     float, dict
         The computed metric value, with format according to `reduction`.
 
 
@@ -1246,36 +1348,36 @@
         distance_measure=distance_measure,
         reduction=reduction,
         allow_y_true_none=False,
         allow_distance_measure_none=False,
     )
 
 
-class EqualizedOddsScorer(_ModelFairnessScorer):
+class EqualizedOddsScorer(_AllGroupPairsModelFairnessScorer):
     """
     Measures the disparity of a model's true positive and false positive rates
-    between subgroups and the rest of the subgroups.
+    between subgroups and the rest of the population.
 
     The disparity is measured by comparing the true positive and false positive
-    rates on instances of a subgroup against the rest of the subgroups.
+    rates on instances of a subgroup against the rest of the population.
 
     True Positive Rate (also known as TPR, recall, or sensitivity) is
     calculated as TP / (TP + FN), where TP and FN are the number of true
     positives and false negatives, respectively.
 
     False Positive Rate (also known as FPR or fall-out) is calculated as
     FP / (FP + TN), where FP and TN are the number of false positives and
     true negatives, respectively.
 
     Equalized Odds [1] is computed by taking the maximum distance between
-    TPR and FPR for a subgroup against the rest of the subgroups.
+    TPR and FPR for a subgroup against the rest of the population.
 
     Perfect score
         A perfect score for this metric means that the model has the same TPR and
-        FPR when comparing a subgroup to the rest of the subgroups. For example,
+        FPR when comparing a subgroup to the rest of the population. For example,
         if the protected attributes are race and sex, then a perfect
         Equalized Odds disparity would mean that all combinations of values for
         race and sex have identical TPR and FPR. Perfect values are:
 
         - 1 if using ``'ratio'`` as ``distance_measure``.
         - 0 if using ``'diff'`` as ``distance_measure``.
 
@@ -1283,26 +1385,28 @@
     ----------
     protected_attributes: pandas.Series, numpy.ndarray, list, str
         Array of attributes or single attribute that should be treated as
         protected. If an attribute is protected, then all of its unique
         values are considered as subgroups.
     distance_measure : str, default='diff'
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
+
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
     reduction : str or None, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
     References
     ----------
     [1] `Moritz Hardt et al. "Equality of Opportunity in Supervised Learning".
     Advances in Neural Information Processing Systems. 2016.
     <https://arxiv.org/pdf/1610.02413.pdf>`_
 
@@ -1335,40 +1439,42 @@
     y_pred: Union[pd.Series, np.ndarray, List],
     subgroups: pd.DataFrame,
     distance_measure: str = DEFAULT_DISTANCE,
     reduction: Optional[str] = DEFAULT_REDUCTION,
 ):
     """
     Measures the disparity of a model's true positive and false positive rates
-    between subgroups and the rest of the subgroups.
+    between subgroups and the rest of the population.
 
     For more details, refer to :class:`.EqualizedOddsScorer`.
 
     Parameters
     ----------
     y_true : pandas.Series, numpy.ndarray, list
         Array of groundtruth labels.
     y_pred : pandas.Series, numpy.ndarray, list
         Array of model predictions.
     subgroups : pandas.DataFrame
         Dataframe containing protected attributes for each instance.
     distance_measure : str, default='diff'
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
+
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
     reduction : str or None, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
     Returns
     -------
     float, dict
         The computed metric value, with format according to `reduction`.
 
 
@@ -1401,57 +1507,61 @@
             eq_odds[key] = np.nanmax([tpr[key], fpr[key]])
     else:
         eq_odds = np.nanmax([tpr, fpr])
 
     return eq_odds
 
 
-class TheilIndexScorer(_ModelFairnessScorer):
+class TheilIndexScorer(_AllGroupPairsModelFairnessScorer):
     """
     Measures the disparity of a model's predictions according to groundtruth
     labels, as proposed by Speicher et al. [1].
 
     Intuitively, the Theil Index can be thought of as a measure of the
     divergence between a subgroup's different error distributions (i.e. false
-    positives and false negatives) against the rest of the subgroups.
+    positives and false negatives) against the rest of the population.
 
     Perfect score
         The perfect score for this metric is 0, meaning that the model does not
         have a different error distribution for any subgroup when compared to the
-        rest of the subgroups. For example, if the protected attributes are
+        rest of the population. For example, if the protected attributes are
         race and sex, then a perfect Theil Index disparity would mean that all
         combinations of values for race and sex have identical error
         distributions.
 
     Parameters
     ----------
     protected_attributes: pandas.Series, numpy.ndarray, list, str
         Array of attributes or single attribute that should be treated as
         protected. If an attribute is protected, then all of its unique
         values are considered as subgroups.
     distance_measure : str or None, default=None
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
+
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
+
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
     reduction : str or None, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
 
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
     References
     ----------
-    [1] `Speicher, Till, et al. "A unified approach to quantifying algorithmic
-    unfairness: Measuring individual & group unfairness via inequality indices."
-    Proceedings of the 24th ACM SIGKDD international conference on knowledge
-    discovery & data mining. 2018. <https://arxiv.org/abs/1807.00787>`_
+    [1]: `Speicher, Till, et al. "A unified approach to quantifying algorithmic
+         unfairness: Measuring individual & group unfairness via inequality
+         indices." Proceedings of the 24th ACM SIGKDD international conference
+         on knowledge discovery & data mining. 2018.
+         <https://arxiv.org/abs/1807.00787>`_
 
     Examples
     --------
     .. code-block:: python
 
         from guardian_ai.fairness.metrics import TheilIndexScorer
         scorer = TheilIndexScorer(['race', 'sex'])
@@ -1492,43 +1602,44 @@
         Array of groundtruth labels.
     y_pred : pandas.Series, numpy.ndarray, list
         Array of model predictions.
     subgroups : pandas.DataFrame
         Dataframe containing protected attributes for each instance.
     distance_measure : str or None, default=None
         Determines the distance used to compare a subgroup's metric against
-        the rest of the subgroups. Possible values are:
+        the rest of the population. Possible values are:
+            * ``'ratio'``: Uses ``(subgroup_val / rest_of_pop_val)``.
+            Inverted to always be >= 1 if needed.
 
-            * ``'ratio'``: Uses ``(subgroup1_val / subgroup2_val)``. Inverted to always be >= 1 if needed.
-            * ``'diff'``: Uses ``| subgroup1_val - subgroup2_val |``.
+            * ``'diff'``: Uses ``| subgroup_val - rest_of_pop_val |``.
 
     reduction : str or None, default='mean'
         Determines how to reduce scores on all subgroups to a single output.
         Possible values are:
-
             * ``'max'``: Returns the maximal value among all subgroup metrics.
             * ``'mean'``: Returns the mean over all subgroup metrics.
-            * ``None``: Returns a ``{subgroup_pair: subgroup_pair_metric, ...}`` dict.
+            * ``None``: Returns a ``{subgroup: subgroup_metric, ...}`` dict.
 
     Returns
     -------
     float, dict
         The computed metric value, with format according to `reduction`.
 
     Raises
     ------
-    GuardianAIValueError
+    AutoMLxValueError
         If distance_measure values are given to Theil Index.
 
     References
     ----------
     [1]: `Speicher, Till, et al. "A unified approach to quantifying algorithmic
-    unfairness: Measuring individual & group unfairness via inequality indices."
-    Proceedings of the 24th ACM SIGKDD international conference on knowledge
-    discovery & data mining. 2018. <https://arxiv.org/abs/1807.00787>`_
+         unfairness: Measuring individual & group unfairness via inequality
+         indices." Proceedings of the 24th ACM SIGKDD international conference
+         on knowledge discovery & data mining. 2018.
+         <https://arxiv.org/abs/1807.00787>`_
 
     Examples
     --------
     .. code-block:: python
 
         from guardian_ai.fairness.metrics import theil_index
         subgroups = X[['race', 'sex']]
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/fairness/metrics/utils.py` & `oracle_guardian_ai-1.1.0/guardian_ai/fairness/metrics/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 """Utils for computing fairness metrics"""
 from __future__ import annotations
 
 import re
 from abc import ABC, abstractmethod
 from itertools import product
-from collections import defaultdict 
+from collections import defaultdict
 from typing import TYPE_CHECKING, Optional
+from functools import partial
 
 from guardian_ai.fairness.utils.lazy_loader import LazyLoader
 from guardian_ai.utils.exception import GuardianAITypeError, GuardianAIValueError
 
 if TYPE_CHECKING:
     import numpy as np
     import pandas as pd
@@ -177,22 +178,28 @@
     display_name = "Difference"
 
     def __call__(self, metrics_obj, metric):
         score = metrics_obj.difference(metric)
 
         return np.abs(score)
 
+    def from_raw_scores(self, score_priv, score_unpriv):
+        return np.abs(score_priv - score_unpriv)
+
 
 class _RatioDistanceMetric(_DistanceMetric):
     display_name = "Ratio"
 
     def __call__(self, metrics_obj, metric, eps=1e-6):
         score_priv = metric(privileged=True)
         score_unpriv = metric(privileged=False)
 
+        return self.from_raw_scores(score_priv, score_unpriv, eps)
+
+    def from_raw_scores(self, score_priv, score_unpriv, eps=1e-6):
         num = max(score_priv, score_unpriv)
         denum = min(score_priv, score_unpriv)
 
         num_is_zero = np.abs(num) <= eps
         denum_is_zero = np.abs(denum) <= eps
 
         # Handle zero-division by-hand
@@ -301,25 +308,42 @@
 
 def _get_check_inputs(
     reduction: Optional[str],
     distance_measure: Optional[str],
     subgroups: pd.DataFrame,
     allow_distance_measure_none: bool,
 ):
-    reduction = _get_check_reduction(reduction)
-    distance = _get_check_distance(distance_measure, allow_distance_measure_none)
+    reduction, distance = _get_check_reduction_distance_subgroups(
+        reduction,
+        distance_measure,
+        subgroups,
+        allow_distance_measure_none,
+    )
 
-    _check_subgroups(subgroups)
     attr_vals_to_idx, attr_idx_to_vals = _get_attr_idx_mappings(subgroups)
 
     subgroup_divisions = _get_subgroup_divisions(subgroups)
 
     return reduction, distance, attr_vals_to_idx, attr_idx_to_vals, subgroup_divisions
 
 
+def _get_check_reduction_distance_subgroups(
+    reduction: Optional[str],
+    distance_measure: Optional[str],
+    subgroups: pd.DataFrame,
+    allow_distance_measure_none: bool,
+):
+    reduction = _get_check_reduction(reduction)
+    distance = _get_check_distance(distance_measure, allow_distance_measure_none)
+
+    _check_subgroups(subgroups)
+
+    return reduction, distance
+
+
 def _get_score_group_from_metrics(
     subgroup_metrics, distance, metric, unpriv_group, priv_group, attr_idx_to_vals
 ):
     metric_fn = getattr(subgroup_metrics, metric)
     score = distance(subgroup_metrics, metric_fn)
 
     group_repr = tuple()
@@ -453,7 +477,125 @@
 
 def _place_space_before_capital_letters(input_str):
     capital_letter_words = capital_letters_regex.findall(input_str)
 
     capital_letter_words = [word.strip() for word in capital_letter_words]
 
     return " ".join(capital_letter_words)
+
+
+def _TP(y_true, y_pred):
+    return np.sum(np.logical_and(y_pred == 1, y_true == 1))
+
+
+def _FN(y_true, y_pred):
+    return np.sum(np.logical_and(y_pred == 0, y_true == 1))
+
+
+def _FP(y_true, y_pred):
+    return np.sum(np.logical_and(y_pred == 1, y_true == 0))
+
+
+def _TN(y_true, y_pred):
+    return np.sum(np.logical_and(y_pred == 0, y_true == 0))
+
+
+def _get_rate(y_true, y_pred, rate):
+    y_pred = y_pred.astype(int)
+    if y_true is not None:
+        y_true = y_true.astype(int)
+
+    if rate == "statistical_parity":
+        # Positive prediction rate
+        return np.mean(y_pred)
+    elif rate == "error_rate":
+        # Rate of all error types
+        return np.mean(np.array(y_pred) != np.array(y_true))
+    elif rate == "TPR":
+        # Sensitivity, hit rate, recall, or true positive rate
+        TP = _TP(y_true, y_pred)
+        FN = _FN(y_true, y_pred)
+
+        return TP / (TP + FN)
+    elif rate == "TNR":
+        # Specificity or true negative rate
+        FP = _FP(y_true, y_pred)
+        TN = _TN(y_true, y_pred)
+
+        return TN / (TN + FP)
+    elif rate == "PPV":
+        # Precision or positive predictive value
+        TP = _TP(y_true, y_pred)
+        FP = _FP(y_true, y_pred)
+
+        return TP / (TP + FP)
+    elif rate == "NPV":
+        # Negative predictive value
+        FN = _FN(y_true, y_pred)
+        TN = _TN(y_true, y_pred)
+
+        return TN / (TN + FN)
+    elif rate == "FPR":
+        # Fall out or false positive rate
+        FP = _FP(y_true, y_pred)
+        TN = _TN(y_true, y_pred)
+
+        return FP / (FP + TN)
+    elif rate == "FNR":
+        # False negative rate
+        TP = _TP(y_true, y_pred)
+        FN = _FN(y_true, y_pred)
+
+        return FN / (TP + FN)
+    elif rate == "FDR":
+        # False discovery rate
+        TP = _TP(y_true, y_pred)
+        FP = _FP(y_true, y_pred)
+
+        return FP / (TP + FP)
+    elif rate == "FOR":
+        # False ommission rate
+        FN = _FN(y_true, y_pred)
+        TN = _TN(y_true, y_pred)
+
+        return FN / (FN + TN)
+    else:
+        raise GuardianAIValueError(f"Undefined rate {rate}")
+
+
+def _get_rate_scorer(fairness_metric_name):
+    return partial(_get_rate, rate=fairness_metric_name)
+
+
+_positive_fairness_names = ["TPR", "statistical_parity"]
+
+_automl_to_aif360_metric_names = {
+    "statistical_parity": "selection_rate",
+    "TPR": "true_positive_rate",
+    "FPR": "false_positive_rate",
+    "FNR": "false_negative_rate",
+    "FOR": "false_omission_rate",
+    "FDR": "false_discovery_rate",
+    "error_rate": "error_rate",
+    "theil_index": "between_group_theil_index",
+}
+
+_aif360_to_automl_metric_names = dict(
+    (v, k) for k, v in _automl_to_aif360_metric_names.items()
+)
+
+_automl_to_fairlearn_metric_names = {
+    "statistical_parity": "demographic_parity",
+    "TPR": "true_positive_rate_parity",
+    "FPR": "false_positive_rate_parity",
+    "FNR": "false_negative_rate_parity",
+}
+
+_inhouse_metrics = [
+    "statistical_parity",
+    "error_rate",
+    "TPR",
+    "FPR",
+    "FNR",
+    "FOR",
+    "FDR",
+]
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/fairness/utils/lazy_loader.py` & `oracle_guardian_ai-1.1.0/guardian_ai/fairness/utils/lazy_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 """Class to lazily load modules."""
 
 import glob
 import importlib
 import os
 from typing import Dict, List, Optional, cast
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/fairness/utils/util.py` & `oracle_guardian_ai-1.1.0/guardian_ai/fairness/utils/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 """Module containing generic helper classes and functions."""
 from typing import Dict, List
 
 _supported_score_metric: Dict[
     str, List[str]
@@ -25,56 +25,15 @@
         "recall_macro",
         "recall_weighted",
         "recall_samples",
         "precision_micro",
         "precision_macro",
         "precision_weighted",
         "precision_samples",
-    ],
-    # f1/precision/roc_auc is not supported in multiclass
-    "multiclass": [
-        "neg_log_loss",
-        "accuracy",
-        "f1_micro",
-        "f1_macro",
-        "f1_weighted",
-        "f1_samples",
-        "recall_macro",
-        "recall_micro",
-        "recall_weighted",
-        "recall_samples",
-        "precision_micro",
-        "precision_macro",
-        "precision_weighted",
-        "precision_samples",
-    ],
-    "continuous": [
-        "neg_mean_squared_error",
-        "r2",
-        "neg_mean_absolute_error",
-        "neg_mean_squared_log_error",
-        "neg_median_absolute_error",
-    ],
-    "continuous_forecast": [
-        "neg_sym_mean_abs_percent_error",
-        "neg_root_mean_squared_percent_error",
-        "neg_mean_abs_scaled_error",
-        "neg_root_mean_squared_error",
-        "neg_mean_squared_error",
-        "neg_max_absolute_error",
-        "neg_mean_absolute_error",
-        "neg_max_abs_error",
-        "neg_mean_abs_error",
-    ],
-    # metrics starting with 'unsupervised' do not require contamination factor to be provided.
-    "unsupervised": [
-        # "unsupervised_n-1_experts",
-        "unsupervised_unify95",
-        "unsupervised_unify95_log_loss",
-    ],
+    ]
 }
 
 
 def dyn_docstring(*args):  # noqa
     """Decorate a method to replace placeholders in the docstring with
     the decorator args.
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/attack.py` & `oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/attack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 from abc import abstractmethod
 import enum
 
 import numpy as np
 import sklearn.metrics
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/attack_runner.py` & `oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/attack_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
-# Licensed under the Universal Permissive License v 1.0 as shown at
-# https://oss.oracle.com/licenses/upl/
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
+# Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 from guardian_ai.privacy_estimation.dataset import (
     ClassificationDataset,
     TargetModelData,
     AttackModelData,
 )
 from guardian_ai.privacy_estimation.attack import (
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/attack_tuner.py` & `oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/attack_tuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import pandas as pd
 from sklearn.model_selection import GridSearchCV
 from typing import List
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/combined_attacks.py` & `oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/combined_attacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import numpy as np
 from sklearn.base import BaseEstimator
 
 from guardian_ai.privacy_estimation.attack import (
     BlackBoxAttack,
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/dataset.py` & `oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 from abc import abstractmethod
 from enum import Enum
 from typing import List, Dict
 
 import numpy as np
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/merlin_attack.py` & `oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/merlin_attack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import numpy as np
 import scipy.sparse as sp
 from sklearn.base import BaseEstimator
 
 from guardian_ai.privacy_estimation.attack import BlackBoxAttack, AttackType
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/model.py` & `oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import pickle
 from abc import abstractmethod
 
 import sklearn.base as base
 from sklearn.ensemble import GradientBoostingClassifier, RandomForestClassifier
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/morgan_attack.py` & `oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/morgan_attack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import numpy as np
 from sklearn.base import BaseEstimator
 from sklearn.utils.validation import check_is_fitted
 
 from guardian_ai.privacy_estimation.attack import (
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/plot_results.py` & `oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/plot_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 
 import pandas as pd
 import os
 import matplotlib.pyplot as plt
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/privacy_estimation/utils.py` & `oracle_guardian_ai-1.1.0/guardian_ai/privacy_estimation/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import numpy as np
 
-def log_loss(
-    y_true,
-    y_pred,
-    labels=None
-    ):
+
+def log_loss(y_true, y_pred, labels=None):
     """
     Calculates the standard log loss function.
 
     Parameters
     ----------
     y_true : array-like list with correct labels for n_samples samples
     y_pred : array-like of float with shape (n_samples, n_classes) or (n_samples,). These
@@ -27,22 +24,18 @@
     loss: float
         The log loss value
     """
 
     return np.average(loss_vector(y_true, y_pred, labels))
 
 
-def log_loss_vector(
-    y_true,
-    y_pred,
-    labels=None
-):
+def log_loss_vector(y_true, y_pred, labels=None):
     """
-    Return the loss vector that is used to compute log loss. The negative sign from the 
-    standard log loss function is distributed through the vector. To get the log loss value 
+    Return the loss vector that is used to compute log loss. The negative sign from the
+    standard log loss function is distributed through the vector. To get the log loss value
     use the `log_loss` function.
 
     This function is used in place of ``sklearn.metrics.log_loss`` because calculations
     need access the loss vector itself and not just the final log loss value.
 
     Parameters
     ----------
@@ -51,15 +44,15 @@
         are the predicted probabilities
     labels : array-like, default=None
         If None, the labels are inferred from ``y_true``
 
     Returns
     -------
     loss vector: np.array
-        The cross entropy loss for each sample. 
+        The cross entropy loss for each sample.
     """
 
     n_samples = len(y_true)
 
     # Preliminary checks
     if labels is not None:
         if set(y_true) != set(labels):
@@ -71,11 +64,16 @@
         raise ValueError("y_pred is not well formed")
 
     spos_dict = dict(zip(labels, range(len(labels))))
 
     # Calculate loss vector
     loss_vector = []
     for i, sample in enumerate(y_true):
-        sample_loss = np.sum([-int(j==spos_dict[sample]) * np.log(y_pred[i][j]) for j in range(len(labels))])
+        sample_loss = np.sum(
+            [
+                -int(j == spos_dict[sample]) * np.log(y_pred[i][j])
+                for j in range(len(labels))
+            ]
+        )
         loss_vector.append(sample_loss)
 
     return np.array(loss_vector)
```

### Comparing `oracle_guardian_ai-1.0.1/guardian_ai/utils/exception.py` & `oracle_guardian_ai-1.1.0/guardian_ai/utils/exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2023 Oracle and/or its affiliates.
+# Copyright (c) 2023, 2024 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 """Exception module."""
 
 
 class GuardianAIError(Exception):
     """GuardianAIError
```

### Comparing `oracle_guardian_ai-1.0.1/pyproject.toml` & `oracle_guardian_ai-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit-core >= 3.8", "setuptools < 60.0",]
 build-backend = "flit_core.buildapi"
 
 
 [project]
 name = "oracle-guardian-ai"
-version = "1.0.1"
+version = "1.1.0"
 description = "Oracle Guardian AI Open Source Project"
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 authors = [
   {name = "Oracle Data Science"}
 ]
@@ -27,28 +27,29 @@
   "License :: OSI Approved :: Universal Permissive License (UPL)",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
-    "numpy==1.22.2",
-    "pandas==1.4.1",
-    "scikit-learn==1.1.1",
+    "numpy",
+    "pandas",
+    "scikit-learn==1.3.2",
 ]
 
 [project.optional-dependencies]
 fairness = [
     "aif360==0.5.0",
     "category-encoders==2.5.0",
     "optuna==3.2.0",
     "plotly==5.4.0",
+    "fairlearn==0.10.0",
 ]
 privacy = [
-    "scipy==1.8.1",
+    "scipy==1.10.0",
     "matplotlib==3.5.3",
 ]
 all-optional = [
     "oracle-guardian-ai[fairness, privacy]",
 ]
 
 [project.urls]
```

### Comparing `oracle_guardian_ai-1.0.1/PKG-INFO` & `oracle_guardian_ai-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: oracle-guardian-ai
-Version: 1.0.1
+Version: 1.1.0
 Summary: Oracle Guardian AI Open Source Project
 Keywords: Oracle Cloud Infrastructure,OCI,Fairness,Bias,Privacy,AI
 Author: Oracle Data Science
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Universal Permissive License (UPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: numpy==1.22.2
-Requires-Dist: pandas==1.4.1
-Requires-Dist: scikit-learn==1.1.1
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: scikit-learn==1.3.2
 Requires-Dist: oracle-guardian-ai[fairness, privacy] ; extra == "all-optional"
 Requires-Dist: aif360==0.5.0 ; extra == "fairness"
 Requires-Dist: category-encoders==2.5.0 ; extra == "fairness"
 Requires-Dist: optuna==3.2.0 ; extra == "fairness"
 Requires-Dist: plotly==5.4.0 ; extra == "fairness"
-Requires-Dist: scipy==1.8.1 ; extra == "privacy"
+Requires-Dist: fairlearn==0.10.0 ; extra == "fairness"
+Requires-Dist: scipy==1.10.0 ; extra == "privacy"
 Requires-Dist: matplotlib==3.5.3 ; extra == "privacy"
 Project-URL: Documentation, https://oralce-guardian-ai.readthedocs.io/en/latest/index.html
 Project-URL: Repository, https://github.com/oracle/guardian-ai
 Provides-Extra: all-optional
 Provides-Extra: fairness
 Provides-Extra: privacy
 
@@ -109,9 +110,7 @@
 
 Consult the security guide [SECURITY.md](https://github.com/oracle/guardian-ai/blob/main/SECURITY.md) for our responsible security vulnerability disclosure process.
 
 ## License
 
 Copyright (c) 2023 Oracle and/or its affiliates. Licensed under the [Universal Permissive License v1.0](https://oss.oracle.com/licenses/upl/).
 
-
-
```

