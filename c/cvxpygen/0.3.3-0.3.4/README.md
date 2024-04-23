# Comparing `tmp/cvxpygen-0.3.3.tar.gz` & `tmp/cvxpygen-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxpygen-0.3.3.tar", last modified: Sun Apr 21 23:41:47 2024, max compression
+gzip compressed data, was "cvxpygen-0.3.4.tar", last modified: Tue Apr 23 00:28:31 2024, max compression
```

## Comparing `cvxpygen-0.3.3.tar` & `cvxpygen-0.3.4.tar`

### file list

```diff
@@ -1,379 +1,379 @@
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.856809 cvxpygen-0.3.3/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.662740 cvxpygen-0.3.3/DEBUG/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-11-18 23:13:31.000000 cvxpygen-0.3.3/DEBUG/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3341 2023-11-18 23:13:31.000000 cvxpygen-0.3.3/DEBUG/cpg_solver.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4182 2023-11-18 23:13:31.000000 cvxpygen-0.3.3/DEBUG/setup.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11349 2022-02-24 20:19:58.000000 cvxpygen-0.3.3/LICENSE
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2991 2023-10-10 06:00:55.000000 cvxpygen-0.3.3/MANIFEST.in
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.664391 cvxpygen-0.3.3/MPC_code/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 22:56:09.000000 cvxpygen-0.3.3/MPC_code/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3402 2024-04-21 22:56:10.000000 cvxpygen-0.3.3/MPC_code/cpg_solver.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4370 2024-04-21 22:56:10.000000 cvxpygen-0.3.3/MPC_code/setup.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     9044 2024-04-21 23:41:47.856958 cvxpygen-0.3.3/PKG-INFO
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8625 2023-10-13 07:10:06.000000 cvxpygen-0.3.3/README.md
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.668450 cvxpygen-0.3.3/cvxpygen/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-10-11 21:20:44.000000 cvxpygen-0.3.3/cvxpygen/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    24467 2024-04-21 19:48:50.000000 cvxpygen-0.3.3/cvxpygen/cpg.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2533 2024-04-21 19:39:52.000000 cvxpygen-0.3.3/cvxpygen/mappings.py
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.654062 cvxpygen-0.3.3/cvxpygen/solvers/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.676892 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      648 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/.clang-format
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       60 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/.git
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      162 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/.gitignore
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      102 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/.gitmodules
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1157 2023-11-18 22:05:30.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/CMakeLists.txt
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.679370 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3792 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/Cargo.toml
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      270 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/pyproject.toml
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       38 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/rustfmt.toml
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.680238 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.689242 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      348 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/adjoint.rs
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.692617 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1998 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/block_concatenate.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    14112 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/core.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8649 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/matrix_math.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      183 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/mod.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     9500 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/utils.rs
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.701242 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    10721 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/blas.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1796 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/blaslike_traits.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1520 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/block_concatenate.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2031 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/cholesky.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     7958 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/core.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2250 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/gemm.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1980 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/gemv.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2218 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/kron.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4633 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/matrix_math.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      396 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/mod.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4384 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/svd.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4545 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/syevr.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1060 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/symv.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1649 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/syr2k.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1738 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/syrk.rs
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.701789 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/densesym3x3/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6914 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/densesym3x3/mod.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      930 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/error_types.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3237 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/floats.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6538 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/math_traits.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1306 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/matrix_traits.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1959 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/matrix_types.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1453 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/mod.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      344 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/reshaped.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      771 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/scalarmath.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      352 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/symmetric.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4815 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/vecmath.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3071 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/lib.rs
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.703832 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/qdldl/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      117 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/qdldl/mod.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    25632 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/qdldl/qdldl.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8608 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/qdldl/test.rs
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.704588 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.707338 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.714885 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11066 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/compositecone.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    13340 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/expcone.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    13721 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/genpowcone.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5367 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/mod.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5798 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/nonnegativecone.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6478 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/nonsymmetric_common.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    14599 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/powcone.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    14247 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/psdtrianglecone.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    15307 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/socone.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     7481 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/supportedcone.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3257 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/symmetric_common.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2912 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/zerocone.rs
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.715573 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.716368 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       35 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/mod.rs
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.718968 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11788 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/datamaps.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    12100 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/directldlkktsolver.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8547 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/kkt_assembly.rs
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.720063 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       15 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/mod.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2743 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/qdldl.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      688 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/mod.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      399 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/mod.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      402 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/mod.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      293 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/settings.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    20101 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/solver.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     7152 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/traits.rs
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.720652 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.727298 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      953 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/equilibration.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11028 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/info.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8217 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/info_print.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8156 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/kktsystem.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      570 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/mod.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4168 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/presolver.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5731 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/problemdata.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2984 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/residuals.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3957 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/settings.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3212 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/solution.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3225 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/solver.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     7639 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/variables.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       77 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/mod.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1931 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/mod.rs
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.729298 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/utils/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      761 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/utils/atomic.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1327 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/utils/infbounds.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       94 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/utils/mod.rs
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.730425 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/timers/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      109 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/timers/mod.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5066 2023-10-09 03:17:24.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/timers/timers.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11357 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/LICENSE.md
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3532 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/README.md
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.731013 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/include/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      511 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/include/Clarabel
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.735510 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/include/c/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      174 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/include/c/ClarabelTypes.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2890 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/include/c/CscMatrix.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1165 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/include/c/DefaultInfo.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3624 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/include/c/DefaultSettings.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1410 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/include/c/DefaultSolution.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4431 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/include/c/DefaultSolver.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8028 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/include/c/SupportedConeT.h
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.737497 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2791 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/CMakeLists.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      613 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/Cargo.toml
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      368 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/cbindgen.toml
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.738985 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1563 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/algebra.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1319 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/core.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       46 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/lib.rs
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.739490 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.740030 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.742764 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1288 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/info.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       65 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/mod.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5197 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/settings.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1086 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/solution.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     9830 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/solver.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       16 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/mod.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       24 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/mod.rs
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.744607 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/utils/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1418 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/utils/csc_matrix.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3048 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/utils/mod.rs
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1790 2023-10-06 23:15:53.000000 cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/utils/supported_cones_T.rs
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.753161 cvxpygen-0.3.3/cvxpygen/solvers/ecos/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6148 2021-11-04 03:37:05.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/.DS_Store
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       87 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/.bumpversion.cfg
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       42 2022-02-23 21:43:27.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/.git
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      296 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/.gitignore
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      477 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/.travis.yml
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4753 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/CMakeLists.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     7272 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/CONTRIBUTING.md
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    35147 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/COPYING
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3377 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/Makefile
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4290 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/README.md
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    86113 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/README.pdf
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1476 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/ecos.mk
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.754669 cvxpygen-0.3.3/cvxpygen/solvers/ecos/ecos_bb/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    40478 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/ecos_bb/ecos_bb.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11665 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/ecos_bb/ecos_bb_preproc.c
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.652640 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.755576 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/SuiteSparse_config/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6482 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/SuiteSparse_config/SuiteSparse_config.h
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.756744 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2027 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/Makefile
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8897 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/README.txt
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.758247 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/include/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    18328 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/include/amd.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     9097 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/include/amd_internal.h
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.767278 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5710 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_1.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    64873 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_2.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4877 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_aat.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1786 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_control.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1253 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_defaults.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5012 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_dump.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3181 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_global.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4173 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_info.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5913 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_order.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3703 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_post_tree.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5509 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_postorder.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3808 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_preprocess.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2980 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_valid.c
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.768567 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/ldl/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      763 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/ldl/Makefile
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5779 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/ldl/README.txt
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.769256 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/ldl/include/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3988 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/ldl/include/ldl.h
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.769863 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/ldl/src/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    20401 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/ldl/src/ldl.c
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.778518 cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6290 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/cone.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1332 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/ctrlc.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    82553 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/data.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    12623 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/ecos.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6689 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/ecos_bb.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1359 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/equil.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2804 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/expcone.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3882 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/glblopts.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4968 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/kkt.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2712 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/spla.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3241 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/splamm.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1717 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/timer.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      822 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/wright_omega.h
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.787644 cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    15297 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/cone.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2721 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/ctrlc.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    54621 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/ecos.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    10355 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/equil.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5076 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/expcone.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    14221 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/kkt.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    32391 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/preproc.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3510 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/runecos.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4039 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/runecos_exp.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4091 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/spla.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     9590 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/splamm.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2578 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/timer.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1962 2021-10-28 22:01:39.000000 cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/wright_omega.c
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.788221 cvxpygen-0.3.3/cvxpygen/solvers/osqp-python/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11357 2021-11-03 20:08:49.000000 cvxpygen-0.3.3/cvxpygen/solvers/osqp-python/LICENSE
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.794515 cvxpygen-0.3.3/cvxpygen/solvers/scs/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6148 2022-02-23 21:12:10.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/.DS_Store
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      296 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/.bumpversion.cfg
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       41 2022-02-23 21:43:27.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/.git
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      488 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/.gitignore
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1009 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/CITATION.cff
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11683 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/CMakeLists.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1110 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/LICENSE.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     7382 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/Makefile
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      922 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/README.md
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.797185 cvxpygen-0.3.3/cvxpygen/solvers/scs/cmake/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8748 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/cmake/AddInstallRPATHSupport.cmake
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2499 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/cmake/AddUninstallTarget.cmake
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    28861 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/cmake/InstallBasicPackageFiles.cmake
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      286 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/cmake/scs_types.h.in
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.805542 cvxpygen-0.3.3/cvxpygen/solvers/scs/include/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3035 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/include/aa.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1611 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/include/cones.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      581 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/include/ctrlc.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5119 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/include/glbopts.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      804 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/include/linalg.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2193 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/include/linsys.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      493 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/include/normalize.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      571 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/include/rw.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    10042 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/include/scs.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1010 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/include/scs_blas.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      437 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/include/scs_types.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2747 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/include/scs_work.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1217 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/include/util.h
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.808101 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.655085 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/cpu/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.809253 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/cpu/direct/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11554 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/cpu/direct/private.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      768 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/cpu/direct/private.h
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.810085 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/cpu/indirect/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     9228 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/cpu/indirect/private.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      681 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/cpu/indirect/private.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2586 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/csparse.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      995 2021-11-08 23:08:19.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/csparse.h
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.655628 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.822129 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2068 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/LICENSE.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    14798 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/SuiteSparse_config.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     9151 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/SuiteSparse_config.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    17956 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5716 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_1.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    64847 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_2.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4868 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_aat.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1876 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_control.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1259 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_defaults.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5012 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_dump.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      941 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_global.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4299 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_info.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     7706 2021-11-08 23:08:19.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_internal.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6084 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_order.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3703 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_post_tree.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     5509 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_postorder.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3808 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_preprocess.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2980 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_valid.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      528 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/changes
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.825609 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/qdldl/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11357 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/qdldl/LICENSE
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4865 2021-11-08 20:11:48.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/qdldl/README.md
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      210 2021-11-08 23:08:19.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/qdldl/changes
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     7683 2021-11-08 23:08:19.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     6397 2021-11-08 23:08:19.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      533 2021-11-08 23:08:19.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl_types.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    12027 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/scs_matrix.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1839 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/scs_matrix.h
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4444 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/scs.mk
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.832110 cvxpygen-0.3.3/cvxpygen/solvers/scs/src/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    14893 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/src/aa.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    26617 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/src/cones.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1770 2021-11-08 23:08:19.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/src/ctrlc.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3996 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/src/linalg.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2556 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/src/normalize.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    13982 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/src/rw.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    39399 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/src/scs.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      147 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/src/scs_version.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3529 2022-03-01 03:33:41.000000 cvxpygen-0.3.3/cvxpygen/solvers/scs/src/util.c
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    49445 2024-04-21 23:35:22.000000 cvxpygen-0.3.3/cvxpygen/solvers.py
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.835366 cvxpygen-0.3.3/cvxpygen/template/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1649 2024-02-23 20:43:11.000000 cvxpygen-0.3.3/cvxpygen/template/CMakeLists.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    11349 2023-08-31 23:26:14.000000 cvxpygen-0.3.3/cvxpygen/template/LICENSE
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     7327 2023-08-31 23:26:14.000000 cvxpygen-0.3.3/cvxpygen/template/README.html
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:19.000000 cvxpygen-0.3.3/cvxpygen/template/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4063 2023-10-11 00:29:46.000000 cvxpygen-0.3.3/cvxpygen/template/setup.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    65804 2024-04-21 23:35:22.000000 cvxpygen-0.3.3/cvxpygen/utils.py
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.671651 cvxpygen-0.3.3/cvxpygen.egg-info/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     9044 2024-04-21 23:41:47.000000 cvxpygen-0.3.3/cvxpygen.egg-info/PKG-INFO
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    15194 2024-04-21 23:41:47.000000 cvxpygen-0.3.3/cvxpygen.egg-info/SOURCES.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        1 2024-04-21 23:41:47.000000 cvxpygen-0.3.3/cvxpygen.egg-info/dependency_links.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      135 2024-04-21 23:41:47.000000 cvxpygen-0.3.3/cvxpygen.egg-info/requires.txt
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      178 2024-04-21 23:41:47.000000 cvxpygen-0.3.3/cvxpygen.egg-info/top_level.txt
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.839024 cvxpygen-0.3.3/cvxpygen_custom_diff_bak/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-10-11 21:20:44.000000 cvxpygen-0.3.3/cvxpygen_custom_diff_bak/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    24706 2024-03-01 01:55:21.000000 cvxpygen-0.3.3/cvxpygen_custom_diff_bak/cpg.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     2583 2024-03-01 00:54:56.000000 cvxpygen-0.3.3/cvxpygen_custom_diff_bak/mappings.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    49890 2024-01-27 00:38:16.000000 cvxpygen-0.3.3/cvxpygen_custom_diff_bak/solvers.py
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.840757 cvxpygen-0.3.3/cvxpygen_custom_diff_bak/template/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:19.000000 cvxpygen-0.3.3/cvxpygen_custom_diff_bak/template/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4063 2023-10-11 00:29:46.000000 cvxpygen-0.3.3/cvxpygen_custom_diff_bak/template/setup.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)    86804 2024-03-01 19:31:11.000000 cvxpygen-0.3.3/cvxpygen_custom_diff_bak/utils.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)      144 2023-08-31 23:29:55.000000 cvxpygen-0.3.3/environment.yml
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.842437 cvxpygen-0.3.3/nonneg_LS/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 20:25:37.000000 cvxpygen-0.3.3/nonneg_LS/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3201 2024-04-21 20:25:37.000000 cvxpygen-0.3.3/nonneg_LS/cpg_solver.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4370 2024-04-21 20:25:37.000000 cvxpygen-0.3.3/nonneg_LS/setup.py
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.844002 cvxpygen-0.3.3/nonneg_LS_bak/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-10-12 18:22:23.000000 cvxpygen-0.3.3/nonneg_LS_bak/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3121 2023-10-12 18:22:36.000000 cvxpygen-0.3.3/nonneg_LS_bak/cpg_solver.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4089 2023-10-12 18:22:36.000000 cvxpygen-0.3.3/nonneg_LS_bak/setup.py
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.845506 cvxpygen-0.3.3/nonneg_LS_proto/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2024-03-01 02:07:13.000000 cvxpygen-0.3.3/nonneg_LS_proto/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3750 2024-03-01 02:07:13.000000 cvxpygen-0.3.3/nonneg_LS_proto/cpg_solver.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4242 2024-03-01 02:07:13.000000 cvxpygen-0.3.3/nonneg_LS_proto/setup.py
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.847192 cvxpygen-0.3.3/proto/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-10-10 01:40:46.000000 cvxpygen-0.3.3/proto/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3198 2023-10-10 01:40:46.000000 cvxpygen-0.3.3/proto/cpg_solver.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4086 2023-10-10 01:40:46.000000 cvxpygen-0.3.3/proto/setup.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)       79 2024-04-21 23:41:47.857494 cvxpygen-0.3.3/setup.cfg
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     1410 2024-04-21 23:35:22.000000 cvxpygen-0.3.3/setup.py
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.848742 cvxpygen-0.3.3/sp_compiled_CLARABEL/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 22:54:03.000000 cvxpygen-0.3.3/sp_compiled_CLARABEL/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3490 2024-04-21 22:54:03.000000 cvxpygen-0.3.3/sp_compiled_CLARABEL/cpg_solver.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4179 2024-04-21 22:54:03.000000 cvxpygen-0.3.3/sp_compiled_CLARABEL/setup.py
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.849589 cvxpygen-0.3.3/sp_compiled_E/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 22:59:08.000000 cvxpygen-0.3.3/sp_compiled_E/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4063 2024-04-21 22:59:08.000000 cvxpygen-0.3.3/sp_compiled_E/setup.py
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.851293 cvxpygen-0.3.3/sp_compiled_ECOS/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 22:59:32.000000 cvxpygen-0.3.3/sp_compiled_ECOS/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3487 2024-04-21 22:59:32.000000 cvxpygen-0.3.3/sp_compiled_ECOS/cpg_solver.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4370 2024-04-21 22:59:32.000000 cvxpygen-0.3.3/sp_compiled_ECOS/setup.py
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.852840 cvxpygen-0.3.3/sp_compiled_SCS/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 21:41:52.000000 cvxpygen-0.3.3/sp_compiled_SCS/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3403 2024-04-21 21:41:52.000000 cvxpygen-0.3.3/sp_compiled_SCS/cpg_solver.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4161 2024-04-21 21:41:52.000000 cvxpygen-0.3.3/sp_compiled_SCS/setup.py
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.854306 cvxpygen-0.3.3/test/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:02:12.000000 cvxpygen-0.3.3/test/__init__.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3590 2023-04-02 15:02:12.000000 cvxpygen-0.3.3/test/cpg_solver.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4275 2023-04-02 15:02:12.000000 cvxpygen-0.3.3/test/setup.py
-drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 23:41:47.856082 cvxpygen-0.3.3/tests/
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     4488 2023-10-11 00:39:44.000000 cvxpygen-0.3.3/tests/test_E2E_LP.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     8793 2024-04-21 19:39:52.000000 cvxpygen-0.3.3/tests/test_E2E_QP.py
--rw-r--r--   0 maximilianschaller   (501) staff       (20)     3831 2023-10-11 00:41:18.000000 cvxpygen-0.3.3/tests/test_E2E_SOCP.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.068959 cvxpygen-0.3.4/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.861830 cvxpygen-0.3.4/DEBUG/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-11-18 23:13:31.000000 cvxpygen-0.3.4/DEBUG/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3341 2023-11-18 23:13:31.000000 cvxpygen-0.3.4/DEBUG/cpg_solver.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4182 2023-11-18 23:13:31.000000 cvxpygen-0.3.4/DEBUG/setup.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11349 2022-02-24 20:19:58.000000 cvxpygen-0.3.4/LICENSE
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2991 2023-10-10 06:00:55.000000 cvxpygen-0.3.4/MANIFEST.in
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.864008 cvxpygen-0.3.4/MPC_code/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2024-04-22 23:37:30.000000 cvxpygen-0.3.4/MPC_code/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3401 2024-04-22 23:37:30.000000 cvxpygen-0.3.4/MPC_code/cpg_solver.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4181 2024-04-22 23:37:30.000000 cvxpygen-0.3.4/MPC_code/setup.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     9044 2024-04-23 00:28:31.069123 cvxpygen-0.3.4/PKG-INFO
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8625 2023-10-13 07:10:06.000000 cvxpygen-0.3.4/README.md
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.868443 cvxpygen-0.3.4/cvxpygen/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-10-11 21:20:44.000000 cvxpygen-0.3.4/cvxpygen/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    24467 2024-04-21 19:48:50.000000 cvxpygen-0.3.4/cvxpygen/cpg.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2533 2024-04-21 19:39:52.000000 cvxpygen-0.3.4/cvxpygen/mappings.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.848806 cvxpygen-0.3.4/cvxpygen/solvers/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.876607 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      648 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/.clang-format
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       60 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/.git
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      162 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/.gitignore
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      102 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/.gitmodules
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1157 2023-11-18 22:05:30.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/CMakeLists.txt
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.879015 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3792 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/Cargo.toml
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      270 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/pyproject.toml
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       38 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/rustfmt.toml
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.879928 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.889592 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      348 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/adjoint.rs
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.894048 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1998 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/block_concatenate.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    14112 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/core.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8649 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/matrix_math.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      183 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/mod.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     9500 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/utils.rs
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.904900 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    10721 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/blas.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1796 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/blaslike_traits.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1520 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/block_concatenate.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2031 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/cholesky.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     7958 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/core.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2250 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/gemm.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1980 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/gemv.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2218 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/kron.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4633 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/matrix_math.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      396 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/mod.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4384 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/svd.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4545 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/syevr.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1060 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/symv.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1649 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/syr2k.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1738 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/syrk.rs
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.905716 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/densesym3x3/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6914 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/densesym3x3/mod.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      930 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/error_types.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3237 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/floats.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6538 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/math_traits.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1306 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/matrix_traits.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1959 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/matrix_types.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1453 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/mod.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      344 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/reshaped.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      771 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/scalarmath.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      352 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/symmetric.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4815 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/vecmath.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3071 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/lib.rs
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.908587 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/qdldl/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      117 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/qdldl/mod.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    25632 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/qdldl/qdldl.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8608 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/qdldl/test.rs
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.909345 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.912442 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.921923 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11066 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/compositecone.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    13340 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/expcone.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    13721 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/genpowcone.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5367 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/mod.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5798 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/nonnegativecone.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6478 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/nonsymmetric_common.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    14599 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/powcone.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    14247 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/psdtrianglecone.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    15307 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/socone.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     7481 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/supportedcone.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3257 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/symmetric_common.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2912 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/zerocone.rs
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.922532 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.923411 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       35 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/mod.rs
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.926833 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11788 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/datamaps.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    12100 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/directldlkktsolver.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8547 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/kkt_assembly.rs
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.928095 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       15 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/mod.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2743 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/qdldl.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      688 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/mod.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      399 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/mod.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      402 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/mod.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      293 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/settings.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    20101 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/solver.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     7152 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/traits.rs
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.928669 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.936752 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      953 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/equilibration.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11028 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/info.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8217 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/info_print.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8156 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/kktsystem.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      570 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/mod.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4168 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/presolver.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5731 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/problemdata.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2984 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/residuals.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3957 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/settings.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3212 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/solution.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3225 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/solver.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     7639 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/variables.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       77 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/mod.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1931 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/mod.rs
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.938664 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/utils/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      761 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/utils/atomic.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1327 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/utils/infbounds.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       94 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/utils/mod.rs
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.939840 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/timers/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      109 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/timers/mod.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5066 2023-10-09 03:17:24.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/timers/timers.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11357 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/LICENSE.md
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3532 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/README.md
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.940530 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/include/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      511 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/include/Clarabel
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.945136 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/include/c/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      174 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/include/c/ClarabelTypes.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2890 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/include/c/CscMatrix.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1165 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/include/c/DefaultInfo.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3624 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/include/c/DefaultSettings.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1410 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/include/c/DefaultSolution.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4431 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/include/c/DefaultSolver.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8028 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/include/c/SupportedConeT.h
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.947171 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2791 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/CMakeLists.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      613 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/Cargo.toml
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      368 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/cbindgen.toml
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.948874 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1563 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/algebra.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1319 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/core.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       46 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/lib.rs
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.949431 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.949991 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.952665 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1288 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/info.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       65 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/mod.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5197 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/settings.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1086 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/solution.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     9830 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/solver.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       16 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/mod.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       24 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/mod.rs
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.954412 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/utils/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1418 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/utils/csc_matrix.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3048 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/utils/mod.rs
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1790 2023-10-06 23:15:53.000000 cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/utils/supported_cones_T.rs
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.962231 cvxpygen-0.3.4/cvxpygen/solvers/ecos/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6148 2021-11-04 03:37:05.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/.DS_Store
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       87 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/.bumpversion.cfg
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       42 2022-02-23 21:43:27.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/.git
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      296 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/.gitignore
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      477 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/.travis.yml
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4753 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/CMakeLists.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     7272 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/CONTRIBUTING.md
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    35147 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/COPYING
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3377 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/Makefile
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4290 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/README.md
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    86113 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/README.pdf
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1476 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/ecos.mk
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.963703 cvxpygen-0.3.4/cvxpygen/solvers/ecos/ecos_bb/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    40478 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/ecos_bb/ecos_bb.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11665 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/ecos_bb/ecos_bb_preproc.c
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.846902 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.964169 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/SuiteSparse_config/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6482 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/SuiteSparse_config/SuiteSparse_config.h
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.965289 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2027 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/Makefile
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8897 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/README.txt
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.966340 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/include/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    18328 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/include/amd.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     9097 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/include/amd_internal.h
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.975881 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5710 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_1.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    64873 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_2.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4877 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_aat.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1786 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_control.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1253 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_defaults.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5012 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_dump.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3181 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_global.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4173 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_info.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5913 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_order.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3703 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_post_tree.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5509 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_postorder.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3808 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_preprocess.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2980 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_valid.c
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.976940 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/ldl/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      763 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/ldl/Makefile
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5779 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/ldl/README.txt
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.977459 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/ldl/include/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3988 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/ldl/include/ldl.h
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.977972 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/ldl/src/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    20401 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/ldl/src/ldl.c
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.987513 cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6290 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/cone.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1332 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/ctrlc.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    82553 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/data.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    12623 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/ecos.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6689 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/ecos_bb.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1359 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/equil.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2804 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/expcone.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3882 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/glblopts.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4968 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/kkt.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2712 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/spla.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3241 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/splamm.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1717 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/timer.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      822 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/wright_omega.h
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.996511 cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    15297 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/cone.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2721 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/ctrlc.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    54621 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/ecos.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    10355 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/equil.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5076 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/expcone.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    14221 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/kkt.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    32391 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/preproc.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3510 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/runecos.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4039 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/runecos_exp.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4091 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/spla.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     9590 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/splamm.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2578 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/timer.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1962 2021-10-28 22:01:39.000000 cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/wright_omega.c
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.996926 cvxpygen-0.3.4/cvxpygen/solvers/osqp-python/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11357 2021-11-03 20:08:49.000000 cvxpygen-0.3.4/cvxpygen/solvers/osqp-python/LICENSE
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.002939 cvxpygen-0.3.4/cvxpygen/solvers/scs/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6148 2022-02-23 21:12:10.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/.DS_Store
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      296 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/.bumpversion.cfg
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       41 2022-02-23 21:43:27.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/.git
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      488 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/.gitignore
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1009 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/CITATION.cff
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11683 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/CMakeLists.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1110 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/LICENSE.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     7382 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/Makefile
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      922 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/README.md
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.006399 cvxpygen-0.3.4/cvxpygen/solvers/scs/cmake/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8748 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/cmake/AddInstallRPATHSupport.cmake
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2499 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/cmake/AddUninstallTarget.cmake
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    28861 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/cmake/InstallBasicPackageFiles.cmake
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      286 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/cmake/scs_types.h.in
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.013208 cvxpygen-0.3.4/cvxpygen/solvers/scs/include/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3035 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/include/aa.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1611 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/include/cones.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      581 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/include/ctrlc.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5119 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/include/glbopts.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      804 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/include/linalg.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2193 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/include/linsys.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      493 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/include/normalize.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      571 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/include/rw.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    10042 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/include/scs.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1010 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/include/scs_blas.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      437 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/include/scs_types.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2747 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/include/scs_work.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1217 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/include/util.h
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.015331 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.850254 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/cpu/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.016270 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/cpu/direct/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11554 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/cpu/direct/private.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      768 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/cpu/direct/private.h
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.017198 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/cpu/indirect/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     9228 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/cpu/indirect/private.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      681 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/cpu/indirect/private.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2586 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/csparse.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      995 2021-11-08 23:08:19.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/csparse.h
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.851153 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.029609 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2068 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/LICENSE.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    14798 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/SuiteSparse_config.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     9151 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/SuiteSparse_config.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    17956 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5716 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_1.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    64847 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_2.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4868 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_aat.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1876 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_control.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1259 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_defaults.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5012 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_dump.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      941 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_global.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4299 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_info.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     7706 2021-11-08 23:08:19.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_internal.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6084 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_order.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3703 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_post_tree.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     5509 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_postorder.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3808 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_preprocess.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2980 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_valid.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      528 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/changes
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.033929 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/qdldl/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11357 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/qdldl/LICENSE
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4865 2021-11-08 20:11:48.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/qdldl/README.md
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      210 2021-11-08 23:08:19.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/qdldl/changes
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     7683 2021-11-08 23:08:19.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     6397 2021-11-08 23:08:19.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      533 2021-11-08 23:08:19.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl_types.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    12027 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/scs_matrix.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1839 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/scs_matrix.h
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4444 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/scs.mk
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.042113 cvxpygen-0.3.4/cvxpygen/solvers/scs/src/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    14893 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/src/aa.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    26617 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/src/cones.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1770 2021-11-08 23:08:19.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/src/ctrlc.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3996 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/src/linalg.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2556 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/src/normalize.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    13982 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/src/rw.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    39399 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/src/scs.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      147 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/src/scs_version.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3529 2022-03-01 03:33:41.000000 cvxpygen-0.3.4/cvxpygen/solvers/scs/src/util.c
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    49703 2024-04-23 00:27:45.000000 cvxpygen-0.3.4/cvxpygen/solvers.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.044998 cvxpygen-0.3.4/cvxpygen/template/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1649 2024-02-23 20:43:11.000000 cvxpygen-0.3.4/cvxpygen/template/CMakeLists.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    11349 2023-08-31 23:26:14.000000 cvxpygen-0.3.4/cvxpygen/template/LICENSE
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     7327 2023-08-31 23:26:14.000000 cvxpygen-0.3.4/cvxpygen/template/README.html
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:19.000000 cvxpygen-0.3.4/cvxpygen/template/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4063 2023-10-11 00:29:46.000000 cvxpygen-0.3.4/cvxpygen/template/setup.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    65804 2024-04-23 00:27:37.000000 cvxpygen-0.3.4/cvxpygen/utils.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:30.871722 cvxpygen-0.3.4/cvxpygen.egg-info/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     9044 2024-04-23 00:28:30.000000 cvxpygen-0.3.4/cvxpygen.egg-info/PKG-INFO
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    15194 2024-04-23 00:28:30.000000 cvxpygen-0.3.4/cvxpygen.egg-info/SOURCES.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        1 2024-04-23 00:28:30.000000 cvxpygen-0.3.4/cvxpygen.egg-info/dependency_links.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      135 2024-04-23 00:28:30.000000 cvxpygen-0.3.4/cvxpygen.egg-info/requires.txt
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      178 2024-04-23 00:28:30.000000 cvxpygen-0.3.4/cvxpygen.egg-info/top_level.txt
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.049264 cvxpygen-0.3.4/cvxpygen_custom_diff_bak/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-10-11 21:20:44.000000 cvxpygen-0.3.4/cvxpygen_custom_diff_bak/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    24706 2024-03-01 01:55:21.000000 cvxpygen-0.3.4/cvxpygen_custom_diff_bak/cpg.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     2583 2024-03-01 00:54:56.000000 cvxpygen-0.3.4/cvxpygen_custom_diff_bak/mappings.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    49890 2024-01-27 00:38:16.000000 cvxpygen-0.3.4/cvxpygen_custom_diff_bak/solvers.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.051241 cvxpygen-0.3.4/cvxpygen_custom_diff_bak/template/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:35:19.000000 cvxpygen-0.3.4/cvxpygen_custom_diff_bak/template/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4063 2023-10-11 00:29:46.000000 cvxpygen-0.3.4/cvxpygen_custom_diff_bak/template/setup.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)    86804 2024-03-01 19:31:11.000000 cvxpygen-0.3.4/cvxpygen_custom_diff_bak/utils.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)      144 2023-08-31 23:29:55.000000 cvxpygen-0.3.4/environment.yml
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.053047 cvxpygen-0.3.4/nonneg_LS/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2024-04-22 22:51:26.000000 cvxpygen-0.3.4/nonneg_LS/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3200 2024-04-22 22:51:26.000000 cvxpygen-0.3.4/nonneg_LS/cpg_solver.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4179 2024-04-22 22:51:26.000000 cvxpygen-0.3.4/nonneg_LS/setup.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.054764 cvxpygen-0.3.4/nonneg_LS_bak/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-10-12 18:22:23.000000 cvxpygen-0.3.4/nonneg_LS_bak/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3121 2023-10-12 18:22:36.000000 cvxpygen-0.3.4/nonneg_LS_bak/cpg_solver.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4089 2023-10-12 18:22:36.000000 cvxpygen-0.3.4/nonneg_LS_bak/setup.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.056429 cvxpygen-0.3.4/nonneg_LS_proto/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2024-03-01 02:07:13.000000 cvxpygen-0.3.4/nonneg_LS_proto/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3750 2024-03-01 02:07:13.000000 cvxpygen-0.3.4/nonneg_LS_proto/cpg_solver.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4242 2024-03-01 02:07:13.000000 cvxpygen-0.3.4/nonneg_LS_proto/setup.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.058166 cvxpygen-0.3.4/proto/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-10-10 01:40:46.000000 cvxpygen-0.3.4/proto/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3198 2023-10-10 01:40:46.000000 cvxpygen-0.3.4/proto/cpg_solver.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4086 2023-10-10 01:40:46.000000 cvxpygen-0.3.4/proto/setup.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)       79 2024-04-23 00:28:31.069715 cvxpygen-0.3.4/setup.cfg
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     1410 2024-04-23 00:27:45.000000 cvxpygen-0.3.4/setup.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.060142 cvxpygen-0.3.4/sp_compiled_CLARABEL/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 22:54:03.000000 cvxpygen-0.3.4/sp_compiled_CLARABEL/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3490 2024-04-21 22:54:03.000000 cvxpygen-0.3.4/sp_compiled_CLARABEL/cpg_solver.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4179 2024-04-21 22:54:03.000000 cvxpygen-0.3.4/sp_compiled_CLARABEL/setup.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.061351 cvxpygen-0.3.4/sp_compiled_E/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 22:59:08.000000 cvxpygen-0.3.4/sp_compiled_E/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4063 2024-04-21 22:59:08.000000 cvxpygen-0.3.4/sp_compiled_E/setup.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.063035 cvxpygen-0.3.4/sp_compiled_ECOS/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 22:59:32.000000 cvxpygen-0.3.4/sp_compiled_ECOS/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3487 2024-04-21 22:59:32.000000 cvxpygen-0.3.4/sp_compiled_ECOS/cpg_solver.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4370 2024-04-21 22:59:32.000000 cvxpygen-0.3.4/sp_compiled_ECOS/setup.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.064947 cvxpygen-0.3.4/sp_compiled_SCS/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2024-04-21 21:41:52.000000 cvxpygen-0.3.4/sp_compiled_SCS/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3403 2024-04-21 21:41:52.000000 cvxpygen-0.3.4/sp_compiled_SCS/cpg_solver.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4161 2024-04-21 21:41:52.000000 cvxpygen-0.3.4/sp_compiled_SCS/setup.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.066587 cvxpygen-0.3.4/test/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)        0 2023-04-02 15:02:12.000000 cvxpygen-0.3.4/test/__init__.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3590 2023-04-02 15:02:12.000000 cvxpygen-0.3.4/test/cpg_solver.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4275 2023-04-02 15:02:12.000000 cvxpygen-0.3.4/test/setup.py
+drwxr-xr-x   0 maximilianschaller   (501) staff       (20)        0 2024-04-23 00:28:31.068232 cvxpygen-0.3.4/tests/
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     4488 2023-10-11 00:39:44.000000 cvxpygen-0.3.4/tests/test_E2E_LP.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     8793 2024-04-23 00:27:37.000000 cvxpygen-0.3.4/tests/test_E2E_QP.py
+-rw-r--r--   0 maximilianschaller   (501) staff       (20)     3831 2023-10-11 00:41:18.000000 cvxpygen-0.3.4/tests/test_E2E_SOCP.py
```

### Comparing `cvxpygen-0.3.3/DEBUG/cpg_solver.py` & `cvxpygen-0.3.4/DEBUG/cpg_solver.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/DEBUG/setup.py` & `cvxpygen-0.3.4/DEBUG/setup.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/LICENSE` & `cvxpygen-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/MANIFEST.in` & `cvxpygen-0.3.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/MPC_code/cpg_solver.py` & `cvxpygen-0.3.4/MPC_code/cpg_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 """
-Auto-generated by CVXPYgen on April 21, 2024 at 15:56:10.
+Auto-generated by CVXPYgen on April 22, 2024 at 16:37:30.
 Content: Custom solve method for CVXPY interface.
 """
 
 import time
 import warnings
 import numpy as np
 from cvxpy.reductions import Solution
