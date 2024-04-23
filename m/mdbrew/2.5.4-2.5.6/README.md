# Comparing `tmp/mdbrew-2.5.4.tar.gz` & `tmp/mdbrew-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdbrew-2.5.4.tar", last modified: Mon Jan 15 14:13:41 2024, max compression
+gzip compressed data, was "mdbrew-2.5.6.tar", last modified: Tue Apr 23 11:50:44 2024, max compression
```

## Comparing `mdbrew-2.5.4.tar` & `mdbrew-2.5.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-01-15 14:13:41.149938 mdbrew-2.5.4/
--rw-r--r--   0 minu       (501) staff       (20)    35823 2024-01-15 14:13:22.000000 mdbrew-2.5.4/LICENSE.md
--rw-r--r--   0 minu       (501) staff       (20)      283 2024-01-15 14:13:41.149813 mdbrew-2.5.4/PKG-INFO
--rw-r--r--   0 minu       (501) staff       (20)      703 2024-01-15 14:13:22.000000 mdbrew-2.5.4/README.md
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-01-15 14:13:41.144768 mdbrew-2.5.4/mdbrew/
--rw-r--r--   0 minu       (501) staff       (20)      207 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)      125 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/__version__.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-01-15 14:13:41.146259 mdbrew-2.5.4/mdbrew/analysis/
--rw-r--r--   0 minu       (501) staff       (20)      192 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/analysis/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     2143 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/analysis/atom.py
--rw-r--r--   0 minu       (501) staff       (20)      373 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/analysis/autocorrelation.py
--rw-r--r--   0 minu       (501) staff       (20)     1146 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/analysis/centerofmass.py
--rw-r--r--   0 minu       (501) staff       (20)     2689 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/analysis/hydrogen_bonding.py
--rw-r--r--   0 minu       (501) staff       (20)     5672 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/analysis/msd.py
--rw-r--r--   0 minu       (501) staff       (20)     6358 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/analysis/rdf.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-01-15 14:13:41.146512 mdbrew-2.5.4/mdbrew/application/
--rw-r--r--   0 minu       (501) staff       (20)       20 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/application/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)    10151 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/application/cp2k.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-01-15 14:13:41.146733 mdbrew-2.5.4/mdbrew/main/
--rw-r--r--   0 minu       (501) staff       (20)      158 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     6040 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/brewery.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-01-15 14:13:41.146845 mdbrew-2.5.4/mdbrew/main/fmt/
--rw-r--r--   0 minu       (501) staff       (20)      328 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/fmt/__init__.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-01-15 14:13:41.147171 mdbrew-2.5.4/mdbrew/main/fmt/gromacs/
--rw-r--r--   0 minu       (501) staff       (20)        0 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/fmt/gromacs/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     1029 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/fmt/gromacs/opener_gro.py
--rw-r--r--   0 minu       (501) staff       (20)     4460 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/fmt/gromacs/opener_trr.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-01-15 14:13:41.147482 mdbrew-2.5.4/mdbrew/main/fmt/lammps/
--rw-r--r--   0 minu       (501) staff       (20)        0 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/fmt/lammps/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)      840 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/fmt/lammps/opener_lammpstrj.py
--rw-r--r--   0 minu       (501) staff       (20)     1506 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/fmt/lammps/writer_lmps.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-01-15 14:13:41.147709 mdbrew-2.5.4/mdbrew/main/fmt/pdb/
--rw-r--r--   0 minu       (501) staff       (20)        0 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/fmt/pdb/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     2229 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/fmt/pdb/opener_pdb.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-01-15 14:13:41.148079 mdbrew-2.5.4/mdbrew/main/fmt/vasp/
--rw-r--r--   0 minu       (501) staff       (20)        0 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/fmt/vasp/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     1447 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/fmt/vasp/opener_xdatcar.py
--rw-r--r--   0 minu       (501) staff       (20)     1481 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/fmt/vasp/writer_poscar.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-01-15 14:13:41.148509 mdbrew-2.5.4/mdbrew/main/fmt/xyz/
--rw-r--r--   0 minu       (501) staff       (20)        0 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/fmt/xyz/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     1675 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/fmt/xyz/opener_extxyz.py
--rw-r--r--   0 minu       (501) staff       (20)      542 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/fmt/xyz/opener_xyz.py
--rw-r--r--   0 minu       (501) staff       (20)      684 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/fmt/xyz/writer_xyz.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-01-15 14:13:41.148831 mdbrew-2.5.4/mdbrew/main/interface/
--rw-r--r--   0 minu       (501) staff       (20)      618 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/interface/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     2166 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/interface/opener.py
--rw-r--r--   0 minu       (501) staff       (20)     1699 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/main/interface/writer.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-01-15 14:13:41.149336 mdbrew-2.5.4/mdbrew/tool/
--rw-r--r--   0 minu       (501) staff       (20)       67 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/tool/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     3618 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/tool/colorfont.py
--rw-r--r--   0 minu       (501) staff       (20)     2031 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/tool/decorator.py
--rw-r--r--   0 minu       (501) staff       (20)      180 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/tool/path.py
--rw-r--r--   0 minu       (501) staff       (20)     1494 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/tool/plot.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-01-15 14:13:41.149632 mdbrew-2.5.4/mdbrew/tool/space/
--rw-r--r--   0 minu       (501) staff       (20)       57 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/tool/space/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)    15735 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/tool/space/_periodic_kdtree.py
--rw-r--r--   0 minu       (501) staff       (20)     2216 2024-01-15 14:13:22.000000 mdbrew-2.5.4/mdbrew/tool/space/_spacer.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-01-15 14:13:41.145324 mdbrew-2.5.4/mdbrew.egg-info/
--rw-r--r--   0 minu       (501) staff       (20)      283 2024-01-15 14:13:41.000000 mdbrew-2.5.4/mdbrew.egg-info/PKG-INFO
--rw-r--r--   0 minu       (501) staff       (20)     1403 2024-01-15 14:13:41.000000 mdbrew-2.5.4/mdbrew.egg-info/SOURCES.txt
--rw-r--r--   0 minu       (501) staff       (20)        1 2024-01-15 14:13:41.000000 mdbrew-2.5.4/mdbrew.egg-info/dependency_links.txt
--rw-r--r--   0 minu       (501) staff       (20)        1 2024-01-15 14:13:34.000000 mdbrew-2.5.4/mdbrew.egg-info/not-zip-safe
--rw-r--r--   0 minu       (501) staff       (20)        7 2024-01-15 14:13:41.000000 mdbrew-2.5.4/mdbrew.egg-info/top_level.txt
--rw-r--r--   0 minu       (501) staff       (20)       38 2024-01-15 14:13:41.149974 mdbrew-2.5.4/setup.cfg
--rw-r--r--   0 minu       (501) staff       (20)      816 2024-01-15 14:13:22.000000 mdbrew-2.5.4/setup.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-04-23 11:50:44.009779 mdbrew-2.5.6/
+-rw-r--r--   0 minu       (501) staff       (20)    35823 2024-04-23 11:50:24.000000 mdbrew-2.5.6/LICENSE.md
+-rw-r--r--   0 minu       (501) staff       (20)      283 2024-04-23 11:50:44.009634 mdbrew-2.5.6/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)      703 2024-04-23 11:50:24.000000 mdbrew-2.5.6/README.md
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-04-23 11:50:44.002820 mdbrew-2.5.6/mdbrew/
+-rw-r--r--   0 minu       (501) staff       (20)      240 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)      125 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/__version__.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-04-23 11:50:44.004752 mdbrew-2.5.6/mdbrew/analysis/
+-rw-r--r--   0 minu       (501) staff       (20)      242 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/analysis/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     2143 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/analysis/atom.py
+-rw-r--r--   0 minu       (501) staff       (20)      338 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/analysis/autocorrelation.py
+-rw-r--r--   0 minu       (501) staff       (20)     1146 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/analysis/centerofmass.py
+-rw-r--r--   0 minu       (501) staff       (20)     4056 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/analysis/hydrogenbonding.py
+-rw-r--r--   0 minu       (501) staff       (20)     5672 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/analysis/msd.py
+-rw-r--r--   0 minu       (501) staff       (20)     6358 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/analysis/rdf.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-04-23 11:50:44.005125 mdbrew-2.5.6/mdbrew/application/
+-rw-r--r--   0 minu       (501) staff       (20)       20 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/application/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)    10151 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/application/cp2k.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-04-23 11:50:44.005508 mdbrew-2.5.6/mdbrew/main/
+-rw-r--r--   0 minu       (501) staff       (20)      158 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     6079 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/brewery.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-04-23 11:50:44.005728 mdbrew-2.5.6/mdbrew/main/fmt/
+-rw-r--r--   0 minu       (501) staff       (20)      328 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/fmt/__init__.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-04-23 11:50:44.006102 mdbrew-2.5.6/mdbrew/main/fmt/gromacs/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/fmt/gromacs/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     1029 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/fmt/gromacs/opener_gro.py
+-rw-r--r--   0 minu       (501) staff       (20)     4460 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/fmt/gromacs/opener_trr.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-04-23 11:50:44.006585 mdbrew-2.5.6/mdbrew/main/fmt/lammps/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/fmt/lammps/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)      840 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/fmt/lammps/opener_lammpstrj.py
+-rw-r--r--   0 minu       (501) staff       (20)     1506 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/fmt/lammps/writer_lmps.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-04-23 11:50:44.006803 mdbrew-2.5.6/mdbrew/main/fmt/pdb/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/fmt/pdb/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     2229 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/fmt/pdb/opener_pdb.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-04-23 11:50:44.007210 mdbrew-2.5.6/mdbrew/main/fmt/vasp/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/fmt/vasp/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     1447 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/fmt/vasp/opener_xdatcar.py
+-rw-r--r--   0 minu       (501) staff       (20)     1481 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/fmt/vasp/writer_poscar.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-04-23 11:50:44.007675 mdbrew-2.5.6/mdbrew/main/fmt/xyz/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/fmt/xyz/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     1675 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/fmt/xyz/opener_extxyz.py
+-rw-r--r--   0 minu       (501) staff       (20)      542 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/fmt/xyz/opener_xyz.py
+-rw-r--r--   0 minu       (501) staff       (20)      684 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/fmt/xyz/writer_xyz.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-04-23 11:50:44.008032 mdbrew-2.5.6/mdbrew/main/interface/
+-rw-r--r--   0 minu       (501) staff       (20)      618 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/interface/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     2145 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/interface/opener.py
+-rw-r--r--   0 minu       (501) staff       (20)     1699 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/main/interface/writer.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-04-23 11:50:44.008965 mdbrew-2.5.6/mdbrew/tool/
+-rw-r--r--   0 minu       (501) staff       (20)      104 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/tool/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     3618 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/tool/colorfont.py
+-rw-r--r--   0 minu       (501) staff       (20)     2037 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/tool/decorator.py
+-rw-r--r--   0 minu       (501) staff       (20)      180 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/tool/path.py
+-rw-r--r--   0 minu       (501) staff       (20)     1497 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/tool/plot.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-04-23 11:50:44.009422 mdbrew-2.5.6/mdbrew/tool/space/
+-rw-r--r--   0 minu       (501) staff       (20)       57 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/tool/space/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)    15735 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/tool/space/_periodic_kdtree.py
+-rw-r--r--   0 minu       (501) staff       (20)     2216 2024-04-23 11:50:24.000000 mdbrew-2.5.6/mdbrew/tool/space/_spacer.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2024-04-23 11:50:44.003558 mdbrew-2.5.6/mdbrew.egg-info/
+-rw-r--r--   0 minu       (501) staff       (20)      283 2024-04-23 11:50:43.000000 mdbrew-2.5.6/mdbrew.egg-info/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)     1402 2024-04-23 11:50:43.000000 mdbrew-2.5.6/mdbrew.egg-info/SOURCES.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2024-04-23 11:50:43.000000 mdbrew-2.5.6/mdbrew.egg-info/dependency_links.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2024-04-23 11:50:43.000000 mdbrew-2.5.6/mdbrew.egg-info/not-zip-safe
+-rw-r--r--   0 minu       (501) staff       (20)        7 2024-04-23 11:50:43.000000 mdbrew-2.5.6/mdbrew.egg-info/top_level.txt
+-rw-r--r--   0 minu       (501) staff       (20)       38 2024-04-23 11:50:44.009826 mdbrew-2.5.6/setup.cfg
+-rw-r--r--   0 minu       (501) staff       (20)      816 2024-04-23 11:50:24.000000 mdbrew-2.5.6/setup.py
```

### Comparing `mdbrew-2.5.4/LICENSE.md` & `mdbrew-2.5.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/README.md` & `mdbrew-2.5.6/README.md`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/analysis/atom.py` & `mdbrew-2.5.6/mdbrew/analysis/atom.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/analysis/centerofmass.py` & `mdbrew-2.5.6/mdbrew/analysis/centerofmass.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/analysis/msd.py` & `mdbrew-2.5.6/mdbrew/analysis/msd.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/analysis/rdf.py` & `mdbrew-2.5.6/mdbrew/analysis/rdf.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/application/cp2k.py` & `mdbrew-2.5.6/mdbrew/application/cp2k.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/main/brewery.py` & `mdbrew-2.5.6/mdbrew/main/brewery.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "fx": float,
     "fy": float,
     "fz": float,
     "vx": float,
     "vy": float,
     "vz": float,
     "id": int,
+    "idx": int,
     "atom": str,
     "element": str,
     "resid": str,
     "type": str,
 }
 
 
@@ -151,15 +152,15 @@
     def order(self, what: str = None):
         return Brewery(trj_file=self._path, fmt=self.fmt, what=what, **self._kwrgs)
 
     def reorder(self):
         return Brewery(trj_file=self._path, fmt=self.fmt, what=self._what, **self._kwrgs)
 
     @color_tqdm(name="FRAME")
-    def frange(self, start: int = 0, end: int = None, step: int = 1, verbose: bool = False):
+    def frange(self, start: int = 0, end: int = None, step: int = 1, *, verbose: bool = False, total: int = None):
         assert end is None or start < end, "start should be lower than end"
         self.move_frame(num=int(start))
         try:
             while self.frame != end:
                 if (self.frame - start) % step == 0:
                     yield self.frame
                 self.next_frame()
```

