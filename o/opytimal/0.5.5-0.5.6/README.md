# Comparing `tmp/opytimal-0.5.5.tar.gz` & `tmp/opytimal-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opytimal-0.5.5.tar", last modified: Tue Apr 23 12:15:00 2024, max compression
+gzip compressed data, was "opytimal-0.5.6.tar", last modified: Tue Apr 23 12:19:51 2024, max compression
```

## Comparing `opytimal-0.5.5.tar` & `opytimal-0.5.6.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:15:00.154488 opytimal-0.5.5/
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     7048 2023-09-12 14:54:54.000000 opytimal-0.5.5/LICENSE
--rw-r--r--   0 natanael  (1001) natanael  (1001)     1080 2024-04-23 12:15:00.154488 opytimal-0.5.5/PKG-INFO
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      488 2023-11-17 15:48:02.000000 opytimal-0.5.5/README.md
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:15:00.150488 opytimal-0.5.5/opytimal/
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     2061 2024-04-23 12:14:57.000000 opytimal-0.5.5/opytimal/__init__.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      613 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/_vars.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    49923 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/analytical.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     9266 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/arrays.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    12180 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/decorator.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:15:00.150488 opytimal-0.5.5/opytimal/demos/
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      752 2023-11-17 17:30:06.000000 opytimal-0.5.5/opytimal/demos/__init__.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    29176 2023-11-17 16:51:20.000000 opytimal-0.5.5/opytimal/demos/optHeat1D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    26417 2023-11-17 16:51:20.000000 opytimal-0.5.5/opytimal/demos/optHeat2D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    22362 2023-11-17 16:51:20.000000 opytimal-0.5.5/opytimal/demos/optPoisson1D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    24873 2023-11-17 16:51:20.000000 opytimal-0.5.5/opytimal/demos/optPoisson2D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    23922 2023-11-17 16:51:20.000000 opytimal-0.5.5/opytimal/demos/optPoisson3D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    27362 2023-11-17 16:51:20.000000 opytimal-0.5.5/opytimal/demos/optStokes2D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    25154 2023-11-17 16:51:20.000000 opytimal-0.5.5/opytimal/demos/optStokes3D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      841 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/dicts.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:15:00.150488 opytimal-0.5.5/opytimal/dolfin/
--rw-r--r--   0 natanael  (1001) natanael  (1001)     9500 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/__init__.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:15:00.150488 opytimal-0.5.5/opytimal/dolfin/common/
--rw-r--r--   0 natanael  (1001) natanael  (1001)      147 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/common/__init__.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)    16151 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/common/plotting.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     2377 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/common/timer.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:15:00.154488 opytimal-0.5.5/opytimal/dolfin/fem/
--rw-r--r--   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/fem/__init__.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     7426 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/fem/adaptivesolving.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)    18500 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/fem/assembling.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     5225 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/fem/dirichletbc.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     3445 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/fem/errorcontrolgenerator.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     3787 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/fem/form.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     4968 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/fem/formmanipulations.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     2543 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/fem/interpolation.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     3189 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/fem/multimeshdirichletbc.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)    10449 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/fem/norms.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     8408 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/fem/problem.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     6417 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/fem/projection.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     1556 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/fem/solvers.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)    19008 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/fem/solving.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:15:00.154488 opytimal-0.5.5/opytimal/dolfin/function/
--rw-r--r--   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/function/__init__.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     4417 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/function/argument.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     4392 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/function/constant.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)    15995 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/function/expression.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)    21184 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/function/function.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     9303 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/function/functionspace.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     5237 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/function/jit.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     9319 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/function/multimeshfunction.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     5537 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/function/multimeshfunctionspace.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     7294 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/function/specialfunctions.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:15:00.154488 opytimal-0.5.5/opytimal/dolfin/io/
--rw-r--r--   0 natanael  (1001) natanael  (1001)     1093 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/io/__init__.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:15:00.154488 opytimal-0.5.5/opytimal/dolfin/jit/
--rw-r--r--   0 natanael  (1001) natanael  (1001)      564 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/jit/__init__.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     6538 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/jit/jit.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     3552 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/jit/pybind11jit.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:15:00.154488 opytimal-0.5.5/opytimal/dolfin/la/
--rw-r--r--   0 natanael  (1001) natanael  (1001)     2150 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/la/__init__.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     2148 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/la/solver.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:15:00.154488 opytimal-0.5.5/opytimal/dolfin/mesh/
--rw-r--r--   0 natanael  (1001) natanael  (1001)     3083 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/mesh/__init__.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     6123 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/mesh/ale.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)      633 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/mesh/meshfunction.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)      703 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/mesh/meshvaluecollection.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     3556 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/mesh/subdomain.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     4148 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/mesh/svgtools.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)      874 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/mesh/ufl_util.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:15:00.154488 opytimal-0.5.5/opytimal/dolfin/multistage/
--rw-r--r--   0 natanael  (1001) natanael  (1001)      588 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/multistage/__init__.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     4886 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/multistage/factorize.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)    29902 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/multistage/multistagescheme.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)     1980 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/multistage/multistagesolvers.py
--rw-r--r--   0 natanael  (1001) natanael  (1001)    22460 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/multistage/rushlarsenschemes.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:15:00.154488 opytimal-0.5.5/opytimal/dolfin/parameter/
--rw-r--r--   0 natanael  (1001) natanael  (1001)     2600 2024-04-23 12:11:01.000000 opytimal-0.5.5/opytimal/dolfin/parameter/__init__.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    63651 2023-11-17 13:15:29.000000 opytimal-0.5.5/opytimal/fenics.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     1208 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/files.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      321 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/functions.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      105 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/mathFunctions.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    13269 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/meshes.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      798 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/modules.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      339 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/numeric.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      912 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/parallel.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    89570 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/plots.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     3695 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/profiler.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     2090 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/settings.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    21633 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/string.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      447 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/symbols.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      344 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/tables.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     1546 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/tests.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     2504 2023-11-17 11:54:51.000000 opytimal-0.5.5/opytimal/types.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:15:00.154488 opytimal-0.5.5/opytimal.egg-info/
--rw-r--r--   0 natanael  (1001) natanael  (1001)     1080 2024-04-23 12:15:00.000000 opytimal-0.5.5/opytimal.egg-info/PKG-INFO
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     2572 2024-04-23 12:15:00.000000 opytimal-0.5.5/opytimal.egg-info/SOURCES.txt
--rw-rw-r--   0 natanael  (1001) natanael  (1001)        1 2024-04-23 12:15:00.000000 opytimal-0.5.5/opytimal.egg-info/dependency_links.txt
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      276 2024-04-23 12:15:00.000000 opytimal-0.5.5/opytimal.egg-info/requires.txt
--rw-rw-r--   0 natanael  (1001) natanael  (1001)        9 2024-04-23 12:15:00.000000 opytimal-0.5.5/opytimal.egg-info/top_level.txt
--rw-rw-r--   0 natanael  (1001) natanael  (1001)       38 2024-04-23 12:15:00.154488 opytimal-0.5.5/setup.cfg
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     1383 2024-04-23 12:14:57.000000 opytimal-0.5.5/setup.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:19:51.743316 opytimal-0.5.6/
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     7048 2023-09-12 14:54:54.000000 opytimal-0.5.6/LICENSE
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     1080 2024-04-23 12:19:51.743316 opytimal-0.5.6/PKG-INFO
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      488 2023-11-17 15:48:02.000000 opytimal-0.5.6/README.md
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:19:51.739316 opytimal-0.5.6/opytimal/
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     2076 2024-04-23 12:19:48.000000 opytimal-0.5.6/opytimal/__init__.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      613 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/_vars.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    49923 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/analytical.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     9266 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/arrays.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    12180 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/decorator.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:19:51.739316 opytimal-0.5.6/opytimal/demos/
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      752 2023-11-17 17:30:06.000000 opytimal-0.5.6/opytimal/demos/__init__.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    29176 2023-11-17 16:51:20.000000 opytimal-0.5.6/opytimal/demos/optHeat1D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    26417 2023-11-17 16:51:20.000000 opytimal-0.5.6/opytimal/demos/optHeat2D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    22362 2023-11-17 16:51:20.000000 opytimal-0.5.6/opytimal/demos/optPoisson1D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    24873 2023-11-17 16:51:20.000000 opytimal-0.5.6/opytimal/demos/optPoisson2D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    23922 2023-11-17 16:51:20.000000 opytimal-0.5.6/opytimal/demos/optPoisson3D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    27362 2023-11-17 16:51:20.000000 opytimal-0.5.6/opytimal/demos/optStokes2D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    25154 2023-11-17 16:51:20.000000 opytimal-0.5.6/opytimal/demos/optStokes3D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      841 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/dicts.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:19:51.739316 opytimal-0.5.6/opytimal/dolfin/
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     9500 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/__init__.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:19:51.739316 opytimal-0.5.6/opytimal/dolfin/common/
+-rw-r--r--   0 natanael  (1001) natanael  (1001)      147 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/common/__init__.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)    16151 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/common/plotting.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     2377 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/common/timer.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:19:51.739316 opytimal-0.5.6/opytimal/dolfin/fem/
+-rw-r--r--   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/fem/__init__.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     7426 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/fem/adaptivesolving.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)    18500 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/fem/assembling.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     5225 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/fem/dirichletbc.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     3445 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/fem/errorcontrolgenerator.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     3787 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/fem/form.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     4968 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/fem/formmanipulations.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     2543 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/fem/interpolation.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     3189 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/fem/multimeshdirichletbc.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)    10449 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/fem/norms.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     8408 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/fem/problem.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     6417 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/fem/projection.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     1556 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/fem/solvers.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)    19008 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/fem/solving.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:19:51.739316 opytimal-0.5.6/opytimal/dolfin/function/
+-rw-r--r--   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/function/__init__.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     4417 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/function/argument.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     4392 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/function/constant.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)    15995 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/function/expression.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)    21184 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/function/function.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     9303 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/function/functionspace.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     5237 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/function/jit.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     9319 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/function/multimeshfunction.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     5537 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/function/multimeshfunctionspace.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     7294 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/function/specialfunctions.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:19:51.743316 opytimal-0.5.6/opytimal/dolfin/io/
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     1093 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/io/__init__.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:19:51.743316 opytimal-0.5.6/opytimal/dolfin/jit/
+-rw-r--r--   0 natanael  (1001) natanael  (1001)      564 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/jit/__init__.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     6538 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/jit/jit.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     3552 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/jit/pybind11jit.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:19:51.743316 opytimal-0.5.6/opytimal/dolfin/la/
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     2150 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/la/__init__.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     2148 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/la/solver.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:19:51.743316 opytimal-0.5.6/opytimal/dolfin/mesh/
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     3083 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/mesh/__init__.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     6123 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/mesh/ale.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)      633 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/mesh/meshfunction.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)      703 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/mesh/meshvaluecollection.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     3556 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/mesh/subdomain.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     4148 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/mesh/svgtools.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)      874 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/mesh/ufl_util.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:19:51.743316 opytimal-0.5.6/opytimal/dolfin/multistage/
+-rw-r--r--   0 natanael  (1001) natanael  (1001)      588 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/multistage/__init__.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     4886 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/multistage/factorize.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)    29902 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/multistage/multistagescheme.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     1980 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/multistage/multistagesolvers.py
+-rw-r--r--   0 natanael  (1001) natanael  (1001)    22460 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/multistage/rushlarsenschemes.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:19:51.743316 opytimal-0.5.6/opytimal/dolfin/parameter/
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     2600 2024-04-23 12:11:01.000000 opytimal-0.5.6/opytimal/dolfin/parameter/__init__.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    63651 2023-11-17 13:15:29.000000 opytimal-0.5.6/opytimal/fenics.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     1208 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/files.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      321 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/functions.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      105 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/mathFunctions.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    13269 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/meshes.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      798 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/modules.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      339 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/numeric.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      912 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/parallel.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    89570 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/plots.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     3695 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/profiler.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     2090 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/settings.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    21633 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/string.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      447 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/symbols.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      344 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/tables.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     1546 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/tests.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     2504 2023-11-17 11:54:51.000000 opytimal-0.5.6/opytimal/types.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 12:19:51.743316 opytimal-0.5.6/opytimal.egg-info/
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     1080 2024-04-23 12:19:51.000000 opytimal-0.5.6/opytimal.egg-info/PKG-INFO
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     2572 2024-04-23 12:19:51.000000 opytimal-0.5.6/opytimal.egg-info/SOURCES.txt
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)        1 2024-04-23 12:19:51.000000 opytimal-0.5.6/opytimal.egg-info/dependency_links.txt
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      276 2024-04-23 12:19:51.000000 opytimal-0.5.6/opytimal.egg-info/requires.txt
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)        9 2024-04-23 12:19:51.000000 opytimal-0.5.6/opytimal.egg-info/top_level.txt
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)       38 2024-04-23 12:19:51.743316 opytimal-0.5.6/setup.cfg
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     1383 2024-04-23 12:19:48.000000 opytimal-0.5.6/setup.py
```

### Comparing `opytimal-0.5.5/LICENSE` & `opytimal-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/PKG-INFO` & `opytimal-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opytimal
-Version: 0.5.5
+Version: 0.5.6
 Summary: Optimal control PDE-based solver
 Author: Natanael Quintino
 Author-email: natanael.quintino@ipiaget.pt
 License: CC0 1.0 Universal
 Keywords: optimalcontrol,FEniCS,FuildDynamics,NavierStokes,Stokes
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opytimal-0.5.5/opytimal/__init__.py` & `opytimal-0.5.6/opytimal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 '''
 Opytimal module
 '''
 
 from .dolfin import *
 