@@ -55,15 +55,15 @@
     prob.var_dict['X'].save_value(np.array(res.cpg_prim.X).reshape((6, 11), order='F'))
     prob.var_dict['U'].save_value(np.array(res.cpg_prim.U).reshape((3, 10), order='F'))
     prob.constraints[0].save_dual_value(np.array(res.cpg_dual.d0).reshape((6, 10), order='F'))
     prob.constraints[1].save_dual_value(np.array(res.cpg_dual.d1).reshape((3, 10), order='F'))
     prob.constraints[2].save_dual_value(np.array(res.cpg_dual.d2).reshape(6))
 
     # store additional solver information in problem object
-    prob._status = "%d (for description visit https://github.com/embotech/ecos/wiki/Usage-from-C)" % res.cpg_info.status
+    prob._status = "%d (for description visit https://oxfordcontrol.github.io/ClarabelDocs/)" % res.cpg_info.status
     if abs(res.cpg_info.obj_val) == 1e30:
         prob._value = np.sign(res.cpg_info.obj_val) * np.inf
     else:
         prob._value = res.cpg_info.obj_val
     primal_vars = {var.id: var.value for var in prob.variables()}
     dual_vars = {c.id: c.dual_value for c in prob.constraints}
     solver_specific_stats = {'obj_val': res.cpg_info.obj_val,
@@ -73,10 +73,10 @@
                              'dua_res': res.cpg_info.dua_res,
                              'time': res.cpg_info.time}
     attr = {'solve_time': t1 - t0, 'solver_specific_stats': solver_specific_stats, 'num_iters': res.cpg_info.iter}
     prob._solution = Solution(prob.status, prob.value, primal_vars, dual_vars, attr)
     results_dict = {'solver_specific_stats': solver_specific_stats,
                     'num_iters': res.cpg_info.iter,
                     'solve_time': t1 - t0}