### Comparing `mdbrew-2.5.4/mdbrew/main/fmt/gromacs/opener_gro.py` & `mdbrew-2.5.6/mdbrew/main/fmt/gromacs/opener_gro.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/main/fmt/gromacs/opener_trr.py` & `mdbrew-2.5.6/mdbrew/main/fmt/gromacs/opener_trr.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/main/fmt/lammps/opener_lammpstrj.py` & `mdbrew-2.5.6/mdbrew/main/fmt/lammps/opener_lammpstrj.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/main/fmt/lammps/writer_lmps.py` & `mdbrew-2.5.6/mdbrew/main/fmt/lammps/writer_lmps.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/main/fmt/pdb/opener_pdb.py` & `mdbrew-2.5.6/mdbrew/main/fmt/pdb/opener_pdb.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/main/fmt/vasp/opener_xdatcar.py` & `mdbrew-2.5.6/mdbrew/main/fmt/vasp/opener_xdatcar.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/main/fmt/vasp/writer_poscar.py` & `mdbrew-2.5.6/mdbrew/main/fmt/vasp/writer_poscar.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/main/fmt/xyz/opener_extxyz.py` & `mdbrew-2.5.6/mdbrew/main/fmt/xyz/opener_extxyz.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/main/fmt/xyz/opener_xyz.py` & `mdbrew-2.5.6/mdbrew/main/fmt/xyz/opener_xyz.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/main/fmt/xyz/writer_xyz.py` & `mdbrew-2.5.6/mdbrew/main/fmt/xyz/writer_xyz.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/main/interface/__init__.py` & `mdbrew-2.5.6/mdbrew/main/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/main/interface/opener.py` & `mdbrew-2.5.6/mdbrew/main/interface/opener.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,16 +59,15 @@
 
     @abstractmethod
     def _make_one_frame_data(self, file):
         pass
 
     def _skip_the_line(self, file):
         if self.read_mode == "r":
