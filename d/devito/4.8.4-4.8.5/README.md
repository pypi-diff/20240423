# Comparing `tmp/devito-4.8.4.tar.gz` & `tmp/devito-4.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devito-4.8.4.tar", last modified: Thu Apr 18 12:32:16 2024, max compression
+gzip compressed data, was "devito-4.8.5.tar", last modified: Tue Apr 23 21:02:32 2024, max compression
```

## Comparing `devito-4.8.4.tar` & `devito-4.8.5.tar`

### file list

```diff
@@ -1,305 +1,308 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.531878 devito-4.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-18 12:32:08.000000 devito-4.8.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-18 12:32:08.000000 devito-4.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-18 12:32:16.531878 devito-4.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-18 12:32:08.000000 devito-4.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.475878 devito-4.8.4/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:08.000000 devito-4.8.4/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.475878 devito-4.8.4/benchmarks/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:08.000000 devito-4.8.4/benchmarks/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.479878 devito-4.8.4/benchmarks/user/advisor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:08.000000 devito-4.8.4/benchmarks/user/advisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-18 12:32:08.000000 devito-4.8.4/benchmarks/user/advisor/advisor_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-04-18 12:32:08.000000 devito-4.8.4/benchmarks/user/advisor/roofline.py
--rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-04-18 12:32:08.000000 devito-4.8.4/benchmarks/user/advisor/run_advisor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16089 2024-04-18 12:32:08.000000 devito-4.8.4/benchmarks/user/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-18 12:32:08.000000 devito-4.8.4/benchmarks/user/make-pbs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.479878 devito-4.8.4/devito/
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-18 12:32:08.000000 devito-4.8.4/devito/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-18 12:32:16.531878 devito-4.8.4/devito/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.479878 devito-4.8.4/devito/arch/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 12:32:08.000000 devito-4.8.4/devito/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29231 2024-04-18 12:32:08.000000 devito-4.8.4/devito/arch/archinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    34728 2024-04-18 12:32:08.000000 devito-4.8.4/devito/arch/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.479878 devito-4.8.4/devito/builtins/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-18 12:32:08.000000 devito-4.8.4/devito/builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-18 12:32:08.000000 devito-4.8.4/devito/builtins/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)    13497 2024-04-18 12:32:08.000000 devito-4.8.4/devito/builtins/initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-18 12:32:08.000000 devito-4.8.4/devito/builtins/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.483878 devito-4.8.4/devito/checkpointing/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-18 12:32:08.000000 devito-4.8.4/devito/checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-18 12:32:08.000000 devito-4.8.4/devito/checkpointing/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.483878 devito-4.8.4/devito/core/
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-18 12:32:08.000000 devito-4.8.4/devito/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-18 12:32:08.000000 devito-4.8.4/devito/core/arm.py
--rw-r--r--   0 runner    (1001) docker     (127)    14142 2024-04-18 12:32:08.000000 devito-4.8.4/devito/core/autotuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    10880 2024-04-18 12:32:08.000000 devito-4.8.4/devito/core/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)    15081 2024-04-18 12:32:08.000000 devito-4.8.4/devito/core/gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-18 12:32:08.000000 devito-4.8.4/devito/core/intel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12818 2024-04-18 12:32:08.000000 devito-4.8.4/devito/core/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-18 12:32:08.000000 devito-4.8.4/devito/core/power.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.483878 devito-4.8.4/devito/data/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-18 12:32:08.000000 devito-4.8.4/devito/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-04-18 12:32:08.000000 devito-4.8.4/devito/data/allocators.py
--rw-r--r--   0 runner    (1001) docker     (127)    26753 2024-04-18 12:32:08.000000 devito-4.8.4/devito/data/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    20809 2024-04-18 12:32:08.000000 devito-4.8.4/devito/data/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-18 12:32:08.000000 devito-4.8.4/devito/data/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-18 12:32:08.000000 devito-4.8.4/devito/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-18 12:32:08.000000 devito-4.8.4/devito/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.487878 devito-4.8.4/devito/finite_differences/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)    15983 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/derivative.py
--rw-r--r--   0 runner    (1001) docker     (127)    31997 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/differentiable.py
--rw-r--r--   0 runner    (1001) docker     (127)    14838 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/elementary.py
--rw-r--r--   0 runner    (1001) docker     (127)     9999 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/finite_difference.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/rsfd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13629 2024-04-18 12:32:08.000000 devito-4.8.4/devito/finite_differences/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.487878 devito-4.8.4/devito/ir/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.487878 devito-4.8.4/devito/ir/clusters/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22427 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/clusters/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/clusters/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    18050 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/clusters/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/clusters/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.487878 devito-4.8.4/devito/ir/equations/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/equations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/equations/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/equations/equation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.487878 devito-4.8.4/devito/ir/iet/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/iet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/iet/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/iet/efunc.py
--rw-r--r--   0 runner    (1001) docker     (127)    42683 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/iet/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/iet/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    47606 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/iet/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.491878 devito-4.8.4/devito/ir/stree/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/stree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/stree/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/stree/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.491878 devito-4.8.4/devito/ir/support/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47211 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/guards.py
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    32039 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/space.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/symregistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/syncs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14397 2024-04-18 12:32:08.000000 devito-4.8.4/devito/ir/support/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-18 12:32:08.000000 devito-4.8.4/devito/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.491878 devito-4.8.4/devito/mpatches/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 12:32:08.000000 devito-4.8.4/devito/mpatches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-18 12:32:08.000000 devito-4.8.4/devito/mpatches/rationaltools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.491878 devito-4.8.4/devito/mpi/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 12:32:08.000000 devito-4.8.4/devito/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23631 2024-04-18 12:32:08.000000 devito-4.8.4/devito/mpi/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    25197 2024-04-18 12:32:08.000000 devito-4.8.4/devito/mpi/halo_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    45401 2024-04-18 12:32:08.000000 devito-4.8.4/devito/mpi/routines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.495878 devito-4.8.4/devito/operations/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 12:32:08.000000 devito-4.8.4/devito/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17943 2024-04-18 12:32:08.000000 devito-4.8.4/devito/operations/interpolators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-18 12:32:08.000000 devito-4.8.4/devito/operations/solve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.495878 devito-4.8.4/devito/operator/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-18 12:32:08.000000 devito-4.8.4/devito/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46775 2024-04-18 12:32:08.000000 devito-4.8.4/devito/operator/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    20840 2024-04-18 12:32:08.000000 devito-4.8.4/devito/operator/profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-18 12:32:08.000000 devito-4.8.4/devito/operator/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-18 12:32:08.000000 devito-4.8.4/devito/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.495878 devito-4.8.4/devito/passes/
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.495878 devito-4.8.4/devito/passes/clusters/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50437 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    11373 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/asynchrony.py
--rw-r--r--   0 runner    (1001) docker     (127)    19927 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)    28912 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/buffering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/cse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/factorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/implicit.py
--rw-r--r--   0 runner    (1001) docker     (127)    17857 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/unevaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/clusters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.499878 devito-4.8.4/devito/passes/equations/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/equations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/equations/linearity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.499878 devito-4.8.4/devito/passes/iet/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/asynchrony.py
--rw-r--r--   0 runner    (1001) docker     (127)    20595 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17777 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)    19919 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/langbase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.499878 devito-4.8.4/devito/passes/iet/languages/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/languages/C.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/languages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/languages/openacc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/languages/openmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/languages/targets.py
--rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/linearization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/orchestration.py
--rw-r--r--   0 runner    (1001) docker     (127)    22751 2024-04-18 12:32:08.000000 devito-4.8.4/devito/passes/iet/parpragma.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.503878 devito-4.8.4/devito/symbolics/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-18 12:32:08.000000 devito-4.8.4/devito/symbolics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-18 12:32:08.000000 devito-4.8.4/devito/symbolics/extended_sympy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-04-18 12:32:08.000000 devito-4.8.4/devito/symbolics/inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-04-18 12:32:08.000000 devito-4.8.4/devito/symbolics/manipulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-04-18 12:32:08.000000 devito-4.8.4/devito/symbolics/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-04-18 12:32:08.000000 devito-4.8.4/devito/symbolics/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-18 12:32:08.000000 devito-4.8.4/devito/symbolics/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-18 12:32:08.000000 devito-4.8.4/devito/symbolics/unevaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.503878 devito-4.8.4/devito/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)    23684 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/dtypes_lowering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/memoization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/os_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-18 12:32:08.000000 devito-4.8.4/devito/tools/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.507878 devito-4.8.4/devito/types/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    16415 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    50787 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)    63536 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    53530 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/dimension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/equation.py
--rw-r--r--   0 runner    (1001) docker     (127)    29934 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/relational.py
--rw-r--r--   0 runner    (1001) docker     (127)    84563 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    18529 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-18 12:32:08.000000 devito-4.8.4/devito/types/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.527878 devito-4.8.4/devito.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-18 12:32:16.000000 devito-4.8.4/devito.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-04-18 12:32:16.000000 devito-4.8.4/devito.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:32:16.000000 devito-4.8.4/devito.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-18 12:32:16.000000 devito-4.8.4/devito.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 12:32:16.000000 devito-4.8.4/devito.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.475878 devito-4.8.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.511878 devito-4.8.4/examples/cfd/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 12:32:08.000000 devito-4.8.4/examples/cfd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-04-18 12:32:08.000000 devito-4.8.4/examples/cfd/example_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-18 12:32:08.000000 devito-4.8.4/examples/cfd/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.511878 devito-4.8.4/examples/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:08.000000 devito-4.8.4/examples/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.511878 devito-4.8.4/examples/misc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:08.000000 devito-4.8.4/examples/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-18 12:32:08.000000 devito-4.8.4/examples/misc/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.511878 devito-4.8.4/examples/mpi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:08.000000 devito-4.8.4/examples/mpi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.511878 devito-4.8.4/examples/performance/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 12:32:08.000000 devito-4.8.4/examples/performance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-18 12:32:08.000000 devito-4.8.4/examples/performance/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.511878 devito-4.8.4/examples/seismic/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.511878 devito-4.8.4/examples/seismic/acoustic/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/acoustic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/acoustic/acoustic_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/acoustic/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/acoustic/wavesolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.515878 devito-4.8.4/examples/seismic/elastic/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/elastic/elastic_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/elastic/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/elastic/wavesolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    17436 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    16122 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/preset_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.515878 devito-4.8.4/examples/seismic/self_adjoint/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/self_adjoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/self_adjoint/example_iso.py
--rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/self_adjoint/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/self_adjoint/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18618 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/self_adjoint/test_wavesolver_iso.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/self_adjoint/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10793 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/self_adjoint/wavesolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/test_seismic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.515878 devito-4.8.4/examples/seismic/tti/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/tti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21999 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/tti/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/tti/tti_example.py
--rw-r--r--   0 runner    (1001) docker     (127)    15733 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/tti/wavesolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.515878 devito-4.8.4/examples/seismic/viscoacoustic/
--rwxr-xr-x   0 runner    (1001) docker     (127)      112 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/viscoacoustic/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22768 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/viscoacoustic/operators.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3351 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/viscoacoustic/viscoacoustic_example.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17366 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/viscoacoustic/wavesolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.515878 devito-4.8.4/examples/seismic/viscoelastic/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/viscoelastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/viscoelastic/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/viscoelastic/viscoelastic_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-18 12:32:08.000000 devito-4.8.4/examples/seismic/viscoelastic/wavesolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.515878 devito-4.8.4/examples/userapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:08.000000 devito-4.8.4/examples/userapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 12:32:08.000000 devito-4.8.4/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-18 12:32:08.000000 devito-4.8.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-18 12:32:16.531878 devito-4.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-18 12:32:08.000000 devito-4.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:32:16.527878 devito-4.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_adjoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_autotuner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)    22230 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_buffering.py
--rw-r--r--   0 runner    (1001) docker     (127)    17450 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    30449 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     9533 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_cinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)    65948 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    35428 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_derivatives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_differentiable.py
--rw-r--r--   0 runner    (1001) docker     (127)    69440 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_dimension.py
--rw-r--r--   0 runner    (1001) docker     (127)    55068 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_dle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)   116568 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_dse.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_error_checking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_fission.py
--rw-r--r--   0 runner    (1001) docker     (127)    57869 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_gpu_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_gpu_openacc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12444 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_gpu_openmp.py
--rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)    13309 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_iet.py
--rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)    37983 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_linearize.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_lower_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_lower_exprs.py
--rw-r--r--   0 runner    (1001) docker     (127)   101814 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)    78996 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    29848 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_roundoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_skewing.py
--rw-r--r--   0 runner    (1001) docker     (127)    18171 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_staggered_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23819 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_subdomains.py
--rw-r--r--   0 runner    (1001) docker     (127)    19566 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_symbolic_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)    20609 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_symbolics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15141 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_tensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_timestepping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_tti.py
--rw-r--r--   0 runner    (1001) docker     (127)    16618 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_unexpansion.py
--rw-r--r--   0 runner    (1001) docker     (127)    10942 2024-04-18 12:32:08.000000 devito-4.8.4/tests/test_visitors.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-18 12:32:08.000000 devito-4.8.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.200468 devito-4.8.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-23 21:02:23.000000 devito-4.8.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-23 21:02:23.000000 devito-4.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-23 21:02:32.200468 devito-4.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-23 21:02:23.000000 devito-4.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.144467 devito-4.8.5/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:23.000000 devito-4.8.5/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.144467 devito-4.8.5/benchmarks/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:23.000000 devito-4.8.5/benchmarks/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.144467 devito-4.8.5/benchmarks/user/advisor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:23.000000 devito-4.8.5/benchmarks/user/advisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-23 21:02:23.000000 devito-4.8.5/benchmarks/user/advisor/advisor_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-04-23 21:02:23.000000 devito-4.8.5/benchmarks/user/advisor/roofline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-04-23 21:02:23.000000 devito-4.8.5/benchmarks/user/advisor/run_advisor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16089 2024-04-23 21:02:23.000000 devito-4.8.5/benchmarks/user/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-23 21:02:23.000000 devito-4.8.5/benchmarks/user/make-pbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.144467 devito-4.8.5/devito/
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-23 21:02:23.000000 devito-4.8.5/devito/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-23 21:02:32.200468 devito-4.8.5/devito/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.148467 devito-4.8.5/devito/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-23 21:02:23.000000 devito-4.8.5/devito/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29231 2024-04-23 21:02:23.000000 devito-4.8.5/devito/arch/archinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34728 2024-04-23 21:02:23.000000 devito-4.8.5/devito/arch/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.148467 devito-4.8.5/devito/builtins/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 21:02:23.000000 devito-4.8.5/devito/builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-23 21:02:23.000000 devito-4.8.5/devito/builtins/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13497 2024-04-23 21:02:23.000000 devito-4.8.5/devito/builtins/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-23 21:02:23.000000 devito-4.8.5/devito/builtins/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.148467 devito-4.8.5/devito/checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-23 21:02:23.000000 devito-4.8.5/devito/checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-23 21:02:23.000000 devito-4.8.5/devito/checkpointing/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.148467 devito-4.8.5/devito/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-23 21:02:23.000000 devito-4.8.5/devito/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-23 21:02:23.000000 devito-4.8.5/devito/core/arm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14142 2024-04-23 21:02:23.000000 devito-4.8.5/devito/core/autotuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10880 2024-04-23 21:02:23.000000 devito-4.8.5/devito/core/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15081 2024-04-23 21:02:23.000000 devito-4.8.5/devito/core/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-23 21:02:23.000000 devito-4.8.5/devito/core/intel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12818 2024-04-23 21:02:23.000000 devito-4.8.5/devito/core/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-23 21:02:23.000000 devito-4.8.5/devito/core/power.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.152467 devito-4.8.5/devito/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-23 21:02:23.000000 devito-4.8.5/devito/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-04-23 21:02:23.000000 devito-4.8.5/devito/data/allocators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26753 2024-04-23 21:02:23.000000 devito-4.8.5/devito/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20809 2024-04-23 21:02:23.000000 devito-4.8.5/devito/data/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-23 21:02:23.000000 devito-4.8.5/devito/data/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-23 21:02:23.000000 devito-4.8.5/devito/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 21:02:23.000000 devito-4.8.5/devito/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.152467 devito-4.8.5/devito/finite_differences/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-23 21:02:23.000000 devito-4.8.5/devito/finite_differences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-04-23 21:02:23.000000 devito-4.8.5/devito/finite_differences/coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15983 2024-04-23 21:02:23.000000 devito-4.8.5/devito/finite_differences/derivative.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31997 2024-04-23 21:02:23.000000 devito-4.8.5/devito/finite_differences/differentiable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14838 2024-04-23 21:02:23.000000 devito-4.8.5/devito/finite_differences/elementary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9999 2024-04-23 21:02:23.000000 devito-4.8.5/devito/finite_differences/finite_difference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-23 21:02:23.000000 devito-4.8.5/devito/finite_differences/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-23 21:02:23.000000 devito-4.8.5/devito/finite_differences/rsfd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13629 2024-04-23 21:02:23.000000 devito-4.8.5/devito/finite_differences/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.152467 devito-4.8.5/devito/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.156467 devito-4.8.5/devito/ir/clusters/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22427 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/clusters/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/clusters/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18050 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/clusters/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/clusters/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.156467 devito-4.8.5/devito/ir/equations/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/equations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/equations/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/equations/equation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.156467 devito-4.8.5/devito/ir/iet/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/iet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/iet/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/iet/efunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42683 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/iet/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/iet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47606 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/iet/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.156467 devito-4.8.5/devito/ir/stree/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/stree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/stree/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/stree/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.160467 devito-4.8.5/devito/ir/support/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47211 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/support/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/support/guards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/support/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32039 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/support/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/support/symregistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/support/syncs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/support/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14397 2024-04-23 21:02:23.000000 devito-4.8.5/devito/ir/support/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-23 21:02:23.000000 devito-4.8.5/devito/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.160467 devito-4.8.5/devito/mpatches/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-23 21:02:23.000000 devito-4.8.5/devito/mpatches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-23 21:02:23.000000 devito-4.8.5/devito/mpatches/rationaltools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.160467 devito-4.8.5/devito/mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 21:02:23.000000 devito-4.8.5/devito/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23631 2024-04-23 21:02:23.000000 devito-4.8.5/devito/mpi/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25197 2024-04-23 21:02:23.000000 devito-4.8.5/devito/mpi/halo_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45401 2024-04-23 21:02:23.000000 devito-4.8.5/devito/mpi/routines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.160467 devito-4.8.5/devito/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 21:02:23.000000 devito-4.8.5/devito/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17943 2024-04-23 21:02:23.000000 devito-4.8.5/devito/operations/interpolators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-23 21:02:23.000000 devito-4.8.5/devito/operations/solve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.164467 devito-4.8.5/devito/operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-23 21:02:23.000000 devito-4.8.5/devito/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46775 2024-04-23 21:02:23.000000 devito-4.8.5/devito/operator/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20840 2024-04-23 21:02:23.000000 devito-4.8.5/devito/operator/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-23 21:02:23.000000 devito-4.8.5/devito/operator/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-23 21:02:23.000000 devito-4.8.5/devito/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.164467 devito-4.8.5/devito/passes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.164467 devito-4.8.5/devito/passes/clusters/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50437 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/clusters/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11373 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/clusters/asynchrony.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19927 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/clusters/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28912 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/clusters/buffering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/clusters/cse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/clusters/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/clusters/factorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/clusters/implicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17857 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/clusters/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/clusters/unevaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/clusters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.164467 devito-4.8.5/devito/passes/equations/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/equations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/equations/linearity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.168468 devito-4.8.5/devito/passes/iet/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/iet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/iet/asynchrony.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20595 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/iet/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17777 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/iet/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/iet/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/iet/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19919 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/iet/langbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.168468 devito-4.8.5/devito/passes/iet/languages/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/iet/languages/C.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/iet/languages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/iet/languages/openacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/iet/languages/openmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/iet/languages/targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/iet/linearization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/iet/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/iet/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/iet/orchestration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22751 2024-04-23 21:02:23.000000 devito-4.8.5/devito/passes/iet/parpragma.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.172468 devito-4.8.5/devito/symbolics/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 21:02:23.000000 devito-4.8.5/devito/symbolics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-23 21:02:23.000000 devito-4.8.5/devito/symbolics/extended_sympy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-04-23 21:02:23.000000 devito-4.8.5/devito/symbolics/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-04-23 21:02:23.000000 devito-4.8.5/devito/symbolics/manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-04-23 21:02:23.000000 devito-4.8.5/devito/symbolics/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-04-23 21:02:23.000000 devito-4.8.5/devito/symbolics/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-23 21:02:23.000000 devito-4.8.5/devito/symbolics/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-23 21:02:23.000000 devito-4.8.5/devito/symbolics/unevaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.172468 devito-4.8.5/devito/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-23 21:02:23.000000 devito-4.8.5/devito/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-04-23 21:02:23.000000 devito-4.8.5/devito/tools/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-23 21:02:23.000000 devito-4.8.5/devito/tools/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23684 2024-04-23 21:02:23.000000 devito-4.8.5/devito/tools/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-23 21:02:23.000000 devito-4.8.5/devito/tools/dtypes_lowering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-23 21:02:23.000000 devito-4.8.5/devito/tools/memoization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-23 21:02:23.000000 devito-4.8.5/devito/tools/os_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-23 21:02:23.000000 devito-4.8.5/devito/tools/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-23 21:02:23.000000 devito-4.8.5/devito/tools/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-04-23 21:02:23.000000 devito-4.8.5/devito/tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-23 21:02:23.000000 devito-4.8.5/devito/tools/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.176468 devito-4.8.5/devito/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16415 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50787 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63536 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53530 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/equation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29934 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/relational.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84563 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18529 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-23 21:02:23.000000 devito-4.8.5/devito/types/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.196468 devito-4.8.5/devito.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-23 21:02:32.000000 devito-4.8.5/devito.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-04-23 21:02:32.000000 devito-4.8.5/devito.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 21:02:32.000000 devito-4.8.5/devito.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-23 21:02:32.000000 devito-4.8.5/devito.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 21:02:32.000000 devito-4.8.5/devito.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.140467 devito-4.8.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.180468 devito-4.8.5/examples/cfd/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 21:02:23.000000 devito-4.8.5/examples/cfd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-04-23 21:02:23.000000 devito-4.8.5/examples/cfd/example_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-23 21:02:23.000000 devito-4.8.5/examples/cfd/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.180468 devito-4.8.5/examples/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:23.000000 devito-4.8.5/examples/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.180468 devito-4.8.5/examples/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:23.000000 devito-4.8.5/examples/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-23 21:02:23.000000 devito-4.8.5/examples/misc/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.180468 devito-4.8.5/examples/mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:23.000000 devito-4.8.5/examples/mpi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.180468 devito-4.8.5/examples/performance/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 21:02:23.000000 devito-4.8.5/examples/performance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-23 21:02:23.000000 devito-4.8.5/examples/performance/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.180468 devito-4.8.5/examples/seismic/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.184468 devito-4.8.5/examples/seismic/acoustic/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/acoustic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/acoustic/acoustic_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/acoustic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/acoustic/wavesolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.184468 devito-4.8.5/examples/seismic/elastic/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/elastic/elastic_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/elastic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/elastic/wavesolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17436 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16122 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/preset_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.184468 devito-4.8.5/examples/seismic/self_adjoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/self_adjoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/self_adjoint/example_iso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/self_adjoint/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/self_adjoint/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18618 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/self_adjoint/test_wavesolver_iso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/self_adjoint/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10793 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/self_adjoint/wavesolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/test_seismic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.184468 devito-4.8.5/examples/seismic/tti/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/tti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21999 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/tti/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/tti/tti_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15733 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/tti/wavesolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.188468 devito-4.8.5/examples/seismic/viscoacoustic/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      112 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/viscoacoustic/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22768 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/viscoacoustic/operators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3351 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/viscoacoustic/viscoacoustic_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17366 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/viscoacoustic/wavesolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.188468 devito-4.8.5/examples/seismic/viscoelastic/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/viscoelastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/viscoelastic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/viscoelastic/viscoelastic_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-23 21:02:23.000000 devito-4.8.5/examples/seismic/viscoelastic/wavesolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.188468 devito-4.8.5/examples/userapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:23.000000 devito-4.8.5/examples/userapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 21:02:23.000000 devito-4.8.5/requirements-mpi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 21:02:23.000000 devito-4.8.5/requirements-nvidia.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-23 21:02:23.000000 devito-4.8.5/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-23 21:02:23.000000 devito-4.8.5/requirements-testing.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-23 21:02:23.000000 devito-4.8.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-23 21:02:32.200468 devito-4.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-23 21:02:23.000000 devito-4.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:02:32.196468 devito-4.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_autotuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22230 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_buffering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17450 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30449 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9533 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_cinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65948 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35428 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_differentiable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69440 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55068 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_dle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116568 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_dse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_error_checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_fission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57869 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_gpu_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_gpu_openacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12444 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_gpu_openmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13309 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_iet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37983 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_linearize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_lower_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_lower_exprs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101814 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78996 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29848 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_roundoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_skewing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18171 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_staggered_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23819 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_subdomains.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19566 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_symbolic_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20609 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_symbolics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15141 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_timestepping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_tti.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16618 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_unexpansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10942 2024-04-23 21:02:23.000000 devito-4.8.5/tests/test_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-23 21:02:23.000000 devito-4.8.5/versioneer.py
```

### Comparing `devito-4.8.4/LICENSE.md` & `devito-4.8.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/PKG-INFO` & `devito-4.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devito
-Version: 4.8.4
+Version: 4.8.5
 Summary: Finite Difference DSL for symbolic computation.
 Home-page: http://www.devitoproject.org
 Author: Imperial College London
 Author-email: g.gorman@imperial.ac.uk
 License: MIT
 Project-URL: Documentation, https://www.devitoproject.org/devito/index.html
 Project-URL: Source Code, https://github.com/devitocodes/devito