-    prob._solver_stats = SolverStats(results_dict, 'ECOS')
+    prob._solver_stats = SolverStats(results_dict, 'CLARABEL')
 
     return prob.value
```

### Comparing `cvxpygen-0.3.3/MPC_code/setup.py` & `cvxpygen-0.3.4/sp_compiled_ECOS/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 """
-Auto-generated by CVXPYgen on April 21, 2024 at 15:56:10.
+Auto-generated by CVXPYgen on April 21, 2024 at 15:59:32.
 Content: Setuptools for compilation of Python wrapper.
 """
 
 import os
 import sys
 from glob import glob
 from platform import system
```

### Comparing `cvxpygen-0.3.3/PKG-INFO` & `cvxpygen-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxpygen
-Version: 0.3.3
+Version: 0.3.4
 Summary: Code generation with CVXPY
 Home-page: https://github.com/cvxgrp/cvxpygen
 Author: Maximilian Schaller, Goran Banjac, Bartolomeo Stellato, Steven Diamond, Akshay Agrawal, Stephen Boyd
 Author-email: mschall@stanford.edu, goranbanjac1989@gmail.com, bstellato@princeton.edu, diamond@cs.stanford.edu, akshayka@cs.stanford.edu, boyd@stanford.edu
 License: Apache License, Version 2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cvxpygen-0.3.3/README.md` & `cvxpygen-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/cpg.py` & `cvxpygen-0.3.4/cvxpygen/cpg.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/mappings.py` & `cvxpygen-0.3.4/cvxpygen/mappings.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/.clang-format` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/.clang-format`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/CMakeLists.txt` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/Cargo.toml` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/block_concatenate.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/block_concatenate.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/core.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/core.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/matrix_math.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/matrix_math.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/utils.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/csc/utils.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/blas.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/blas.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/blaslike_traits.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/blaslike_traits.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/block_concatenate.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/block_concatenate.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/cholesky.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/cholesky.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/core.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/core.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/gemm.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/gemm.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/gemv.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/gemv.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/kron.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/kron.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/matrix_math.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/matrix_math.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/svd.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/svd.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/syevr.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/syevr.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/symv.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/symv.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/syr2k.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/syr2k.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/syrk.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/dense/syrk.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/densesym3x3/mod.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/densesym3x3/mod.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/error_types.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/error_types.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/floats.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/floats.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/math_traits.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/math_traits.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/matrix_traits.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/matrix_traits.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/matrix_types.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/matrix_types.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/mod.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/mod.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/scalarmath.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/scalarmath.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/vecmath.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/algebra/vecmath.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/lib.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/qdldl/qdldl.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/qdldl/qdldl.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/qdldl/test.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/qdldl/test.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/compositecone.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/compositecone.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/expcone.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/expcone.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/genpowcone.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/genpowcone.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/mod.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/mod.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/nonnegativecone.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/nonnegativecone.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/nonsymmetric_common.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/nonsymmetric_common.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/powcone.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/powcone.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/psdtrianglecone.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/psdtrianglecone.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/socone.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/socone.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/supportedcone.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/supportedcone.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/symmetric_common.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/symmetric_common.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/zerocone.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/cones/zerocone.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/datamaps.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/datamaps.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/directldlkktsolver.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/directldlkktsolver.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/kkt_assembly.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/kkt_assembly.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/qdldl.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/qdldl.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/mod.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/kktsolvers/direct/quasidef/mod.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/solver.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/solver.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/traits.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/core/traits.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/equilibration.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/equilibration.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/info.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/info.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/info_print.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/info_print.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/kktsystem.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/kktsystem.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/mod.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/mod.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/presolver.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/presolver.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/problemdata.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/problemdata.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/residuals.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/residuals.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/settings.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/settings.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/solution.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/solution.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/solver.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/solver.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/variables.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/implementations/default/variables.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/mod.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/mod.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/utils/atomic.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/utils/atomic.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/utils/infbounds.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/solver/utils/infbounds.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/timers/timers.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/Clarabel.rs/src/timers/timers.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/LICENSE.md` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/README.md` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/README.md`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/include/c/CscMatrix.h` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/include/c/CscMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/include/c/DefaultInfo.h` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/include/c/DefaultInfo.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/include/c/DefaultSettings.h` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/include/c/DefaultSettings.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/include/c/DefaultSolution.h` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/include/c/DefaultSolution.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/include/c/DefaultSolver.h` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/include/c/DefaultSolver.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/include/c/SupportedConeT.h` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/include/c/SupportedConeT.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/CMakeLists.txt` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/Cargo.toml` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/Cargo.toml`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/algebra.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/algebra.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/core.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/core.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/info.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/info.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/settings.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/settings.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/solution.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/solution.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/solver.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/solver/implementations/default/solver.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/utils/csc_matrix.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/utils/csc_matrix.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/utils/mod.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/utils/supported_cones_T.rs` & `cvxpygen-0.3.4/cvxpygen/solvers/Clarabel.cpp/rust_wrapper/src/utils/supported_cones_T.rs`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/.DS_Store` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/.DS_Store`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/CMakeLists.txt` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/CONTRIBUTING.md` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/COPYING` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/COPYING`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/Makefile` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/Makefile`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/README.md` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/README.md`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/README.pdf` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/README.pdf`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/ecos.mk` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/ecos.mk`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/ecos_bb/ecos_bb.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/ecos_bb/ecos_bb.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/ecos_bb/ecos_bb_preproc.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/ecos_bb/ecos_bb_preproc.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/SuiteSparse_config/SuiteSparse_config.h` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/SuiteSparse_config/SuiteSparse_config.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/Makefile` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/Makefile`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/README.txt` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/README.txt`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/include/amd.h` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/include/amd.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/include/amd_internal.h` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/include/amd_internal.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_1.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_1.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_2.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_2.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_aat.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_aat.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_control.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_control.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_defaults.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_defaults.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_dump.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_dump.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_global.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_global.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_info.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_info.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_order.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_order.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_post_tree.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_post_tree.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_postorder.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_postorder.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_preprocess.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_preprocess.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/amd/src/amd_valid.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/amd/src/amd_valid.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/ldl/Makefile` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/ldl/Makefile`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/ldl/README.txt` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/ldl/README.txt`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/ldl/include/ldl.h` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/ldl/include/ldl.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/external/ldl/src/ldl.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/external/ldl/src/ldl.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/cone.h` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/cone.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/ctrlc.h` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/ctrlc.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/data.h` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/data.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/ecos.h` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/ecos.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/ecos_bb.h` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/ecos_bb.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/equil.h` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/equil.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/expcone.h` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/expcone.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/glblopts.h` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/glblopts.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/kkt.h` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/kkt.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/spla.h` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/spla.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/splamm.h` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/splamm.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/timer.h` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/timer.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/include/wright_omega.h` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/include/wright_omega.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/cone.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/cone.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/ctrlc.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/ctrlc.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/ecos.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/ecos.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/equil.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/equil.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/expcone.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/expcone.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/kkt.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/kkt.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/preproc.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/preproc.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/runecos.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/runecos.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/runecos_exp.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/runecos_exp.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/spla.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/spla.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/splamm.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/splamm.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/timer.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/timer.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/ecos/src/wright_omega.c` & `cvxpygen-0.3.4/cvxpygen/solvers/ecos/src/wright_omega.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/osqp-python/LICENSE` & `cvxpygen-0.3.4/cvxpygen/solvers/osqp-python/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/.DS_Store` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/.DS_Store`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/CITATION.cff` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/CITATION.cff`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/CMakeLists.txt` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/LICENSE.txt` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/Makefile` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/Makefile`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/README.md` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/README.md`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/cmake/AddInstallRPATHSupport.cmake` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/cmake/AddInstallRPATHSupport.cmake`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/cmake/AddUninstallTarget.cmake` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/cmake/AddUninstallTarget.cmake`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/cmake/InstallBasicPackageFiles.cmake` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/cmake/InstallBasicPackageFiles.cmake`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/include/aa.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/include/aa.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/include/cones.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/include/cones.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/include/ctrlc.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/include/ctrlc.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/include/glbopts.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/include/glbopts.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/include/linalg.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/include/linalg.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/include/linsys.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/include/linsys.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/include/rw.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/include/rw.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/include/scs.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/include/scs.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/include/scs_blas.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/include/scs_blas.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/include/scs_work.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/include/scs_work.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/include/util.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/include/util.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/cpu/direct/private.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/cpu/direct/private.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/cpu/direct/private.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/cpu/direct/private.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/cpu/indirect/private.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/cpu/indirect/private.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/cpu/indirect/private.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/cpu/indirect/private.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/csparse.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/csparse.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/csparse.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/csparse.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/LICENSE.txt` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/SuiteSparse_config.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/SuiteSparse_config.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/SuiteSparse_config.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/SuiteSparse_config.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_1.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_1.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_2.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_2.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_aat.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_aat.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_control.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_control.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_defaults.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_defaults.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_dump.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_dump.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_global.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_global.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_info.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_info.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_internal.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_internal.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_order.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_order.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_post_tree.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_post_tree.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_postorder.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_postorder.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_preprocess.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_preprocess.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/amd_valid.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/amd_valid.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/amd/changes` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/amd/changes`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/qdldl/LICENSE` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/qdldl/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/qdldl/README.md` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/qdldl/README.md`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl_types.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/external/qdldl/qdldl_types.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/scs_matrix.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/scs_matrix.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/linsys/scs_matrix.h` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/linsys/scs_matrix.h`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/scs.mk` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/scs.mk`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/src/aa.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/src/aa.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/src/cones.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/src/cones.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/src/ctrlc.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/src/ctrlc.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/src/linalg.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/src/linalg.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/src/normalize.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/src/normalize.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/src/rw.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/src/rw.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/src/scs.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/src/scs.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers/scs/src/util.c` & `cvxpygen-0.3.4/cvxpygen/solvers/scs/src/util.c`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/solvers.py` & `cvxpygen-0.3.4/cvxpygen/solvers.py`

 * *Files 2% similar despite different names*

