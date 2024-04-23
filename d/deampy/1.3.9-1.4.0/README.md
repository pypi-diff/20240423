# Comparing `tmp/deampy-1.3.9.tar.gz` & `tmp/deampy-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deampy-1.3.9.tar", last modified: Tue Apr  2 18:57:20 2024, max compression
+gzip compressed data, was "deampy-1.4.0.tar", last modified: Tue Apr 23 18:51:33 2024, max compression
```

## Comparing `deampy-1.3.9.tar` & `deampy-1.4.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 18:57:20.529688 deampy-1.3.9/
--rw-rw-rw-   0        0        0     1108 2023-09-20 19:39:29.000000 deampy-1.3.9/LICENSE
--rw-rw-rw-   0        0        0      477 2024-04-02 18:57:20.527694 deampy-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0       59 2023-09-20 19:39:29.000000 deampy-1.3.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 18:57:20.471843 deampy-1.3.9/deampy/
--rw-rw-rw-   0        0        0      262 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/__init__.py
--rw-rw-rw-   0        0        0    22678 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/data_structure.py
--rw-rw-rw-   0        0        0     9513 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/decision_tree.py
--rw-rw-rw-   0        0        0     2096 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/discrete_event_sim.py
--rw-rw-rw-   0        0        0   147709 2023-11-09 17:09:13.000000 deampy-1.3.9/deampy/econ_eval.py
--rw-rw-rw-   0        0        0     5053 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/format_functions.py
--rw-rw-rw-   0        0        0     9288 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/in_out_functions.py
--rw-rw-rw-   0        0        0     9637 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/markov.py
--rw-rw-rw-   0        0        0     1907 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/models.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:57:20.492787 deampy-1.3.9/deampy/optimization/
--rw-rw-rw-   0        0        0        0 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/optimization/__init__.py
--rw-rw-rw-   0        0        0    26227 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/optimization/appx_policy_itr.py
--rw-rw-rw-   0        0        0     1079 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/optimization/learning_exploring_rules.py
--rw-rw-rw-   0        0        0      298 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/optimization/opt_support.py
--rw-rw-rw-   0        0        0     8766 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/optimization/stoch_approx.py
--rw-rw-rw-   0        0        0    21553 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/parameter_estimation.py
--rw-rw-rw-   0        0        0    24387 2023-11-16 03:14:19.000000 deampy-1.3.9/deampy/parameters.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:57:20.511736 deampy-1.3.9/deampy/plots/
--rw-rw-rw-   0        0        0        0 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/plots/__init__.py
--rw-rw-rw-   0        0        0     7501 2023-11-09 17:27:55.000000 deampy-1.3.9/deampy/plots/econ_eval_plots.py
--rw-rw-rw-   0        0        0     1368 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/plots/eff_sample_size.py
--rw-rw-rw-   0        0        0     7019 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/plots/histogram.py
--rw-rw-rw-   0        0        0     2825 2023-10-13 19:50:23.000000 deampy-1.3.9/deampy/plots/plot_support.py
--rw-rw-rw-   0        0        0     6492 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/plots/pop_pyramids.py
--rw-rw-rw-   0        0        0    26140 2023-11-14 02:11:09.000000 deampy-1.3.9/deampy/plots/prob_dists.py
--rw-rw-rw-   0        0        0    10328 2024-01-31 15:50:48.000000 deampy-1.3.9/deampy/plots/sample_paths.py
--rw-rw-rw-   0        0        0    42089 2023-11-14 02:10:47.000000 deampy-1.3.9/deampy/random_variates.py
--rw-rw-rw-   0        0        0    16282 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/regression_models.py
--rw-rw-rw-   0        0        0     9436 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/sample_path.py
--rw-rw-rw-   0        0        0     6676 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/sensitivity_analysis.py
--rw-rw-rw-   0        0        0    47843 2024-04-02 18:56:41.000000 deampy-1.3.9/deampy/statistics.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:57:20.522708 deampy-1.3.9/deampy/support/
--rw-rw-rw-   0        0        0        0 2023-09-20 19:39:30.000000 deampy-1.3.9/deampy/support/__init__.py
--rw-rw-rw-   0        0        0    10009 2023-09-20 19:39:30.000000 deampy-1.3.9/deampy/support/econ_eval_support.py
--rw-rw-rw-   0        0        0      659 2023-09-20 19:39:30.000000 deampy-1.3.9/deampy/support/misc_classes.py
--rw-rw-rw-   0        0        0     7094 2023-09-20 19:39:30.000000 deampy-1.3.9/deampy/support/misc_functions.py
--rw-rw-rw-   0        0        0     6635 2023-09-20 19:39:30.000000 deampy-1.3.9/deampy/support/simulation.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:57:20.525699 deampy-1.3.9/deampy.egg-info/
--rw-rw-rw-   0        0        0      477 2024-04-02 18:57:20.000000 deampy-1.3.9/deampy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1135 2024-04-02 18:57:20.000000 deampy-1.3.9/deampy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 18:57:20.000000 deampy-1.3.9/deampy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-02 18:57:20.000000 deampy-1.3.9/deampy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 18:57:20.000000 deampy-1.3.9/deampy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 18:57:20.529688 deampy-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0      706 2024-04-02 18:56:58.000000 deampy-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:51:33.818045 deampy-1.4.0/
+-rw-rw-rw-   0        0        0     1108 2023-09-20 19:39:29.000000 deampy-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0      477 2024-04-23 18:51:33.816052 deampy-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2023-09-20 19:39:29.000000 deampy-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 18:51:33.742259 deampy-1.4.0/deampy/
+-rw-rw-rw-   0        0        0      262 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/__init__.py
+-rw-rw-rw-   0        0        0    22678 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/data_structure.py
+-rw-rw-rw-   0        0        0     9513 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/decision_tree.py
+-rw-rw-rw-   0        0        0     2096 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/discrete_event_sim.py
+-rw-rw-rw-   0        0        0   147494 2024-04-23 18:50:23.000000 deampy-1.4.0/deampy/econ_eval.py
+-rw-rw-rw-   0        0        0     5053 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/format_functions.py
+-rw-rw-rw-   0        0        0     9288 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/in_out_functions.py
+-rw-rw-rw-   0        0        0     9637 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/markov.py
+-rw-rw-rw-   0        0        0     1907 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/models.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:51:33.767181 deampy-1.4.0/deampy/optimization/
+-rw-rw-rw-   0        0        0        0 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/optimization/__init__.py
+-rw-rw-rw-   0        0        0    26227 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/optimization/appx_policy_itr.py
+-rw-rw-rw-   0        0        0     1079 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/optimization/learning_exploring_rules.py
+-rw-rw-rw-   0        0        0      298 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/optimization/opt_support.py
+-rw-rw-rw-   0        0        0     8766 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/optimization/stoch_approx.py
+-rw-rw-rw-   0        0        0    21553 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/parameter_estimation.py
+-rw-rw-rw-   0        0        0    24387 2023-11-16 03:14:19.000000 deampy-1.4.0/deampy/parameters.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:51:33.795106 deampy-1.4.0/deampy/plots/
+-rw-rw-rw-   0        0        0        0 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/plots/__init__.py
+-rw-rw-rw-   0        0        0     8846 2024-04-23 18:50:23.000000 deampy-1.4.0/deampy/plots/econ_eval_plots.py
+-rw-rw-rw-   0        0        0     1368 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/plots/eff_sample_size.py
+-rw-rw-rw-   0        0        0     7137 2024-04-23 18:50:23.000000 deampy-1.4.0/deampy/plots/histogram.py
+-rw-rw-rw-   0        0        0     4196 2024-04-23 18:50:23.000000 deampy-1.4.0/deampy/plots/plot_support.py
+-rw-rw-rw-   0        0        0     6492 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/plots/pop_pyramids.py
+-rw-rw-rw-   0        0        0    26140 2023-11-14 02:11:09.000000 deampy-1.4.0/deampy/plots/prob_dists.py
+-rw-rw-rw-   0        0        0    10328 2024-01-31 15:50:48.000000 deampy-1.4.0/deampy/plots/sample_paths.py
+-rw-rw-rw-   0        0        0    42089 2023-11-14 02:10:47.000000 deampy-1.4.0/deampy/random_variates.py
+-rw-rw-rw-   0        0        0    16282 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/regression_models.py
+-rw-rw-rw-   0        0        0     9436 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/sample_path.py
+-rw-rw-rw-   0        0        0     6676 2023-09-20 19:39:29.000000 deampy-1.4.0/deampy/sensitivity_analysis.py
+-rw-rw-rw-   0        0        0    48203 2024-04-05 20:32:47.000000 deampy-1.4.0/deampy/statistics.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:51:33.810068 deampy-1.4.0/deampy/support/
+-rw-rw-rw-   0        0        0        0 2023-09-20 19:39:30.000000 deampy-1.4.0/deampy/support/__init__.py
+-rw-rw-rw-   0        0        0    10009 2023-09-20 19:39:30.000000 deampy-1.4.0/deampy/support/econ_eval_support.py
+-rw-rw-rw-   0        0        0      659 2023-09-20 19:39:30.000000 deampy-1.4.0/deampy/support/misc_classes.py
+-rw-rw-rw-   0        0        0     7094 2023-09-20 19:39:30.000000 deampy-1.4.0/deampy/support/misc_functions.py
+-rw-rw-rw-   0        0        0     6635 2023-09-20 19:39:30.000000 deampy-1.4.0/deampy/support/simulation.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:51:33.814056 deampy-1.4.0/deampy.egg-info/
+-rw-rw-rw-   0        0        0      477 2024-04-23 18:51:33.000000 deampy-1.4.0/deampy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1135 2024-04-23 18:51:33.000000 deampy-1.4.0/deampy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 18:51:33.000000 deampy-1.4.0/deampy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-23 18:51:33.000000 deampy-1.4.0/deampy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-23 18:51:33.000000 deampy-1.4.0/deampy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 18:51:33.818045 deampy-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      706 2024-04-23 18:50:42.000000 deampy-1.4.0/setup.py
```

### Comparing `deampy-1.3.9/LICENSE` & `deampy-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/data_structure.py` & `deampy-1.4.0/deampy/data_structure.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/decision_tree.py` & `deampy-1.4.0/deampy/decision_tree.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/discrete_event_sim.py` & `deampy-1.4.0/deampy/discrete_event_sim.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/econ_eval.py` & `deampy-1.4.0/deampy/econ_eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import stat
 import string
 import warnings
 
 import matplotlib.cm as cm
 import matplotlib.pyplot as plt
 import scipy.stats as stat
 # from scipy.stats import pearsonr