```

### Comparing `devito-4.8.4/README.md` & `devito-4.8.5/README.md`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/benchmarks/user/advisor/advisor_logging.py` & `devito-4.8.5/benchmarks/user/advisor/advisor_logging.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/benchmarks/user/advisor/roofline.py` & `devito-4.8.5/benchmarks/user/advisor/roofline.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/benchmarks/user/advisor/run_advisor.py` & `devito-4.8.5/benchmarks/user/advisor/run_advisor.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/benchmarks/user/benchmark.py` & `devito-4.8.5/benchmarks/user/benchmark.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/benchmarks/user/make-pbs.py` & `devito-4.8.5/benchmarks/user/make-pbs.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/__init__.py` & `devito-4.8.5/devito/__init__.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/arch/archinfo.py` & `devito-4.8.5/devito/arch/archinfo.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/arch/compiler.py` & `devito-4.8.5/devito/arch/compiler.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/builtins/arithmetic.py` & `devito-4.8.5/devito/builtins/arithmetic.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/builtins/initializers.py` & `devito-4.8.5/devito/builtins/initializers.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/builtins/utils.py` & `devito-4.8.5/devito/builtins/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/checkpointing/checkpoint.py` & `devito-4.8.5/devito/checkpointing/checkpoint.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/core/__init__.py` & `devito-4.8.5/devito/core/__init__.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/core/autotuning.py` & `devito-4.8.5/devito/core/autotuning.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/core/cpu.py` & `devito-4.8.5/devito/core/cpu.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/core/gpu.py` & `devito-4.8.5/devito/core/gpu.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/core/operator.py` & `devito-4.8.5/devito/core/operator.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/data/allocators.py` & `devito-4.8.5/devito/data/allocators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/data/data.py` & `devito-4.8.5/devito/data/data.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/data/decomposition.py` & `devito-4.8.5/devito/data/decomposition.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/data/meta.py` & `devito-4.8.5/devito/data/meta.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/data/utils.py` & `devito-4.8.5/devito/data/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/finite_differences/coefficients.py` & `devito-4.8.5/devito/finite_differences/coefficients.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/finite_differences/derivative.py` & `devito-4.8.5/devito/finite_differences/derivative.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/finite_differences/differentiable.py` & `devito-4.8.5/devito/finite_differences/differentiable.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/finite_differences/elementary.py` & `devito-4.8.5/devito/finite_differences/elementary.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/finite_differences/finite_difference.py` & `devito-4.8.5/devito/finite_differences/finite_difference.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/finite_differences/operators.py` & `devito-4.8.5/devito/finite_differences/operators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/finite_differences/rsfd.py` & `devito-4.8.5/devito/finite_differences/rsfd.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/finite_differences/tools.py` & `devito-4.8.5/devito/finite_differences/tools.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/clusters/algorithms.py` & `devito-4.8.5/devito/ir/clusters/algorithms.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/clusters/analysis.py` & `devito-4.8.5/devito/ir/clusters/analysis.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/clusters/cluster.py` & `devito-4.8.5/devito/ir/clusters/cluster.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/clusters/visitors.py` & `devito-4.8.5/devito/ir/clusters/visitors.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/equations/algorithms.py` & `devito-4.8.5/devito/ir/equations/algorithms.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/equations/equation.py` & `devito-4.8.5/devito/ir/equations/equation.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/iet/algorithms.py` & `devito-4.8.5/devito/ir/iet/algorithms.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/iet/efunc.py` & `devito-4.8.5/devito/ir/iet/efunc.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/iet/nodes.py` & `devito-4.8.5/devito/ir/iet/nodes.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/iet/utils.py` & `devito-4.8.5/devito/ir/iet/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/iet/visitors.py` & `devito-4.8.5/devito/ir/iet/visitors.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/stree/algorithms.py` & `devito-4.8.5/devito/ir/stree/algorithms.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/stree/tree.py` & `devito-4.8.5/devito/ir/stree/tree.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/support/basic.py` & `devito-4.8.5/devito/ir/support/basic.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/support/guards.py` & `devito-4.8.5/devito/ir/support/guards.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/support/properties.py` & `devito-4.8.5/devito/ir/support/properties.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/support/space.py` & `devito-4.8.5/devito/ir/support/space.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/support/symregistry.py` & `devito-4.8.5/devito/ir/support/symregistry.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/support/syncs.py` & `devito-4.8.5/devito/ir/support/syncs.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/support/utils.py` & `devito-4.8.5/devito/ir/support/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/ir/support/vector.py` & `devito-4.8.5/devito/ir/support/vector.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/logger.py` & `devito-4.8.5/devito/logger.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/mpatches/rationaltools.py` & `devito-4.8.5/devito/mpatches/rationaltools.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/mpi/distributed.py` & `devito-4.8.5/devito/mpi/distributed.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/mpi/halo_scheme.py` & `devito-4.8.5/devito/mpi/halo_scheme.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/mpi/routines.py` & `devito-4.8.5/devito/mpi/routines.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/operations/interpolators.py` & `devito-4.8.5/devito/operations/interpolators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/operations/solve.py` & `devito-4.8.5/devito/operations/solve.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/operator/operator.py` & `devito-4.8.5/devito/operator/operator.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/operator/profiling.py` & `devito-4.8.5/devito/operator/profiling.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/operator/registry.py` & `devito-4.8.5/devito/operator/registry.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/parameters.py` & `devito-4.8.5/devito/parameters.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/__init__.py` & `devito-4.8.5/devito/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/clusters/aliases.py` & `devito-4.8.5/devito/passes/clusters/aliases.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/clusters/asynchrony.py` & `devito-4.8.5/devito/passes/clusters/asynchrony.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/clusters/blocking.py` & `devito-4.8.5/devito/passes/clusters/blocking.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/clusters/buffering.py` & `devito-4.8.5/devito/passes/clusters/buffering.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/clusters/cse.py` & `devito-4.8.5/devito/passes/clusters/cse.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/clusters/derivatives.py` & `devito-4.8.5/devito/passes/clusters/derivatives.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/clusters/factorization.py` & `devito-4.8.5/devito/passes/clusters/factorization.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/clusters/implicit.py` & `devito-4.8.5/devito/passes/clusters/implicit.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/clusters/misc.py` & `devito-4.8.5/devito/passes/clusters/misc.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/clusters/unevaluate.py` & `devito-4.8.5/devito/passes/clusters/unevaluate.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/clusters/utils.py` & `devito-4.8.5/devito/passes/clusters/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/equations/linearity.py` & `devito-4.8.5/devito/passes/equations/linearity.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/iet/asynchrony.py` & `devito-4.8.5/devito/passes/iet/asynchrony.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/iet/definitions.py` & `devito-4.8.5/devito/passes/iet/definitions.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/iet/engine.py` & `devito-4.8.5/devito/passes/iet/engine.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/iet/errors.py` & `devito-4.8.5/devito/passes/iet/errors.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/iet/instrument.py` & `devito-4.8.5/devito/passes/iet/instrument.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/iet/langbase.py` & `devito-4.8.5/devito/passes/iet/langbase.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/iet/languages/C.py` & `devito-4.8.5/devito/passes/iet/languages/C.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/iet/languages/openacc.py` & `devito-4.8.5/devito/passes/iet/languages/openacc.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/iet/languages/openmp.py` & `devito-4.8.5/devito/passes/iet/languages/openmp.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/iet/languages/targets.py` & `devito-4.8.5/devito/passes/iet/languages/targets.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/iet/linearization.py` & `devito-4.8.5/devito/passes/iet/linearization.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/iet/misc.py` & `devito-4.8.5/devito/passes/iet/misc.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/iet/mpi.py` & `devito-4.8.5/devito/passes/iet/mpi.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/iet/orchestration.py` & `devito-4.8.5/devito/passes/iet/orchestration.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/passes/iet/parpragma.py` & `devito-4.8.5/devito/passes/iet/parpragma.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/symbolics/extended_sympy.py` & `devito-4.8.5/devito/symbolics/extended_sympy.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/symbolics/inspection.py` & `devito-4.8.5/devito/symbolics/inspection.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/symbolics/manipulation.py` & `devito-4.8.5/devito/symbolics/manipulation.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/symbolics/printer.py` & `devito-4.8.5/devito/symbolics/printer.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/symbolics/queries.py` & `devito-4.8.5/devito/symbolics/queries.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/symbolics/search.py` & `devito-4.8.5/devito/symbolics/search.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/symbolics/unevaluation.py` & `devito-4.8.5/devito/symbolics/unevaluation.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/tools/abc.py` & `devito-4.8.5/devito/tools/abc.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/tools/algorithms.py` & `devito-4.8.5/devito/tools/algorithms.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/tools/data_structures.py` & `devito-4.8.5/devito/tools/data_structures.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/tools/dtypes_lowering.py` & `devito-4.8.5/devito/tools/dtypes_lowering.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/tools/memoization.py` & `devito-4.8.5/devito/tools/memoization.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/tools/os_helper.py` & `devito-4.8.5/devito/tools/os_helper.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/tools/threading.py` & `devito-4.8.5/devito/tools/threading.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/tools/timing.py` & `devito-4.8.5/devito/tools/timing.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/tools/utils.py` & `devito-4.8.5/devito/tools/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/tools/visitors.py` & `devito-4.8.5/devito/tools/visitors.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/__init__.py` & `devito-4.8.5/devito/types/__init__.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/args.py` & `devito-4.8.5/devito/types/args.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/array.py` & `devito-4.8.5/devito/types/array.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/basic.py` & `devito-4.8.5/devito/types/basic.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/caching.py` & `devito-4.8.5/devito/types/caching.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/constant.py` & `devito-4.8.5/devito/types/constant.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/dense.py` & `devito-4.8.5/devito/types/dense.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/dimension.py` & `devito-4.8.5/devito/types/dimension.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/equation.py` & `devito-4.8.5/devito/types/equation.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/grid.py` & `devito-4.8.5/devito/types/grid.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/lazy.py` & `devito-4.8.5/devito/types/lazy.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/misc.py` & `devito-4.8.5/devito/types/misc.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/object.py` & `devito-4.8.5/devito/types/object.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/parallel.py` & `devito-4.8.5/devito/types/parallel.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/relational.py` & `devito-4.8.5/devito/types/relational.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/sparse.py` & `devito-4.8.5/devito/types/sparse.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/tensor.py` & `devito-4.8.5/devito/types/tensor.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito/types/utils.py` & `devito-4.8.5/devito/types/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/devito.egg-info/PKG-INFO` & `devito-4.8.5/devito.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devito
-Version: 4.8.4
+Version: 4.8.5
 Summary: Finite Difference DSL for symbolic computation.
 Home-page: http://www.devitoproject.org
 Author: Imperial College London
 Author-email: g.gorman@imperial.ac.uk
 License: MIT
 Project-URL: Documentation, https://www.devitoproject.org/devito/index.html
 Project-URL: Source Code, https://github.com/devitocodes/devito
```