```diff
@@ -985,17 +985,21 @@
                 f.write('\nfind_package(LAPACK REQUIRED)')
                 link_libraries = 'libclarabel_c_static ${BLAS_LIBRARIES} ${LAPACK_LIBRARIES}'
             else:
                 link_libraries = 'libclarabel_c_static'
             f.write(f'\ntarget_link_libraries(cpg_example PRIVATE {link_libraries})')
             f.write(f'\ntarget_link_libraries(cpg PRIVATE {link_libraries})\n')
 
-        # remove examples target from Clarabel.cpp/CMakeLists.txt
+        # remove examples target from Clarabel.cpp/CMakeLists.txt and set build type to Release
+        replacements = [
+            ('add_subdirectory(examples)', '# add_subdirectory(examples)'),
+            ('set(CMAKE_C_STANDARD_REQUIRED True)', 'set(CMAKE_C_STANDARD_REQUIRED True)\n\n# set build type to Release\nset(CMAKE_BUILD_TYPE Release)')
+        ]
         read_write_file(os.path.join(code_dir, 'c', 'solver_code', 'CMakeLists.txt'),
-                        lambda x: x.replace('add_subdirectory(examples)', '# add_subdirectory(examples)'))
+                        lambda x: multiple_replace(x, replacements))
 
         # add sdp flag
         if is_sdp:
             read_write_file(os.path.join(code_dir, 'c', 'solver_code', 'CMakeLists.txt'),
                             lambda x: x.replace('set(CLARABEL_FEATURE_SDP "none"', 'set(CLARABEL_FEATURE_SDP "sdp-openblas"'))
 
         # adjust paths in Clarabel.cpp/rust_wrapper/CMakeLists.txt
@@ -1009,15 +1013,15 @@
         # adjust Clarabel
         read_write_file(os.path.join(code_dir, 'c', 'solver_code', 'include', 'Clarabel'),
                         lambda x: x.replace('cpp/', 'c/'))
 
         # adjust setup.py
         read_write_file(os.path.join(code_dir, 'setup.py'),
                         lambda x: x.replace("extra_objects=[cpg_lib])",
-                                            "extra_objects=[cpg_lib, os.path.join(cpg_dir, 'solver_code', 'rust_wrapper', 'target', 'debug', 'libclarabel_c.a')])"))
+                                            "extra_objects=[cpg_lib, os.path.join(cpg_dir, 'solver_code', 'rust_wrapper', 'target', 'release', 'libclarabel_c.a')])"))
 
     
     def declare_workspace(self, f, prefix, parameter_canon) -> None:
         f.write('\n// Clarabel workspace\n')
         f.write(f'extern ClarabelCscMatrix {prefix}P;\n')
         f.write(f'extern ClarabelCscMatrix {prefix}A;\n')
         f.write(f'extern ClarabelSupportedConeT {prefix}cones[{self.canon_constants["n_cone_types"]}];\n')
```

