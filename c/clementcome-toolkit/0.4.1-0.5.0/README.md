# Comparing `tmp/clementcome_toolkit-0.4.1.tar.gz` & `tmp/clementcome_toolkit-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clementcome_toolkit-0.4.1.tar", max compression
+gzip compressed data, was "clementcome_toolkit-0.5.0.tar", max compression
```

## Comparing `clementcome_toolkit-0.4.1.tar` & `clementcome_toolkit-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0      263 2024-03-25 16:14:02.498436 clementcome_toolkit-0.4.1/README.md
--rw-r--r--   0        0        0        0 2024-03-25 16:14:02.498436 clementcome_toolkit-0.4.1/cc_tk/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 16:14:02.498436 clementcome_toolkit-0.4.1/cc_tk/feature/__init__.py
--rw-r--r--   0        0        0    19087 2024-03-25 16:14:02.498436 clementcome_toolkit-0.4.1/cc_tk/feature/correlation.py
--rw-r--r--   0        0        0        0 2024-03-25 16:14:02.498436 clementcome_toolkit-0.4.1/cc_tk/plot/__init__.py
--rw-r--r--   0        0        0     3405 2024-03-25 16:14:02.498436 clementcome_toolkit-0.4.1/cc_tk/plot/classification.py
--rw-r--r--   0        0        0      355 2024-03-25 16:14:02.498436 clementcome_toolkit-0.4.1/cc_tk/relationship/__init__.py
--rw-r--r--   0        0        0     3909 2024-03-25 16:14:02.498436 clementcome_toolkit-0.4.1/cc_tk/relationship/distribution.py
--rw-r--r--   0        0        0     4307 2024-03-25 16:14:02.498436 clementcome_toolkit-0.4.1/cc_tk/relationship/schema.py
--rw-r--r--   0        0        0     8634 2024-03-25 16:14:02.498436 clementcome_toolkit-0.4.1/cc_tk/relationship/significance.py
--rw-r--r--   0        0        0     6980 2024-03-25 16:14:02.498436 clementcome_toolkit-0.4.1/cc_tk/relationship/summary.py
--rw-r--r--   0        0        0     2290 2024-03-25 16:14:02.498436 clementcome_toolkit-0.4.1/cc_tk/relationship/utils.py
--rw-r--r--   0        0        0        0 2024-03-25 16:14:02.498436 clementcome_toolkit-0.4.1/cc_tk/util/__init__.py
--rw-r--r--   0        0        0      213 2024-03-25 16:14:02.498436 clementcome_toolkit-0.4.1/cc_tk/util/types.py
--rw-r--r--   0        0        0     1631 2024-03-25 16:14:02.502436 clementcome_toolkit-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 clementcome_toolkit-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1164 2024-04-23 15:03:18.317690 clementcome_toolkit-0.5.0/README.md
+-rw-r--r--   0        0        0       32 2024-04-23 15:03:18.317690 clementcome_toolkit-0.5.0/cc_tk/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-23 15:03:18.317690 clementcome_toolkit-0.5.0/cc_tk/feature/__init__.py
+-rw-r--r--   0        0        0    19567 2024-04-23 15:03:18.317690 clementcome_toolkit-0.5.0/cc_tk/feature/correlation.py
+-rw-r--r--   0        0        0       32 2024-04-23 15:03:18.317690 clementcome_toolkit-0.5.0/cc_tk/plot/__init__.py
+-rw-r--r--   0        0        0     3401 2024-04-23 15:03:18.317690 clementcome_toolkit-0.5.0/cc_tk/plot/classification.py
+-rw-r--r--   0        0        0      235 2024-04-23 15:03:18.317690 clementcome_toolkit-0.5.0/cc_tk/relationship/__init__.py
+-rw-r--r--   0        0        0     3912 2024-04-23 15:03:18.317690 clementcome_toolkit-0.5.0/cc_tk/relationship/distribution.py
+-rw-r--r--   0        0        0     4993 2024-04-23 15:03:18.317690 clementcome_toolkit-0.5.0/cc_tk/relationship/schema.py
+-rw-r--r--   0        0        0     3744 2024-04-23 15:03:18.317690 clementcome_toolkit-0.5.0/cc_tk/relationship/significance/__init__.py
+-rw-r--r--   0        0        0     6549 2024-04-23 15:03:18.317690 clementcome_toolkit-0.5.0/cc_tk/relationship/significance/base.py
+-rw-r--r--   0        0        0     8567 2024-04-23 15:03:18.317690 clementcome_toolkit-0.5.0/cc_tk/relationship/significance/predictiveness.py
+-rw-r--r--   0        0        0     8733 2024-04-23 15:03:18.317690 clementcome_toolkit-0.5.0/cc_tk/relationship/significance/statistical.py
+-rw-r--r--   0        0        0     8596 2024-04-23 15:03:18.317690 clementcome_toolkit-0.5.0/cc_tk/relationship/summary.py
+-rw-r--r--   0        0        0     2582 2024-04-23 15:03:18.317690 clementcome_toolkit-0.5.0/cc_tk/relationship/utils.py
+-rw-r--r--   0        0        0       47 2024-04-23 15:03:18.317690 clementcome_toolkit-0.5.0/cc_tk/util/__init__.py
+-rw-r--r--   0        0        0      213 2024-04-23 15:03:18.317690 clementcome_toolkit-0.5.0/cc_tk/util/types.py
+-rw-r--r--   0        0        0     1835 2024-04-23 15:03:18.321689 clementcome_toolkit-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1965 1970-01-01 00:00:00.000000 clementcome_toolkit-0.5.0/PKG-INFO
```

### Comparing `clementcome_toolkit-0.4.1/cc_tk/feature/correlation.py` & `clementcome_toolkit-0.5.0/cc_tk/feature/correlation.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,42 +16,50 @@
 from cc_tk.util.types import ArrayLike1D, ArrayLike2D
 
 logger = logging.getLogger(__name__)
 
 
 # pylint: disable=W0201
 class CorrelationToTarget(BaseEstimator, TransformerMixin):
-    """
-    Select columns with correlation to target above a threshold.
+    """Select columns with correlation to target above a threshold.
 
     Parameters
     ----------
     threshold : float, optional
         The threshold for the correlation to the target.
         Default is 0.1.