-            for _ in range(self.skip_head):
-                file.readline()
+            [next(file) for _ in range(self.skip_head)]
         elif self.read_mode == "rb":
             file.read(self.skip_head)
         else:
             raise ValueError("plz input correct read mode")
 
 
 opener_programs: Dict[str, Type[OpenerInterface]] = {}
```

### Comparing `mdbrew-2.5.4/mdbrew/main/interface/writer.py` & `mdbrew-2.5.6/mdbrew/main/interface/writer.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/tool/colorfont.py` & `mdbrew-2.5.6/mdbrew/tool/colorfont.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/tool/decorator.py` & `mdbrew-2.5.6/mdbrew/tool/decorator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from time import time
 from tqdm import tqdm
 from ..tool.colorfont import color
 
+
 __all__ = ["check_tab", "color_print", "color_print_verbose"]
 
 
 # determine the tab
 def check_tab(name: str) -> int:
     TAB_SIZE = 8
     str_number = len(name)
@@ -51,16 +52,16 @@
 
     return deco
 
 
 def color_tqdm(name):
     def deco(func):
         def inner(*args, **kwrgs):
-            verbose = kwrgs.pop("verbose", False)
-            if verbose:
-                return tqdm(func(verbose=verbose, *args, **kwrgs), desc=f"[ {color.font_magenta}{name}{color.reset} ]")
-            else:
-                return func(verbose=verbose, *args, **kwrgs)
+            if kwrgs.get("verbose", False):
+                total = kwrgs.get("total", None)
+                desc = f"[ {color.font_magenta}{name}{color.reset} ]"
+                return tqdm(func(*args, **kwrgs), desc=desc, total=total)
+            return func(*args, **kwrgs)
 
         return inner
 
     return deco