### Comparing `cvxpygen-0.3.3/cvxpygen/template/CMakeLists.txt` & `cvxpygen-0.3.4/cvxpygen/template/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/template/LICENSE` & `cvxpygen-0.3.4/cvxpygen/template/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/template/README.html` & `cvxpygen-0.3.4/cvxpygen/template/README.html`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/template/setup.py` & `cvxpygen-0.3.4/cvxpygen/template/setup.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen/utils.py` & `cvxpygen-0.3.4/cvxpygen/utils.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen.egg-info/PKG-INFO` & `cvxpygen-0.3.4/cvxpygen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxpygen
-Version: 0.3.3
+Version: 0.3.4
 Summary: Code generation with CVXPY
 Home-page: https://github.com/cvxgrp/cvxpygen
 Author: Maximilian Schaller, Goran Banjac, Bartolomeo Stellato, Steven Diamond, Akshay Agrawal, Stephen Boyd
 Author-email: mschall@stanford.edu, goranbanjac1989@gmail.com, bstellato@princeton.edu, diamond@cs.stanford.edu, akshayka@cs.stanford.edu, boyd@stanford.edu
 License: Apache License, Version 2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cvxpygen-0.3.3/cvxpygen.egg-info/SOURCES.txt` & `cvxpygen-0.3.4/cvxpygen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen_custom_diff_bak/cpg.py` & `cvxpygen-0.3.4/cvxpygen_custom_diff_bak/cpg.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen_custom_diff_bak/mappings.py` & `cvxpygen-0.3.4/cvxpygen_custom_diff_bak/mappings.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen_custom_diff_bak/solvers.py` & `cvxpygen-0.3.4/cvxpygen_custom_diff_bak/solvers.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen_custom_diff_bak/template/setup.py` & `cvxpygen-0.3.4/cvxpygen_custom_diff_bak/template/setup.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/cvxpygen_custom_diff_bak/utils.py` & `cvxpygen-0.3.4/cvxpygen_custom_diff_bak/utils.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/nonneg_LS/cpg_solver.py` & `cvxpygen-0.3.4/nonneg_LS/cpg_solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 """
-Auto-generated by CVXPYgen on April 21, 2024 at 13:25:37.
+Auto-generated by CVXPYgen on April 22, 2024 at 15:51:26.
 Content: Custom solve method for CVXPY interface.
 """
 
 import time
 import warnings
 import numpy as np
 from cvxpy.reductions import Solution