+import dolfin
+
 from .numeric import getPow10
 from .profiler import ProgressBar
 from .tests import testLoop
 from .parallel import parallel
 from .types import Tuple, Union
 from .files import createFolder
 from .profiler import tic, toc, ticRAM, tocRAM
@@ -32,15 +34,15 @@
                      getDomainLabels, replaceBoundNameByMark,
                      getMeasure, evaluateErrors, Zero, getAdjointSystem,
                      getOptimalConditionsSystem, evaluateCost,
                      getLocal, setLocal, showProblemData,
                      getFunctionExpressions)
 
 
-__version__ = "0.5.5"
+__version__ = "0.5.6"
 
 def __getattr__(attr):
     # Warn for expired attributes
     import warnings
 
     if attr == "demos":
         import opytimal.demos as demos
```

### Comparing `opytimal-0.5.5/opytimal/_vars.py` & `opytimal-0.5.6/opytimal/_vars.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/analytical.py` & `opytimal-0.5.6/opytimal/analytical.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/arrays.py` & `opytimal-0.5.6/opytimal/arrays.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/decorator.py` & `opytimal-0.5.6/opytimal/decorator.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/demos/__init__.py` & `opytimal-0.5.6/opytimal/demos/__init__.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/demos/optHeat1D.py` & `opytimal-0.5.6/opytimal/demos/optHeat1D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/demos/optHeat2D.py` & `opytimal-0.5.6/opytimal/demos/optHeat2D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/demos/optPoisson1D.py` & `opytimal-0.5.6/opytimal/demos/optPoisson1D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/demos/optPoisson2D.py` & `opytimal-0.5.6/opytimal/demos/optPoisson2D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/demos/optPoisson3D.py` & `opytimal-0.5.6/opytimal/demos/optPoisson3D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/demos/optStokes2D.py` & `opytimal-0.5.6/opytimal/demos/optStokes2D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/demos/optStokes3D.py` & `opytimal-0.5.6/opytimal/demos/optStokes3D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dicts.py` & `opytimal-0.5.6/opytimal/dicts.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/__init__.py` & `opytimal-0.5.6/opytimal/dolfin/__init__.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/common/plotting.py` & `opytimal-0.5.6/opytimal/dolfin/common/plotting.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/common/timer.py` & `opytimal-0.5.6/opytimal/dolfin/common/timer.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/fem/adaptivesolving.py` & `opytimal-0.5.6/opytimal/dolfin/fem/adaptivesolving.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/fem/assembling.py` & `opytimal-0.5.6/opytimal/dolfin/fem/assembling.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/fem/dirichletbc.py` & `opytimal-0.5.6/opytimal/dolfin/fem/dirichletbc.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/fem/errorcontrolgenerator.py` & `opytimal-0.5.6/opytimal/dolfin/fem/errorcontrolgenerator.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/fem/form.py` & `opytimal-0.5.6/opytimal/dolfin/fem/form.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/fem/formmanipulations.py` & `opytimal-0.5.6/opytimal/dolfin/fem/formmanipulations.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/fem/interpolation.py` & `opytimal-0.5.6/opytimal/dolfin/fem/interpolation.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/fem/multimeshdirichletbc.py` & `opytimal-0.5.6/opytimal/dolfin/fem/multimeshdirichletbc.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/fem/norms.py` & `opytimal-0.5.6/opytimal/dolfin/fem/norms.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/fem/problem.py` & `opytimal-0.5.6/opytimal/dolfin/fem/problem.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/fem/projection.py` & `opytimal-0.5.6/opytimal/dolfin/fem/projection.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/fem/solvers.py` & `opytimal-0.5.6/opytimal/dolfin/fem/solvers.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/fem/solving.py` & `opytimal-0.5.6/opytimal/dolfin/fem/solving.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/function/argument.py` & `opytimal-0.5.6/opytimal/dolfin/function/argument.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/function/constant.py` & `opytimal-0.5.6/opytimal/dolfin/function/constant.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/function/expression.py` & `opytimal-0.5.6/opytimal/dolfin/function/expression.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/function/function.py` & `opytimal-0.5.6/opytimal/dolfin/function/function.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/function/functionspace.py` & `opytimal-0.5.6/opytimal/dolfin/function/functionspace.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/function/jit.py` & `opytimal-0.5.6/opytimal/dolfin/function/jit.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/function/multimeshfunction.py` & `opytimal-0.5.6/opytimal/dolfin/function/multimeshfunction.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/function/multimeshfunctionspace.py` & `opytimal-0.5.6/opytimal/dolfin/function/multimeshfunctionspace.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/function/specialfunctions.py` & `opytimal-0.5.6/opytimal/dolfin/function/specialfunctions.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/io/__init__.py` & `opytimal-0.5.6/opytimal/dolfin/io/__init__.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/jit/__init__.py` & `opytimal-0.5.6/opytimal/dolfin/jit/__init__.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/jit/jit.py` & `opytimal-0.5.6/opytimal/dolfin/jit/jit.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/jit/pybind11jit.py` & `opytimal-0.5.6/opytimal/dolfin/jit/pybind11jit.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/la/__init__.py` & `opytimal-0.5.6/opytimal/dolfin/la/__init__.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/la/solver.py` & `opytimal-0.5.6/opytimal/dolfin/la/solver.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/mesh/__init__.py` & `opytimal-0.5.6/opytimal/dolfin/mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/mesh/ale.py` & `opytimal-0.5.6/opytimal/dolfin/mesh/ale.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/mesh/meshfunction.py` & `opytimal-0.5.6/opytimal/dolfin/mesh/meshfunction.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/mesh/meshvaluecollection.py` & `opytimal-0.5.6/opytimal/dolfin/mesh/meshvaluecollection.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/mesh/subdomain.py` & `opytimal-0.5.6/opytimal/dolfin/mesh/subdomain.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/mesh/svgtools.py` & `opytimal-0.5.6/opytimal/dolfin/mesh/svgtools.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/mesh/ufl_util.py` & `opytimal-0.5.6/opytimal/dolfin/mesh/ufl_util.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/multistage/__init__.py` & `opytimal-0.5.6/opytimal/dolfin/multistage/__init__.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/multistage/factorize.py` & `opytimal-0.5.6/opytimal/dolfin/multistage/factorize.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/multistage/multistagescheme.py` & `opytimal-0.5.6/opytimal/dolfin/multistage/multistagescheme.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/multistage/multistagesolvers.py` & `opytimal-0.5.6/opytimal/dolfin/multistage/multistagesolvers.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/multistage/rushlarsenschemes.py` & `opytimal-0.5.6/opytimal/dolfin/multistage/rushlarsenschemes.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/dolfin/parameter/__init__.py` & `opytimal-0.5.6/opytimal/dolfin/parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/fenics.py` & `opytimal-0.5.6/opytimal/fenics.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/files.py` & `opytimal-0.5.6/opytimal/files.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/meshes.py` & `opytimal-0.5.6/opytimal/meshes.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/modules.py` & `opytimal-0.5.6/opytimal/modules.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/parallel.py` & `opytimal-0.5.6/opytimal/parallel.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/plots.py` & `opytimal-0.5.6/opytimal/plots.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/profiler.py` & `opytimal-0.5.6/opytimal/profiler.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/settings.py` & `opytimal-0.5.6/opytimal/settings.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/string.py` & `opytimal-0.5.6/opytimal/string.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/tests.py` & `opytimal-0.5.6/opytimal/tests.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal/types.py` & `opytimal-0.5.6/opytimal/types.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/opytimal.egg-info/PKG-INFO` & `opytimal-0.5.6/opytimal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opytimal
-Version: 0.5.5
+Version: 0.5.6
 Summary: Optimal control PDE-based solver
 Author: Natanael Quintino
 Author-email: natanael.quintino@ipiaget.pt
 License: CC0 1.0 Universal
 Keywords: optimalcontrol,FEniCS,FuildDynamics,NavierStokes,Stokes
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opytimal-0.5.5/opytimal.egg-info/SOURCES.txt` & `opytimal-0.5.6/opytimal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opytimal-0.5.5/setup.py` & `opytimal-0.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.5.5"
+VERSION = "0.5.6"
 DESCRIPTION = 'Optimal control PDE-based solver'
 LONG_DESCRIPTION = 'Opytimal is a Python/FEniCS framework that have the main goal solve Optimal Control problems considering multiple and mixed controls based to linear and nonlinear PDEs, in addition to can also solve PDEs simply and clearly'
 
 setup(
     name="opytimal",
     version=VERSION,
     description=DESCRIPTION,
```

