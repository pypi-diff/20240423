# Comparing `tmp/opytimal-0.6.0.tar.gz` & `tmp/opytimal-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opytimal-0.6.0.tar", last modified: Tue Apr 23 12:58:17 2024, max compression
+gzip compressed data, was "opytimal-0.6.1.tar", last modified: Tue Apr 23 13:17:02 2024, max compression
```

## Comparing `opytimal-0.6.0.tar` & `opytimal-0.6.1.tar`

### file list

```diff
@@ -1,101 +1,44 @@
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:58:17.886665 opytimal-0.6.0/
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     7048 2023-09-12 14:54:54.000000 opytimal-0.6.0/LICENSE
--rw-r--r--   0 natanael  (1001) natanael  (1001)     1080 2024-04-23 12:58:17.886665 opytimal-0.6.0/PKG-INFO
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      488 2023-11-17 15:48:02.000000 opytimal-0.6.0/README.md
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:58:17.882665 opytimal-0.6.0/opytimal/
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     2063 2024-04-23 12:58:14.000000 opytimal-0.6.0/opytimal/__init__.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      613 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/_vars.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    49923 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/analytical.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     9266 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/arrays.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    12180 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/decorator.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:58:17.882665 opytimal-0.6.0/opytimal/demos/
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      752 2023-11-17 17:30:06.000000 opytimal-0.6.0/opytimal/demos/__init__.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    29176 2023-11-17 16:51:20.000000 opytimal-0.6.0/opytimal/demos/optHeat1D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    26417 2023-11-17 16:51:20.000000 opytimal-0.6.0/opytimal/demos/optHeat2D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    22362 2023-11-17 16:51:20.000000 opytimal-0.6.0/opytimal/demos/optPoisson1D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    24873 2023-11-17 16:51:20.000000 opytimal-0.6.0/opytimal/demos/optPoisson2D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    23922 2023-11-17 16:51:20.000000 opytimal-0.6.0/opytimal/demos/optPoisson3D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    27362 2023-11-17 16:51:20.000000 opytimal-0.6.0/opytimal/demos/optStokes2D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    25154 2023-11-17 16:51:20.000000 opytimal-0.6.0/opytimal/demos/optStokes3D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      841 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/dicts.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:58:17.882665 opytimal-0.6.0/opytimal/dolfin/
--rw-r--r--   0 natanael  (1001) natanael  (1001)     9500 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/__init__.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:58:17.882665 opytimal-0.6.0/opytimal/dolfin/common/
--rw-r--r--   0 natanael  (1001) natanael  (1001)      147 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/common/__init__.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)    16151 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/common/plotting.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     2377 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/common/timer.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:58:17.882665 opytimal-0.6.0/opytimal/dolfin/fem/
--rw-r--r--   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/fem/__init__.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     7426 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/fem/adaptivesolving.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)    18500 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/fem/assembling.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     5225 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/fem/dirichletbc.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     3445 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/fem/errorcontrolgenerator.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     3787 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/fem/form.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     4968 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/fem/formmanipulations.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     2543 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/fem/interpolation.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     3189 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/fem/multimeshdirichletbc.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)    10449 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/fem/norms.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     8408 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/fem/problem.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     6417 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/fem/projection.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     1556 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/fem/solvers.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)    19008 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/fem/solving.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:58:17.882665 opytimal-0.6.0/opytimal/dolfin/function/
--rw-r--r--   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/function/__init__.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     4417 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/function/argument.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     4392 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/function/constant.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)    15995 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/function/expression.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)    21184 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/function/function.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     9303 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/function/functionspace.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     5237 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/function/jit.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     9319 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/function/multimeshfunction.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     5537 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/function/multimeshfunctionspace.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     7294 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/function/specialfunctions.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:58:17.882665 opytimal-0.6.0/opytimal/dolfin/io/
--rw-r--r--   0 natanael  (1001) natanael  (1001)     1093 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/io/__init__.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:58:17.882665 opytimal-0.6.0/opytimal/dolfin/jit/
--rw-r--r--   0 natanael  (1001) natanael  (1001)      564 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/jit/__init__.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     6538 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/jit/jit.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     3552 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/jit/pybind11jit.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:58:17.886665 opytimal-0.6.0/opytimal/dolfin/la/
--rw-r--r--   0 natanael  (1001) natanael  (1001)     2150 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/la/__init__.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     2148 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/la/solver.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:58:17.886665 opytimal-0.6.0/opytimal/dolfin/mesh/
--rw-r--r--   0 natanael  (1001) natanael  (1001)     3083 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/mesh/__init__.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     6123 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/mesh/ale.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)      633 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/mesh/meshfunction.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)      703 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/mesh/meshvaluecollection.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     3556 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/mesh/subdomain.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     4148 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/mesh/svgtools.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)      874 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/mesh/ufl_util.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:58:17.886665 opytimal-0.6.0/opytimal/dolfin/multistage/
--rw-r--r--   0 natanael  (1001) natanael  (1001)      588 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/multistage/__init__.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     4886 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/multistage/factorize.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)    29902 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/multistage/multistagescheme.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     1980 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/multistage/multistagesolvers.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)    22460 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/multistage/rushlarsenschemes.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:58:17.886665 opytimal-0.6.0/opytimal/dolfin/parameter/
--rw-r--r--   0 natanael  (1001) natanael  (1001)     2600 2024-04-23 12:11:01.000000 opytimal-0.6.0/opytimal/dolfin/parameter/__init__.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    63651 2023-11-17 13:15:29.000000 opytimal-0.6.0/opytimal/fenics.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     1208 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/files.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      321 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/functions.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      105 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/mathFunctions.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    13269 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/meshes.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      798 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/modules.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      339 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/numeric.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      912 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/parallel.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    89570 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/plots.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     3695 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/profiler.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     2090 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/settings.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    21633 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/strings.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      447 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/symbols.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      344 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/tables.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     1546 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/tests.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     2504 2023-11-17 11:54:51.000000 opytimal-0.6.0/opytimal/types.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:58:17.886665 opytimal-0.6.0/opytimal.egg-info/
--rw-r--r--   0 natanael  (1001) natanael  (1001)     1080 2024-04-23 12:58:17.000000 opytimal-0.6.0/opytimal.egg-info/PKG-INFO
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     2573 2024-04-23 12:58:17.000000 opytimal-0.6.0/opytimal.egg-info/SOURCES.txt
--rw-rw-r--   0 natanael  (1001) natanael  (1001)        1 2024-04-23 12:58:17.000000 opytimal-0.6.0/opytimal.egg-info/dependency_links.txt
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      276 2024-04-23 12:58:17.000000 opytimal-0.6.0/opytimal.egg-info/requires.txt
--rw-rw-r--   0 natanael  (1001) natanael  (1001)        9 2024-04-23 12:58:17.000000 opytimal-0.6.0/opytimal.egg-info/top_level.txt
--rw-rw-r--   0 natanael  (1001) natanael  (1001)       38 2024-04-23 12:58:17.886665 opytimal-0.6.0/setup.cfg
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     1383 2024-04-23 12:58:14.000000 opytimal-0.6.0/setup.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 13:17:02.353218 opytimal-0.6.1/
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     7048 2023-09-12 14:54:54.000000 opytimal-0.6.1/LICENSE
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     1080 2024-04-23 13:17:02.353218 opytimal-0.6.1/PKG-INFO
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      488 2023-11-17 15:48:02.000000 opytimal-0.6.1/README.md
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 13:17:02.353218 opytimal-0.6.1/opytimal/
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     2063 2024-04-23 13:16:59.000000 opytimal-0.6.1/opytimal/__init__.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      613 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/_vars.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    49923 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/analytical.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     9266 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/arrays.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    12180 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/decorator.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 13:17:02.353218 opytimal-0.6.1/opytimal/demos/
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      752 2023-11-17 17:30:06.000000 opytimal-0.6.1/opytimal/demos/__init__.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    29176 2023-11-17 16:51:20.000000 opytimal-0.6.1/opytimal/demos/optHeat1D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    26417 2023-11-17 16:51:20.000000 opytimal-0.6.1/opytimal/demos/optHeat2D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    22362 2023-11-17 16:51:20.000000 opytimal-0.6.1/opytimal/demos/optPoisson1D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    24873 2023-11-17 16:51:20.000000 opytimal-0.6.1/opytimal/demos/optPoisson2D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    23922 2023-11-17 16:51:20.000000 opytimal-0.6.1/opytimal/demos/optPoisson3D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    27362 2023-11-17 16:51:20.000000 opytimal-0.6.1/opytimal/demos/optStokes2D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    25154 2023-11-17 16:51:20.000000 opytimal-0.6.1/opytimal/demos/optStokes3D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      841 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/dicts.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    63651 2023-11-17 13:15:29.000000 opytimal-0.6.1/opytimal/fenics.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     1208 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/files.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      321 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/functions.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      105 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/mathFunctions.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    13269 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/meshes.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      798 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/modules.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      339 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/numeric.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      912 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/parallel.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    89570 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/plots.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     3695 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/profiler.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     2090 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/settings.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    21633 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/strings.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      447 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/symbols.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      344 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/tables.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     1546 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/tests.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     2504 2023-11-17 11:54:51.000000 opytimal-0.6.1/opytimal/types.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 13:17:02.353218 opytimal-0.6.1/opytimal.egg-info/
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     1080 2024-04-23 13:17:02.000000 opytimal-0.6.1/opytimal.egg-info/PKG-INFO
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      862 2024-04-23 13:17:02.000000 opytimal-0.6.1/opytimal.egg-info/SOURCES.txt
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)        1 2024-04-23 13:17:02.000000 opytimal-0.6.1/opytimal.egg-info/dependency_links.txt
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      276 2024-04-23 13:17:02.000000 opytimal-0.6.1/opytimal.egg-info/requires.txt
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)        9 2024-04-23 13:17:02.000000 opytimal-0.6.1/opytimal.egg-info/top_level.txt
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)       38 2024-04-23 13:17:02.353218 opytimal-0.6.1/setup.cfg
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     1383 2024-04-23 13:16:59.000000 opytimal-0.6.1/setup.py
```

### Comparing `opytimal-0.6.0/LICENSE` & `opytimal-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/PKG-INFO` & `opytimal-0.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opytimal
-Version: 0.6.0
+Version: 0.6.1
 Summary: Optimal control PDE-based solver
 Author: Natanael Quintino
 Author-email: natanael.quintino@ipiaget.pt
 License: CC0 1.0 Universal
 Keywords: optimalcontrol,FEniCS,FuildDynamics,NavierStokes,Stokes
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opytimal-0.6.0/opytimal/__init__.py` & `opytimal-0.6.1/opytimal/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                      getDomainLabels, replaceBoundNameByMark,
                      getMeasure, evaluateErrors, Zero, getAdjointSystem,
                      getOptimalConditionsSystem, evaluateCost,
                      getLocal, setLocal, showProblemData,
                      getFunctionExpressions)
 
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 def __getattr__(attr):
     # Warn for expired attributes
     import warnings
 
     if attr == "demos":
         import opytimal.demos as demos