@@ -57,15 +57,15 @@
 
     # store solution in problem object
     prob._clear_solution()
     prob.var_dict['x'].save_value(np.array(res.cpg_prim.x).reshape(2))
     prob.constraints[0].save_dual_value(np.array(res.cpg_dual.d0).reshape(2))
 
     # store additional solver information in problem object
-    prob._status = "%d (for description visit https://github.com/embotech/ecos/wiki/Usage-from-C)" % res.cpg_info.status
+    prob._status = "%d (for description visit https://oxfordcontrol.github.io/ClarabelDocs/)" % res.cpg_info.status
     if abs(res.cpg_info.obj_val) == 1e30:
         prob._value = np.sign(res.cpg_info.obj_val) * np.inf
     else:
         prob._value = res.cpg_info.obj_val
     primal_vars = {var.id: var.value for var in prob.variables()}
     dual_vars = {c.id: c.dual_value for c in prob.constraints}
     solver_specific_stats = {'obj_val': res.cpg_info.obj_val,
@@ -75,10 +75,10 @@
                              'dua_res': res.cpg_info.dua_res,
                              'time': res.cpg_info.time}
     attr = {'solve_time': t1 - t0, 'solver_specific_stats': solver_specific_stats, 'num_iters': res.cpg_info.iter}
     prob._solution = Solution(prob.status, prob.value, primal_vars, dual_vars, attr)
     results_dict = {'solver_specific_stats': solver_specific_stats,
                     'num_iters': res.cpg_info.iter,
                     'solve_time': t1 - t0}