@@ -9,15 +10,15 @@
 from numpy import exp, power, average
 from numpy.random import RandomState
 
 import deampy.format_functions as F
 from deampy.in_out_functions import write_csv
 from deampy.plots.econ_eval_plots import add_curves_to_ax, add_min_monte_carlo_samples_to_ax, add_grids
 from deampy.plots.plot_support import output_figure
-from deampy.statistics import SummaryStat
+from deampy.statistics import SummaryStat, RatioOfMeansStatPaired
 from deampy.support.econ_eval_support import *
 from deampy.support.misc_classes import *
 from deampy.support.misc_functions import convert_lnl_to_prob, get_prob_x_greater_than_ys
 
 Params = {
     'plot.legend.fontsize': 7,
     'plot.legend.loc': 'upper left',
@@ -2743,39 +2744,22 @@
             if r1 < 0:
                 return [np.nan, np.nan]
             else:
                 return [r1, r2]
 
         elif method == 'bootstrap' or method == 'Bootstrap':
             # bootstrap algorithm
-            icer_bootstrap_means = np.zeros(num_bootstrap_samples)
-            for i in range(num_bootstrap_samples):
-                # because cost and health observations are paired,
-                # we sample delta cost and delta health together
-                indices = rng.choice(a=range(n_obs),
-                                     size=n_obs,
-                                     replace=True)
-                sampled_delta_costs = self._deltaCosts[indices]
-                sampled_delta_effects = self._deltaEffects[indices]
-
-                ave_delta_cost = np.average(sampled_delta_costs)
-                ave_delta_effect = np.average(sampled_delta_effects)
-
-                # assert all the means should not be 0
-                if ave_delta_effect <= 0:
-                    warnings.warn(
-                        self.name + ': Mean marginal health is 0 or less for one bootstrap sample, '
-                                    'ICER is not computable')
-                    self._isDefined = False
-                    return [math.nan, math.nan]
 
-                icer_bootstrap_means[i] = ave_delta_cost / ave_delta_effect - self._ICER
+            ratio_stat = RatioOfMeansStatPaired(
+                x=self._deltaCosts,
+                y_ref=self._deltaEffects,
+                name='ICER'
+            )
 
-            # return the bootstrap interval
-            return self._ICER - np.percentile(icer_bootstrap_means, [100 * (1 - alpha / 2.0), 100 * alpha / 2.0])
+            return ratio_stat.get_bootstrap_CI(alpha=alpha, num_samples=num_bootstrap_samples)
 
         else:
             raise ValueError('Invalid method. Method should be either bootstrap or Bayesian.')
 
     def get_PI(self, alpha=0.05):
         """
         :param alpha: significance level, a value from [0, 1]
@@ -2788,14 +2772,33 @@
                           "marginal effect is negative or zero.".format(self.name))
             return [math.nan, math.nan]
         else:
             icers = np.divide(self._deltaCosts, self._deltaEffects)
 
         return np.percentile(icers, [100 * alpha / 2.0, 100 * (1 - alpha / 2.0)])
 
+    def get_icer_over_iterations(self):
+        """
+        :return: ICER over iterations
+        """
+        mean_delta_cost = Stat.DiscreteTimeStat(name='Mean Delta Cost')
+        mean_delta_effect = Stat.DiscreteTimeStat(name='Mean Delta Effect')
+        icer_over_iterations = []
+
+        for i in range(len(self._deltaCosts)):
+            mean_delta_cost.record(self._deltaCosts[i])
+            mean_delta_effect.record(self._deltaEffects[i])
+
+            # if ICER so far is defined
+            if mean_delta_effect.get_mean() > 0 and mean_delta_cost.get_mean() >= 0:
+                icer_over_iterations.append(mean_delta_cost.get_mean() / mean_delta_effect.get_mean())
+            else:
+                icer_over_iterations.append(math.nan)
+
+        return icer_over_iterations
 
 class ICER_Indp(_ICER):
 
     def __init__(self, costs_new, effects_new, costs_base, effects_base, health_measure='u', name=''):
         """
         :param costs_new: (list or numpy.array) cost data for the new strategy
         :param effects_new: (list or numpy.array) health data for the new strategy
@@ -2828,15 +2831,15 @@
         :return: confidence interval in the format of list [l, u]
         """
 
         if not self._isDefined:
             return [math.nan, math.nan]
 
         if method == 'Bayesian':
-            raise ValueError('The Bayesian approach is not yet implemented. Use bootsrap instead.')
+            raise ValueError('The Bayesian approach is not yet implemented. Use bootstrap instead.')
 
         # create a new random number generator if one is not provided.
         if rng is None:
             rng = RandomState(seed=1)
 
         # vector to store bootstrap ICERs
         icer_bootstrap_means = np.zeros(num_bootstrap_samples)
```

### Comparing `deampy-1.3.9/deampy/format_functions.py` & `deampy-1.4.0/deampy/format_functions.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/in_out_functions.py` & `deampy-1.4.0/deampy/in_out_functions.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/markov.py` & `deampy-1.4.0/deampy/markov.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/models.py` & `deampy-1.4.0/deampy/models.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/optimization/appx_policy_itr.py` & `deampy-1.4.0/deampy/optimization/appx_policy_itr.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/optimization/learning_exploring_rules.py` & `deampy-1.4.0/deampy/optimization/learning_exploring_rules.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/optimization/stoch_approx.py` & `deampy-1.4.0/deampy/optimization/stoch_approx.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/parameter_estimation.py` & `deampy-1.4.0/deampy/parameter_estimation.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/parameters.py` & `deampy-1.4.0/deampy/parameters.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/plots/econ_eval_plots.py` & `deampy-1.4.0/deampy/plots/econ_eval_plots.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,64 @@
+import matplotlib.pyplot as plt
 import numpy as np
 from scipy.interpolate import interp1d
 
+from deampy.plots.plot_support import output_figure, calculate_ticks, format_axis_tick_labels
+
 
 def format_ax(ax,
               x_range=None, x_delta=None,
-              y_range=None, y_delta=None, if_y_axis_prob=True,
-              if_format_y_numbers=True, y_axis_decimal=1):
+              y_range=None, y_delta=None, if_y_axis_prob=False,
+              x_axis_format_deci=None, y_axis_format_deci=None):
 
     # the range of x and y-axis are set so that we can get the
     # tick values and label
     if y_range is None and if_y_axis_prob:
         ax.set_ylim((-0.01, 1.01))
     if y_range:
         ax.set_ylim(y_range)
     if x_range:
         ax.set_xlim(x_range)
 
     # get x ticks
     if x_delta is None:
         vals_x = ax.get_xticks()
     else:
-        vals_x = []
-        x = x_range[0]
-        while x <= x_range[1]:
-            vals_x.append(x)
-            x += x_delta
+        vals_x = calculate_ticks(interval=x_range, delta=x_delta)
 
     # get y ticks
     if y_delta is None:
         vals_y = ax.get_yticks()
     else:
-        vals_y = []
-        y = y_range[0]
-        while y <= y_range[1]:
-            vals_y.append(y)
-            y += y_delta
+        vals_y = calculate_ticks(interval=y_range, delta=y_delta)
 
     # format x-axis
     ax.set_xticks(vals_x)
-    ax.set_xticklabels(['{:,.{prec}f}'.format(x, prec=0) for x in vals_x])
+    if x_axis_format_deci is None:
+        format_axis_tick_labels(ax=ax, axis='x', format_deci=(',', 0))
+    else:
+        format_axis_tick_labels(ax=ax, axis='x', format_deci=x_axis_format_deci)
 
-    d = 2 * (x_range[1] - x_range[0]) / 200
-    ax.set_xlim([x_range[0] - d, x_range[1] + d])
+    # d = 2 * (x_range[1] - x_range[0]) / 200
+    # ax.set_xlim([x_range[0] - d, x_range[1] + d])
 
     # format y-axis
-    if y_range is None:
-        ax.set_yticks(vals_y)
+    # if y_range is None:
+    ax.set_yticks(vals_y)
     if if_y_axis_prob:
-        ax.set_yticklabels(['{:.{prec}f}'.format(x, prec=1) for x in vals_y])
-    elif if_format_y_numbers:
-        ax.set_yticklabels(['{:,.{prec}f}'.format(x, prec=y_axis_decimal) for x in vals_y])
+        format_axis_tick_labels(ax=ax, axis='y', format_deci=(None, 1))
+    if y_axis_format_deci is not None:
+        format_axis_tick_labels(ax=ax, axis='y', format_deci=y_axis_format_deci)
 
     if y_range is None and if_y_axis_prob:
         ax.set_ylim((-0.01, 1.01))
     if y_range:
         ax.set_ylim(y_range)
+    else:
+        ax.set_ylim([vals_y[0], vals_y[-1]])
 
     if not if_y_axis_prob:
         ax.axhline(y=0, c='k', ls='--', linewidth=0.5)
 
 
 def add_grids(ax, grid_info):
 
@@ -150,16 +150,15 @@
     # grids
     add_grids(ax=ax, grid_info=grid_info)
 
     # do the other formatting
     format_ax(ax=ax, y_range=y_range,
               x_range=x_range, x_delta=x_delta,
               if_y_axis_prob=if_y_axis_prob,
-              if_format_y_numbers=if_format_y_numbers,
-              y_axis_decimal=y_axis_decimal)
+              y_axis_format_deci=[',', y_axis_decimal])
 
 
 def add_min_monte_carlo_samples_to_ax(
         ax, dict_of_ns, epsilons, x_range=None, y_range=None, x_multiplier=1):
 
     colors = ('purple', 'blue', 'green', 'red')
     markers = ('o', 'v', '^', 's')
@@ -206,7 +205,48 @@
     vals_x = ax.get_xticks()
     ax.set_xticklabels(['${:,.{prec}f}'.format(x, prec=0) for x in vals_x])
 
     vals_y = ax.get_yticks()
     ax.set_yticklabels(['{:,.{prec}f}'.format(y, prec=0) for y in vals_y])
 
     ax.legend(fontsize=8)
+
+
+def add_icer_over_itr_to_ax(ax, icer_over_itr, x_range=None, y_range=None, y_delta=None):
+
+    ax.plot(icer_over_itr, 'b-', linewidth=0.5)
+
+    # if y_range:
+    #     ax.set_ylim(y_range)
+    #
+    # if x_range:
+    #     ax.set_xlim(x_range)
+
+    format_ax(ax=ax,
+              x_range=x_range, x_axis_format_deci=(',', 0),
+              y_range=y_range, y_delta=y_delta, y_axis_format_deci=('$', 0))
+    #
+    #
+    # format_axis_tick_labels(ax=ax, axis='x', format_deci=(',', 0))
+    #
+    #
+    # if y_delta is None:
+    #     vals_y = ax.get_yticks()
+    # else:
+    #     vals_y = calculate_ticks(interval=y_range, delta=y_delta)
+    # ax.set_yticks(vals_y)
+    # ax.set_yticklabels(['${:,.0f}'.format(y) for y in vals_y])
+
+
+def plot_icer_over_itrs(icer_over_itr, x_range=None, y_range=None, legend=None, figure_size=None, file_name=None):
+
+    fig, ax = plt.subplots(figsize=figure_size)
+
+    # add icer over iterations
+    add_icer_over_itr_to_ax(ax=ax, icer_over_itr=icer_over_itr, x_range=x_range, y_range=y_range)
+
+    # add legend if provided
+    if legend is not None:
+        ax.legend([legend])
+
+    # output figure
+    output_figure(fig, file_name)
```

### Comparing `deampy-1.3.9/deampy/plots/eff_sample_size.py` & `deampy-1.4.0/deampy/plots/eff_sample_size.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/plots/histogram.py` & `deampy-1.4.0/deampy/plots/histogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
-from deampy.plots.plot_support import output_figure
+from deampy.plots.plot_support import output_figure, format_axis_tick_labels
 
 
 def add_histogram_to_ax(ax, data, title=None, label=None, color=None, bin_width=None,
                         x_label=None, y_label=None, x_range=None, y_range=None,
                         transparency=0.75, format_deci=None,
                         linewidth=0.5, x_delta=None):
     """
@@ -51,23 +51,24 @@
             x += x_delta
         ax.set_xticks(vals_x)
 
     ax.set_xlim(x_range)
     ax.set_ylim(y_range)
 
     if format_deci is not None:
-        vals = ax.get_xticks()
-        if format_deci[0] is None or format_deci[0] == '':
-            ax.set_xticklabels(['{:.{prec}f}'.format(x, prec=format_deci[1]) for x in vals])
-        elif format_deci[0] == ',':
-            ax.set_xticklabels(['{:,.{prec}f}'.format(x, prec=format_deci[1]) for x in vals])
-        elif format_deci[0] == '$':
-            ax.set_xticklabels(['${:,.{prec}f}'.format(x, prec=format_deci[1]) for x in vals])
-        elif format_deci[0] == '%':
-            ax.set_xticklabels(['{:,.{prec}%}'.format(x, prec=format_deci[1]) for x in vals])
+        format_axis_tick_labels(ax=ax, axis='x', format_deci=format_deci)
+        # vals = ax.get_xticks()
+        # if format_deci[0] is None or format_deci[0] == '':
+        #     ax.set_xticklabels(['{:.{prec}f}'.format(x, prec=format_deci[1]) for x in vals])
+        # elif format_deci[0] == ',':
+        #     ax.set_xticklabels(['{:,.{prec}f}'.format(x, prec=format_deci[1]) for x in vals])
+        # elif format_deci[0] == '$':
+        #     ax.set_xticklabels(['${:,.{prec}f}'.format(x, prec=format_deci[1]) for x in vals])
+        # elif format_deci[0] == '%':
+        #     ax.set_xticklabels(['{:,.{prec}%}'.format(x, prec=format_deci[1]) for x in vals])
 
 
 def plot_histogram(data, title=None,
                    x_label=None, y_label=None, bin_width=None, transparency=0.5,
                    x_range=None, y_range=None, figure_size=None,
                    color=None, legend=None, file_name=None):
     """ plot a histogram
```

### Comparing `deampy-1.3.9/deampy/plots/pop_pyramids.py` & `deampy-1.4.0/deampy/plots/pop_pyramids.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/plots/prob_dists.py` & `deampy-1.4.0/deampy/plots/prob_dists.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/plots/sample_paths.py` & `deampy-1.4.0/deampy/plots/sample_paths.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/random_variates.py` & `deampy-1.4.0/deampy/random_variates.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/regression_models.py` & `deampy-1.4.0/deampy/regression_models.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/sample_path.py` & `deampy-1.4.0/deampy/sample_path.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/sensitivity_analysis.py` & `deampy-1.4.0/deampy/sensitivity_analysis.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/statistics.py` & `deampy-1.4.0/deampy/statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -732,14 +732,15 @@
         """
         _ComparativeStat.__init__(self, x, y_ref, name)
 
         self._ifComputable = True  # if any element of the denominator is 0, ratio is not computable
 
 
 class RatioStatPaired(_RatioStat):
+    # E[X/Y] when X and Y are paired
 
     def __init__(self, x, y_ref, name=None):
         """
         :param x: list or numpy.array of first set of observations
         :param y_ref: list or numpy.array of second set of observations
         """
         _RatioStat.__init__(self, x, y_ref, name)
@@ -804,14 +805,15 @@
         if self._ifComputable:
             return self._ratioStat.get_PI(alpha)
         else:
             return [math.nan, math.nan]
 
 
 class RatioOfMeansStatPaired(_RatioStat):
+    # E[X]/E[Y] when X and Y are paired
 
     def __init__(self, x, y_ref, name=None):
         """
         :param x: list or numpy.array of first set of observations
         :param y_ref: list or numpy.array of second set of observations
         """
         _RatioStat.__init__(self, x, y_ref, name)
@@ -875,14 +877,15 @@
         return mean - np.percentile(delta, [100 * (1 - alpha / 2.0), 100 * alpha / 2.0])
 
     def get_PI(self, alpha):
         return [np.nan, np.nan]
 
 
 class RatioStatIndp(_RatioStat):
+    # E[X/Y] when X and Y are independent
 
     def __init__(self, x, y_ref, name=None):
         """
         :param x: list or numpy.array of first set of observations
         :param y_ref: list or numpy.array of second set of observations (reference)
 
         https://en.wikipedia.org/wiki/Ratio_distribution
@@ -1021,14 +1024,15 @@
         if self._ifComputable:
             return self._sum_stat_sample_ratio.get_PI(alpha)
         else:
             return [math.nan, math.nan]
 
 
 class RatioOfMeansStatIndp(_RatioStat):
+    # E[X]/E[Y] when X and Y are independent
 
     def __init__(self, x, y_ref, name=None):
         """
         :param x: list or numpy.array of first set of observations
         :param y_ref: list or numpy.array of second set of observations
         """
         _RatioStat.__init__(self, x, y_ref, name)
@@ -1096,14 +1100,15 @@
         """
         _ComparativeStat.__init__(self, x, y_ref, name)
         self._order = order
         self._ifComputable = True  # if any element of the denominator is 0, ratio is not computable
 
 
 class RelativeDifferencePaired(_RelativeDifference):
+    # E[(X-Y)/Y] when X and Y are paired
 
     def __init__(self, x, y_ref, order=0, name=None):
         """
         :param x: list or numpy.array of first set of observations
         :param y_ref: list or numpy.array of second set of observations
         :param order: set to 0 to calculate (X-Y_ref)/Y_ref and to 1 to calculate (Y_ref-X)/Y_ref
         """
@@ -1177,14 +1182,15 @@
         if self._ifComputable:
             return self._relativeDiffStat.get_PI(alpha)
         else:
             return [math.nan, math.nan]
 
 
 class RelativeDiffOfMeansPaired(_RelativeDifference):
+    # (E[X]-E[Y])/E[Y] when X and Y are paired
 
     def __init__(self, x, y_ref, order=0, name=None):
         """
         :param x: list or numpy.array of first set of observations
         :param y_ref: list or numpy.array of second set of observations
         :param order: set to 0 to calculate (X-Y_ref)/Y_ref and to 1 to calculate (Y_ref-X)/Y_ref
         """
@@ -1225,14 +1231,16 @@
             return [1 - interval[1], 1 - interval[0]]
 
     def get_PI(self, alpha):
         return [np.nan, np.nan]
 
 
 class RelativeDifferenceIndp(_RelativeDifference):
+    # E[(X-Y)/Y] when X and Y are independent
+
     def __init__(self, x, y_ref, order=0, name=None):
         """
         :param x: list or numpy.array of first set of observations
         :param y_ref: list or numpy.array of second set of observations
         :param order: set to 0 to calculate (X-Y_ref)/Y_ref and to 1 to calculate (Y_ref-X)/Y_ref
         """
         _RelativeDifference.__init__(self, x, y_ref, order, name)
@@ -1316,14 +1324,15 @@
         if self._order == 0:
             return [interval[0] - 1, interval[1] - 1]
         else:
             return [1 - interval[1], 1 - interval[0]]
 
 
 class RelativeDiffOfMeansIndp(_RelativeDifference):
+    # (E[X]-E[Y])/E[Y] when X and Y are independent
 
     def __init__(self, x, y_ref, order=0, name=None):
         """
         :param x: list or numpy.array of first set of observations
         :param y_ref: list or numpy.array of second set of observations
         :param order: set to 0 to calculate (X-Y_ref)/Y_ref and to 1 to calculate (Y_ref-X)/Y_ref
         """
```

### Comparing `deampy-1.3.9/deampy/support/econ_eval_support.py` & `deampy-1.4.0/deampy/support/econ_eval_support.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/support/misc_classes.py` & `deampy-1.4.0/deampy/support/misc_classes.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/support/misc_functions.py` & `deampy-1.4.0/deampy/support/misc_functions.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy/support/simulation.py` & `deampy-1.4.0/deampy/support/simulation.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/deampy.egg-info/SOURCES.txt` & `deampy-1.4.0/deampy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deampy-1.3.9/setup.py` & `deampy-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='deampy',
-    version='1.3.9',
+    version='1.4.0',
     install_requires=['numpy', 'matplotlib', 'scipy', 'statsmodels', 'scikit-learn'],
     packages=['deampy', 'deampy.optimization', 'deampy.plots', 'deampy.support'],
     url='https://github.com/modeling-health-care-decisions/deampy',
     license='MIT License',
     author='Reza Yaesoubi',
     author_email='reza.yaesoubi@yale.edu',
     description='Decision analysis in medicine and public health',
```