```

### Comparing `mdbrew-2.5.4/mdbrew/tool/plot.py` & `mdbrew-2.5.6/mdbrew/tool/plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import matplotlib.pyplot as plt
 
 
-def set_format():
+def set_format(font: str = "sans serif"):
     plt.rc("text")  # , usetex=True)
-    plt.rcParams["font.family"] = "Serif"
+    plt.rcParams["font.family"] = font
     plt.rcParams["mathtext.fontset"] = "custom"
-    plt.rcParams["mathtext.it"] = "Serif"
-    plt.rcParams["mathtext.rm"] = "Serif"
-    plt.rcParams["mathtext.tt"] = "Serif"
-    plt.rcParams["mathtext.bf"] = "Serif"
-    plt.rcParams["mathtext.cal"] = "Serif"
-    plt.rcParams["mathtext.sf"] = "Serif"
+    plt.rcParams["mathtext.it"] = font
+    plt.rcParams["mathtext.rm"] = font
+    plt.rcParams["mathtext.tt"] = font
+    plt.rcParams["mathtext.bf"] = font
+    plt.rcParams["mathtext.cal"] = font
+    plt.rcParams["mathtext.sf"] = font
 
     plt.rcParams["lines.linewidth"] = 2.0
     plt.rcParams["errorbar.capsize"] = 4
     plt.rcParams["figure.dpi"] = 330
 
     plt.rcParams["xtick.major.size"] = 5
     plt.rcParams["ytick.major.size"] = 5