```

### Comparing `opytimal-0.6.0/opytimal/_vars.py` & `opytimal-0.6.1/opytimal/_vars.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/analytical.py` & `opytimal-0.6.1/opytimal/analytical.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/arrays.py` & `opytimal-0.6.1/opytimal/arrays.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/decorator.py` & `opytimal-0.6.1/opytimal/decorator.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/demos/__init__.py` & `opytimal-0.6.1/opytimal/demos/__init__.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/demos/optHeat1D.py` & `opytimal-0.6.1/opytimal/demos/optHeat1D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/demos/optHeat2D.py` & `opytimal-0.6.1/opytimal/demos/optHeat2D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/demos/optPoisson1D.py` & `opytimal-0.6.1/opytimal/demos/optPoisson1D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/demos/optPoisson2D.py` & `opytimal-0.6.1/opytimal/demos/optPoisson2D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/demos/optPoisson3D.py` & `opytimal-0.6.1/opytimal/demos/optPoisson3D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/demos/optStokes2D.py` & `opytimal-0.6.1/opytimal/demos/optStokes2D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/demos/optStokes3D.py` & `opytimal-0.6.1/opytimal/demos/optStokes3D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/dicts.py` & `opytimal-0.6.1/opytimal/dicts.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/dolfin/function/function.py` & `opytimal-0.6.1/opytimal/strings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,571 +1,885 @@
-# -*- coding: utf-8 -*-
-"""This module handles the Function class in Python.
-
-"""
-# Copyright (C) 2009-2014 Johan Hake
-#
-# This file is part of DOLFIN.
-#
-# DOLFIN is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# DOLFIN is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-# GNU Lesser General Public License for more details.
-#
-# You should have received a copy of the GNU Lesser General Public License
-# along with DOLFIN. If not, see <http://www.gnu.org/licenses/>.
+'''
+Module of the strings proccessment methods
+'''
+
+__all__ = ['replaceFormat', 'replaceProgressive', 'replaceAll',
+           'functionToStr', 'setFunction', 'splitParcels', 'string',
+           'showInfo', 'showProgress', 'eraseProgress', 'convertTime',
+           'formatBytes', 'generateId', 'showErrors', 'splitPathFile',
+           'convertInt', 'basename']
+
+import os
+import re
+import sys
+import textwrap
+import copy
 
+import sympy as sp
 import numpy as np
-import ufl_legacy as ufl
-from ufl_legacy.classes import ComponentTensor, Sum, Product, Division
-from ufl_legacy.utils.indexflattening import shape_to_strides, flatten_multiindex
-import dolfin.cpp as cpp
-import dolfin.la as la
-from dolfin.function.functionspace import FunctionSpace, MixedFunctionSpace
-from dolfin.function.expression import Expression
-from dolfin.function.constant import Constant
+from termcolor import colored
+from ufl.algorithms.replace import replace as uflReplace
 