+
     """
 
     def __init__(self, threshold: float = 0.1) -> None:
+        """Initialize the transformer.
+
+        Parameters
+        ----------
+        threshold : float, optional
+            The threshold for the correlation to the target, by default 0.1.
+
+        """
         super().__init__()
         self.threshold = threshold
 
     def fit(
         self,
         features: ArrayLike2D,
         y: ArrayLike1D,
     ) -> "CorrelationToTarget":
-        """
-        Fit the transformer to the data.
+        """Fit the transformer to the data.
 
         Parameters
         ----------
         features : ArrayLike2D
             The features.
         y : ArrayLike1D
             The target.
+
         """
         features_, y = check_X_y(features, y, y_numeric=True)
         self.n_features_in_ = features_.shape[1]
         self._corr = np.corrcoef(features_.T, y)[-1, :-1]
         self.mask_selection_ = abs(self._corr) > self.threshold
         if self.mask_selection_.sum() == 0:
             logger.warning(
@@ -86,16 +94,17 @@
         -------
         ArrayLike2D
             The selected features.
 
         Raises
         ------
         ValueError
-            If the number of columns in features is different from the number of
-            columns in the training data.
+            If the number of columns in features is different from the number
+            of columns in the training data.
+
         """
         check_is_fitted(self, ["mask_selection_", "n_features_in_"])
         features = check_array(features)
         if features.shape[1] != self.n_features_in_:
             raise ValueError(
                 "Shape of input is different from what was seen in `fit`"
             )
@@ -132,57 +141,66 @@
         )
         ax.set_xlabel("Correlation to target")
         ax.legend().remove()
 
 
 # pylint: disable=W0201
 class ClusteringCorrelation(BaseEstimator, TransformerMixin):
-    """Scikit-learn like estimator to deal with group of correlated features."""
+    """Feature selector based on Clustering of correlations."""
 
     def __init__(
         self,
         threshold: float = 0.1,
         summary_method: Literal["first", "pca"] = "first",
         n_variables_by_cluster: int = 1,
     ) -> None:
-        """
-        Initialize the Feature selector based on Clustering of correlations
-        https://kobia.fr/automatiser-la-reduction-des-correlations-par-clustering/
+        """Initialize the Feature selector based on Clustering of correlations.
 
         Parameters
         ----------
         threshold : float, optional
             Correlation threshold to consider that a group of variables
             are all correlated together, by default 0.1
             0.1 means that all variables in the same cluster have a correlation
             of less than 0.1
         summary_method : str, optional
-            Method to summarize each cluster of variables, implemented methods are:
+            Method to summarize each cluster of variables,
+            implemented methods are:
             - "first" = keep only first variable
-            - "pca" = performs principal component analysis to keep only the first
-                component
+            - "pca" = performs principal component analysis to keep only the
+                first component
             , by default "first"
         n_variables_by_cluster : int, optional
             Number of variables to extract by cluster, by default 1
+
+        Notes
+        -----
+        See https://kobia.fr/automatiser-la-reduction-des-correlations-par-clustering/
+        for more details.
+
         """
         self.threshold = threshold
-        assert summary_method in ["first", "pca"]
+        if summary_method not in ["first", "pca"]:
+            raise ValueError(
+                "summary_method should be either 'first' or 'pca', "
+                f"got {summary_method}"
+            )
         self.summary_method = summary_method
         self.n_variables_by_cluster = n_variables_by_cluster
 
     def fit(self, features: pd.DataFrame, y: pd.Series = None):
-        """
-        Fit the feature selection to features
+        """Fit the feature selection to features.
 
         Parameters
         ----------
         features : pd.DataFrame
             Features to fit the feature selection to
         y : pd.Series, optional
             Target, by default None
+
         """
         features_, y = check_X_y(features, y, ensure_min_features=2)
         self.n_features_in_ = features_.shape[1]
         if isinstance(features, pd.DataFrame):
             self._columns = features.columns
         else:
             self._columns = np.arange(features_.shape[1])
@@ -232,29 +250,28 @@
 
         return self
 
     # pylint: disable=W0613
     def transform(
         self, features: pd.DataFrame, y: pd.Series = None
     ) -> pd.DataFrame:
-        """
-        Apply feature selection to DataFrame features and return the
-        transformed variables
+        """Transform the features with the feature selection.
 
         Parameters
         ----------
         features : pd.DataFrame
             Features
         y : pd.Series, optional
             Target, by default None
 
         Returns
         -------
         pd.DataFrame
             Transformed features with feature selection
+
         """
         features_ = check_array(features)
         check_is_fitted(self, ["clusters_col_", "n_features_in_"])
         if features_.shape[1] != self.n_features_in_:
             raise ValueError(
                 "Shape of input is different from what was seen in `fit`"
             )
@@ -263,20 +280,23 @@
             return features_[:, self.mask_selection_]
         if self.summary_method == "pca":
             check_is_fitted(self, ["pca_by_cluster_"])
             features_by_cluster = []
             for pca, cluster, pca_output_columns in zip(
                 self.pca_by_cluster_, self.clusters_col_, self._output_columns
             ):
-                assert all(
+                if not all(
                     map(
                         lambda value: str(value) in pca_output_columns[0],
                         cluster,
                     )
-                )
+                ):
+                    raise ValueError(
+                        f"Columns {cluster} are not in the PCA output columns"
+                    )
                 pca_output = pca.transform(
                     features_[:, np.isin(self._columns, cluster)]
                 )
                 if isinstance(pca_output, pd.DataFrame):
                     pca_output.columns = pca_output_columns
                 else:
                     pca_output = pd.DataFrame(
@@ -288,53 +308,54 @@
             if isinstance(features, pd.DataFrame):
                 features_transform.index = features.index
                 return features_transform
             return features_transform.values
         return features
 
     def plot_dendro(self, ax: plt.Axes = None) -> Dict[str, Any]:
-        """
-        Plot dendrogram of the correlation matrix.
+        """Plot dendrogram of the correlation matrix.
 
         Parameters
         ----------
         ax : plt.Axes, optional
             Axis to plot the dendrogram on, by default None
 
         Returns
         -------
         Dict[str, Any]
             Dendrogram object
+
         """
         self.dendro = hierarchy.dendrogram(
             self._corr_linkage,
             orientation="right",
             labels=self._columns,
             color_threshold=self.threshold,
             ax=ax,
         )
         return self.dendro
 
     def plot_correlation_matrix(
         self, fig=None, ax: plt.Axes = None
     ) -> plt.Axes:
-        """
-        Plot correlation matrix of the features.
+        """Plot correlation matrix of the features.
 
         Parameters
         ----------
         fig : plt.Figure, optional
             Figure to plot the correlation matrix on, by default None
         ax : plt.Axes, optional
             Axis to plot the correlation matrix on, by default None
 
         Returns
         -------
         plt.Axes
-            Axis with the correlation matrix"""
+        Axis with the correlation matrix
+
+        """
         if ax is None:
             fig = plt.gcf()
             ax = plt.gca()
         plot = ax.pcolor(
             abs(self._corr[self.dendro["leaves"], :][:, self.dendro["leaves"]])
         )
         dendro_idx = np.arange(0, len(self.dendro["ivl"]))
@@ -343,26 +364,26 @@
         ax.set_xticklabels(self.dendro["ivl"], rotation="vertical")
         ax.set_yticklabels(self.dendro["ivl"])
 
         fig.colorbar(plot, format=ticker.PercentFormatter(xmax=1))
         return ax
 
     def get_clusters(self, linkage: np.ndarray) -> List[List[str]]:
-        """
-        Retrieves the cluster of variables given a specific threshold
+        """Retrieve the cluster of variables given a specific threshold.
 
         Parameters
         ----------
         linkage : np.ndarray
             Linkage matrix from scipy.cluster.hierarchy
 
         Returns
         -------
         List[List[str]]
             List of lists of variable names according to each cluster
+
         """
         # Récupération des clusters à partir de la hiérarchie
         cluster_ids = hierarchy.fcluster(
             linkage, self.threshold, criterion="distance"
         )
         # Assignation des index de chaque variable dans un dictionnaire
         cluster_id_to_feature_ids = defaultdict(list)
@@ -378,24 +399,29 @@
         return clusters_col
 
 
 class PairwiseCorrelationDrop(BaseEstimator, TransformerMixin):
     """Scikit-learn like estimator to deal with pair-wise correlation."""
 
     def __init__(self, threshold: float = 0.9) -> None:
-        """
-        Implements the variable selection based on pair-wise correlation
-        through a scikit-learn transformer explained in
-        https://towardsdatascience.com/are-you-dropping-too-many-correlated-features-d1c96654abe6
+        """Implement the variable selection based on pair-wise correlation.
+
+        Scikit-learn transformer-like implementation
 
         Parameters
         ----------
         threshold : float, optional
             pairwise correlation threshold to consider dropping one of the two
             variables in the pair, by default 0.9
+
+        Notes
+        -----
+        See https://towardsdatascience.com/are-you-dropping-too-many-correlated-features-d1c96654abe6
+        for more details.
+
         """
         super().__init__()
         self.threshold = threshold
 
     def fit(
         self, features: ArrayLike2D, y: ArrayLike1D = None
     ) -> "PairwiseCorrelationDrop":
@@ -408,14 +434,15 @@
         y : ArrayLike1D, optional
             Target, by default None
 
         Returns
         -------
         PairwiseCorrelationDrop
             Fitted transformer
+
         """
         features_, y = check_X_y(
             features, y, ensure_min_features=2, ensure_min_samples=2
         )
         self.n_features_in_ = features_.shape[1]
         self.mask_selection_ = self.compute_mask_selection(
             features_, self.threshold
@@ -442,42 +469,44 @@
         -------
         ArrayLike2D
             Selected features
 
         Raises
         ------
         ValueError
-            If the number of columns in features is different from the number of
-            columns in the training data.
+            If the number of columns in features is different from the number
+            of columns in the training data.
+
         """
         features = check_array(features, ensure_min_features=2)
         check_is_fitted(self, ["mask_selection_", "n_features_in_"])
         if features.shape[1] != self.n_features_in_:
             raise ValueError(
                 "Shape of input is different from what was seen in `fit`"
             )
         return features[:, self.mask_selection_]
 
     @classmethod
     def compute_mask_selection(
         cls, features: np.ndarray, cut: float = 0.9
     ) -> np.ndarray:
-        """Computes the mask of variables to keep based on pair-wise correlation.
+        """Compute the mask of variables to keep.
 
         Parameters
         ----------
         features : np.ndarray
             Features
         cut : float, optional
             Correlation threshold, by default 0.9
 
         Returns
         -------
         np.ndarray
             Mask of variables to keep
+
         """
         # Get correlation matrix and upper triagle
         corr_mtx = np.corrcoef(features, rowvar=False)
         avg_corr = np.mean(corr_mtx, axis=1)
         up = np.triu(corr_mtx, k=1)
 
         dropcols = np.zeros(features.shape[1], dtype=bool)
@@ -525,25 +554,26 @@
 
         return mask_selection
 
     @staticmethod
     def compute_drop_indices_from_detailed_steps(
         res: pd.DataFrame,
     ) -> np.ndarray:
-        """Computes the indices of variables to drop from the detailed steps.
+        """Compute the indices of variables to drop from the detailed steps.
 
         Parameters
         ----------
         res : pd.DataFrame
             Detailed steps of the pairwise correlation drop
 
         Returns
         -------
         np.ndarray
             Indices of variables to drop
+
         """
         # All variables with correlation > cutoff
         all_corr_vars = list(set(res["v1"].tolist() + res["v2"].tolist()))
 
         # All unique variables in drop column
         poss_drop = list(set(res["drop"].tolist()))
```

### Comparing `clementcome_toolkit-0.4.1/cc_tk/plot/classification.py` & `clementcome_toolkit-0.5.0/cc_tk/plot/classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 @validate_call(config=ConfigDict(arbitrary_types_allowed=True))
 def plot_confusion(
     confusion_matrix: ArrayLike2D,
     fmt: str = "d",
     near_diag: int = 1,
     vrange: Union[Literal["global", "local"], Tuple[float]] = "global",
 ) -> None:
-    """
-    Plot a confusion matrix with green, blue and red color scales.
+    """Plot a confusion matrix with green, blue and red color scales.
 
     Parameters
     ----------
     confusion_matrix : ArrayLike2D
         The confusion matrix to plot.
     fmt : str
         The format string for the annotations in the heatmap.
@@ -46,14 +45,15 @@
     .. plot::
         :include-source:
 
         >>> from cc_tk.plot.classification import plot_confusion
         >>> import numpy as np
         >>> confusion_matrix = np.array([[15, 3, 1], [2, 10, 0], [0, 0, 5]])
         >>> plot_confusion(confusion_matrix, fmt=".2f")
+
     """
     n = confusion_matrix.shape[0]
 
     # Create a mask to separate diagonal, near-diagonal and off-diagonal cells
     mask_neardiag = np.zeros((n, n))
     for i in range(1, near_diag + 1):
         mask_neardiag += np.eye(n, k=i) + np.eye(n, k=-i)
```

### Comparing `clementcome_toolkit-0.4.1/cc_tk/relationship/distribution.py` & `clementcome_toolkit-0.5.0/cc_tk/relationship/distribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     numeric_features : pd.DataFrame
         Numeric features to compute the distribution of.
 
     Returns
     -------
     pd.DataFrame
         Distribution of the features.
+
     """
     if numeric_features.empty:
         return pd.DataFrame()
     distribution_df = numeric_features.describe().T
     distribution_df.index.name = "Variable"
     distribution_df = distribution_df.reset_index()
     return distribution_df
@@ -45,14 +46,15 @@
     categorical_features : pd.DataFrame
         Categorical features to compute the distribution of.
 
     Returns
     -------
     pd.DataFrame
         Distribution of the features.
+
     """
     if categorical_features.empty:
         return pd.DataFrame()
     distribution_dict = {}
     for feature in categorical_features.columns:
         distribution_dict[feature] = pd.concat(
             (
@@ -83,14 +85,15 @@
     target : pd.Series
         Target to group by. It must be categorical.
 
     Returns
     -------
     numeric_summary, catecorigal_summary : Tuple[pd.DataFrame, pd.DataFrame]
         Distribution of the features by target group.
+
     """
     # Compute the distribution of numeric features by target group
     numeric_features = features.select_dtypes(include="number")
     if numeric_features.empty:
         numeric_distribution_df = pd.DataFrame()
     else:
         numeric_distribution_df = (
```

### Comparing `clementcome_toolkit-0.4.1/cc_tk/relationship/schema.py` & `clementcome_toolkit-0.5.0/cc_tk/relationship/schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,19 +9,45 @@
 import pandas as pd
 from pandera import Check, DataFrameSchema
 from pydantic import validate_call
 
 from cc_tk.util.types import ArrayLike1D
 
 
-def all_columns_numeric(df):
+def all_columns_numeric(df: pd.DataFrame) -> bool:
+    """Check if all columns in a DataFrame are numeric.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        The DataFrame to check.
+
+    Returns
+    -------
+    bool
+        True if all columns are numeric, False otherwise.
+
+    """
     return df.select_dtypes(include=[np.number]).shape[1] == df.shape[1]
 
 
-def all_columns_categorical(df):
+def all_columns_categorical(df: pd.DataFrame) -> bool:
+    """Check if all columns in a DataFrame are categorical.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        The DataFrame to check.
+
+    Returns
+    -------
+    bool
+        True if all columns are categorical, False otherwise.
+
+    """
     return df.select_dtypes(exclude=[np.number]).shape[1] == df.shape[1]
 
 
 OnlyNumericSchema = DataFrameSchema(checks=Check(all_columns_numeric))
 OnlyCategoricalSchema = DataFrameSchema(checks=Check(all_columns_categorical))
 
 
@@ -29,16 +55,18 @@
 class SeriesType(str, Enum):
     """Defines the type of a series."""
 
     NUMERIC = "numeric"
     CATEGORICAL = "categorical"
 
 
-def check_series_in_signature(func: Callable, *arg_names: str) -> inspect.Signature:
-    """Checks that the specified arguments are pd.Series.
+def check_series_in_signature(
+    func: Callable, *arg_names: str
+) -> inspect.Signature:
+    """Check that the specified arguments are pd.Series.
 
     Parameters
     ----------
     func : Callable
         The function to check.
     *arg_names : str
         The names of the arguments to check.
@@ -50,41 +78,47 @@
 
     Raises
     ------
     ValueError
         If an argument does not exist.
     TypeError
         If an argument is not a pd.Series.
+
     """
     signature = inspect.signature(func)
     for arg_name in arg_names:
         if arg_name not in signature.parameters:
             raise ValueError(f"Argument '{arg_name}' does not exist")
         elif (
             sys.version_info >= (3, 10)
-            and not issubclass(signature.parameters[arg_name].annotation, ArrayLike1D)
-        ) or signature.parameters[arg_name].annotation not in get_args(ArrayLike1D):
+            and not issubclass(
+                signature.parameters[arg_name].annotation, ArrayLike1D
+            )
+        ) or signature.parameters[arg_name].annotation not in get_args(
+            ArrayLike1D
+        ):
             raise TypeError(f"Argument '{arg_name}' must be a 1D-array.")
     return signature
 
 
 @validate_call
 def check_input_types(*type_specs: Tuple[str, SeriesType]) -> Callable:
-    """Checks the types of the arguments of the decorated function.
+    """Check the types of the arguments of the decorated function.
 
     Parameters
     ----------
     *type_specs : Tuple[str, SeriesType]
         A tuple of tuples, each tuple contains the name of the argument and the
         expected type of the argument.
 
     Returns
     -------
     Callable
         The decorator.
+
     """
 
     def decorator(func: Callable) -> Callable:
         signature = check_series_in_signature(
             func, *[arg_name for arg_name, _ in type_specs]
         )
 
@@ -101,36 +135,39 @@
                     and not pd.api.types.is_numeric_dtype(series)
                 ):
                     raise TypeError(f"Argument '{arg_name}' must be numeric")
                 elif (
                     expected_type == SeriesType.CATEGORICAL
                     and pd.api.types.is_numeric_dtype(series)
                 ):
-                    raise TypeError(f"Argument '{arg_name}' must be categorical")
+                    raise TypeError(
+                        f"Argument '{arg_name}' must be categorical"
+                    )
 
             return func(*args, **kwargs)
 
         return wrapper
 
     return decorator
 
 
 @validate_call
 def check_input_index(*arg_names: str) -> Callable:
-    """Checks that the specified arguments have the same index.
+    """Check that the specified arguments have the same index.
 
     Parameters
     ----------
     *arg_names : str
         The names of the arguments to check.
 
     Returns
     -------
     Callable
         The decorator.
+
     """
 
     def decorator(func):
         signature = check_series_in_signature(func, *arg_names)
 
         @wraps(func)
         def wrapper(*args, **kwargs):
@@ -140,14 +177,16 @@
             series_list = [
                 bound_arguments.arguments[arg_name] for arg_name in arg_names
             ]
 
             first_series_index = series_list[0].index
             for series in series_list[1:]:
                 if not series.index.equals(first_series_index):
-                    raise ValueError("All specified Series must have the same index.")
+                    raise ValueError(
+                        "All specified Series must have the same index."
+                    )
 
             return func(*args, **kwargs)
 
         return wrapper
 
     return decorator
```

### Comparing `clementcome_toolkit-0.4.1/cc_tk/relationship/significance.py` & `clementcome_toolkit-0.5.0/cc_tk/relationship/significance/statistical.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,294 +1,273 @@
-"""Evaluate the significance of the relationship between 2 variables.
-
-Usually this consists in evaluating the relationship between a feature and
-the target variable.
-"""
-from enum import Enum, unique
-from typing import Tuple
+"""Significance tests based on statistical methods."""
+from typing import Optional, Tuple
 
 import pandas as pd
-from pydantic import BaseModel, ConfigDict, validate_call
 from scipy import stats
 
-from cc_tk.relationship.schema import (
-    SeriesType,
-    check_input_index,
-    check_input_types,
+from cc_tk.relationship.significance.base import (
+    Constants,
+    SignificanceCategoricalCategorical,
+    SignificanceCategoricalNumeric,
+    SignificanceNumericCategorical,
+    SignificanceNumericNumeric,
+    SignificanceOutput,
 )
 from cc_tk.relationship.utils import cut_influence, influence_from_correlation
 
 
-class Constants:
-    """
-    Constants for the relationship functions
-    """
-
-    WEAK_THRESHOLD = 0.1
-    STRONG_THRESHOLD = 0.05
+class PearsonSignificance(SignificanceNumericNumeric):
+    """Significance test based on Pearson correlation."""
 
+    def _evaluate(
+        self, numeric_values_1: pd.Series, numeric_values_2: pd.Series
+    ) -> SignificanceOutput:
+        """Pearson correlation-based significance.
+
+        The significance is based on the test of pearson correlation not being
+        null.
+
+        Parameters
+        ----------
+        numeric_values_1 : pd.Series
+            First numeric values
+        numeric_values_2 : pd.Series
+            Second numeric values
+
+        Returns
+        -------
+        SignificanceOutput
+            Output of the significance function
 
-@unique
-class SignificanceEnum(str, Enum):
-    WEAK_VALUE = "weak"
-    MEDIUM_VALUE = "medium"
-    STRONG_VALUE = "strong"
+        """
+        corr_results = stats.pearsonr(numeric_values_1, numeric_values_2)
+        correlation = corr_results.statistic
+        pvalue = corr_results.pvalue
+
+        influence = influence_from_correlation(correlation)
+        influence = pd.Series([influence])
+
+        output = SignificanceOutput(
+            pvalue=pvalue,
+            influence=influence,
+            statistic=correlation,
+        )
 
+        return output
 
-class SignificanceOutput(BaseModel):
-    """
-    Output of the significance functions
-    """
 
-    pvalue: float
-    influence: pd.Series
-    statistic: float
-    message: str = ""
+class AnovaSignificance:
+    """Base class for ANOVA significance tests."""
 
-    model_config = ConfigDict(arbitrary_types_allowed=True)
+    def compute_significance(
+        self, numeric_values: pd.Series, categorical_values: pd.Series
+    ) -> SignificanceOutput:
+        """Anova or Kruskal-Wallis significance test.
+
+        Parameters
+        ----------
+        numeric_values : pd.Series
+            Numeric values which we are interested in knowing if there is a
+            difference in distribution
+        categorical_values : pd.Series
+            Categorical values to divide the numeric values in groups
+
+        Returns
+        -------
+        SignificanceOutput
+            Output of the significance function
 
-    @property
-    def significance(self) -> SignificanceEnum:
-        """
-        Computing significativity based on pvalue.
         """
-        significance = SignificanceEnum.WEAK_VALUE
-        if self.pvalue < Constants.WEAK_THRESHOLD:
-            significance = SignificanceEnum.MEDIUM_VALUE
-        if self.pvalue < Constants.STRONG_THRESHOLD:
-            significance = SignificanceEnum.STRONG_VALUE
+        group_info = self._compute_group_info(
+            numeric_values, categorical_values
+        )
+        ks_pvalue_series, bartlett_pvalue = self._perform_tests(group_info)
 
-        return significance
+        # If any of the groups is not gaussian: ks_pvalue_series < 0.05 OR
+        # If any of the groups does not have equal variance:
+        #   bartlett_pvalue < 0.05
+        # Then we use Kruskal-Wallis test
+        if (ks_pvalue_series < Constants.STRONG_THRESHOLD).any() or (
+            bartlett_pvalue < Constants.STRONG_THRESHOLD
+        ):
+            test = stats.kruskal(
+                *[info["values"] for info in group_info.values()]
+            )
+            message = (
+                f"{numeric_values.name} grouped by {categorical_values.name} "
+                f"are not gaussians with equal variances. "
+                f"Computing Kruskal-Wallis p-value."
+            )
+
+        else:
+            # If all the groups are gaussian and have equal variances
+            # we use ANOVA test
+            test = stats.f_oneway(
+                *[info["values"] for info in group_info.values()]
+            )
+            message = (
+                f"{numeric_values.name} grouped by {categorical_values.name} "
+                f"are gaussians and have equal variances. Computing "
+                f"ANOVA p-value."
+            )
+
+        statistic = test.statistic
+        pvalue = test.pvalue
+
+        mean_by_group = pd.Series(
+            {key: info["mean"] for key, info in group_info.items()}
+        )
+        influence = cut_influence(mean_by_group)
+
+        output = SignificanceOutput(
+            pvalue=pvalue,
+            influence=influence,
+            statistic=statistic,
+            message=message,
+        )
+
+        return output
+
+    @staticmethod
+    def _compute_group_info(
+        numeric_values: pd.Series, categorical_values: pd.Series
+    ) -> dict:
+        """Compute information for each categorical group.
+
+        Informations computed are: mean, std, normalized values and
+        Kolmogorov-Smirnov test.
+
+        Parameters
+        ----------
+        numeric_values : pd.Series
+            Numeric values to divide in groups
+        categorical_values : pd.Series
+            Categorical values to divide the numeric values in groups
+
+        Returns
+        -------
+        dict
+            Dictionary with the information of each group
 
-    def to_dataframe(self) -> pd.DataFrame:
-        """
-        Convert the output to a dataframe
         """
-        return pd.DataFrame(
-            {
-                "influence": self.influence,
-                "pvalue": self.pvalue,
-                "statistic": self.statistic,
-                "message": self.message,
-                "significance": self.significance.value,
+        group_info = {}
+        for categorical_value in categorical_values.unique():
+            group_values = numeric_values[
+                categorical_values == categorical_value
+            ]
+            group_mean = group_values.mean()
+            group_std = group_values.std()
+            group_normalized_values = (group_values - group_mean) / group_std
+            group_test_ks = stats.kstest(group_normalized_values, "norm")
+            group_info[categorical_value] = {
+                "values": group_values,
+                "normalized_values": group_normalized_values,
+                "mean": group_mean,
+                "std": group_std,
+                "ks_test": group_test_ks,
             }
-        )
+        return group_info
 
+    @staticmethod
+    def _perform_tests(group_info: dict) -> Tuple[pd.Series, float]:
+        """Perform Kolmogorov-Smirnov and Bartlett tests for the groups.
 
-@check_input_types(
-    ("numeric_values_1", SeriesType.NUMERIC),
-    ("numeric_values_2", SeriesType.NUMERIC),
-)
-@check_input_index("numeric_values_1", "numeric_values_2")
-@validate_call(config={"arbitrary_types_allowed": True})
-def significance_numeric_numeric(
-    numeric_values_1: pd.Series, numeric_values_2: pd.Series
-) -> Tuple[str, float, float]:
-    """
-    Computes the correlation and the significance of this correlation to be
-    non-zero
-
-    Parameters
-    ----------
-    numeric_values_1 : pd.Series
-        First numeric values
-    numeric_values_2 : pd.Series
-        Second numeric values
-
-    Returns
-    -------
-    SignificanceOutput
-        Output of the significance function
-    """
-    corr_results = stats.pearsonr(numeric_values_1, numeric_values_2)
-    correlation = corr_results.statistic
-    pvalue = corr_results.pvalue
-
-    influence = influence_from_correlation(correlation)
-    influence = pd.Series([influence])
-
-    output = SignificanceOutput(
-        pvalue=pvalue,
-        influence=influence,
-        statistic=correlation,
-    )
-
-    return output
-
-
-@check_input_types(
-    ("numeric_values", SeriesType.NUMERIC),
-    ("categorical_values", SeriesType.CATEGORICAL),
-)
-@check_input_index("numeric_values", "categorical_values")
-@validate_call(config={"arbitrary_types_allowed": True})
-def significance_numeric_categorical(
-    numeric_values: pd.Series, categorical_values: pd.Series
-) -> SignificanceOutput:
-    """
-    Computes the significance of distibution difference of a numeric
-    variable against categories
-
-    Parameters
-    ----------
-    numeric_values : pd.Series
-        Numeric values which we are interested in knowing if there is a
-        difference in distribution
-    categorical_values : pd.Series
-        Categorical values to divide the numeric values in groups
-
-    Returns
-    -------
-    SignificanceOutput
-        Output of the significance function
-    """
-    group_info = _compute_group_info(numeric_values, categorical_values)
-    ks_pvalue_series, bartlett_pvalue = _perform_tests(group_info)
-
-    # If any of the groups is not gaussian: ks_pvalue_series < 0.05 OR
-    # If any of the groups does not have equal variance: bartlett_pvalue < 0.05
-    # Then we use Kruskal-Wallis test
-    if (ks_pvalue_series < 0.05).any() or (bartlett_pvalue < 0.05):
-        test = stats.kruskal(*[info["values"] for info in group_info.values()])
-        message = (
-            f"{numeric_values.name} grouped by {categorical_values.name} "
-            f"are not gaussians with equal variances. "
-            f"Computing Kruskal-Wallis p-value."
+        - Kolmogorov-Smirnov test is used to check if the groups are gaussian
+        - Bartlett test is used to check if the groups have equal variances
+        """
+        ks_pvalue_series = pd.Series(
+            [group_info[key]["ks_test"].pvalue for key in group_info.keys()]
         )
+        bartlett_pvalue = stats.bartlett(
+            *[info["values"] for info in group_info.values()]
+        ).pvalue
+        return ks_pvalue_series, bartlett_pvalue
 
-    else:
-        # If all the groups are gaussian and have equal variances
-        # we use ANOVA test
-        test = stats.f_oneway(*[info["values"] for info in group_info.values()])
-        message = (
-            f"{numeric_values.name} grouped by {categorical_values.name} "
-            f"are gaussians and have equal variances. Computing "
-            f"ANOVA p-value."
-        )
 
-    statistic = test.statistic
-    pvalue = test.pvalue
+class AnovaSignificanceNumericTarget(
+    SignificanceCategoricalNumeric, AnovaSignificance
+):
+    """Anova significance test with numeric target."""
 
-    mean_by_group = pd.Series({key: info["mean"] for key, info in group_info.items()})
-    influence = cut_influence(mean_by_group)
+    def _evaluate(
+        self, categorical_values: pd.Series, numeric_values: pd.Series
+    ) -> SignificanceOutput:
+        return self.compute_significance(numeric_values, categorical_values)
 
-    output = SignificanceOutput(
-        pvalue=pvalue,
-        influence=influence,
-        statistic=statistic,
-        message=message,
-    )
-
-    return output
-
-
-def _compute_group_info(
-    numeric_values: pd.Series, categorical_values: pd.Series
-) -> dict:
-    """
-    Compute the mean, std, normalized values and Kolmogorov-Smirnov test for
-    each group of values
-
-    Parameters
-    ----------
-    numeric_values : pd.Series
-        Numeric values to divide in groups
-    categorical_values : pd.Series
-        Categorical values to divide the numeric values in groups
-
-    Returns
-    -------
-    dict
-        Dictionary with the information of each group
-    """
-    group_info = {}
-    for categorical_value in categorical_values.unique():
-        group_values = numeric_values[categorical_values == categorical_value]
-        group_mean = group_values.mean()
-        group_std = group_values.std()
-        group_normalized_values = (group_values - group_mean) / group_std
-        group_test_ks = stats.kstest(group_normalized_values, "norm")
-        group_info[categorical_value] = {
-            "values": group_values,
-            "normalized_values": group_normalized_values,
-            "mean": group_mean,
-            "std": group_std,
-            "ks_test": group_test_ks,
-        }
-    return group_info
-
-
-def _perform_tests(group_info: dict) -> Tuple[pd.Series, float]:
-    """
-    Perform the Kolmogorov-Smirnov test and the Bartlett test for the
-    groups of values
-    - Kolmogorov-Smirnov test is used to check if the groups are gaussian
-    - Bartlett test is used to check if the groups have equal variances
-    """
-    ks_pvalue_series = pd.Series(
-        [group_info[key]["ks_test"].pvalue for key in group_info.keys()]
-    )
-    bartlett_pvalue = stats.bartlett(
-        *[info["values"] for info in group_info.values()]
-    ).pvalue
-    return ks_pvalue_series, bartlett_pvalue
-
-
-@check_input_types(
-    ("categorical_values_1", SeriesType.CATEGORICAL),
-    ("categorical_values_2", SeriesType.CATEGORICAL),
-)
-@check_input_index(
-    "categorical_values_1",
-    "categorical_values_2",
-)
-@validate_call(config={"arbitrary_types_allowed": True})
-def significance_categorical_categorical(
-    categorical_values_1: pd.Series, categorical_values_2: pd.Series
-) -> SignificanceOutput:
-    """
-    Computes the significance of the difference between 2 categorical
-    variables
-
-    Parameters
-    ----------
-    categorical_values_1 : pd.Series
-        First categorical series
-    categorical_values_2 : pd.Series
-        Second categorical series
-
-    Returns
-    -------
-    SignificanceOutput
-        Output of the significance function
-    """
-    contingency_table = pd.crosstab(categorical_values_1, categorical_values_2)
-    if (contingency_table < 5).any().any():
-        hypotheses_verified = False
-    else:
-        hypotheses_verified = True
-
-    chi2_results = stats.chi2_contingency(contingency_table)
-    statistic = chi2_results.statistic
-    pvalue = chi2_results.pvalue
-
-    # Influence is computed based on the relative difference between actual
-    # values and expected frequencies
-    influence = cut_influence(
-        (contingency_table - chi2_results.expected_freq)
-        .divide(chi2_results.expected_freq)
-        .unstack()
-    )
-
-    if hypotheses_verified:
-        message = "Hypotheses verified."
-    else:
-        message = "Hypotheses not verified."
-
-    output = SignificanceOutput(
-        pvalue=pvalue,
-        influence=influence,
-        statistic=statistic,
-        message=message,
-    )
 
-    return output
+class AnovaSignificanceCategoricalTarget(
+    SignificanceNumericCategorical, AnovaSignificance
+):
+    """Anova significance test with categorical target."""
+
+    def _evaluate(
+        self, numeric_values: pd.Series, categorical_values: pd.Series
+    ) -> SignificanceOutput:
+        return self.compute_significance(numeric_values, categorical_values)
+
+
+class Chi2Significance(SignificanceCategoricalCategorical):
+    """Significance based on Chi2 test."""
+
+    def __init__(self, hypotheses_threshold: Optional[int] = 5) -> None:
+        """Initialize the Chi2 significance test.
+
+        Parameters
+        ----------
+        hypotheses_threshold : Optional[int], optional
+            Threshold for hypotheses verification, by default 5
+
+        """
+        self.hypotheses_threshold = hypotheses_threshold
+
+    def _evaluate(
+        self, categorical_values_1: pd.Series, categorical_values_2: pd.Series
+    ) -> SignificanceOutput:
+        """Chi2 significance test for categorical/categorical variables.
+
+        Parameters
+        ----------
+        categorical_values_1 : pd.Series
+            First categorical series
+        categorical_values_2 : pd.Series
+            Second categorical series
+
+        Returns
+        -------
+        SignificanceOutput
+            Output of the significance function
+
+        """
+        contingency_table = pd.crosstab(
+            categorical_values_1,
+            categorical_values_2,
+        )
+        if (contingency_table < self.hypotheses_threshold).any().any():
+            hypotheses_verified = False
+        else:
+            hypotheses_verified = True
+
+        chi2_results = stats.chi2_contingency(contingency_table)
+        statistic = chi2_results.statistic
+        pvalue = chi2_results.pvalue
+
+        # Influence is computed based on the relative difference between actual
+        # values and expected frequencies
+        influence = cut_influence(
+            (contingency_table - chi2_results.expected_freq)
+            .divide(chi2_results.expected_freq)
+            .unstack()
+        )
+
+        if hypotheses_verified:
+            message = "Hypotheses verified."
+        else:
+            message = "Hypotheses not verified."
+
+        output = SignificanceOutput(
+            pvalue=pvalue,
+            influence=influence,
+            statistic=statistic,
+            message=message,
+        )
+
+        return output
```

### Comparing `clementcome_toolkit-0.4.1/cc_tk/relationship/summary.py` & `clementcome_toolkit-0.5.0/cc_tk/relationship/summary.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,48 +3,70 @@
 from typing import Optional, Tuple
 
 import numpy as np
 import pandas as pd
 from pydantic import BaseModel
 from pydantic.config import ConfigDict
 
-from cc_tk.relationship import distribution, significance
+from cc_tk.relationship import distribution
+from cc_tk.relationship.significance import (
+    SignificanceType,
+    VariableType,
+    get_significance,
+)
 
 
 class SummaryOutput(BaseModel):
+    """Output of the relationship summary.
+
+    Parameters
+    ----------
+    numeric_distribution : pd.DataFrame
+        The numeric distribution.
+    categorical_distribution : pd.DataFrame
+        The categorical distribution.
+    numeric_significance : pd.DataFrame
+        The numeric significance.
+    categorical_significance : pd.DataFrame
+        The categorical significance.
+
+    """
+
     numeric_distribution: pd.DataFrame
     categorical_distribution: pd.DataFrame
     numeric_significance: pd.DataFrame
     categorical_significance: pd.DataFrame
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     def to_excel(self, path: str) -> None:
         """Write the summary to an Excel file.
 
         Parameters
         ----------
         path : str
             Path to the Excel file.
+
         """
         with pd.ExcelWriter(path) as writer:
             for name, df in self.model_dump().items():
-                df.to_excel(writer, sheet_name=name)
+                df.to_excel(writer, sheet_name=name, merge_cells=False)
 
 
 class RelationshipSummary:
-    """Class for building and summarizing the relationship between features and
-    target variable.
+    """Builds the relationship summary.
 
     Parameters
     ----------
     features : pd.DataFrame
         The input features.
     target : pd.Series
         The target variable.
+    significance_type : Optional[SignificanceType]
+        The type of significance to compute, by default "statistical".
 
     Attributes
     ----------
     features : pd.DataFrame
         The input features.
     target : pd.Series
         The target variable.
@@ -73,28 +95,62 @@
     _build_categorical_significance() -> pd.DataFrame:
         Build the categorical significance.
     _build_distribution_by_target() -> Tuple[pd.DataFrame, pd.DataFrame]:
         Build the distribution by target.
 
     """
 
-    def __init__(self, features: pd.DataFrame, target: pd.Series):
+    def __init__(
+        self,
+        features: pd.DataFrame,
+        target: pd.Series,
+        significance_type: SignificanceType = SignificanceType.STATISTICAL,
+    ):
+        """Initialize the relationship summary.
+
+        Parameters
+        ----------
+        features : pd.DataFrame
+            The input features.
+        target : pd.Series
+            The target variable.
+        significance_type : SignificanceType, optional
+            The type of significance to compute, by default "statistical".
+
+        """
         self.features = features
         self.target = target
-        self.numeric_features = self.features.select_dtypes(include=[np.number])
-        self.categorical_features = self.features.select_dtypes(exclude=[np.number])
+        self.target_type = (
+            VariableType.NUMERIC
+            if pd.api.types.is_numeric_dtype(self.target)
+            else VariableType.CATEGORICAL
+        )
+        self.significance_type = significance_type
+        self.numeric_features = self.features.select_dtypes(
+            include=[np.number]
+        )
+        self.categorical_features = self.features.select_dtypes(
+            exclude=[np.number]
+        )
         self.summary_output: Optional[SummaryOutput] = None
+        self.numeric_significance_function = get_significance(
+            VariableType.NUMERIC, self.target_type, self.significance_type
+        )
+        self.categorical_significance_function = get_significance(
+            VariableType.CATEGORICAL, self.target_type, self.significance_type
+        )
 
     def build_summary(self) -> SummaryOutput:
         """Build the relationship summary.
 
         Returns
         -------
         SummaryOutput
             Relationship summary.
+
         """
         (
             numeric_distribution_by_target_class,
             categorical_distribution_by_target_class,
         ) = self._build_distribution_by_target()
         self.summary_output = SummaryOutput(
             numeric_distribution=self._build_numeric_distribution(),
@@ -119,14 +175,15 @@
     def to_excel(self, path: str) -> None:
         """Write the summary to an Excel file.
 
         Parameters
         ----------
         path : str
             Path to the Excel file.
+
         """
         if self.summary_output is None:
             self.build_summary()
         self.summary_output.to_excel(path)
 
     def _build_numeric_distribution(self) -> pd.DataFrame:
         return distribution.numeric_distribution(self.numeric_features)
@@ -136,62 +193,66 @@
 
     def _build_numeric_significance(self) -> pd.DataFrame:
         if self.numeric_features.empty:
             return pd.DataFrame()
         if pd.api.types.is_numeric_dtype(self.target):
             significance_df = pd.concat(
                 {
-                    feature_name: significance.significance_numeric_numeric(
+                    feature_name: self.numeric_significance_function(
                         self.features[feature_name], self.target
                     ).to_dataframe()
                     for feature_name in self.numeric_features
                 }
             ).reset_index(level=1, drop=True)
             significance_df.index.name = "Variable"
             return significance_df
         significance_df = pd.concat(
             {
-                feature_name: significance.significance_numeric_categorical(
+                feature_name: self.numeric_significance_function(
                     self.features[feature_name], self.target
                 ).to_dataframe()
                 for feature_name in self.numeric_features
             }
         ).sort_index()
         significance_df.index.names = ["Variable", "Target"]
         return significance_df
 
     def _build_categorical_significance(self) -> pd.DataFrame:
         if self.categorical_features.empty:
             return pd.DataFrame()
         if pd.api.types.is_numeric_dtype(self.target):
             significance_df = pd.concat(
                 {
-                    feature_name: significance.significance_numeric_categorical(
-                        self.target, self.features[feature_name]
+                    feature_name: self.categorical_significance_function(
+                        self.features[feature_name], self.target
                     ).to_dataframe()
                     for feature_name in self.categorical_features
                 }
             ).sort_index()
             significance_df.index.names = ["Variable", "Value"]
             return significance_df
         significance_df = pd.concat(
             {
-                feature_name: significance.significance_categorical_categorical(
+                feature_name: self.categorical_significance_function(
                     self.features[feature_name], self.target
                 ).to_dataframe()
                 for feature_name in self.categorical_features
             }
         ).sort_index()
         significance_df.index.names = ["Variable", "Target", "Value"]
         return significance_df
 
-    def _build_distribution_by_target(self) -> Tuple[pd.DataFrame, pd.DataFrame]:
+    def _build_distribution_by_target(
+        self,
+    ) -> Tuple[pd.DataFrame, pd.DataFrame]:
         if not pd.api.types.is_numeric_dtype(self.target):
             (
                 numeric_distribution_by_target_class,
                 categorical_distribution_by_target_class,
-            ) = distribution.summary_distribution_by_target(self.features, self.target)
+            ) = distribution.summary_distribution_by_target(
+                self.features, self.target
+            )
             return (
                 numeric_distribution_by_target_class,
                 categorical_distribution_by_target_class,
             )
         return pd.DataFrame(), pd.DataFrame()
```

### Comparing `clementcome_toolkit-0.4.1/cc_tk/relationship/utils.py` & `clementcome_toolkit-0.5.0/cc_tk/relationship/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility functions to perform caracterisation."""
+
 import numpy as np
 import pandas as pd
 
 
 def cut_influence(influence_values: pd.Series) -> pd.Series:
     """Cut influence values into categories.
 
@@ -19,30 +20,35 @@
     influence_values : pd.Series
         Influence values to cut.
 
     Returns
     -------
     pd.Series
         Categorical influence values.
+
     """
     # cut_values are used to determine the thresholds between categories
     cut_values = influence_values.quantile(np.linspace(0, 1, 7))
 
+    # duplicate_threshold is used to determine if two cut_values are equal
+    duplicate_threshold = 0.01
+
     # correction_factor is used to correct the cut_values in case of duplicates
     correction_factor = (
-        cut_values.diff().mask(cut_values.diff() < 0.01).min() * 0.01
+        cut_values.diff().mask(cut_values.diff() < duplicate_threshold).min()
+        * duplicate_threshold
     )
     if np.isnan(correction_factor):
-        correction_factor = 0.001
+        correction_factor = duplicate_threshold**2
 
     # duplicate_correction is used to shift cut_values in case of duplicates
     # (i.e. when two or more cut_values are equal)
     # This shifts are centered so it does not add any bias
     duplicate_correction = (
-        cut_values.diff().abs() < 0.01
+        cut_values.diff().abs() < duplicate_threshold
     ).cumsum() * correction_factor
     duplicate_correction = (
         duplicate_correction - duplicate_correction.max() / 2
     )
 
     cut_values = cut_values + duplicate_correction
 
@@ -64,17 +70,20 @@
     correlation_value : float
         Correlation value to compute the influence from.
 
     Returns
     -------
     str
         Influence value.
+
     """
-    if correlation_value < -0.6:
+    strong_correlation = 0.6
+    weak_correlation = 0.3
+    if correlation_value < -strong_correlation:
         return "--"
-    if correlation_value < -0.3:
+    if correlation_value < -weak_correlation:
         return "-"
-    if correlation_value < 0.3:
+    if correlation_value < weak_correlation:
         return ""
-    if correlation_value < 0.6:
+    if correlation_value < strong_correlation:
         return "+"
     return "++"
```

### Comparing `clementcome_toolkit-0.4.1/pyproject.toml` & `clementcome_toolkit-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clementcome-toolkit"
-version = "0.4.1"
+version = "0.5.0"
 description = "My data science toolkit."
 authors = ["Clément Côme <clement.come98@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "cc_tk" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
@@ -65,20 +65,30 @@
 line_length = 79
 known_first_party = "cc_tk"
 
 [tool.black]
 line-length = 79
 
 [tool.ruff]
-exclude = ["tests/**"]
+line-length = 79
+exclude = ["tests/**", "docs/**"]
+select = ["B", "D", "E", "F", "I", "N", "PL", "S", "W"]
 
 [tool.pytest.ini_options]
 addopts = [
-    # "-v",
-    # "--cov=cc_tk",
-    # "--cov-report=xml",
-    # "--cov-report=term",
-    # "--cov-fail-under=70",
+    "-v",
+    "--cov=cc_tk",
+    "--cov-report=xml",
+    "--cov-report=term",
+    "--cov-fail-under=70",
+]
+
+[tool.coverage.report]
+exclude_lines = [
+    "pragma: no cover",
+    "def __repr__",
+    "def __str__",
+    "@abstractmethod",
 ]
 
 [tool.pylint]
 fail-under = 8.0
```