```

### Comparing `mdbrew-2.5.4/mdbrew/tool/space/_periodic_kdtree.py` & `mdbrew-2.5.6/mdbrew/tool/space/_periodic_kdtree.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew/tool/space/_spacer.py` & `mdbrew-2.5.6/mdbrew/tool/space/_spacer.py`

 * *Files identical despite different names*

### Comparing `mdbrew-2.5.4/mdbrew.egg-info/SOURCES.txt` & `mdbrew-2.5.6/mdbrew.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 mdbrew.egg-info/dependency_links.txt
 mdbrew.egg-info/not-zip-safe
 mdbrew.egg-info/top_level.txt
 mdbrew/analysis/__init__.py
 mdbrew/analysis/atom.py
 mdbrew/analysis/autocorrelation.py
 mdbrew/analysis/centerofmass.py
-mdbrew/analysis/hydrogen_bonding.py
+mdbrew/analysis/hydrogenbonding.py
 mdbrew/analysis/msd.py
 mdbrew/analysis/rdf.py
 mdbrew/application/__init__.py
 mdbrew/application/cp2k.py
 mdbrew/main/__init__.py
 mdbrew/main/brewery.py
 mdbrew/main/fmt/__init__.py
```

### Comparing `mdbrew-2.5.4/setup.py` & `mdbrew-2.5.6/setup.py`

 * *Files identical despite different names*