### Comparing `devito-4.8.4/devito.egg-info/SOURCES.txt` & `devito-4.8.5/devito.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 LICENSE.md
 MANIFEST.in
 README.md
+requirements-mpi.txt
+requirements-nvidia.txt
 requirements-optional.txt
+requirements-testing.txt
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 benchmarks/__init__.py
 benchmarks/user/__init__.py
 benchmarks/user/benchmark.py
```

### Comparing `devito-4.8.4/devito.egg-info/requires.txt` & `devito-4.8.5/devito.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/cfd/example_diffusion.py` & `devito-4.8.5/examples/cfd/example_diffusion.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/cfd/tools.py` & `devito-4.8.5/examples/cfd/tools.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/misc/linalg.py` & `devito-4.8.5/examples/misc/linalg.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/performance/utils.py` & `devito-4.8.5/examples/performance/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/acoustic/acoustic_example.py` & `devito-4.8.5/examples/seismic/acoustic/acoustic_example.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/acoustic/operators.py` & `devito-4.8.5/examples/seismic/acoustic/operators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/acoustic/wavesolver.py` & `devito-4.8.5/examples/seismic/acoustic/wavesolver.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/elastic/elastic_example.py` & `devito-4.8.5/examples/seismic/elastic/elastic_example.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/elastic/operators.py` & `devito-4.8.5/examples/seismic/elastic/operators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/elastic/wavesolver.py` & `devito-4.8.5/examples/seismic/elastic/wavesolver.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/model.py` & `devito-4.8.5/examples/seismic/model.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/plotting.py` & `devito-4.8.5/examples/seismic/plotting.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/preset_models.py` & `devito-4.8.5/examples/seismic/preset_models.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/self_adjoint/example_iso.py` & `devito-4.8.5/examples/seismic/self_adjoint/example_iso.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/self_adjoint/operators.py` & `devito-4.8.5/examples/seismic/self_adjoint/operators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/self_adjoint/test_utils.py` & `devito-4.8.5/examples/seismic/self_adjoint/test_utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/self_adjoint/test_wavesolver_iso.py` & `devito-4.8.5/examples/seismic/self_adjoint/test_wavesolver_iso.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/self_adjoint/utils.py` & `devito-4.8.5/examples/seismic/self_adjoint/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/self_adjoint/wavesolver.py` & `devito-4.8.5/examples/seismic/self_adjoint/wavesolver.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/source.py` & `devito-4.8.5/examples/seismic/source.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/test_seismic_utils.py` & `devito-4.8.5/examples/seismic/test_seismic_utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/tti/operators.py` & `devito-4.8.5/examples/seismic/tti/operators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/tti/tti_example.py` & `devito-4.8.5/examples/seismic/tti/tti_example.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/tti/wavesolver.py` & `devito-4.8.5/examples/seismic/tti/wavesolver.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/utils.py` & `devito-4.8.5/examples/seismic/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/viscoacoustic/operators.py` & `devito-4.8.5/examples/seismic/viscoacoustic/operators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/viscoacoustic/viscoacoustic_example.py` & `devito-4.8.5/examples/seismic/viscoacoustic/viscoacoustic_example.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/viscoacoustic/wavesolver.py` & `devito-4.8.5/examples/seismic/viscoacoustic/wavesolver.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/viscoelastic/operators.py` & `devito-4.8.5/examples/seismic/viscoelastic/operators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/viscoelastic/viscoelastic_example.py` & `devito-4.8.5/examples/seismic/viscoelastic/viscoelastic_example.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/examples/seismic/viscoelastic/wavesolver.py` & `devito-4.8.5/examples/seismic/viscoelastic/wavesolver.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/setup.py` & `devito-4.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_adjoint.py` & `devito-4.8.5/tests/test_adjoint.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_autotuner.py` & `devito-4.8.5/tests/test_autotuner.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_benchmark.py` & `devito-4.8.5/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_buffering.py` & `devito-4.8.5/tests/test_buffering.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_builtins.py` & `devito-4.8.5/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_caching.py` & `devito-4.8.5/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_checkpointing.py` & `devito-4.8.5/tests/test_checkpointing.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_cinterface.py` & `devito-4.8.5/tests/test_cinterface.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_constant.py` & `devito-4.8.5/tests/test_constant.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_data.py` & `devito-4.8.5/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_derivatives.py` & `devito-4.8.5/tests/test_derivatives.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_differentiable.py` & `devito-4.8.5/tests/test_differentiable.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_dimension.py` & `devito-4.8.5/tests/test_dimension.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_dle.py` & `devito-4.8.5/tests/test_dle.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_docstrings.py` & `devito-4.8.5/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_dse.py` & `devito-4.8.5/tests/test_dse.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_error_checking.py` & `devito-4.8.5/tests/test_error_checking.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_fission.py` & `devito-4.8.5/tests/test_fission.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_gpu_common.py` & `devito-4.8.5/tests/test_gpu_common.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_gpu_openacc.py` & `devito-4.8.5/tests/test_gpu_openacc.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_gpu_openmp.py` & `devito-4.8.5/tests/test_gpu_openmp.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_gradient.py` & `devito-4.8.5/tests/test_gradient.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_iet.py` & `devito-4.8.5/tests/test_iet.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_interpolation.py` & `devito-4.8.5/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_ir.py` & `devito-4.8.5/tests/test_ir.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_linearize.py` & `devito-4.8.5/tests/test_linearize.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_lower_clusters.py` & `devito-4.8.5/tests/test_lower_clusters.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_lower_exprs.py` & `devito-4.8.5/tests/test_lower_exprs.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_mpi.py` & `devito-4.8.5/tests/test_mpi.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_operator.py` & `devito-4.8.5/tests/test_operator.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_pickle.py` & `devito-4.8.5/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_resample.py` & `devito-4.8.5/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_roundoff.py` & `devito-4.8.5/tests/test_roundoff.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_save.py` & `devito-4.8.5/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_skewing.py` & `devito-4.8.5/tests/test_skewing.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_sparse.py` & `devito-4.8.5/tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_staggered_utils.py` & `devito-4.8.5/tests/test_staggered_utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_subdomains.py` & `devito-4.8.5/tests/test_subdomains.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_symbolic_coefficients.py` & `devito-4.8.5/tests/test_symbolic_coefficients.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_symbolics.py` & `devito-4.8.5/tests/test_symbolics.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_tensors.py` & `devito-4.8.5/tests/test_tensors.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_threading.py` & `devito-4.8.5/tests/test_threading.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_timestepping.py` & `devito-4.8.5/tests/test_timestepping.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_tools.py` & `devito-4.8.5/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_tti.py` & `devito-4.8.5/tests/test_tti.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_unexpansion.py` & `devito-4.8.5/tests/test_unexpansion.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/tests/test_visitors.py` & `devito-4.8.5/tests/test_visitors.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.4/versioneer.py` & `devito-4.8.5/versioneer.py`

 * *Files identical despite different names*