+from .tests import testLoop
+from .functions import getVars
+from .types import Any, Union, Tuple, Function, File
+
+def extractScalars(
+    expr: str,
+    vars: list[str] = None,
+    simplify: bool = False
+        ) -> (Tuple[list[str], str]):
+    'Extract scalars from expression'
+
+    if vars is None:
+        # Set default value
+        vars = []
+
+    # Init the scalars and varsCatched lists
+    scalars = []
+    varsCatched = []
+
+    if '*' in expr:
+        # Split scalar and term
+        eSplit = split(expr, '*', 1)
+
+        # Get the scalar and raw term
+        scalar = eSplit[0]
+        rawTerm = eSplit[1]
+
+        if scalar not in vars:
+            # Add respective scalar to list
+            scalars.append(scalar)
+        else:
+            varsCatched.append(scalar)
+
+        if '*' in rawTerm:
+            # Aplly recursivity
+            scalar, rawTerm = extractScalars(rawTerm, vars)
 
-def _assign_error():
-    raise RuntimeError("Expected only linear combinations of Functions in the same FunctionSpaces")
+            # Add to scalars list
+            scalars.extend(scalar)
 
+    else:
+        # The expression is the term
+        rawTerm = expr
 
-def _check_mul_and_division(e, linear_comb, scalar_weight=1.0, multi_index=None):
-    """
-    Utility func for checking division and multiplication of a Function
-    with scalars in linear combinations of Functions
-    """
-    from ufl_legacy.constantvalue import ScalarValue
-    from ufl_legacy.classes import ComponentTensor, MultiIndex, Indexed
-    from ufl_legacy.algebra import Division, Product, Sum
-    # ops = e.ufl_operands
-
-    # FIXME: What should be checked!?
-    # martinal: This code has never done anything sensible,
-    #   but I don't know what it was supposed to do so I can't fix it.
-    # same_multi_index = lambda x, y: (x.ufl_free_indices == y.ufl_free_indices \
-    #                        and x.ufl_index_dimensions == y.ufl_index_dimensions)
-
-    assert isinstance(scalar_weight, float)
-
-    # Split passed expression into scalar and expr
-    if isinstance(e, Product):
-        for i, op in enumerate(e.ufl_operands):
-            if isinstance(op, ScalarValue) or \
-               (isinstance(op, Constant) and op.value_size() == 1):
-                scalar = op
-                expr = e.ufl_operands[1 - i]
+    # Looping in var catched as scalars
+    for var in varsCatched:
+        # Multiply the var to rawTerm end
+        rawTerm = f'{rawTerm}*{var}'
+
+    if simplify:
+        # Simplify the rawTerm expression
+        rawTerm = sp.simplify(rawTerm)
+
+    return scalars, rawTerm
+
+
+def adjustParenthesisOccurrences(
+    parcels: list[str],
+    inplace: bool = True
+        ) -> (list[str]):
+
+    if not inplace:
+        # Get a parcels copy
+        pacerls = parcels.copy()
+
+    # Init the index counter
+    idx = 0
+
+    # Looping to make the parenthesis adjustment
+    while True:
+
+        while parcels[idx].count('(') != parcels[idx].count(')'):
+            # Join current parcel to previous parcel
+            parcels[idx] = f'{parcels[idx]} + {parcels[idx+1]}'
+
+            # Remove current parcel from parcels
+            del(parcels[idx+1])
+
+            # Security condition
+            if idx+1 == len(parcels):
+                # Stop the loop
                 break
-        else:
-            _assign_error()
 