-    prob._solver_stats = SolverStats(results_dict, 'ECOS')
+    prob._solver_stats = SolverStats(results_dict, 'CLARABEL')
 
     return prob.value
```

### Comparing `cvxpygen-0.3.3/nonneg_LS/setup.py` & `cvxpygen-0.3.4/test/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 """
-Auto-generated by CVXPYgen on April 21, 2024 at 13:25:37.
+Auto-generated by CVXPYgen on April 02, 2023 at 17:02:12.
 Content: Setuptools for compilation of Python wrapper.
 """
 
 import os
 import sys
 from glob import glob
 from platform import system
@@ -26,15 +26,14 @@
         import pybind11
         return pybind11.get_include(self.user)
 
 
 # Add parameters to cmake_args and define_macros
 cmake_args = ['-DCMAKE_POSITION_INDEPENDENT_CODE=ON', '-Wno-dev']
 if system() == 'Windows':
-    cmake_args.append('-DCMAKE_PREFIX_PATH=C:/vcpkg/packages/eigen3_x64-windows/share/eigen3')
     # try to find installation of Visual Studio and set as CMake generator, otherwise let CMake choose default generator
     vs_versions = []
     vswhere_exe = 'C:\\Program Files (x86)\\Microsoft Visual Studio\\Installer\\vswhere.exe'
     if os.path.isfile(vswhere_exe):
         out = check_output(vswhere_exe)
         out = out.decode('utf-8')
         out = out.splitlines()