-        scalar_weight *= float(scalar)
-    elif isinstance(e, Division):
-        expr, scalar = e.ufl_operands
-        if not (isinstance(scalar, ScalarValue) or
-                isinstance(scalar, Constant) and scalar.value_rank() == 1):
-            _assign_error()
-        scalar_weight /= float(scalar)
-    else:
-        _assign_error()
-
-    # If a CoefficientTensor is passed we expect the expr to be either
-    # a Function or another ComponentTensor, where the latter wil
-    # result in a recursive call
-    if multi_index is not None:
-        assert isinstance(multi_index, MultiIndex)
-        assert isinstance(expr, Indexed)
-
-        # Unpack Indexed and check equality with passed multi_index
-        expr, multi_index2 = expr.ufl_operands
-        assert isinstance(multi_index2, MultiIndex)
-        # if not same_multi_index(multi_index, multi_index2):
-        #    _assign_error()
-
-    if isinstance(expr, Function):
-        linear_comb.append((expr, scalar_weight))
-
-    elif isinstance(expr, (ComponentTensor, Product, Division, Sum)):
-        # If componentTensor we need to unpack the MultiIndices
-        if isinstance(expr, ComponentTensor):
-            expr, multi_index = expr.ufl_operands
-            # if not same_multi_index(multi_index, multi_index2):
-            #    _error()
-
-        if isinstance(expr, (Product, Division)):
-            linear_comb = _check_mul_and_division(expr, linear_comb, scalar_weight, multi_index)
-        elif isinstance(expr, Sum):
-            linear_comb = _check_and_extract_functions(expr, linear_comb, scalar_weight, multi_index)
+        # Update the index
+        idx += 1
+
+        if idx == len(parcels):
+            # Stop the loop
+            break
+
+    return parcels
+
+
+def splitParcels(expr: str) -> (list[str]):
+    # Change minus to plus minus 1
+    expr = expr.replace('-','+-1*')
+
+    # Get the parcels
+    parcels = expr.split('+')
+
+    # Trailling white spaces from parcels
+    parcels = [parcel.strip() for parcel in parcels]
+
+    # Adjust parenthesis occurrences
+    adjustParenthesisOccurrences(parcels, inplace=True)
+
+    return parcels
+
+
+def setFunction(
+    funcName: str,
+    funcArgs: tuple[str],
+    funcReturn: str = '',
+    funcCode: str = '',
+    funcDoc: str = '',
+    funcAnnotations: tuple[str] = None,
+    funcDefaults: dict[str: Any] = None,
+    removeNullMultiplications: bool = False,
+    indent: int = 4,
+    **funcConstants: dict[str: Any]
+        ) -> (Function):
+
+    # Set the indentation
+    indent = indent*' '
+
+    if funcAnnotations is not None:
+
+        if len(funcAnnotations) < len(funcArgs):
+            # Adjust annotations size
+            funcAnnotations += (len(funcArgs) - len(funcAnnotations))*('Any', )
+
+        # Put the args annotations
+        funcArgs = [
+            f'{arg}: {annot}' for arg, annot in zip(funcArgs, funcAnnotations)
+            ]
+
+    # Join the function args
+    funcArgs = ', '.join(funcArgs)
+
+    if funcDefaults is not None:
+
+        for k, v in funcDefaults.items():
+            # Default structure
+            defaultStruct = f'{k}={v}'
+
+            # Turn respective var to default
+            funcArgs = funcArgs.replace(k, defaultStruct)
+
+            # # Add default value in function code
+            # funcCode = f'{k}={v}\n{indent if any(funcCode) else ""}{funcCode}'
+
+    # Evaluate the function constants
+    funcCode = replaceProgressive(funcCode, funcConstants.items())
+    funcReturn = replaceProgressive(funcReturn, funcConstants.items())
+
+    if any(funcCode):
+        # Adjust indentation from funcCode
+        funcCode = funcCode.replace(indent, '$')\
+                           .replace('  ', '')\
+                           .replace('\n', f'\n{indent}')\
+                           .replace('$', indent)
+
+    if removeNullMultiplications:
+        # Remove null multiplications
+        funcReturn = str(sp.simplify(funcReturn))
+
+    # Set the pyfunction definition
+    funcDef = textwrap.dedent('''
+        def {name}({args}):
+        {indent}"""{doc}"""
+        {code}
+
+        {indent}return {value}
+        ''').format(
+            name=funcName,
+            args=funcArgs,
+            indent=indent,
+            doc=funcDoc,
+            code=funcCode,
+            value=funcReturn
+            )
+
+    # Execute the func definition
+    exec(funcDef, globals(), locals())
+
+    return locals()[funcName]
+
+
+def functionToStr(
+    func: Function
+        ) -> (str):
+    '''Turn function return to str'''
+
+    # Get the function varibables
+    args = getVars(func)
+
+    # Turn args to symbols
+    args = sp.symbols(','.join(args))
+
+    # Apply the function on symbols
+    funcStr = func(*args)
+
+    return funcStr
+
+
+def replaceFormat(
+    string: str,
+    old: str,
+    new: str
+        ) -> (str):
+    'Make replacement in string with regular expression'
+
+    # Replace the marker to chars identifier
+    chars = '([A-Za-z0-9\(\)\_\*\+\-\/\[\]\:\,\!\;\@\&\%\'\"\. ]*)'
+
+    # Prepare the old format
+    old = replaceProgressive(
+        old, [('(', '\('), (')', '\)'),
+              ('[', '\['), (']', '\]'),
+              ('#', chars)]
+        )
+
+    # Prepare the new string
+    new = new.replace('#', r'\1')
+
+    # Make the replacement
+    string = re.sub(old, new, string)
+
+    return string
+
+
+def replaceProgressive(
+    string: str,
+    replacements: list[tuple[str, str]],
+    preserveds: list[str] = None
+        ) -> (str):
+
+    if preserveds is not None:
+
+        # Looping in replacements
+        for repl in replacements:
+            # Set a default value
+            restoreNeed = False
+
+            # Get the old and new substrings
+            old, new = repl
+
+            # Verify the substring to be preserved
+            if any([preserved in string for preserved in preserveds]):
+                # Make the preservation
+                string = preserveSubstring(string, preserveds)
+
+                # Update the "restoreNeed" var
+                restoreNeed = True
+
+            if type(string) is str:
+                # Turn to string type
+                repl = map(str, repl)
+
+                # Set the replacer
+                replacer = lambda s, repl: s.replace(*repl)
+                # # Make the replacement
+                # string = string.replace(*repl)
+            else:
+                # Set the replacer
+                replacer = lambda s, repl: uflReplace(s, dict([repl]))
+                # # Make the replacement
+                # string = uflReplace(string, dict([repl]))
+
+            # Make the replacement
+            string = replacer(string, repl)
+
+            if restoreNeed:
+                # Make the restoration
+                string = restoreSubstring(string, preserveds)
+
+    else:
+
+        # Looping in replacements
+        for repl in replacements:
+
+            if type(string) is str:
+                # Turn to string type
+                repl = map(str, repl)
+
+                # Set the replacer
+                replacer = lambda s, repl: s.replace(*repl)
+                # # Make the replacement
+                # string = string.replace(*repl)
+            else:
+                # Set the replacer
+                replacer = lambda s, repl: uflReplace(s, dict([repl]))
+                # # Make the replacement
+                # string = uflReplace(string, dict([repl]))
+
+            # Make the replacement
+            string = replacer(string, repl)
+
+    return string
+
+
+def preserveSubstring(string: str, preserveds: list[str], mark: str = '#'):
+    'Protect the "preserved" substring in string'
+
+    if type(preserveds) is not list:
+        # Turn to list
+        preserveds = [preserveds]
+
+    # Looping in preserved substrings
+    for i, preserved in enumerate(preserveds):
+        # Make the preservation
+        string = string.replace(preserved, f'{mark}{i}')
+
+    return string
+
+
+def restoreSubstring(string: str, preserveds: str, mark: str = '#'):
+    'Restore the "preserved" substring in string'
+
+    if type(preserveds) is not list:
+        # Turn to list
+        preserveds = [preserveds]
+
+    # Get len of preserveds list
+    tam = len(preserveds)-1
+
+    # Looping in preserved substrings
+    for i, preserved in enumerate(preserveds[::-1]):
+        # Make the restoration
+        string = string.replace(f'{mark}{tam - i}', preserved)
+
+    return string
+
+
+def replaceAll(
+    string: str,
+    target: Union[str, list[str]],
+    replacement: str = ''
+        ) -> str:
+
+    if type(target) is str:
+        # Turn in list
+        target = [target]
+
+    # Apply the replacement
+    string = replaceProgressive(
+        string,
+        zip(target, len(target)*[replacement])
+        )
+
+    return string
+
+
+def split(string: str, sub: str, count: int = None):
+    if count is None:
+        # Split all occurrences
+        output = string.split(sub)
+    else:
+        # Split any count-th occurrences
+        output = string.replace(sub, '#TARGET#', count).split('#TARGET#')
+    return output
+
+
+def adjustId(id):
+    return f'_{id}' if id is not None else ''
+
+
+def generateId(
+    label: str,
+    globalVars: dict[str: Any] = globals()
+        ) -> (str):
+
+    # Adjust label
+    label = label.upper().replace(' ', '_')
+
+    # Set a id global var name
+    idGlobalVar = f"ID_{label}"
+
+    if idGlobalVar in globalVars:
+        globalVars[idGlobalVar] += 1
+
+    else:
+        globalVars[idGlobalVar] = 1
+
+    # Get the respective id
+    id = globalVars[idGlobalVar]
+
+    return id
+
+
+def showInfo(
+    *infos: str,
+    repeatMsg: Union[str, list[str]] = None,
+    breakStart: bool = False,
+    tab: int = 0,
+    err: bool = False,
+    color: str = None,
+    end: str = '\n',
+    delimiters: bool = True,
+    alignment: str = None,
+    cleanConsole: bool = False,
+    startLine: int = 3,
+    linesClean: int = '',
+    initialCleanConsole: bool = False,
+    outputName: str = None,
+    copyTo: File = None,
+    ignoreEmptyLines: bool = False
+        ) -> (None):
+    'Report a formated message'
+
+    if cleanConsole:# and type(outputName) is not str:
+
+        if initialCleanConsole:
+            # Breaklines
+            print(end=initialCleanConsole*'\n')
+
+        # Clear the console
+        print(f"\033[{startLine}H\033[{linesClean}J", end='\r')
+
+    if alignment is not None:
+        # Get the position of the all alignments char
+        positions = list(
+            map(lambda s: s.index(alignment)
+                    if alignment in s
+                    else len(s)//2,
+                infos)
+            )
+
+        # Get the greater position
+        maxPos = max(positions)
+
+        # Calcule the compensation tab
+        tabs = list(map(lambda v: (tab + maxPos - v)*' ', positions))
+
+    else:
+        # Set a default value
+        tabs = len(infos)*[tab*' ']
+
+    # Init the content
+    content = ''
+
+    for i, info in enumerate(infos):
+
+        if ignoreEmptyLines and not any(info):
+            # Skip the empty lines
+            continue
+
+        # Colorize info
+        if err:
+            info = colored(info, None, 'on_red')
+        elif color is not None:
+            info = colored(info, 'red', f'on_{color}')
+
+        # Add info to content
+        content += f'{tabs[i]}{info}\n'
+
+    # Set a delimiter
+    delimit = delimiter(
+        max(map(len, infos))+tab, color='red' if err else color
+        )
+
+    # Add tab
+    delimit = f'{tab*" "}{delimit}'
+
+    if type(outputName) is str and 'outputTxt' not in globals():
+        # Open a external file to print
+        output = globals()['outputTxt'] = open(outputName, 'w')
+
+    elif outputName is not None and 'outputTxt' in globals():
+        # Get the opened external file to print
+        output = globals()['outputTxt']
+
+    elif outputName is not None:
+        # Get the opened external file to print
+        output = outputName
+
+    else:
+        # Get default internal output
+        output = sys.stdout
+
+    if repeatMsg is not None:
+        if type(repeatMsg) not in [list, tuple]:
+            repeatMsg = [repeatMsg]
+
+        for msg in repeatMsg:
+            # Make the repeat message replacement
+            content = content.replace(msg, '#repeatMsg#', 1)\
+                             .replace(msg, len(msg)*' ')\
+                             .replace('#repeatMsg#', msg)
+
+    if delimiters:
+        # Set the print content
+        content = [
+            (breakStart - 1)*'\n', # Break line in start
+            delimit,
+            content.strip('\n'),
+            delimit
+            ]
+
+        # Set the respective separator
+        sep = '\n'
+
+    else:
+        # Set the print content
+        content = [
+            breakStart*'\n', # Break line in start
+            content.strip('\n')
+            ]
+
+        # Set the separator
+        sep = ''
+
+    # Show the info
+    print(
+        *content,
+        sep=sep,
+        end=end,
+        file=output
+        )
+
+    if copyTo is not None:
+        # Write a copy of the print content
+        print(
+            *content,
+            sep=sep,
+            end=end,
+            file=copyTo
+            )
+
+    if 'outputTxt' in globals() and globals()['outputTxt'].mode=='w':
+        globals()['outputTxt'].close()
+        globals()['outputTxt'] = open(outputName, 'a')
+
+    return None
+
+
+def formatBytes(
+    bytesValues: int,
+    toStr: bool = True
+        ) -> (str):
+    "Format the 'bytesValues'"
+
+    # Separate in giga, mega, kbytes and byte values
+    giga  = int(bytesValues//1e9)
+    mega  = int(bytesValues%1e9//1e6)
+    kbyte = int(bytesValues%1e9%1e6//1e3)
+    byte  = int(bytesValues%1e9%1e6%1e3)
+
+    if toStr:
+        # Init the value formated
+        formated = ''
+
+        # Format value
+        if   (giga  != 0):
+            formated += f'{giga},{mega:03} Gb'
+            #formated += str(giga) +','+(3-len(str(mega))) *'0'+str(mega)+' Gb'
+
+        elif (mega  != 0):
+            formated += f'{mega},{kbyte:03} Mb'
+            #formated += str(mega) +','+(3-len(str(kbyte)))*'0'+str(kbyte)+' Mb'
+
+        elif (kbyte != 0):
+            formated += f'{kbyte},{byte:03} Kb'
+            #formated += str(kbyte)+','+(3-len(str(byte))) *'0'+str(byte)+' Kb'
+
         else:
-            _assign_error()
+            formated += str(byte) + '  b'
+
+        # Set the output
+        output = formated.strip()
+
     else:
-        _assign_error()
+        # Set the output
+        output = giga
 
-    return linear_comb
+    return output
 
 
-def _check_and_extract_functions(e, linear_comb=None, scalar_weight=1.0,
-                                 multi_index=None):
+def convertInt(
+    num: Union[int, float],
+    precision=3
+        ) -> str:
+    output = ('{:1.0%df} M'%precision).format(num/1e6)\
+        if num > 1e6\
+        else (('{:1.0%df} K'%precision).format(num/1e3)
+            if num > 1e3
+            else ('{}').format(num))
+    return output
+
+
+def convertTime(
+    T: int,
+    title: str = '',
+    prec: int = 3
+        ) -> (str):
     """
-    Utility func for extracting Functions and scalars in linear
-    combinations of Functions
+    Convert the time T into format 'HH:MM:SS.CS'
     """
-    from ufl_legacy.classes import ComponentTensor, Sum, Product, Division
-    linear_comb = linear_comb or []
 
-    # First check u
-    if isinstance(e, Function):
-        linear_comb.append((e, scalar_weight))
-        return linear_comb
+    # Separate quantities
+    hours, minutes = divmod(T, 3600)
+    minutes, seconds = divmod(minutes, 60)
+    seconds, centsSeconds = divmod(seconds, 1)
+
+    # Convert to int
+    hours, minutes, seconds = map(int, [hours, minutes, seconds])
+
+    # Adjust the cents of seconds
+    centsSeconds = int(10**prec*round(centsSeconds, prec))
+
+    # Exhibition format
+    T_format = ("{:02}:{:02}:{:02}.{:0"+str(prec)+"}").format(
+        hours, minutes, seconds, centsSeconds
+        )
+
+    return T_format
+
+
+def delimiter(
+    titleTam: Union[str, int],
+    symbol: str = '▬',
+    tab: int = 0,
+    color: str = None
+        ) -> (str):
+    'Return a string delimiter to text'
+
+    # Set the tam of title
+    tam = len(titleTam) if type(titleTam) is str else titleTam
+
+    output = tab*'\t'
+    output += colored(tam*symbol, None, f"on_{color}")\
+        if color is not None else tam*symbol
+
+    return output
+
+def showProgress(
+    message: str,
+    k: int,
+    total: int = None,
+    label: str = None,
+    printer: bool = True,
+    formatter: str = '',
+    markers: str = ["○", '◔', '◑', '◕'],
+    suffix: str = ''
+        ) -> (str):
+
+    if k == 0:
+        # Break a line
+        print()
+
+    # Progress structure
+    if label is not None:
+        structure = '{label} = {k:%s}'%formatter
+        kwargs = {'k': k, 'label': label}
+    elif total is not None:
+        structure = '{k:0%s}/{total:0%s}'%(2*(formatter,))
+        kwargs = {'k': k, 'total': total}
+    else:
+        # Set default values
+        structure = ''
+        kwargs = {}
+
+    if total is not None:
+        v = k/total
+        if v < 0.25:
+            marker = markers[0]
+        elif 0.25 <= v and v < 0.5:
+            marker = markers[1]
+        elif 0.5 <= v and v < 0.75:
+            marker = markers[2]
+        elif 0.75 <= v and v <= 1:
+            marker = markers[3]
+        else:
+            marker = markers[3]
+    else:
+        marker = ''
+
+    # Format the progress
+    progress = f'{message}{structure.format(**kwargs)}'
+
+    if marker is not None and any(marker):
+        # Add prefixed marker
+        progress = f'{marker} ' + progress
+
+    if suffix is not None:
+        # Add suffix
+        progress += f' {suffix}'
+
+    if printer:
+        print(progress, end='\r')
+
+    return progress
+
+
+def eraseProgress(message: str, printer: bool = True):
+    eraser = len(message)*' '
+
+    if printer:
+        print(eraser, end='\033[F')
+
+    return eraser
 
-    # Second check a*u*b, u/a/b, a*u/b where a and b are scalars
-    elif isinstance(e, (Product, Division)):
-        linear_comb = _check_mul_and_division(e, linear_comb, scalar_weight, multi_index)
-        return linear_comb
 
-    # Third check a*u*b, u/a/b, a*u/b where a and b are scalars and u
-    # is a Tensor
-    elif isinstance(e, ComponentTensor):
-        e, multi_index = e.ufl_operands
-        linear_comb = _check_mul_and_division(e, linear_comb, scalar_weight, multi_index)
-        return linear_comb
+def replaceMathFunctions(
+    string: str
+        ) -> str:
 
-    # If not Product or Division we expect Sum
-    elif isinstance(e, Sum):
-        for op in e.ufl_operands:
-            linear_comb = _check_and_extract_functions(op, linear_comb,
-                                                       scalar_weight, multi_index)
+    newString = replaceProgressive(
+        string, [('exp', 'self.exp'),
+                 ('log', 'self.log'),
+                 ('ln', 'self.ln'),
+                 ('sin', 'self.sin'),
+                 ('cos', 'self.cos'),
+                 ('tan', 'self.tan')]
+        )
+    return newString
+
+
+def generateId(
+    label: str,
+    globalVars: dict[str: Any] = globals()
+        ) -> (str):
+
+    # Adjust label
+    label = label.upper().replace(' ', '_')
+
+    # Set a id global var name
+    idGlobalVar = f"ID_{label}"
+
+    if idGlobalVar in globalVars:
+        globalVars[idGlobalVar] += 1
 
     else:
-        _assign_error()
+        globalVars[idGlobalVar] = 1
 
-    return linear_comb
+    # Get the respective id
+    id = globalVars[idGlobalVar]
 
+    return id
 
-def _check_and_contract_linear_comb(expr, self, multi_index):
-    """
-    Utility func for checking and contracting linear combinations of
-    Functions
-    """
-    linear_comb = _check_and_extract_functions(expr, multi_index=multi_index)
-    funcs = []
-    weights = []
-    funcspace = None
-    for func, weight in linear_comb:
-        funcspace = funcspace or func.function_space()
-        if func not in funcspace:
-            _assign_error()
-        try:
-            # Check if the exact same Function is already present
-            ind = funcs.index(func)
-            weights[ind] += weight
-        except Exception:
-            funcs.append(func)
-            weights.append(weight)
-
-    # Check that rhs does not include self
-    for ind, func in enumerate(funcs):
-        if func == self:
-            # If so make a copy
-            funcs[ind] = self.copy(deepcopy=True)
-            break
 
-    return list(zip(funcs, weights))
+def showErrors(
+    errors: dict[str:float],
+    mode: str = 'horizontal', # ['vertical', 'horizontal']
+    show: bool = False,
+    indent: int = 0,
+    preffix: str = ''
+        ) -> str:
 
+    # Set the indentation
+    indent = indent*' '\
+        if mode == 'vertical'\
+        else ''
 
-class Function(ufl.Coefficient):
+    # Set the preffix
+    preffix = ''\
+        if mode == 'vertical'\
+        else preffix
 
-    def __init__(self, *args, **kwargs):
-        """Initialize Function."""
+    # Set the respective separator
+    sep = '\n'\
+        if mode == 'vertical'\
+        else ' | '
 
-        # For MixedFunctionSpace use
-        self._functions = None
-        self._part = None
-
-        if isinstance(args[0], Function):
-            other = args[0]
-            if len(args) == 1:
-                # Copy constructor used to be here
-                raise RuntimeError("Use 'Function.copy(deepcopy=True)' for copying.")
-            elif len(args) == 2:
-                i = args[1]
-                if not isinstance(i, int):
-                    raise TypeError("Invalid subfunction number %s" % (i,))
-                num_sub_spaces = other.function_space().num_sub_spaces()
-                if num_sub_spaces == 1:
-                    raise RuntimeError("No subfunctions to extract")
-                if not i < num_sub_spaces:
-                    raise RuntimeError("Can only extract subfunctions "
-                                       "with i = 0..%d" % num_sub_spaces)
-                self._cpp_object = cpp.function.Function(other._cpp_object, i)
-                ufl.Coefficient.__init__(self, self.function_space().ufl_function_space(),
-                                         count=self._cpp_object.id())
-            else:
-                raise TypeError("expected one or two arguments when "
-                                "instantiating from another Function")
-        elif isinstance(args[0], cpp.function.Function):
-            self._cpp_object = args[0]
-            ufl.Coefficient.__init__(self, self.function_space().ufl_function_space(),
-                                     count=self._cpp_object.id())
-        elif isinstance(args[0], FunctionSpace):
-            V = args[0]
-
-            # If initialising from a FunctionSpace
-            if len(args) == 1:
-                # If passing only the FunctionSpace
-                self._cpp_object = cpp.function.Function(V._cpp_object)
-            elif len(args) == 2:
-                if isinstance(args[1], cpp.la.GenericVector):
-                    self._cpp_object = cpp.function.Function(V._cpp_object, args[1])
-                elif isinstance(args[1], cpp.function.Function):
-                    self._cpp_object = args[1]
-                elif isinstance(args[1], str):
-                    # Read from xml filename in string
-                    self._cpp_object = cpp.function.Function(V._cpp_object, args[1])
-                elif isinstance(args[1], int):
-                    # Specify the part associated with the Function (mixed-domains)
-                    self._cpp_object = cpp.function.Function(V._cpp_object)
-                    self._part = args[1]
-                else:
-                    raise RuntimeError("Don't know what to do with ", type(args[1]))
-            else:
-                raise RuntimeError("Don't know what to do yet")
+    # Set the error structure
+    error = len(errors)*(
+        '%(indent)s{:8>} = {:1.03e}%(sep)s' % {'indent': indent, 'sep': sep}
+        )
 
-            # Initialize the ufl.FunctionSpace
-            ufl.Coefficient.__init__(self, V.ufl_function_space(), count=self._cpp_object.id())
-        elif isinstance(args[0], MixedFunctionSpace):
-            V = args[0]
-            self._functions = [Function(s, i) for i, s in enumerate(V.sub_spaces())]
-        else:
-            raise TypeError("Expected a FunctionSpace or a Function as argument 1")
+    # Add the preffix
+    error = f'{preffix}{error}'
 
-        # Set name as given or automatic
-        if isinstance(args[0], MixedFunctionSpace):
-            for i in range(len(self._functions)):
-                name = kwargs.get("name") or "f_%d" % self._functions[i].count()
-                self._functions[i].rename("%s_%d" % (name, i), "a Function")
-        else:
-            name = kwargs.get("name") or "f_%d" % self.count()
-            self.rename(name, "a Function")
+    # Fix the last term
+    error = error.rstrip(' |')
 
-    def part(self):
-        return self._part
+    # Flatten the erros dict.items
+    errorsFlatten = []
+    [errorsFlatten.extend(kv) for kv in errors.items()]
 
-    def function_space(self):
-        "Return the FunctionSpace"
-        return FunctionSpace(self._cpp_object.function_space())
-
-    def value_rank(self):
-        return self._cpp_object.value_rank()
-
-    def value_dimension(self, i):
-        return self._cpp_object.value_dimension(i)
-
-    def value_shape(self):
-        return self._cpp_object.value_shape
-
-    def ufl_evaluate(self, x, component, derivatives):
-        """Function used by ufl to evaluate the Expression"""
-        # FIXME: same as dolfin.expression.Expression version. Find
-        # way to re-use.
-        assert derivatives == ()   # TODO: Handle derivatives
-
-        if component:
-            shape = self.ufl_shape
-            assert len(shape) == len(component)
-            value_size = ufl.product(shape)
-            index = flatten_multiindex(component, shape_to_strides(shape))
-            values = np.zeros(value_size)
-            # FIXME: use a function with a return value
-            self(*x, values=values)
-            return values[index]
-        else:
-            # Scalar evaluation
-            return self(*x)
+    # Fill the error structure
+    error = error.format(*errorsFlatten)
 
-    def __call__(self, *args, **kwargs):
-        # GNW: This function is copied from the old DOLFIN Python
-        # code. It is far too complicated. There is no need to provide
-        # so many ways of doing the same thing.
-        #
-        # Deprecate as many options as possible, and maybe share with
-        # dolfin.expression.Expresssion.
-
-        if len(args) == 0:
-            raise TypeError("expected at least 1 argument")
-
-        # Test for ufl restriction
-        if len(args) == 1 and isinstance(args[0], str):
-            if args[0] in ('+', '-'):
-                return ufl.Coefficient.__call__(self, *args)
-
-        # Test for ufl mapping
-        if len(args) == 2 and isinstance(args[1], dict) and self in args[1]:
-            return ufl.Coefficient.__call__(self, *args)
-
-        # Some help variables
-        value_size = ufl.product(self.ufl_element().value_shape())
-
-        # If values (return argument) is passed, check the type and length
-        values = kwargs.get("values", None)
-        if values is not None:
-            if not isinstance(values, np.ndarray):
-                raise TypeError("expected a NumPy array for 'values'")
-            if len(values) != value_size or \
-               not np.issubdtype(values.dtype, np.float64):
-                raise TypeError("expected a double NumPy array of length"
-                                " %d for return values." % value_size)
-            values_provided = True
-        else:
-            values_provided = False
-            values = np.zeros(value_size, dtype='d')
+    if show:
+        # Print the error
+        print(error)
 
-        # Get the geometric dimension we live in
-        dim = self.ufl_domain().geometric_dimension()
+    return error
 
-        # Assume all args are x argument
-        x = args
 
-        # If only one x argument has been provided, unpack it if it's
-        # an iterable
-        if len(x) == 1:
-            if isinstance(x[0], cpp.geometry.Point):
-                x = [x[0][i] for i in range(dim)]
-            elif hasattr(x[0], '__iter__'):
-                x = x[0]
-
-        # Convert it to an 1D numpy array
-        try:
-            x = np.fromiter(x, 'd')
-        except (TypeError, ValueError, AssertionError):
-            raise TypeError("expected scalar arguments for the coordinates")
-
-        if len(x) == 0:
-            raise TypeError("coordinate argument too short")
-
-        if len(x) != dim:
-            raise TypeError("expected the geometry argument to be of "
-                            "length %d" % dim)
-
-        # The actual evaluation
-        self._cpp_object.eval(values, x)
-
-        # If scalar return statement, return scalar value.
-        if value_size == 1 and not values_provided:
-            return values[0]
-
-        return values
-
-    # def _assign(self, u):
-    #    if isinstance(u, cpp.function.FunctionAXPY):
-    #        self._cpp_object._assign(u)
-
-    def eval_cell(self, u, x, cell):
-        return self._cpp_object.eval(u, x, cell)
-
-    def eval(self, u, x):
-        return self._cpp_object.eval(u, x)
-
-    def extrapolate(self, u):
-        if isinstance(u, ufl.Coefficient):
-            self._cpp_object.extrapolate(u._cpp_object)
-        else:
-            self._cpp_object.extrapolate(u)
+def getSetOperatorsPositions(
+    string: str
+        ) -> dict[str: str]:
 
-    def interpolate(self, u):
-        if isinstance(u, ufl.Coefficient):
-            self._cpp_object.interpolate(u._cpp_object)
-        else:
-            self._cpp_object.interpolate(u)
+    # Set the operators list
+    operators = ['&', '|', '\\']
 
-    def compute_vertex_values(self, mesh=None):
-        if mesh is not None:
-            return self._cpp_object.compute_vertex_values(mesh)
-        else:
-            return self._cpp_object.compute_vertex_values()
+    # Init the operators positions dict
+    operatorsPositions = {}
 
-    def set_allow_extrapolation(self, value):
-        self._cpp_object.set_allow_extrapolation(value)
+    # Split string characteres in an array
+    chars = np.array(list(string))
 
-    def get_allow_extrapolation(self):
-        return self._cpp_object.get_allow_extrapolation()
+    # Get the indexes array
+    indexes = np.arange(len(string))
 
-    def copy(self, deepcopy=False):
-        # See https://bitbucket.org/fenics-project/dolfin/issues/702
-        if deepcopy:
-            return Function(self.function_space(), self._cpp_object.vector().copy())
-        return Function(self.function_space(), self._cpp_object.vector())
-
-    def vector(self):
-        return self._cpp_object.vector()
-
-    def assign(self, rhs):
-        """
-        Assign either a Function or linear combination of Functions.
-
-        *Arguments*
-            rhs (_Function_)
-                A Function or a linear combination of Functions. If a linear
-                combination is passed all Functions need to be in the same
-                FunctionSpaces.
-        """
-
-        if isinstance(rhs, (cpp.function.Function, cpp.function.Expression, cpp.function.FunctionAXPY)):
-            # Avoid self assignment
-            if self == rhs:
-                return
-            self._cpp_object._assign(rhs)
-        elif isinstance(rhs, (Constant, Function, Expression)):
-            # Avoid self assignment
-            if self == rhs:
-                return
-            self._cpp_object._assign(rhs._cpp_object)
-        elif isinstance(rhs, (Sum, Product, Division, ComponentTensor)):
-            if isinstance(rhs, ComponentTensor):
-                rhs, multi_index = rhs.ufl_operands
-            else:
-                multi_index = None
-            linear_comb = _check_and_contract_linear_comb(rhs, self, multi_index)
-            assert (linear_comb)
-
-            # If the assigned Function lives in a different FunctionSpace
-            # we cannot operate on this function directly
-            same_func_space = linear_comb[0][0] in self.function_space()
-            func, weight = linear_comb.pop()
-
-            # Assign values from first func
-            if not same_func_space:
-                self._cpp_object._assign(func._cpp_object)
-                vector = self.vector()
-            else:
-                vector = self.vector()
-                vector[:] = func.vector()
+    # Looping in operators
+    for op in operators:
+        # Get the respective positions
+        positions = indexes[chars == op]
 
-            # If first weight is not 1 scale
-            if weight != 1.0:
-                vector *= weight
-
-            # AXPY the other functions
-            for func, weight in linear_comb:
-                if weight == 0.0:
-                    continue
-                vector.axpy(weight, func.vector())
+        # Set the respective dict
+        operatorsPositions.update(
+            dict(zip(positions, positions.size*op))
+            )
 
-        else:
-            raise RuntimeError("Expected a Function or linear combinations of Functions in the same FunctionSpace")
+    return operatorsPositions
 
-    def __float__(self):
-        # FIXME: this could be made simple on the C++ (in particular,
-        # with dolfin::Scalar)
-        if self.ufl_shape != ():
-            raise RuntimeError("Cannot convert nonscalar function to float.")
-        elm = self.ufl_element()
-        if elm.family() != "Real":
-            raise RuntimeError("Cannot convert spatially varying function to float.")
-        # FIXME: This could be much simpler be exploiting that the
-        # vector is ghosted
-        # Gather value directly from vector in a parallel safe way
-        vec = self.vector()
-        indices = np.zeros(1, dtype=la.la_index_dtype())
-        values = vec.gather(indices)
-        return float(values[0])
-
-    def name(self):
-        return self._cpp_object.name()
-
-    def rename(self, name, s):
-        self._cpp_object.rename(name, s)
-
-    def id(self):
-        return self._cpp_object.id()
-
-    def __str__(self):
-        """Return a pretty print representation of it self."""
-        return self.name()
-
-    def root_node(self):
-        u = self._cpp_object.root_node()
-        return Function(FunctionSpace(u.function_space()), u.vector())
-
-    def leaf_node(self):
-        u = self._cpp_object.leaf_node()
-        return Function(FunctionSpace(u.function_space()), u.vector())
-
-    def cpp_object(self):
-        return self._cpp_object
-
-    def restrict(self, element, cell):
-        """
-        Returns expansion coefficients of function restricted to local cell.
-
-        *Arguments*
-             element : cpp.fem.FiniteElement
-                 The element.
-             cell : Cell
-                 The cell.
-        """
-        return self._cpp_object.restrict(element, cell)
-
-    def num_sub_spaces(self):
-        if self._functions is not None:
-            return len(self._functions)
-        else:
-            return self.function_space().num_sub_spaces()
 
-    def sub(self, i, deepcopy=False):
-        """
-        Return a sub function.
-
-        The sub functions are numbered from i = 0..N-1, where N is the
-        total number of sub spaces.
-
-        *Arguments*
-            i : int
-                The number of the sub function
-
-        """
-        if not isinstance(i, int):
-            raise TypeError("expects an 'int' as first argument")
-
-        if self._functions is not None:
-            if deepcopy:
-                return self._functions[i].copy(True)
-            else:
-                return self._functions[i]
+def getSetOperatorsOrder(
+    string: str
+        ) -> dict[str: str]:
 
-        num_sub_spaces = self.num_sub_spaces()
-        if num_sub_spaces == 1:
-            raise RuntimeError("No subfunctions to extract")
-        if not i < num_sub_spaces:
-            raise RuntimeError("Can only extract subfunctions with i = 0..%d"
-                               % num_sub_spaces)
-
-        # Create and instantiate the Function
-        if deepcopy:
-            return Function(self.function_space().sub(i),
-                            self.cpp_object().sub(i),
-                            name='%s-%d' % (str(self), i))
-        else:
-            return Function(self, i, name='%s-%d' % (str(self), i))
+    # Get the operators positions
+    operatorsPositions = getSetOperatorsPositions(string)
+
+    # Order operators by positions
+    positions = sorted(operatorsPositions.items(), key=lambda x: x[0])
+
+    # Order the operators
+    operatorsOrdered = np.array(positions)[:, 1]
+
+    return operatorsOrdered
+
+
+def basename(filePath: str) -> (str):
+    return os.path.basename(filePath)
+
+
+def splitPathFile(filePath: str) -> Tuple[str, str]:
+    # Get the diretory path
+    path = os.path.dirname(filePath)
+    # Get the file name
+    file = os.path.basename(filePath)
 
-    def split(self, deepcopy=False):
-        """Extract any sub functions.
+    if os.path.isdir(filePath):
+        # Join the "file" to path
+        path = '/'.join([path, file])
 
-        A sub function can be extracted from a discrete function that
-        is in a mixed, vector, or tensor FunctionSpace. The sub
-        function resides in the subspace of the mixed space.
+        # Set a empty file name
+        file = ''
 
-        *Arguments*
-            deepcopy
-                Copy sub function vector instead of sharing
+    return path, file
 
-        """
 
-        num_sub_spaces = self.num_sub_spaces()
-        if num_sub_spaces == 1:
-            raise RuntimeError("No subfunctions to extract")
-        return tuple(self.sub(i, deepcopy) for i in range(num_sub_spaces))
+def convertInt(
+    num: Union[int, float],
+    precision=3
+        ) -> (str):
+    output = ('{:1.0%df} M'%precision).format(num/1e6)\
+        if num > 1e6\
+        else (('{:1.0%df} K'%precision).format(num/1e3)
+            if num > 1e3
+            else ('{}').format(num))
+    return output
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `opytimal-0.6.0/opytimal/fenics.py` & `opytimal-0.6.1/opytimal/fenics.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/files.py` & `opytimal-0.6.1/opytimal/files.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/meshes.py` & `opytimal-0.6.1/opytimal/meshes.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/modules.py` & `opytimal-0.6.1/opytimal/modules.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/parallel.py` & `opytimal-0.6.1/opytimal/parallel.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/plots.py` & `opytimal-0.6.1/opytimal/plots.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/profiler.py` & `opytimal-0.6.1/opytimal/profiler.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/settings.py` & `opytimal-0.6.1/opytimal/settings.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/tests.py` & `opytimal-0.6.1/opytimal/tests.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal/types.py` & `opytimal-0.6.1/opytimal/types.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.0/opytimal.egg-info/PKG-INFO` & `opytimal-0.6.1/opytimal.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opytimal
-Version: 0.6.0
+Version: 0.6.1
 Summary: Optimal control PDE-based solver
 Author: Natanael Quintino
 Author-email: natanael.quintino@ipiaget.pt
 License: CC0 1.0 Universal
 Keywords: optimalcontrol,FEniCS,FuildDynamics,NavierStokes,Stokes
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opytimal-0.6.0/setup.py` & `opytimal-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.6.0"
+VERSION = "0.6.1"
 DESCRIPTION = 'Optimal control PDE-based solver'
 LONG_DESCRIPTION = 'Opytimal is a Python/FEniCS framework that have the main goal solve Optimal Control problems considering multiple and mixed controls based to linear and nonlinear PDEs, in addition to can also solve PDEs simply and clearly'
 
 setup(
     name="opytimal",
     version=VERSION,
     description=DESCRIPTION,
```