```

### Comparing `cvxpygen-0.3.3/nonneg_LS_bak/cpg_solver.py` & `cvxpygen-0.3.4/nonneg_LS_bak/cpg_solver.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/nonneg_LS_bak/setup.py` & `cvxpygen-0.3.4/nonneg_LS_bak/setup.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/nonneg_LS_proto/cpg_solver.py` & `cvxpygen-0.3.4/nonneg_LS_proto/cpg_solver.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/nonneg_LS_proto/setup.py` & `cvxpygen-0.3.4/nonneg_LS_proto/setup.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/proto/cpg_solver.py` & `cvxpygen-0.3.4/proto/cpg_solver.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/proto/setup.py` & `cvxpygen-0.3.4/proto/setup.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/setup.py` & `cvxpygen-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
-MICRO = 3
+MICRO = 4
 VERSION = '%d.%d.%d' % (MAJOR, MINOR, MICRO)
 
 
 def readme():
     with open('README.md') as f:
         content = f.read()
     return content[:content.find('## Tests')]
```

### Comparing `cvxpygen-0.3.3/sp_compiled_CLARABEL/cpg_solver.py` & `cvxpygen-0.3.4/sp_compiled_CLARABEL/cpg_solver.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/sp_compiled_CLARABEL/setup.py` & `cvxpygen-0.3.4/sp_compiled_CLARABEL/setup.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/sp_compiled_E/setup.py` & `cvxpygen-0.3.4/sp_compiled_E/setup.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/sp_compiled_ECOS/cpg_solver.py` & `cvxpygen-0.3.4/sp_compiled_ECOS/cpg_solver.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/sp_compiled_ECOS/setup.py` & `cvxpygen-0.3.4/sp_compiled_SCS/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 """
-Auto-generated by CVXPYgen on April 21, 2024 at 15:59:32.
+Auto-generated by CVXPYgen on April 21, 2024 at 14:41:52.
 Content: Setuptools for compilation of Python wrapper.
 """
 
 import os
 import sys
 from glob import glob
 from platform import system
@@ -94,17 +94,15 @@
 
 
 cpg = Extension('cpg_module',
                 sources=glob(os.path.join('cpp', 'src', '*.cpp')),
                 include_dirs=['c',
                               os.path.join('cpp', 'include'),
                               os.path.join('c', 'solver_code', 'include'),
-                              os.path.join('c', 'solver_code', 'external', 'SuiteSparse_config'),
-                              os.path.join('c', 'solver_code', 'external', 'amd', 'include'),
-                              os.path.join('c', 'solver_code', 'external', 'ldl', 'include'),
+                              os.path.join('c', 'solver_code', 'linsys'),
                               get_pybind_include(),
                               get_pybind_include(user=False)],
                 language='c++',
                 extra_compile_args=extra_compile_args,
                 extra_objects=[cpg_lib])
 
 
@@ -112,12 +110,12 @@
       description='Python wrapper around C/C++ code generated by CVXPYGEN',
       long_description='Python wrapper around C/C++ code generated by CVXPYGEN',
       long_description_content_type='text/markdown',
       package_dir={'cpg': 'module'},
       include_package_data=False,
       setup_requires=["setuptools>=18.0", "pybind11"],
       install_requires=["cvxpy >= 1.1", "numpy >= 1.7", "scipy >= 0.13.2"],
-      license='GPL 3.0',
+      license='Apache 2.0',
       url="https://github.com/cvxgrp/codegen",
       cmdclass={'build_ext': build_ext_cpg},
       ext_modules=[cpg],
       )
```

### Comparing `cvxpygen-0.3.3/sp_compiled_SCS/cpg_solver.py` & `cvxpygen-0.3.4/sp_compiled_SCS/cpg_solver.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/sp_compiled_SCS/setup.py` & `cvxpygen-0.3.4/nonneg_LS/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 """
-Auto-generated by CVXPYgen on April 21, 2024 at 14:41:52.
+Auto-generated by CVXPYgen on April 22, 2024 at 15:51:26.
 Content: Setuptools for compilation of Python wrapper.
 """
 
 import os
 import sys
 from glob import glob
 from platform import system
@@ -94,20 +94,19 @@
 
 
 cpg = Extension('cpg_module',
                 sources=glob(os.path.join('cpp', 'src', '*.cpp')),
                 include_dirs=['c',
                               os.path.join('cpp', 'include'),
                               os.path.join('c', 'solver_code', 'include'),
-                              os.path.join('c', 'solver_code', 'linsys'),
                               get_pybind_include(),
                               get_pybind_include(user=False)],
                 language='c++',
                 extra_compile_args=extra_compile_args,
-                extra_objects=[cpg_lib])
+                extra_objects=[cpg_lib, os.path.join(cpg_dir, 'solver_code', 'rust_wrapper', 'target', 'debug', 'libclarabel_c.a')])
 
 
 setup(name='cpg_module',
       description='Python wrapper around C/C++ code generated by CVXPYGEN',
       long_description='Python wrapper around C/C++ code generated by CVXPYGEN',
       long_description_content_type='text/markdown',
       package_dir={'cpg': 'module'},
```

### Comparing `cvxpygen-0.3.3/test/cpg_solver.py` & `cvxpygen-0.3.4/test/cpg_solver.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/test/setup.py` & `cvxpygen-0.3.4/MPC_code/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 """
-Auto-generated by CVXPYgen on April 02, 2023 at 17:02:12.
+Auto-generated by CVXPYgen on April 22, 2024 at 16:37:30.
 Content: Setuptools for compilation of Python wrapper.
 """
 
 import os
 import sys
 from glob import glob
 from platform import system
@@ -26,14 +26,15 @@
         import pybind11
         return pybind11.get_include(self.user)
 
 
 # Add parameters to cmake_args and define_macros
 cmake_args = ['-DCMAKE_POSITION_INDEPENDENT_CODE=ON', '-Wno-dev']
 if system() == 'Windows':
+    cmake_args.append('-DCMAKE_PREFIX_PATH=C:/vcpkg/packages/eigen3_x64-windows/share/eigen3')
     # try to find installation of Visual Studio and set as CMake generator, otherwise let CMake choose default generator
     vs_versions = []
     vswhere_exe = 'C:\\Program Files (x86)\\Microsoft Visual Studio\\Installer\\vswhere.exe'
     if os.path.isfile(vswhere_exe):
         out = check_output(vswhere_exe)
         out = out.decode('utf-8')
         out = out.splitlines()
@@ -93,30 +94,27 @@
 
 
 cpg = Extension('cpg_module',
                 sources=glob(os.path.join('cpp', 'src', '*.cpp')),
                 include_dirs=['c',
                               os.path.join('cpp', 'include'),
                               os.path.join('c', 'solver_code', 'include'),
-                              os.path.join('c', 'solver_code', 'external', 'SuiteSparse_config'),
-                              os.path.join('c', 'solver_code', 'external', 'amd', 'include'),
-                              os.path.join('c', 'solver_code', 'external', 'ldl', 'include'),
                               get_pybind_include(),
                               get_pybind_include(user=False)],
                 language='c++',
                 extra_compile_args=extra_compile_args,
-                extra_objects=[cpg_lib])
+                extra_objects=[cpg_lib, os.path.join(cpg_dir, 'solver_code', 'rust_wrapper', 'target', 'release', 'libclarabel_c.a')])
 
 
 setup(name='cpg_module',
       description='Python wrapper around C/C++ code generated by CVXPYGEN',
       long_description='Python wrapper around C/C++ code generated by CVXPYGEN',
       long_description_content_type='text/markdown',
       package_dir={'cpg': 'module'},
       include_package_data=False,
       setup_requires=["setuptools>=18.0", "pybind11"],
       install_requires=["cvxpy >= 1.1", "numpy >= 1.7", "scipy >= 0.13.2"],
-      license='GPL 3.0',
+      license='Apache 2.0',
       url="https://github.com/cvxgrp/codegen",
       cmdclass={'build_ext': build_ext_cpg},
       ext_modules=[cpg],
       )
```

### Comparing `cvxpygen-0.3.3/tests/test_E2E_LP.py` & `cvxpygen-0.3.4/tests/test_E2E_LP.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/tests/test_E2E_QP.py` & `cvxpygen-0.3.4/tests/test_E2E_QP.py`

 * *Files identical despite different names*

### Comparing `cvxpygen-0.3.3/tests/test_E2E_SOCP.py` & `cvxpygen-0.3.4/tests/test_E2E_SOCP.py`

 * *Files identical despite different names*

