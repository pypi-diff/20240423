# Comparing `tmp/scikit-fem-9.0.1.tar.gz` & `tmp/scikit_fem-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-fem-9.0.1.tar", last modified: Fri Jan 12 15:27:01 2024, max compression
+gzip compressed data, was "scikit_fem-9.1.1.tar", last modified: Tue Apr 23 20:03:21 2024, max compression
```

## Comparing `scikit-fem-9.0.1.tar` & `scikit_fem-9.1.1.tar`

### file list

```diff
@@ -1,418 +1,179 @@
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.513788 scikit-fem-9.0.1/
--rw-r--r--   0 gustaft1   (502) staff       (20)     1469 2023-08-05 11:58:55.000000 scikit-fem-9.0.1/LICENSE
--rw-r--r--   0 gustaft1   (502) staff       (20)    31650 2024-01-12 15:27:01.513203 scikit-fem-9.0.1/PKG-INFO
--rw-r--r--   0 gustaft1   (502) staff       (20)    30535 2024-01-12 15:19:11.000000 scikit-fem-9.0.1/README.md
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.734621 scikit-fem-9.0.1/meshio/
--rw-r--r--   0 gustaft1   (502) staff       (20)      286 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/__about__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1258 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/__init__.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.765112 scikit-fem-9.0.1/meshio/_cli/
--rw-r--r--   0 gustaft1   (502) staff       (20)       44 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/_cli/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1869 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/_cli/_ascii.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1821 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/_cli/_binary.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2391 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/_cli/_compress.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2173 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/_cli/_convert.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1480 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/_cli/_decompress.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1112 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/_cli/_info.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1935 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/_cli/_main.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     3883 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/_common.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.770217 scikit-fem-9.0.1/meshio/_cxml/
--rw-r--r--   0 gustaft1   (502) staff       (20)       41 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/_cxml/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1865 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/_cxml/etree.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      122 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/_exceptions.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      365 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/_files.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     5599 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/_helpers.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    14281 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/_mesh.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     7121 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/_vtk_common.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.776421 scikit-fem-9.0.1/meshio/abaqus/
--rw-r--r--   0 gustaft1   (502) staff       (20)       62 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/abaqus/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    13601 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/abaqus/_abaqus.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.782029 scikit-fem-9.0.1/meshio/ansys/
--rw-r--r--   0 gustaft1   (502) staff       (20)       61 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/ansys/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    15364 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/ansys/_ansys.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.788092 scikit-fem-9.0.1/meshio/avsucd/
--rw-r--r--   0 gustaft1   (502) staff       (20)       62 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/avsucd/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     7381 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/avsucd/_avsucd.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.793060 scikit-fem-9.0.1/meshio/cgns/
--rw-r--r--   0 gustaft1   (502) staff       (20)       60 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/cgns/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2949 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/cgns/_cgns.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.799787 scikit-fem-9.0.1/meshio/dolfin/
--rw-r--r--   0 gustaft1   (502) staff       (20)       62 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/dolfin/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     8106 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/dolfin/_dolfin.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.817160 scikit-fem-9.0.1/meshio/exodus/
--rw-r--r--   0 gustaft1   (502) staff       (20)       62 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/exodus/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    13072 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/exodus/_exodus.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.824447 scikit-fem-9.0.1/meshio/flac3d/
--rw-r--r--   0 gustaft1   (502) staff       (20)       62 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/flac3d/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    18660 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/flac3d/_flac3d.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.843189 scikit-fem-9.0.1/meshio/gmsh/
--rw-r--r--   0 gustaft1   (502) staff       (20)      233 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/gmsh/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    14683 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/gmsh/_gmsh22.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    14659 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/gmsh/_gmsh40.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    28989 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/gmsh/_gmsh41.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     8761 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/gmsh/common.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     3439 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/gmsh/main.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.848381 scikit-fem-9.0.1/meshio/h5m/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/h5m/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     8950 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/h5m/_h5m.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.856441 scikit-fem-9.0.1/meshio/hmf/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/hmf/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     4406 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/hmf/_hmf.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.864382 scikit-fem-9.0.1/meshio/mdpa/
--rw-r--r--   0 gustaft1   (502) staff       (20)       60 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/mdpa/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    16498 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/mdpa/_mdpa.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.871087 scikit-fem-9.0.1/meshio/med/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/med/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    16848 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/med/_med.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.881940 scikit-fem-9.0.1/meshio/medit/
--rw-r--r--   0 gustaft1   (502) staff       (20)       61 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/medit/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    17144 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/medit/_medit.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    10519 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/medit/_medit_internal.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.887087 scikit-fem-9.0.1/meshio/nastran/
--rw-r--r--   0 gustaft1   (502) staff       (20)       63 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/nastran/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    18070 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/nastran/_nastran.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.892980 scikit-fem-9.0.1/meshio/netgen/
--rw-r--r--   0 gustaft1   (502) staff       (20)       62 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/netgen/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    13227 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/netgen/_netgen.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.900485 scikit-fem-9.0.1/meshio/neuroglancer/
--rw-r--r--   0 gustaft1   (502) staff       (20)       68 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/neuroglancer/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2824 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/neuroglancer/_neuroglancer.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.904226 scikit-fem-9.0.1/meshio/obj/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/obj/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     4110 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/obj/_obj.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.907992 scikit-fem-9.0.1/meshio/off/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/off/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2842 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/off/_off.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.912705 scikit-fem-9.0.1/meshio/permas/
--rw-r--r--   0 gustaft1   (502) staff       (20)       62 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/permas/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     8797 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/permas/_permas.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.917609 scikit-fem-9.0.1/meshio/ply/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/ply/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    17515 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/ply/_ply.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.922268 scikit-fem-9.0.1/meshio/stl/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/stl/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     8143 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/stl/_stl.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.927042 scikit-fem-9.0.1/meshio/su2/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/su2/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    11830 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/su2/_su2.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.931757 scikit-fem-9.0.1/meshio/svg/
--rw-r--r--   0 gustaft1   (502) staff       (20)       45 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/svg/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     3363 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/svg/_svg.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.940575 scikit-fem-9.0.1/meshio/tecplot/
--rw-r--r--   0 gustaft1   (502) staff       (20)       63 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/tecplot/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    15144 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/tecplot/_tecplot.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.949235 scikit-fem-9.0.1/meshio/tetgen/
--rw-r--r--   0 gustaft1   (502) staff       (20)       62 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/tetgen/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     6101 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/tetgen/_tetgen.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.954475 scikit-fem-9.0.1/meshio/ugrid/
--rw-r--r--   0 gustaft1   (502) staff       (20)       61 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/ugrid/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     9072 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/ugrid/_ugrid.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.965190 scikit-fem-9.0.1/meshio/vtk/
--rw-r--r--   0 gustaft1   (502) staff       (20)       60 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/vtk/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1027 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/vtk/_main.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    24679 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/vtk/_vtk_42.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    21563 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/vtk/_vtk_51.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.970250 scikit-fem-9.0.1/meshio/vtu/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/vtu/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    33923 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/vtu/_vtu.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.975766 scikit-fem-9.0.1/meshio/wkt/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/wkt/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2821 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/wkt/_wkt.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:00.986271 scikit-fem-9.0.1/meshio/xdmf/
--rw-r--r--   0 gustaft1   (502) staff       (20)      230 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/xdmf/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     5436 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/xdmf/common.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    19112 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/xdmf/main.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    16573 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/meshio/xdmf/time_series.py
--rw-r--r--   0 gustaft1   (502) staff       (20)       93 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/pyproject.toml
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.510511 scikit-fem-9.0.1/scikit_fem.egg-info/
--rw-r--r--   0 gustaft1   (502) staff       (20)    31650 2024-01-12 15:27:00.000000 scikit-fem-9.0.1/scikit_fem.egg-info/PKG-INFO
--rw-r--r--   0 gustaft1   (502) staff       (20)    10308 2024-01-12 15:27:00.000000 scikit-fem-9.0.1/scikit_fem.egg-info/SOURCES.txt
--rw-r--r--   0 gustaft1   (502) staff       (20)        1 2024-01-12 15:27:00.000000 scikit-fem-9.0.1/scikit_fem.egg-info/dependency_links.txt
--rw-r--r--   0 gustaft1   (502) staff       (20)       44 2024-01-12 15:27:00.000000 scikit-fem-9.0.1/scikit_fem.egg-info/requires.txt
--rw-r--r--   0 gustaft1   (502) staff       (20)       13 2024-01-12 15:27:00.000000 scikit-fem-9.0.1/scikit_fem.egg-info/top_level.txt
--rw-r--r--   0 gustaft1   (502) staff       (20)     1117 2024-01-12 15:27:01.516294 scikit-fem-9.0.1/setup.cfg
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.020756 scikit-fem-9.0.1/skfem/
--rw-r--r--   0 gustaft1   (502) staff       (20)      445 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/__about__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      925 2023-12-11 08:08:03.000000 scikit-fem-9.0.1/skfem/__init__.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.024273 scikit-fem-9.0.1/skfem/assembly/
--rw-r--r--   0 gustaft1   (502) staff       (20)     2963 2023-12-11 08:08:03.000000 scikit-fem-9.0.1/skfem/assembly/__init__.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.036816 scikit-fem-9.0.1/skfem/assembly/basis/
--rw-r--r--   0 gustaft1   (502) staff       (20)      397 2023-12-11 08:08:03.000000 scikit-fem-9.0.1/skfem/assembly/basis/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    16695 2024-01-12 15:16:56.000000 scikit-fem-9.0.1/skfem/assembly/basis/abstract_basis.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    10514 2023-06-04 15:41:44.000000 scikit-fem-9.0.1/skfem/assembly/basis/cell_basis.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     8196 2023-01-19 20:25:59.000000 scikit-fem-9.0.1/skfem/assembly/basis/facet_basis.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1304 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/assembly/basis/interior_facet_basis.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    16524 2024-01-12 15:16:56.000000 scikit-fem-9.0.1/skfem/assembly/dofs.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.053970 scikit-fem-9.0.1/skfem/assembly/form/
--rw-r--r--   0 gustaft1   (502) staff       (20)      216 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/assembly/form/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     5412 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/assembly/form/bilinear_form.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     5399 2023-10-25 05:37:49.000000 scikit-fem-9.0.1/skfem/assembly/form/coo_data.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     4186 2023-12-11 08:08:03.000000 scikit-fem-9.0.1/skfem/assembly/form/form.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1841 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/assembly/form/functional.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1448 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/assembly/form/linear_form.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2184 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/assembly/form/trilinear_form.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.084328 scikit-fem-9.0.1/skfem/element/
--rw-r--r--   0 gustaft1   (502) staff       (20)     4734 2023-06-14 06:46:41.000000 scikit-fem-9.0.1/skfem/element/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     3216 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/discrete_field.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     4642 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     4126 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_composite.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1699 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_dg.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     6880 2023-12-23 22:12:15.000000 scikit-fem-9.0.1/skfem/element/element_global.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      898 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_h1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2595 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_hcurl.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1767 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_hdiv.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.108604 scikit-fem-9.0.1/skfem/element/element_hex/
--rw-r--r--   0 gustaft1   (502) staff       (20)      365 2023-06-14 06:46:41.000000 scikit-fem-9.0.1/skfem/element/element_hex/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      424 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_hex/element_hex0.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2241 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_hex/element_hex1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    30688 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_hex/element_hex2.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     3523 2023-06-14 06:46:41.000000 scikit-fem-9.0.1/skfem/element/element_hex/element_hex_c1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1219 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_hex/element_hex_rt1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2887 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_hex/element_hex_s2.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      653 2023-06-02 20:13:04.000000 scikit-fem-9.0.1/skfem/element/element_hex/element_hex_skeleton0.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.122510 scikit-fem-9.0.1/skfem/element/element_line/
--rw-r--r--   0 gustaft1   (502) staff       (20)      337 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_line/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      687 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_line/element_line_hermite.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      794 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_line/element_line_mini.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      404 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_line/element_line_p0.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      686 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_line/element_line_p1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      770 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_line/element_line_p2.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1647 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_line/element_line_pp.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      825 2023-04-19 14:25:14.000000 scikit-fem-9.0.1/skfem/element/element_matrix.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.142289 scikit-fem-9.0.1/skfem/element/element_quad/
--rw-r--r--   0 gustaft1   (502) staff       (20)      416 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_quad/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      423 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_quad/element_quad0.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      958 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_quad/element_quad1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2501 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_quad/element_quad2.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1242 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_quad/element_quad_bfs.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      931 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_quad/element_quad_n1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      755 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_quad/element_quad_rt1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2044 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_quad/element_quad_s2.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2618 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_quad/element_quadp.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.164668 scikit-fem-9.0.1/skfem/element/element_tet/
--rw-r--r--   0 gustaft1   (502) staff       (20)      466 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tet/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     6214 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tet/element_tet_ccr.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1072 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tet/element_tet_cr.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1346 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tet/element_tet_mini.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1685 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tet/element_tet_n1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      409 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tet/element_tet_p0.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1117 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tet/element_tet_p1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2799 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tet/element_tet_p2.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      901 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tet/element_tet_rt1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      564 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tet/element_tet_skeleton_p0.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.218682 scikit-fem-9.0.1/skfem/element/element_tri/
--rw-r--r--   0 gustaft1   (502) staff       (20)     1212 2023-04-19 14:25:14.000000 scikit-fem-9.0.1/skfem/element/element_tri/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1995 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_15param_plate.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1961 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_argyris.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2028 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_bdm1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1423 2023-04-15 15:49:59.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_bell.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      789 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_cr.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1184 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_hermite.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2562 2023-04-19 14:25:14.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_hhj.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1102 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_morley.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      761 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_n1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1844 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_n2.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      405 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_p0.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      846 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_p1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1049 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_p1b.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      570 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_p1g.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1399 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_p2.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1692 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_p2b.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      854 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_p2g.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     3929 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_p3.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     8967 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_p4.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      744 2023-02-14 20:19:31.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_rt1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1695 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_rt2.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      511 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_skeleton_p0.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1003 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_tri/element_tri_skeleton_p1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1653 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_vector.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1532 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/element/element_wedge_1.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.220441 scikit-fem-9.0.1/skfem/experimental/
--rw-r--r--   0 gustaft1   (502) staff       (20)      230 2023-12-11 08:08:03.000000 scikit-fem-9.0.1/skfem/experimental/__init__.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.225174 scikit-fem-9.0.1/skfem/experimental/autodiff/
--rw-r--r--   0 gustaft1   (502) staff       (20)     3172 2023-04-12 07:43:17.000000 scikit-fem-9.0.1/skfem/experimental/autodiff/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2006 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/experimental/autodiff/helpers.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.227466 scikit-fem-9.0.1/skfem/experimental/supermeshing/
--rw-r--r--   0 gustaft1   (502) staff       (20)      217 2023-12-11 08:08:03.000000 scikit-fem-9.0.1/skfem/experimental/supermeshing/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1203 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/generic_utils.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     6226 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/helpers.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.232912 scikit-fem-9.0.1/skfem/io/
--rw-r--r--   0 gustaft1   (502) staff       (20)       40 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/io/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2178 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/io/json.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     9632 2024-01-12 15:16:56.000000 scikit-fem-9.0.1/skfem/io/meshio.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.244446 scikit-fem-9.0.1/skfem/io/meshiolib/
--rw-r--r--   0 gustaft1   (502) staff       (20)      286 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/__about__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1258 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/__init__.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.255768 scikit-fem-9.0.1/skfem/io/meshiolib/_cli/
--rw-r--r--   0 gustaft1   (502) staff       (20)       44 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/_cli/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1869 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/_cli/_ascii.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1821 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/_cli/_binary.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2391 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/_cli/_compress.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2173 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/_cli/_convert.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1480 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/_cli/_decompress.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1112 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/_cli/_info.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1935 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/_cli/_main.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     3883 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/_common.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.257381 scikit-fem-9.0.1/skfem/io/meshiolib/_cxml/
--rw-r--r--   0 gustaft1   (502) staff       (20)       41 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/_cxml/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1865 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/_cxml/etree.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      122 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/_exceptions.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      365 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/_files.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     5599 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/_helpers.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    14281 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/_mesh.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     7121 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/_vtk_common.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.260829 scikit-fem-9.0.1/skfem/io/meshiolib/abaqus/
--rw-r--r--   0 gustaft1   (502) staff       (20)       62 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/abaqus/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    13601 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/abaqus/_abaqus.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.265613 scikit-fem-9.0.1/skfem/io/meshiolib/ansys/
--rw-r--r--   0 gustaft1   (502) staff       (20)       61 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/ansys/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    15364 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/ansys/_ansys.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.268211 scikit-fem-9.0.1/skfem/io/meshiolib/avsucd/
--rw-r--r--   0 gustaft1   (502) staff       (20)       62 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/avsucd/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     7381 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/avsucd/_avsucd.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.270913 scikit-fem-9.0.1/skfem/io/meshiolib/cgns/
--rw-r--r--   0 gustaft1   (502) staff       (20)       60 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/cgns/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2949 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/cgns/_cgns.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.273959 scikit-fem-9.0.1/skfem/io/meshiolib/dolfin/
--rw-r--r--   0 gustaft1   (502) staff       (20)       62 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/dolfin/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     8106 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/dolfin/_dolfin.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.278543 scikit-fem-9.0.1/skfem/io/meshiolib/exodus/
--rw-r--r--   0 gustaft1   (502) staff       (20)       62 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/exodus/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    13072 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/exodus/_exodus.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.282207 scikit-fem-9.0.1/skfem/io/meshiolib/flac3d/
--rw-r--r--   0 gustaft1   (502) staff       (20)       62 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/flac3d/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    18660 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/flac3d/_flac3d.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.297863 scikit-fem-9.0.1/skfem/io/meshiolib/gmsh/
--rw-r--r--   0 gustaft1   (502) staff       (20)      233 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/gmsh/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    14683 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/gmsh/_gmsh22.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    14659 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/gmsh/_gmsh40.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    28989 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/gmsh/_gmsh41.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     8761 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/gmsh/common.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     3439 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/gmsh/main.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.301939 scikit-fem-9.0.1/skfem/io/meshiolib/h5m/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/h5m/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     8950 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/h5m/_h5m.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.305694 scikit-fem-9.0.1/skfem/io/meshiolib/hmf/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/hmf/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     4391 2024-01-08 22:03:04.000000 scikit-fem-9.0.1/skfem/io/meshiolib/hmf/_hmf.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.309549 scikit-fem-9.0.1/skfem/io/meshiolib/mdpa/
--rw-r--r--   0 gustaft1   (502) staff       (20)       60 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/mdpa/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    16498 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/mdpa/_mdpa.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.314784 scikit-fem-9.0.1/skfem/io/meshiolib/med/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/med/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    16838 2024-01-08 22:00:57.000000 scikit-fem-9.0.1/skfem/io/meshiolib/med/_med.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.322201 scikit-fem-9.0.1/skfem/io/meshiolib/medit/
--rw-r--r--   0 gustaft1   (502) staff       (20)       61 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/medit/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    17144 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/medit/_medit.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    10519 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/medit/_medit_internal.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.326022 scikit-fem-9.0.1/skfem/io/meshiolib/nastran/
--rw-r--r--   0 gustaft1   (502) staff       (20)       63 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/nastran/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    18070 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/nastran/_nastran.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.330093 scikit-fem-9.0.1/skfem/io/meshiolib/netgen/
--rw-r--r--   0 gustaft1   (502) staff       (20)       62 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/netgen/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    13227 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/netgen/_netgen.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.332649 scikit-fem-9.0.1/skfem/io/meshiolib/neuroglancer/
--rw-r--r--   0 gustaft1   (502) staff       (20)       68 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/neuroglancer/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2824 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/neuroglancer/_neuroglancer.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.336191 scikit-fem-9.0.1/skfem/io/meshiolib/obj/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/obj/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     4110 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/obj/_obj.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.338818 scikit-fem-9.0.1/skfem/io/meshiolib/off/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/off/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2842 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/off/_off.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.342512 scikit-fem-9.0.1/skfem/io/meshiolib/permas/
--rw-r--r--   0 gustaft1   (502) staff       (20)       62 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/permas/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     8797 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/permas/_permas.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.346472 scikit-fem-9.0.1/skfem/io/meshiolib/ply/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/ply/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    17515 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/ply/_ply.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.349328 scikit-fem-9.0.1/skfem/io/meshiolib/stl/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/stl/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     8143 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/stl/_stl.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.354050 scikit-fem-9.0.1/skfem/io/meshiolib/su2/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/su2/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    11830 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/su2/_su2.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.358942 scikit-fem-9.0.1/skfem/io/meshiolib/svg/
--rw-r--r--   0 gustaft1   (502) staff       (20)       45 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/svg/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     3363 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/svg/_svg.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.365044 scikit-fem-9.0.1/skfem/io/meshiolib/tecplot/
--rw-r--r--   0 gustaft1   (502) staff       (20)       63 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/tecplot/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    15144 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/tecplot/_tecplot.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.368273 scikit-fem-9.0.1/skfem/io/meshiolib/tetgen/
--rw-r--r--   0 gustaft1   (502) staff       (20)       62 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/tetgen/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     6101 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/tetgen/_tetgen.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.371991 scikit-fem-9.0.1/skfem/io/meshiolib/ugrid/
--rw-r--r--   0 gustaft1   (502) staff       (20)       61 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/ugrid/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     9072 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/ugrid/_ugrid.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.380064 scikit-fem-9.0.1/skfem/io/meshiolib/vtk/
--rw-r--r--   0 gustaft1   (502) staff       (20)       60 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/vtk/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1027 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/vtk/_main.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    24679 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/vtk/_vtk_42.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    21563 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/vtk/_vtk_51.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.384200 scikit-fem-9.0.1/skfem/io/meshiolib/vtu/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/vtu/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    33923 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/vtu/_vtu.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.386606 scikit-fem-9.0.1/skfem/io/meshiolib/wkt/
--rw-r--r--   0 gustaft1   (502) staff       (20)       59 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/wkt/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2821 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/wkt/_wkt.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.395773 scikit-fem-9.0.1/skfem/io/meshiolib/xdmf/
--rw-r--r--   0 gustaft1   (502) staff       (20)      230 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/xdmf/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     5436 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/xdmf/common.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    19112 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/xdmf/main.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    16573 2022-03-11 03:11:22.000000 scikit-fem-9.0.1/skfem/io/meshiolib/xdmf/time_series.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.405768 scikit-fem-9.0.1/skfem/mapping/
--rw-r--r--   0 gustaft1   (502) staff       (20)      368 2023-12-11 08:08:03.000000 scikit-fem-9.0.1/skfem/mapping/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2882 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/mapping/mapping.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     8056 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/mapping/mapping_affine.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     9382 2023-12-23 22:12:15.000000 scikit-fem-9.0.1/skfem/mapping/mapping_isoparametric.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.452591 scikit-fem-9.0.1/skfem/mesh/
--rw-r--r--   0 gustaft1   (502) staff       (20)     2701 2023-06-04 15:41:44.000000 scikit-fem-9.0.1/skfem/mesh/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    43062 2024-01-12 15:16:56.000000 scikit-fem-9.0.1/skfem/mesh/mesh.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      693 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/mesh/mesh_2d.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      512 2023-12-23 22:12:15.000000 scikit-fem-9.0.1/skfem/mesh/mesh_2d_2.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1823 2024-01-12 15:16:56.000000 scikit-fem-9.0.1/skfem/mesh/mesh_3d.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     3751 2023-12-23 22:12:15.000000 scikit-fem-9.0.1/skfem/mesh/mesh_dg.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     5486 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/mesh/mesh_hex_1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      325 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/mesh/mesh_hex_1_dg.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1413 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/mesh/mesh_hex_2.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2764 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/mesh/mesh_line_1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      386 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/mesh/mesh_line_1_dg.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     7163 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/mesh/mesh_quad_1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      334 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/mesh/mesh_quad_1_dg.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      864 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/mesh/mesh_quad_2.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      835 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/mesh/mesh_simplex.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    15149 2023-10-25 05:45:58.000000 scikit-fem-9.0.1/skfem/mesh/mesh_tet_1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1923 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/mesh/mesh_tet_2.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    14811 2023-06-02 20:13:04.000000 scikit-fem-9.0.1/skfem/mesh/mesh_tri_1.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      931 2023-12-23 22:12:15.000000 scikit-fem-9.0.1/skfem/mesh/mesh_tri_1_dg.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1587 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/mesh/mesh_tri_2.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1363 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/mesh/mesh_wedge_1.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.461541 scikit-fem-9.0.1/skfem/models/
--rw-r--r--   0 gustaft1   (502) staff       (20)      152 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/models/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1129 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/models/elasticity.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      432 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/models/general.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      369 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/models/poisson.py
--rw-r--r--   0 gustaft1   (502) staff       (20)   121022 2023-06-04 15:41:44.000000 scikit-fem-9.0.1/skfem/quadrature.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     7766 2023-12-23 22:12:15.000000 scikit-fem-9.0.1/skfem/refdom.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     3647 2023-12-11 08:08:03.000000 scikit-fem-9.0.1/skfem/supermeshing.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    22693 2023-12-23 22:12:15.000000 scikit-fem-9.0.1/skfem/utils.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.474823 scikit-fem-9.0.1/skfem/visuals/
--rw-r--r--   0 gustaft1   (502) staff       (20)        7 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/visuals/__init__.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2075 2023-12-23 22:12:15.000000 scikit-fem-9.0.1/skfem/visuals/glvis.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    12010 2023-12-23 22:12:15.000000 scikit-fem-9.0.1/skfem/visuals/matplotlib.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     5232 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/visuals/svg.py
--rw-r--r--   0 gustaft1   (502) staff       (20)      690 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/skfem/visuals/vedo.py
-drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-01-12 15:27:01.509247 scikit-fem-9.0.1/tests/
--rw-r--r--   0 gustaft1   (502) staff       (20)    20423 2023-12-23 22:12:15.000000 scikit-fem-9.0.1/tests/test_assembly.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    18534 2024-01-08 21:58:16.000000 scikit-fem-9.0.1/tests/test_basis.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    14690 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/tests/test_convergence.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     4077 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/tests/test_convergence_h2.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     6407 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/tests/test_convergence_hdiv.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     3260 2024-01-12 15:16:56.000000 scikit-fem-9.0.1/tests/test_dofs.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    11550 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/tests/test_elements.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    10385 2023-12-23 22:12:15.000000 scikit-fem-9.0.1/tests/test_examples.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    12824 2023-01-19 20:25:59.000000 scikit-fem-9.0.1/tests/test_manufactured.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     2437 2023-12-11 08:08:03.000000 scikit-fem-9.0.1/tests/test_mapping.py
--rw-r--r--   0 gustaft1   (502) staff       (20)    21327 2024-01-08 21:58:16.000000 scikit-fem-9.0.1/tests/test_mesh.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     3219 2023-01-19 20:24:53.000000 scikit-fem-9.0.1/tests/test_p_convergence.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     4732 2023-02-14 18:46:32.000000 scikit-fem-9.0.1/tests/test_utils.py
--rw-r--r--   0 gustaft1   (502) staff       (20)     1950 2024-01-12 15:16:51.000000 scikit-fem-9.0.1/tests/test_visuals.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:21.228057 scikit_fem-9.1.1/
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1469 2023-08-05 11:58:55.000000 scikit_fem-9.1.1/LICENSE
+-rw-r--r--   0 gustaft1   (502) staff       (20)    32132 2024-04-23 20:03:21.227617 scikit_fem-9.1.1/PKG-INFO
+-rw-r--r--   0 gustaft1   (502) staff       (20)    31017 2024-04-23 20:02:01.000000 scikit_fem-9.1.1/README.md
+-rw-r--r--   0 gustaft1   (502) staff       (20)       93 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/pyproject.toml
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:21.225613 scikit_fem-9.1.1/scikit_fem.egg-info/
+-rw-r--r--   0 gustaft1   (502) staff       (20)    32132 2024-04-23 20:03:20.000000 scikit_fem-9.1.1/scikit_fem.egg-info/PKG-INFO
+-rw-r--r--   0 gustaft1   (502) staff       (20)     5257 2024-04-23 20:03:20.000000 scikit_fem-9.1.1/scikit_fem.egg-info/SOURCES.txt
+-rw-r--r--   0 gustaft1   (502) staff       (20)        1 2024-04-23 20:03:20.000000 scikit_fem-9.1.1/scikit_fem.egg-info/dependency_links.txt
+-rw-r--r--   0 gustaft1   (502) staff       (20)       44 2024-04-23 20:03:20.000000 scikit_fem-9.1.1/scikit_fem.egg-info/requires.txt
+-rw-r--r--   0 gustaft1   (502) staff       (20)        6 2024-04-23 20:03:20.000000 scikit_fem-9.1.1/scikit_fem.egg-info/top_level.txt
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1117 2024-04-23 20:03:21.230569 scikit_fem-9.1.1/setup.cfg
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:20.822672 scikit_fem-9.1.1/skfem/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      445 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/__about__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      925 2023-12-11 08:08:03.000000 scikit_fem-9.1.1/skfem/__init__.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:20.830626 scikit_fem-9.1.1/skfem/assembly/
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2963 2023-12-11 08:08:03.000000 scikit_fem-9.1.1/skfem/assembly/__init__.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:20.847919 scikit_fem-9.1.1/skfem/assembly/basis/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      397 2023-12-11 08:08:03.000000 scikit_fem-9.1.1/skfem/assembly/basis/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    16815 2024-04-23 19:59:43.000000 scikit_fem-9.1.1/skfem/assembly/basis/abstract_basis.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    10871 2024-04-07 19:42:42.000000 scikit_fem-9.1.1/skfem/assembly/basis/cell_basis.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     8553 2024-04-07 19:42:42.000000 scikit_fem-9.1.1/skfem/assembly/basis/facet_basis.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1397 2024-03-20 12:15:10.000000 scikit_fem-9.1.1/skfem/assembly/basis/interior_facet_basis.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    16524 2024-01-12 15:16:56.000000 scikit_fem-9.1.1/skfem/assembly/dofs.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:20.865499 scikit_fem-9.1.1/skfem/assembly/form/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      216 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/assembly/form/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     5412 2024-03-21 13:16:20.000000 scikit_fem-9.1.1/skfem/assembly/form/bilinear_form.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     5357 2024-03-20 12:18:23.000000 scikit_fem-9.1.1/skfem/assembly/form/coo_data.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     4186 2023-12-11 08:08:03.000000 scikit_fem-9.1.1/skfem/assembly/form/form.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1841 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/assembly/form/functional.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1448 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/assembly/form/linear_form.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2184 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/assembly/form/trilinear_form.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:20.902118 scikit_fem-9.1.1/skfem/element/
+-rw-r--r--   0 gustaft1   (502) staff       (20)     4734 2023-06-14 06:46:41.000000 scikit_fem-9.1.1/skfem/element/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     3216 2024-01-13 08:42:21.000000 scikit_fem-9.1.1/skfem/element/discrete_field.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     4642 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     4126 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_composite.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1699 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_dg.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     6880 2023-12-23 22:12:15.000000 scikit_fem-9.1.1/skfem/element/element_global.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      898 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_h1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2595 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_hcurl.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1767 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_hdiv.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:20.927704 scikit_fem-9.1.1/skfem/element/element_hex/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      365 2023-06-14 06:46:41.000000 scikit_fem-9.1.1/skfem/element/element_hex/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      424 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_hex/element_hex0.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2241 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_hex/element_hex1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    30688 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_hex/element_hex2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     3523 2023-06-14 06:46:41.000000 scikit_fem-9.1.1/skfem/element/element_hex/element_hex_c1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1219 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_hex/element_hex_rt1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2887 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_hex/element_hex_s2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      653 2023-06-02 20:13:04.000000 scikit_fem-9.1.1/skfem/element/element_hex/element_hex_skeleton0.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:20.945348 scikit_fem-9.1.1/skfem/element/element_line/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      337 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_line/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      687 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_line/element_line_hermite.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      794 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_line/element_line_mini.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      404 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_line/element_line_p0.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      686 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_line/element_line_p1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      770 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_line/element_line_p2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1647 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_line/element_line_pp.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      825 2023-04-19 14:25:14.000000 scikit_fem-9.1.1/skfem/element/element_matrix.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:20.975340 scikit_fem-9.1.1/skfem/element/element_quad/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      416 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_quad/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      423 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_quad/element_quad0.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      958 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_quad/element_quad1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2501 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_quad/element_quad2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1242 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_quad/element_quad_bfs.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      931 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_quad/element_quad_n1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      755 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_quad/element_quad_rt1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2044 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_quad/element_quad_s2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2618 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_quad/element_quadp.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:21.002830 scikit_fem-9.1.1/skfem/element/element_tet/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      466 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tet/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     6214 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tet/element_tet_ccr.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1072 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tet/element_tet_cr.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1346 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tet/element_tet_mini.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1685 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tet/element_tet_n1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      412 2024-04-14 20:12:32.000000 scikit_fem-9.1.1/skfem/element/element_tet/element_tet_p0.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1117 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tet/element_tet_p1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2799 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tet/element_tet_p2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      901 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tet/element_tet_rt1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      564 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tet/element_tet_skeleton_p0.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:21.064374 scikit_fem-9.1.1/skfem/element/element_tri/
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1212 2023-04-19 14:25:14.000000 scikit_fem-9.1.1/skfem/element/element_tri/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1995 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_15param_plate.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1961 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_argyris.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2028 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_bdm1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1423 2023-04-15 15:49:59.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_bell.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      789 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_cr.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1184 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_hermite.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2562 2023-04-19 14:25:14.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_hhj.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1102 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_morley.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      761 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_n1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1844 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_n2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      407 2024-04-14 20:12:32.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_p0.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      846 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_p1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1049 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_p1b.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      570 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_p1g.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1399 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_p2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1692 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_p2b.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      854 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_p2g.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     3929 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_p3.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     8967 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_p4.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      744 2023-02-14 20:19:31.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_rt1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1695 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_rt2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      511 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_skeleton_p0.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1003 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_tri/element_tri_skeleton_p1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1653 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_vector.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1532 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/element/element_wedge_1.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:21.066319 scikit_fem-9.1.1/skfem/experimental/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      230 2023-12-11 08:08:03.000000 scikit_fem-9.1.1/skfem/experimental/__init__.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:21.071884 scikit_fem-9.1.1/skfem/experimental/autodiff/
+-rw-r--r--   0 gustaft1   (502) staff       (20)     5614 2024-04-14 21:00:43.000000 scikit_fem-9.1.1/skfem/experimental/autodiff/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1953 2024-02-06 20:09:36.000000 scikit_fem-9.1.1/skfem/experimental/autodiff/helpers.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:21.073993 scikit_fem-9.1.1/skfem/experimental/supermeshing/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      217 2023-12-11 08:08:03.000000 scikit_fem-9.1.1/skfem/experimental/supermeshing/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1203 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/generic_utils.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     6226 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/helpers.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:21.083065 scikit_fem-9.1.1/skfem/io/
+-rw-r--r--   0 gustaft1   (502) staff       (20)       40 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/io/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2178 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/io/json.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     9238 2024-04-14 20:12:32.000000 scikit_fem-9.1.1/skfem/io/meshio.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:21.095692 scikit_fem-9.1.1/skfem/mapping/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      368 2023-12-11 08:08:03.000000 scikit_fem-9.1.1/skfem/mapping/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2882 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/mapping/mapping.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    10389 2024-03-19 10:45:00.000000 scikit_fem-9.1.1/skfem/mapping/mapping_affine.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     9382 2023-12-23 22:12:15.000000 scikit_fem-9.1.1/skfem/mapping/mapping_isoparametric.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:21.152695 scikit_fem-9.1.1/skfem/mesh/
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2701 2023-06-04 15:41:44.000000 scikit_fem-9.1.1/skfem/mesh/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    44802 2024-04-14 20:12:32.000000 scikit_fem-9.1.1/skfem/mesh/mesh.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      693 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/mesh/mesh_2d.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      512 2023-12-23 22:12:15.000000 scikit_fem-9.1.1/skfem/mesh/mesh_2d_2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1823 2024-01-12 15:16:56.000000 scikit_fem-9.1.1/skfem/mesh/mesh_3d.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     3751 2023-12-23 22:12:15.000000 scikit_fem-9.1.1/skfem/mesh/mesh_dg.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     5486 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/mesh/mesh_hex_1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      325 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/mesh/mesh_hex_1_dg.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1413 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/mesh/mesh_hex_2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2764 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/mesh/mesh_line_1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      386 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/mesh/mesh_line_1_dg.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     7163 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/mesh/mesh_quad_1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      334 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/mesh/mesh_quad_1_dg.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      864 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/mesh/mesh_quad_2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      835 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/mesh/mesh_simplex.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    15162 2024-02-06 20:09:36.000000 scikit_fem-9.1.1/skfem/mesh/mesh_tet_1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1923 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/mesh/mesh_tet_2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    14811 2023-06-02 20:13:04.000000 scikit_fem-9.1.1/skfem/mesh/mesh_tri_1.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      931 2023-12-23 22:12:15.000000 scikit_fem-9.1.1/skfem/mesh/mesh_tri_1_dg.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1587 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/mesh/mesh_tri_2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1363 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/mesh/mesh_wedge_1.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:21.164018 scikit_fem-9.1.1/skfem/models/
+-rw-r--r--   0 gustaft1   (502) staff       (20)      152 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/models/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1129 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/models/elasticity.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      432 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/models/general.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      369 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/models/poisson.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)   121022 2023-06-04 15:41:44.000000 scikit_fem-9.1.1/skfem/quadrature.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     7766 2023-12-23 22:12:15.000000 scikit_fem-9.1.1/skfem/refdom.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     3647 2023-12-11 08:08:03.000000 scikit_fem-9.1.1/skfem/supermeshing.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    22725 2024-04-09 21:31:21.000000 scikit_fem-9.1.1/skfem/utils.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:21.179019 scikit_fem-9.1.1/skfem/visuals/
+-rw-r--r--   0 gustaft1   (502) staff       (20)        7 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/visuals/__init__.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2075 2023-12-23 22:12:15.000000 scikit_fem-9.1.1/skfem/visuals/glvis.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    12010 2023-12-23 22:12:15.000000 scikit_fem-9.1.1/skfem/visuals/matplotlib.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     5232 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/visuals/svg.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)      690 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/skfem/visuals/vedo.py
+drwxr-xr-x   0 gustaft1   (502) staff       (20)        0 2024-04-23 20:03:21.224026 scikit_fem-9.1.1/tests/
+-rw-r--r--   0 gustaft1   (502) staff       (20)    20423 2023-12-23 22:12:15.000000 scikit_fem-9.1.1/tests/test_assembly.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     3914 2024-03-20 12:15:10.000000 scikit_fem-9.1.1/tests/test_autodiff.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    19282 2024-03-20 12:15:10.000000 scikit_fem-9.1.1/tests/test_basis.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    14690 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/tests/test_convergence.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     4077 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/tests/test_convergence_h2.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     6407 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/tests/test_convergence_hdiv.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     3260 2024-01-12 15:16:56.000000 scikit_fem-9.1.1/tests/test_dofs.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    11550 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/tests/test_elements.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    10385 2023-12-23 22:12:15.000000 scikit_fem-9.1.1/tests/test_examples.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    12824 2023-01-19 20:25:59.000000 scikit_fem-9.1.1/tests/test_manufactured.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     2884 2024-03-19 10:45:00.000000 scikit_fem-9.1.1/tests/test_mapping.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)    22252 2024-04-14 20:12:32.000000 scikit_fem-9.1.1/tests/test_mesh.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     3219 2023-01-19 20:24:53.000000 scikit_fem-9.1.1/tests/test_p_convergence.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     4732 2023-02-14 18:46:32.000000 scikit_fem-9.1.1/tests/test_utils.py
+-rw-r--r--   0 gustaft1   (502) staff       (20)     1950 2024-01-12 15:16:51.000000 scikit_fem-9.1.1/tests/test_visuals.py
```

### Comparing `scikit-fem-9.0.1/LICENSE` & `scikit_fem-9.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/PKG-INFO` & `scikit_fem-9.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-fem
-Version: 9.0.1
+Version: 9.1.1
 Summary: Simple finite element assemblers
 Home-page: https://github.com/kinnala/scikit-fem
 Author: Tom Gustafsson
 License: BSD-3-Clause
 Project-URL: Code, https://github.com/kinnala/scikit-fem
 Project-URL: Issues, https://github.com/kinnala/scikit-fem/issues
 Classifier: Intended Audience :: Science/Research
@@ -235,14 +235,26 @@
 
 ## Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html)
 with respect to documented and/or tested features.
 
+### [9.1.1] - 2024-04-23
+
+- Fixed: Tests now pass with `numpy==2.0rc1`
+- Fixed: `MappingAffine` now uses lazy evaluation also for element
+  mappings, in addition to boundary mappings
+- Fixed: `MeshTet.init_tensor` uses significantly less memory for
+  large meshes
+- Fixed: `Mesh.load` uses less memory when loading and matching tags
+- Added: `Basis` has new optional `disable_doflocs` kwarg which
+  can be set to `True` to avoid computing `Basis.doflocs`, to reduce memory
+  usage
+
 ### [9.0.1] - 2024-01-12
 
 - Fixed: `ElementVector` works also for split_bases/split_indices in case `mesh.dim() != elem.dim`
 
 ### [9.0.0] - 2023-12-24
 
 - Removed: Python 3.7 support
```

### Comparing `scikit-fem-9.0.1/README.md` & `scikit_fem-9.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,26 @@
 
 ## Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html)
 with respect to documented and/or tested features.
 
+### [9.1.1] - 2024-04-23
+
+- Fixed: Tests now pass with `numpy==2.0rc1`
+- Fixed: `MappingAffine` now uses lazy evaluation also for element
+  mappings, in addition to boundary mappings
+- Fixed: `MeshTet.init_tensor` uses significantly less memory for
+  large meshes
+- Fixed: `Mesh.load` uses less memory when loading and matching tags
+- Added: `Basis` has new optional `disable_doflocs` kwarg which
+  can be set to `True` to avoid computing `Basis.doflocs`, to reduce memory
+  usage
+
 ### [9.0.1] - 2024-01-12
 
 - Fixed: `ElementVector` works also for split_bases/split_indices in case `mesh.dim() != elem.dim`
 
 ### [9.0.0] - 2023-12-24
 
 - Removed: Python 3.7 support
```

### Comparing `scikit-fem-9.0.1/scikit_fem.egg-info/PKG-INFO` & `scikit_fem-9.1.1/scikit_fem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-fem
-Version: 9.0.1
+Version: 9.1.1
 Summary: Simple finite element assemblers
 Home-page: https://github.com/kinnala/scikit-fem
 Author: Tom Gustafsson
 License: BSD-3-Clause
 Project-URL: Code, https://github.com/kinnala/scikit-fem
 Project-URL: Issues, https://github.com/kinnala/scikit-fem/issues
 Classifier: Intended Audience :: Science/Research
@@ -235,14 +235,26 @@
 
 ## Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html)
 with respect to documented and/or tested features.
 
+### [9.1.1] - 2024-04-23
+
+- Fixed: Tests now pass with `numpy==2.0rc1`
+- Fixed: `MappingAffine` now uses lazy evaluation also for element
+  mappings, in addition to boundary mappings
+- Fixed: `MeshTet.init_tensor` uses significantly less memory for
+  large meshes
+- Fixed: `Mesh.load` uses less memory when loading and matching tags
+- Added: `Basis` has new optional `disable_doflocs` kwarg which
+  can be set to `True` to avoid computing `Basis.doflocs`, to reduce memory
+  usage
+
 ### [9.0.1] - 2024-01-12
 
 - Fixed: `ElementVector` works also for split_bases/split_indices in case `mesh.dim() != elem.dim`
 
 ### [9.0.0] - 2023-12-24
 
 - Removed: Python 3.7 support
```

### Comparing `scikit-fem-9.0.1/setup.cfg` & `scikit_fem-9.1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scikit-fem
-version = 9.0.1
+version = 9.1.1
 author = Tom Gustafsson
 description = Simple finite element assemblers
 url = https://github.com/kinnala/scikit-fem
 project_urls = 
 	Code=https://github.com/kinnala/scikit-fem
 	Issues=https://github.com/kinnala/scikit-fem/issues
 long_description = file: README.md
```

### Comparing `scikit-fem-9.0.1/skfem/__init__.py` & `scikit_fem-9.1.1/skfem/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/assembly/__init__.py` & `scikit_fem-9.1.1/skfem/assembly/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/assembly/basis/abstract_basis.py` & `scikit_fem-9.1.1/skfem/assembly/basis/abstract_basis.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,34 +43,36 @@
     def __init__(self,
                  mesh: Mesh,
                  elem: Element,
                  mapping: Optional[Mapping] = None,
                  intorder: Optional[int] = None,
                  quadrature: Optional[Tuple[ndarray, ndarray]] = None,
                  refdom: Type[Refdom] = Refdom,
-                 dofs: Optional[Dofs] = None):
+                 dofs: Optional[Dofs] = None,
+                 disable_doflocs: bool = False):
 
         if mesh.refdom != elem.refdom:
             raise ValueError("Incompatible Mesh and Element.")
 
         self.mapping = mesh._mapping() if mapping is None else mapping
         self.dofs = Dofs(mesh, elem) if dofs is None else dofs
 
         # global degree-of-freedom location
-        try:
-            doflocs = self.mapping.F(elem.doflocs.T)
-            self.doflocs = np.zeros((doflocs.shape[0], self.N))
-
-            # match mapped dofs and global dof numbering
-            for itr in range(doflocs.shape[0]):
-                for jtr in range(self.dofs.element_dofs.shape[0]):
-                    self.doflocs[itr, self.dofs.element_dofs[jtr]] =\
-                        doflocs[itr, :, jtr]
-        except Exception:
-            logger.warning("Unable to calculate global DOF locations.")
+        if not disable_doflocs:
+            try:
+                doflocs = self.mapping.F(elem.doflocs.T)
+                self.doflocs = np.zeros((doflocs.shape[0], self.N))
+
+                # match mapped dofs and global dof numbering
+                for itr in range(doflocs.shape[0]):
+                    for jtr in range(self.dofs.element_dofs.shape[0]):
+                        self.doflocs[itr, self.dofs.element_dofs[jtr]] =\
+                            doflocs[itr, :, jtr]
+            except Exception:
+                logger.warning("Unable to calculate global DOF locations.")
 
         self.mesh = mesh
         self.elem = elem
 
         self.Nbfun = self.dofs.element_dofs.shape[0]
 
         self.nelems = 0  # subclasses should overwrite
```

### Comparing `scikit-fem-9.0.1/skfem/assembly/basis/cell_basis.py` & `scikit_fem-9.1.1/skfem/assembly/basis/cell_basis.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,16 @@
     def __init__(self,
                  mesh: Mesh,
                  elem: Element,
                  mapping: Optional[Mapping] = None,
                  intorder: Optional[int] = None,
                  elements: Optional[Any] = None,
                  quadrature: Optional[Tuple[ndarray, ndarray]] = None,
-                 dofs: Optional[Dofs] = None):
+                 dofs: Optional[Dofs] = None,
+                 disable_doflocs: bool = False):
         """Combine :class:`~skfem.mesh.Mesh` and
         :class:`~skfem.element.Element` into a set of precomputed global basis
         functions.
 
         Parameters
         ----------
         mesh
@@ -66,27 +67,32 @@
             is specified.
         elements
             Optional subset of element indices.
         quadrature
             Optional tuple of quadrature points and weights.
         dofs
             Optional :class:`~skfem.assembly.Dofs` object.
+        disable_doflocs
+            If `True`, the computation of global DOF locations is
+            disabled.  This may save memory on large meshes if DOF
+            locations are not required.
 
         """
         logger.info("Initializing {}({}, {})".format(type(self).__name__,
                                                      type(mesh).__name__,
                                                      type(elem).__name__))
         super(CellBasis, self).__init__(
             mesh,
             elem,
             mapping,
             intorder,
             quadrature,
             mesh.refdom,
             dofs,
+            disable_doflocs,
         )
 
         if elements is None:
             self.tind = None
             self.nelems = mesh.nelements
         else:
             self.tind = mesh.normalize_elements(elements)
@@ -287,14 +293,16 @@
             function (to be projected) evaluated at global quadrature points.
             If a function is given, then :class:`~skfem.element.DiscreteField`
             is created by passing an array of global quadrature point locations
             to the function.
         elements
             Optionally perform the projection on a subset of elements.  The
             values of the remaining DOFs are zero.
+        dtype
+            Set to `np.complex64` or similar to use complex numbers.
 
         """
         from skfem.utils import solve, condense
 
         M, f = self._projection(interp, dtype=dtype)
 
         if elements is not None:
```

### Comparing `scikit-fem-9.0.1/skfem/assembly/basis/facet_basis.py` & `scikit_fem-9.1.1/skfem/assembly/basis/facet_basis.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,16 @@
                  mesh: Mesh,
                  elem: Element,
                  mapping: Optional[Mapping] = None,
                  intorder: Optional[int] = None,
                  quadrature: Optional[Tuple[ndarray, ndarray]] = None,
                  facets: Optional[Any] = None,
                  dofs: Optional[Dofs] = None,
-                 side: int = 0):
+                 side: int = 0,
+                 disable_doflocs: bool = False):
         """Precomputed global basis on boundary facets.
 
         Parameters
         ----------
         mesh
             An object of type :class:`~skfem.mesh.Mesh`.
         elem
@@ -47,28 +48,33 @@
             is specified.
         quadrature
             Optional tuple of quadrature points and weights.
         facets
             Optional subset of facet indices.
         dofs
             Optional :class:`~skfem.assembly.Dofs` object.
+        disable_doflocs
+            If `True`, the computation of global DOF locations is
+            disabled.  This may save memory on large meshes if DOF
+            locations are not required.
 
         """
         typestr = ("{}({}, {})".format(type(self).__name__,
                                        type(mesh).__name__,
                                        type(elem).__name__))
         logger.info("Initializing {}".format(typestr))
         super(FacetBasis, self).__init__(
             mesh,
             elem,
             mapping,
             intorder,
             quadrature,
             mesh.brefdom,
             dofs,
+            disable_doflocs,
         )
 
         # by default use boundary facets
         if facets is None:
             self.find = np.nonzero(self.mesh.f2t[1] == -1)[0]
         else:
             self.find = mesh.normalize_facets(facets)
@@ -207,14 +213,16 @@
             function (to be projected) evaluated at global quadrature points at
             the boundary of the domain.  If a function is given, then
             :class:`~skfem.element.DiscreteField` is created by passing
             an array of global quadrature point locations to the function.
         facets
             Optionally perform the projection on a subset of facets.  The
             values of the remaining DOFs are zero.
+        dtype
+            Set to `np.complex64` or similar to use complex numbers.
 
         """
         from skfem.utils import solve, condense
 
         M, f = self._projection(interp, dtype=dtype)
 
         if facets is not None:
```

### Comparing `scikit-fem-9.0.1/skfem/assembly/basis/interior_facet_basis.py` & `scikit_fem-9.1.1/skfem/assembly/basis/interior_facet_basis.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,16 @@
                  mesh: Mesh,
                  elem: Element,
                  mapping: Optional[Mapping] = None,
                  intorder: Optional[int] = None,
                  quadrature: Optional[Tuple[ndarray, ndarray]] = None,
                  facets: Optional[Any] = None,
                  dofs: Optional[Dofs] = None,
-                 side: int = 0):
+                 side: int = 0,
+                 disable_doflocs: bool = False):
         """Precomputed global basis on interior facets."""
 
         if facets is None:
             facets = np.nonzero(mesh.f2t[1] != -1)[0]
 
         facets = mesh.normalize_facets(facets)
 
@@ -38,8 +39,9 @@
             elem,
             mapping=mapping,
             intorder=intorder,
             quadrature=quadrature,
             facets=facets,
             dofs=dofs,
             side=side,
+            disable_doflocs=disable_doflocs,
         )
```

### Comparing `scikit-fem-9.0.1/skfem/assembly/dofs.py` & `scikit_fem-9.1.1/skfem/assembly/dofs.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/assembly/form/bilinear_form.py` & `scikit_fem-9.1.1/skfem/assembly/form/bilinear_form.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/assembly/form/coo_data.py` & `scikit_fem-9.1.1/skfem/assembly/form/coo_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,14 @@
             Optionally, sum local facet matrices to form elemental matrices if
             the corresponding :class:`skfem.assembly.FacetBasis` is provided.
 
         """
         if self.local_shape is None:
             raise NotImplementedError("Cannot build local matrices if "
                                       "local_shape is not specified.")
-        assert len(self.local_shape) == 2
 
         local = np.moveaxis(self.data.reshape(self.local_shape + (-1,),
                                               order='C'), -1, 0)
         if basis is not None:
             out = np.zeros((basis.mesh.nfacets,) + local.shape[1:])
             out[basis.find] = local
             local = np.sum(out[basis.mesh.t2f], axis=0)
```

### Comparing `scikit-fem-9.0.1/skfem/assembly/form/form.py` & `scikit_fem-9.1.1/skfem/assembly/form/form.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/assembly/form/functional.py` & `scikit_fem-9.1.1/skfem/assembly/form/functional.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/assembly/form/linear_form.py` & `scikit_fem-9.1.1/skfem/assembly/form/linear_form.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/assembly/form/trilinear_form.py` & `scikit_fem-9.1.1/skfem/assembly/form/trilinear_form.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/__init__.py` & `scikit_fem-9.1.1/skfem/element/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/discrete_field.py` & `scikit_fem-9.1.1/skfem/element/discrete_field.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element.py` & `scikit_fem-9.1.1/skfem/element/element.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_composite.py` & `scikit_fem-9.1.1/skfem/element/element_composite.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_dg.py` & `scikit_fem-9.1.1/skfem/element/element_dg.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_global.py` & `scikit_fem-9.1.1/skfem/element/element_global.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_h1.py` & `scikit_fem-9.1.1/skfem/element/element_h1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_hcurl.py` & `scikit_fem-9.1.1/skfem/element/element_hcurl.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_hdiv.py` & `scikit_fem-9.1.1/skfem/element/element_hdiv.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_hex/element_hex1.py` & `scikit_fem-9.1.1/skfem/element/element_hex/element_hex1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_hex/element_hex2.py` & `scikit_fem-9.1.1/skfem/element/element_hex/element_hex2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_hex/element_hex_c1.py` & `scikit_fem-9.1.1/skfem/element/element_hex/element_hex_c1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_hex/element_hex_rt1.py` & `scikit_fem-9.1.1/skfem/element/element_hex/element_hex_rt1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_hex/element_hex_s2.py` & `scikit_fem-9.1.1/skfem/element/element_hex/element_hex_s2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_hex/element_hex_skeleton0.py` & `scikit_fem-9.1.1/skfem/element/element_hex/element_hex_skeleton0.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_line/element_line_hermite.py` & `scikit_fem-9.1.1/skfem/element/element_line/element_line_hermite.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_line/element_line_mini.py` & `scikit_fem-9.1.1/skfem/element/element_line/element_line_mini.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_line/element_line_p1.py` & `scikit_fem-9.1.1/skfem/element/element_line/element_line_p1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_line/element_line_p2.py` & `scikit_fem-9.1.1/skfem/element/element_line/element_line_p2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_line/element_line_pp.py` & `scikit_fem-9.1.1/skfem/element/element_line/element_line_pp.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_matrix.py` & `scikit_fem-9.1.1/skfem/element/element_matrix.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_quad/element_quad1.py` & `scikit_fem-9.1.1/skfem/element/element_quad/element_quad1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_quad/element_quad2.py` & `scikit_fem-9.1.1/skfem/element/element_quad/element_quad2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_quad/element_quad_bfs.py` & `scikit_fem-9.1.1/skfem/element/element_quad/element_quad_bfs.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_quad/element_quad_n1.py` & `scikit_fem-9.1.1/skfem/element/element_quad/element_quad_n1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_quad/element_quad_rt1.py` & `scikit_fem-9.1.1/skfem/element/element_quad/element_quad_rt1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_quad/element_quad_s2.py` & `scikit_fem-9.1.1/skfem/element/element_quad/element_quad_s2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_quad/element_quadp.py` & `scikit_fem-9.1.1/skfem/element/element_quad/element_quadp.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tet/element_tet_ccr.py` & `scikit_fem-9.1.1/skfem/element/element_tet/element_tet_ccr.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tet/element_tet_cr.py` & `scikit_fem-9.1.1/skfem/element/element_tet/element_tet_cr.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tet/element_tet_mini.py` & `scikit_fem-9.1.1/skfem/element/element_tet/element_tet_mini.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tet/element_tet_n1.py` & `scikit_fem-9.1.1/skfem/element/element_tet/element_tet_n1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tet/element_tet_p1.py` & `scikit_fem-9.1.1/skfem/element/element_tet/element_tet_p1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tet/element_tet_p2.py` & `scikit_fem-9.1.1/skfem/element/element_tet/element_tet_p2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tet/element_tet_rt1.py` & `scikit_fem-9.1.1/skfem/element/element_tet/element_tet_rt1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tet/element_tet_skeleton_p0.py` & `scikit_fem-9.1.1/skfem/element/element_tet/element_tet_skeleton_p0.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/__init__.py` & `scikit_fem-9.1.1/skfem/element/element_tri/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_15param_plate.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_15param_plate.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_argyris.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_argyris.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_bdm1.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_bdm1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_bell.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_bell.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_cr.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_cr.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_hermite.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_hermite.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_hhj.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_hhj.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_morley.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_morley.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_n1.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_n1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_n2.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_n2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_p1.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_p1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_p1b.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_p1b.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_p1g.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_p1g.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_p2.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_p2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_p2b.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_p2b.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_p2g.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_p2g.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_p3.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_p3.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_p4.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_p4.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_rt1.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_rt1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_rt2.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_rt2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_tri/element_tri_skeleton_p1.py` & `scikit_fem-9.1.1/skfem/element/element_tri/element_tri_skeleton_p1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_vector.py` & `scikit_fem-9.1.1/skfem/element/element_vector.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/element/element_wedge_1.py` & `scikit_fem-9.1.1/skfem/element/element_wedge_1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/experimental/autodiff/helpers.py` & `scikit_fem-9.1.1/skfem/experimental/autodiff/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,87 @@
-import autograd.numpy as np
-from autograd.builtins import isinstance
+import jax.numpy as jnp
 
-from skfem import DiscreteField
+from . import JaxDiscreteField
 
 
 def dot(u, v):
-    if isinstance(u, tuple):
-        u = u[0]
-    if isinstance(v, tuple):
-        v = v[0]
-    return np.einsum('i...,i...', u, v)
+    if isinstance(u, JaxDiscreteField):
+        u = u.value
+    if isinstance(v, JaxDiscreteField):
+        v = v.value
+    return jnp.einsum('i...,i...', u, v)
 
 
 def ddot(u, v):
-    if isinstance(u, tuple):
-        u = u[0]
-    if isinstance(v, tuple):
-        v = v[0]
-    return np.einsum('ij...,ij...', u, v)
+    if isinstance(u, JaxDiscreteField):
+        u = u.value
+    if isinstance(v, JaxDiscreteField):
+        v = v.value
+    return jnp.einsum('ij...,ij...', u, v)
 
 
 def dddot(u, v):
-    if isinstance(u, tuple):
-        u = u[0]
-    if isinstance(v, tuple):
-        v = v[0]
-    return np.einsum('ijk...,ijk...', u, v)
+    if isinstance(u, JaxDiscreteField):
+        u = u.value
+    if isinstance(v, JaxDiscreteField):
+        v = v.value
+    return jnp.einsum('ijk...,ijk...', u, v)
 
 
 def grad(u):
-    if isinstance(u, DiscreteField):
-        return u.grad
-    return u[1]
+    return u.grad
 
 
 def sym_grad(u):
-    if isinstance(u, DiscreteField):
-        return .5 * (u.grad + transpose(u.grad))
-    return .5 * (u[1] + transpose(u[1]))
+    return .5 * (u.grad + transpose(u.grad))
 
 
 def div(u):
-    if len(u[1].shape) == 4:
-        return np.einsum('ii...', u[1])
-    return u[2]
+    if len(u.grad.shape) == 4:
+        return jnp.einsum('ii...', u.grad)
+    return u.div
 
 
 def dd(u):
-    if isinstance(u, DiscreteField):
-        return u.hess
-    return u[4]
+    return u.hess
 
 
 def transpose(T):
-    if isinstance(T, tuple):
-        T = T[0]
-    return np.einsum('ij...->ji...', T)
+    if isinstance(T, JaxDiscreteField):
+        T = T.value
+    return jnp.einsum('ij...->ji...', T)
 
 
 def mul(A, B):
-    if isinstance(A, tuple):
-        A = A[0]
-    if isinstance(B, tuple):
-        B = B[0]
+    if isinstance(A, JaxDiscreteField):
+        A = A.value
+    if isinstance(B, JaxDiscreteField):
+        B = B.value
     if len(A.shape) == len(B.shape):
-        return np.einsum('ij...,jk...->ik...', A, B)
-    return np.einsum('ij...,j...->i...', A, B)
+        return jnp.einsum('ij...,jk...->ik...', A, B)
+    return jnp.einsum('ij...,j...->i...', A, B)
 
 
 def trace(T):
-    if isinstance(T, tuple):
-        T = T[0]
-    return np.einsum('ii...', T)
+    if isinstance(T, JaxDiscreteField):
+        T = T.value
+    return jnp.einsum('ii...', T)
 
 
 def eye(w, size):
-    return np.array([[w if i == j else 0. * w for i in range(size)]
+    return jnp.array([[w if i == j else 0. * w
+                       for i in range(size)]
                      for j in range(size)])
 
 
 def det(A):
-    detA = np.zeros_like(A[0, 0])
+    detA = jnp.zeros_like(A[0, 0])
     if A.shape[0] == 3:
-        detA = A[0, 0] * (A[1, 1] * A[2, 2] -
-                          A[1, 2] * A[2, 1]) -\
-               A[0, 1] * (A[1, 0] * A[2, 2] -
-                          A[1, 2] * A[2, 0]) +\
-               A[0, 2] * (A[1, 0] * A[2, 1] -
-                          A[1, 1] * A[2, 0])
+        detA = (A[0, 0] * (A[1, 1] * A[2, 2]
+                           - A[1, 2] * A[2, 1])
+                - A[0, 1] * (A[1, 0] * A[2, 2] -
+                             - A[1, 2] * A[2, 0])
+                + A[0, 2] * (A[1, 0] * A[2, 1]
+                             - A[1, 1] * A[2, 0]))
     elif A.shape[0] == 2:
         detA = A[0, 0] * A[1, 1] - A[1, 0] * A[0, 1]
     return detA
```

### Comparing `scikit-fem-9.0.1/skfem/generic_utils.py` & `scikit_fem-9.1.1/skfem/generic_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/helpers.py` & `scikit_fem-9.1.1/skfem/helpers.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/io/json.py` & `scikit_fem-9.1.1/skfem/io/json.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/io/meshio.py` & `scikit_fem-9.1.1/skfem/io/meshio.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """Import/export any formats supported by meshio."""
 
+import logging
 from pathlib import Path
 
 import meshio
 import numpy as np
 
 from skfem.mesh import (MeshTet1, MeshTet2, MeshHex1, MeshHex2, MeshWedge1,
                         MeshTri1, MeshTri2, MeshQuad1, MeshQuad2, MeshLine1)
 from skfem.generic_utils import OrientedBoundary
 
 
+logger = logging.getLogger(__name__)
+
+
 MESH_TYPE_MAPPING = {
     'tetra': MeshTet1,
     'tetra10': MeshTet2,
     'hexahedron': MeshHex1,
     'hexahedron27': MeshHex2,
     'wedge': MeshWedge1,
     'triangle': MeshTri1,
@@ -50,14 +54,17 @@
 def from_meshio(m,
                 out=None,
                 int_data_to_sets=False,
                 force_meshio_type=None,
                 ignore_orientation=False,
                 ignore_interior_facets=False):
 
+    if ignore_interior_facets:
+        logger.warning("kwarg ignore_interior_facets is unused.")
+
     cells = m.cells_dict
     meshio_type = None
 
     if force_meshio_type is None:
         # detect 3D
         for k in cells:
             if k in {'tetra',
@@ -117,64 +124,50 @@
 
     # create temporary mesh for matching boundary elements
     mtmp = mesh_type(p, t, validate=False)
     bnd_type = BOUNDARY_TYPE_MAPPING[meshio_type]
 
     # parse boundaries from cell_sets
     if m.cell_sets and bnd_type in m.cells_dict:
-        oriented_facets = {
-            k: [tuple(f) for f in m.cells_dict[bnd_type][v[bnd_type]]]
-            for k, v in m.cell_sets_dict.items()
-            if bnd_type in v and k.split(":")[0] != "gmsh"
-        }
-        sorted_facets = {k: [tuple(np.sort(f)) for f in v]
-                         for k, v in oriented_facets.items()}
-        for k, v in oriented_facets.items():
-            if ignore_orientation or ignore_interior_facets:
-                a = np.array(sorted_facets[k])
-                if ignore_interior_facets:
-                    b = mtmp.facets[:, mtmp.boundary_facets()].T
-                else:
-                    b = mtmp.facets.T
-                boundaries[k] = np.nonzero((a == b[:, None])
-                                           .all(axis=2)
-                                           .any(axis=1))[0]
-            else:
-                indices = []
-                oris = []
-                for i, f in enumerate(map(tuple, mtmp.facets.T)):
-                    if f in sorted_facets[k]:
-                        indices.append(i)
-                        ix = sorted_facets[k].index(f)
-                        facet = v[ix]
-                        t1, t2 = mtmp.f2t[:, i]
-                        if t2 == -1:
-                            # orientation on boundary is 0
-                            oris.append(0)
-                            continue
-                        if len(f) == 2:
-                            # rotate tangent to find normal
-                            tangent = (mtmp.p[:, facet[1]]
-                                       - mtmp.p[:, facet[0]])
-                            normal = np.array([-tangent[1], tangent[0]])
-                        elif len(f) == 3:
-                            # cross product to find normal
-                            tangent1 = (mtmp.p[:, facet[1]]
-                                        - mtmp.p[:, facet[0]])
-                            tangent2 = (mtmp.p[:, facet[2]]
-                                        - mtmp.p[:, facet[0]])
-                            normal = -np.cross(tangent1, tangent2)
+        p2f = mtmp.p2f
+        for k, v in m.cell_sets_dict.items():
+            if bnd_type in v and k.split(":")[0] != "gmsh":
+                facets = m.cells_dict[bnd_type][v[bnd_type]].T
+                sorted_facets = np.sort(facets, axis=0)
+                ind = p2f[:, sorted_facets[0]]
+                for itr in range(sorted_facets.shape[0] - 1):
+                    ind = ind.multiply(p2f[:, sorted_facets[itr + 1]])
+                boundaries[k] = np.nonzero(ind)[0]
+
+                if not ignore_orientation:
+                    try:
+                        ori = np.zeros_like(boundaries[k], dtype=np.float64)
+                        t1, _ = mtmp.f2t[:, boundaries[k]]
+                        if facets.shape[0] == 2:
+                            tangents = (mtmp.p[:, facets[1]]
+                                        - mtmp.p[:, facets[0]])
+                            normals = np.array([-tangents[1], tangents[0]])
+                        elif facets.shape[0] == 3:
+                            tangents1 = (mtmp.p[:, facets[1]]
+                                         - mtmp.p[:, facets[0]])
+                            tangents2 = (mtmp.p[:, facets[2]]
+                                         - mtmp.p[:, facets[0]])
+                            normals = -np.cross(tangents1.T, tangents2.T).T
                         else:
                             raise NotImplementedError
-                        # find another vector using node outside of boundary
-                        third = np.setdiff1d(mtmp.t[:, t1],
-                                             np.array(f))[0]
-                        outplane = mtmp.p[:, f[0]] - mtmp.p[:, third]
-                        oris.append(1 if np.dot(normal, outplane) > 0 else 0)
-                boundaries[k] = OrientedBoundary(indices, oris)
+                        for itr in range(mtmp.t.shape[0]):
+                            ori += np.sum(normals
+                                          * (mtmp.p[:, facets[0]]
+                                             - mtmp.p[:, mtmp.t[itr, t1]]),
+                                          axis=0)
+                        ori = 1 * (ori > 0)
+                        boundaries[k] = OrientedBoundary(boundaries[k],
+                                                         ori)
+                    except Exception:
+                        logger.warning("Failure to orient a boundary.")
 
     # MSH 2.2 tag parsing
     if len(boundaries) == 0 and m.cell_data and m.field_data:
         try:
             elements_tag = m.cell_data_dict['gmsh:physical'][meshio_type]
             subdomains = {}
             tags = np.unique(elements_tag)
@@ -208,15 +201,15 @@
             tags = index[:, 0]
             boundaries = {}
             for tag in np.unique(tags):
                 tagindex = np.nonzero(tags == tag)[0]
                 boundaries[find_tagname(tag)] = index[tagindex, 1]
 
         except Exception:
-            pass
+            logger.warning("Failure to parse tags from meshio.")
 
     # attempt parsing skfem tags
     if m.cell_data:
         _boundaries, _subdomains = mtmp._decode_cell_data(m.cell_data)
         boundaries.update(_boundaries)
         subdomains.update(_subdomains)
```

### Comparing `scikit-fem-9.0.1/skfem/mapping/mapping.py` & `scikit_fem-9.1.1/skfem/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/mapping/mapping_isoparametric.py` & `scikit_fem-9.1.1/skfem/mapping/mapping_isoparametric.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/mesh/__init__.py` & `scikit_fem-9.1.1/skfem/mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/mesh/mesh.py` & `scikit_fem-9.1.1/skfem/mesh/mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,59 @@
 
     @property
     def t2e(self):
         if not hasattr(self, '_t2e'):
             self._init_edges()
         return self._t2e
 
+    @property
+    def p2f(self):
+        """Incidence matrix between facets and vertices.
+
+        Examples
+        --------
+        To find facets with point 5:
+
+        >>> import numpy as np
+        >>> from skfem import MeshTet
+        >>> mesh = MeshTet().refined()
+        >>> np.nonzero(mesh.p2f[:, 5])[0]
+        array([33, 34, 35], dtype=int32)
+
+        """
+        from scipy.sparse import coo_matrix
+        facets = self.facets.flatten('C')
+        return coo_matrix(
+            (np.ones(len(facets), dtype=np.int32),
+             (np.concatenate((np.arange(self.nfacets),)
+                             * self.facets.shape[0]), facets)),
+            shape=(self.nfacets, self.nvertices),
+            dtype=np.int32,
+        ).tocsc()
+
+    @property
+    def p2t(self):
+        """Incidence matrix between elements and vertices."""
+        from scipy.sparse import coo_matrix
+        t = self.t.flatten('C')
+        return coo_matrix(
+            (np.ones(len(t), dtype=np.int32),
+             (np.concatenate((np.arange(self.nelements),)
+                             * self.nnodes), t)),
+            shape=(self.nelements, self.nvertices),
+            dtype=np.int32,
+        ).tocsc()
+
+    @property
+    def p2e(self):
+        """Incidence matrix between edges and vertices."""
+        p2t = self.p2t
+        edges = self.edges
+        return p2t[:, edges[0]].multiply(p2t[:, edges[1]])
+
     def dim(self):
         return self.elem.refdom.dim()
 
     def boundary_facets(self) -> ndarray:
         """Return an array of boundary facet indices."""
         return np.nonzero(self.f2t[1] == -1)[0]
 
@@ -584,15 +629,24 @@
         return True
 
     @staticmethod
     def _remove_duplicate_nodes(p, t):
         tmp = np.ascontiguousarray(p.T)
         tmp, ixa, ixb = np.unique(tmp.view([('', tmp.dtype)] * tmp.shape[1]),
                                   return_index=True, return_inverse=True)
-        return p[:, ixa], ixb[t]
+        return p[:, ixa], Mesh._squeeze_if(ixb[t])
+
+    @staticmethod
+    def _squeeze_if(arr):
+        # Workaround for the additional dimension introduced in
+        # numpy 2.0 for the output of np.unique when using
+        # return_index=True
+        if len(arr.shape) > 2:
+            return arr.squeeze(axis=2)
+        return arr
 
     def __iter__(self):
         return iter((self.doflocs, self.t))
 
     def __rmatmul__(self, other):
         out = self.__matmul__(other)
         return out[1:] + out[0:1]
@@ -605,16 +659,16 @@
         if isinstance(other, list):
             p = np.hstack((self.p,) + tuple([mesh.p for mesh in other]))
             pT = np.ascontiguousarray(p.T)
             _, ixa, ixb = np.unique(pT.view([('', pT.dtype)] * pT.shape[1]),
                                     return_index=True, return_inverse=True)
             p = p[:, ixa]
             return [
-                cls(p, ixb[self.t]),
-                *[type(m)(p, ixb[m.t + self.p.shape[1]])
+                cls(p, self._squeeze_if(ixb[self.t])),
+                *[type(m)(p, self._squeeze_if(ixb[m.t + self.p.shape[1]]))
                   for i, m in enumerate(other)],
             ]
         raise NotImplementedError
 
     def __add__(self, other):
         """Join two meshes."""
         cls = type(self)
```

### Comparing `scikit-fem-9.0.1/skfem/mesh/mesh_2d.py` & `scikit_fem-9.1.1/skfem/mesh/mesh_2d.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/mesh/mesh_2d_2.py` & `scikit_fem-9.1.1/skfem/mesh/mesh_2d_2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/mesh/mesh_3d.py` & `scikit_fem-9.1.1/skfem/mesh/mesh_3d.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/mesh/mesh_dg.py` & `scikit_fem-9.1.1/skfem/mesh/mesh_dg.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/mesh/mesh_hex_1.py` & `scikit_fem-9.1.1/skfem/mesh/mesh_hex_1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/mesh/mesh_hex_2.py` & `scikit_fem-9.1.1/skfem/mesh/mesh_hex_2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/mesh/mesh_line_1.py` & `scikit_fem-9.1.1/skfem/mesh/mesh_line_1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/mesh/mesh_quad_1.py` & `scikit_fem-9.1.1/skfem/mesh/mesh_quad_1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/mesh/mesh_quad_2.py` & `scikit_fem-9.1.1/skfem/mesh/mesh_quad_2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/mesh/mesh_simplex.py` & `scikit_fem-9.1.1/skfem/mesh/mesh_simplex.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/mesh/mesh_tet_1.py` & `scikit_fem-9.1.1/skfem/mesh/mesh_tet_1.py`

 * *Files 6% similar despite different names*

```diff
@@ -377,21 +377,21 @@
                 .copy()
                 .flatten())
         t[7] = (ix[1:npy, 1:npx, 1:npz]
                 .reshape(ne, 1, order='F')
                 .copy()
                 .flatten())
 
-        T = np.zeros((4, 0))
-        T = np.hstack((T, t[[0, 1, 5, 7]]))
-        T = np.hstack((T, t[[0, 1, 4, 7]]))
-        T = np.hstack((T, t[[0, 2, 4, 7]]))
-        T = np.hstack((T, t[[0, 3, 5, 7]]))
-        T = np.hstack((T, t[[0, 2, 6, 7]]))
-        T = np.hstack((T, t[[0, 3, 6, 7]]))
+        T = np.zeros((4, 6 * ne))
+        T[:, :ne] = t[[0, 1, 5, 7]]
+        T[:, ne:(2 * ne)] = t[[0, 1, 4, 7]]
+        T[:, (2 * ne):(3 * ne)] = t[[0, 2, 4, 7]]
+        T[:, (3 * ne):(4 * ne)] = t[[0, 3, 5, 7]]
+        T[:, (4 * ne):(5 * ne)] = t[[0, 2, 6, 7]]
+        T[:, (5 * ne):] = t[[0, 3, 6, 7]]
 
         return cls(p, T.astype(np.int64))
 
     @classmethod
     def init_ball(cls: Type,
                   nrefs: int = 3):
         """Initialize a ball mesh.
```

### Comparing `scikit-fem-9.0.1/skfem/mesh/mesh_tet_2.py` & `scikit_fem-9.1.1/skfem/mesh/mesh_tet_2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/mesh/mesh_tri_1.py` & `scikit_fem-9.1.1/skfem/mesh/mesh_tri_1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/mesh/mesh_tri_1_dg.py` & `scikit_fem-9.1.1/skfem/mesh/mesh_tri_1_dg.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/mesh/mesh_tri_2.py` & `scikit_fem-9.1.1/skfem/mesh/mesh_tri_2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/mesh/mesh_wedge_1.py` & `scikit_fem-9.1.1/skfem/mesh/mesh_wedge_1.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/models/elasticity.py` & `scikit_fem-9.1.1/skfem/models/elasticity.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/quadrature.py` & `scikit_fem-9.1.1/skfem/quadrature.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/refdom.py` & `scikit_fem-9.1.1/skfem/refdom.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/supermeshing.py` & `scikit_fem-9.1.1/skfem/supermeshing.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/utils.py` & `scikit_fem-9.1.1/skfem/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,17 +303,17 @@
 
     D = _flatten_dofs(D)
     I = _flatten_dofs(I)
 
     if I is None and D is None:
         raise Exception("Either I or D must be given!")
     elif I is None and D is not None:
-        I = np.setdiff1d(np.arange(A.shape[0]), D)
+        I = np.setdiff1d(np.arange(A.shape[0], dtype=np.int64), D)
     elif D is None and I is not None:
-        D = np.setdiff1d(np.arange(A.shape[0]), I)
+        D = np.setdiff1d(np.arange(A.shape[0], dtype=np.int64), I)
     else:
         raise Exception("Give only I or only D!")
 
     assert isinstance(I, ndarray)
     assert isinstance(D, ndarray)
 
     if x is None:
```

### Comparing `scikit-fem-9.0.1/skfem/visuals/glvis.py` & `scikit_fem-9.1.1/skfem/visuals/glvis.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/visuals/matplotlib.py` & `scikit_fem-9.1.1/skfem/visuals/matplotlib.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/visuals/svg.py` & `scikit_fem-9.1.1/skfem/visuals/svg.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/skfem/visuals/vedo.py` & `scikit_fem-9.1.1/skfem/visuals/vedo.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/tests/test_assembly.py` & `scikit_fem-9.1.1/tests/test_assembly.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/tests/test_basis.py` & `scikit_fem-9.1.1/tests/test_basis.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import numpy as np
 from numpy.testing import (assert_allclose, assert_almost_equal,
                            assert_array_equal)
 
 from skfem import BilinearForm, LinearForm, asm, solve, condense, projection
 from skfem.mesh import (Mesh, MeshTri, MeshTet, MeshHex,
                         MeshQuad, MeshLine1, MeshWedge1)
-from skfem.assembly import CellBasis, FacetBasis, Dofs, Functional
+from skfem.assembly import (CellBasis, FacetBasis, Dofs, Functional,
+                            InteriorFacetBasis)
 from skfem.mapping import MappingIsoparametric
 from skfem.element import (ElementVectorH1, ElementTriP2, ElementTriP1,
                            ElementTetP2, ElementHexS2, ElementHex2,
                            ElementQuad2, ElementLineP2, ElementTriP0,
                            ElementLineP0, ElementQuad1, ElementQuad0,
                            ElementTetP1, ElementTetP0, ElementHex1,
                            ElementHex0, ElementLineP1, ElementLineMini,
@@ -642,7 +643,24 @@
     basis_half = basis.with_elements('a')
 
     assert basis.mesh == basis_half.mesh
     assert basis.elem == basis_half.elem
     assert basis.mapping == basis_half.mapping
     assert basis.quadrature == basis_half.quadrature
     assert all(basis_half.tind == basis.mesh.normalize_elements('a'))
+
+
+def test_disable_doflocs():
+    mesh = MeshTri().refined(3)
+    basis = CellBasis(mesh, ElementTriP1())
+    basisd = CellBasis(mesh, ElementTriP1(), disable_doflocs=True)
+    fbasis = FacetBasis(mesh, ElementTriP1())
+    fbasisd = FacetBasis(mesh, ElementTriP1(), disable_doflocs=True)
+    ifbasis = InteriorFacetBasis(mesh, ElementTriP1())
+    ifbasisd = InteriorFacetBasis(mesh, ElementTriP1(),
+                                  disable_doflocs=True)
+    assert not hasattr(fbasisd, 'doflocs')
+    assert hasattr(fbasis, 'doflocs')
+    assert not hasattr(basisd, 'doflocs')
+    assert hasattr(basis, 'doflocs')
+    assert not hasattr(ifbasisd, 'doflocs')
+    assert hasattr(ifbasis, 'doflocs')
```

### Comparing `scikit-fem-9.0.1/tests/test_convergence.py` & `scikit_fem-9.1.1/tests/test_convergence.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/tests/test_convergence_h2.py` & `scikit_fem-9.1.1/tests/test_convergence_h2.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/tests/test_convergence_hdiv.py` & `scikit_fem-9.1.1/tests/test_convergence_hdiv.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/tests/test_dofs.py` & `scikit_fem-9.1.1/tests/test_dofs.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/tests/test_elements.py` & `scikit_fem-9.1.1/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/tests/test_examples.py` & `scikit_fem-9.1.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/tests/test_manufactured.py` & `scikit_fem-9.1.1/tests/test_manufactured.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/tests/test_mapping.py` & `scikit_fem-9.1.1/tests/test_mapping.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import unittest
 import numpy as np
 
-from skfem.mesh import MeshHex, MeshQuad, MeshTri
+from skfem.mesh import MeshHex, MeshQuad, MeshTri, MeshTet
 from skfem.element import ElementHex1, ElementQuad1, ElementHex2
 from skfem.assembly import FacetBasis
+from skfem.mapping import MappingAffine
 
 
 class TestIsoparamNormals(unittest.TestCase):
     """Test that normals on x[i] == 0 are correct."""
 
     mesh = MeshHex
     elem = ElementHex1
@@ -83,7 +84,20 @@
         return m
 
 
 class TestInverseMappingHex2(TestInverseMappingHex):
     """This should be equivalent to TestInverseMappingHex."""
 
     element = ElementHex2
+
+
+def test_mapping_memory_optimization():
+
+    m = MeshTet.init_tensor(np.linspace(0, 1, 100),
+                            np.linspace(0, 1, 100),
+                            np.linspace(0, 1, 100))
+    m = m.with_subdomains({
+        'omega0': [0, 1, 2, 3, 4, 5],
+    })
+    orig = MappingAffine(m)
+    opt = MappingAffine(m, tind=m.subdomains['omega0'])
+    assert len(orig.detA) > len(opt.detA)
```

### Comparing `scikit-fem-9.0.1/tests/test_mesh.py` & `scikit_fem-9.1.1/tests/test_mesh.py`

 * *Files 3% similar despite different names*

```diff
@@ -509,14 +509,29 @@
     assert_array_equal(M.t, m.t)
     for key in m.boundaries:
         assert_array_equal(M.boundaries[key].sort(),
                            m.boundaries[key].sort())
 
 
 @pytest.mark.parametrize(
+    "mtype, path, ignore_orientation",
+    [
+        (MeshTet, MESH_PATH / 'box.msh', False),
+        (MeshTet, MESH_PATH / 'box.msh', True),
+        (MeshTri, MESH_PATH / 'tagged_gmsh4.msh', False),
+        (MeshTri, MESH_PATH / 'tagged_gmsh4.msh', True),
+    ]
+)
+def test_load_file(mtype, path, ignore_orientation):
+
+    m = mtype.load(path, ignore_orientation=ignore_orientation)
+    assert len(m.boundaries) > 0
+
+
+@pytest.mark.parametrize(
     "m",
     [
         MeshTri(),
         MeshQuad(),
         MeshHex(),
         MeshTet(),
     ]
@@ -551,15 +566,15 @@
     assert_array_equal(m.p, m2.p)
     assert_array_equal(m.t, m2.t)
 
 
 @pytest.mark.parametrize(
     "fmt, kwargs",
     [
-        ('.msh', {}),
+        ('.msh', {'file_format': 'gmsh'}),
         ('.msh', {'file_format': 'gmsh22'}),
         ('.vtk', {}),
         #('.xdmf', {}),
         ('.vtu', {}),
         #('.med', {}),
     ]
 )
@@ -753,7 +768,27 @@
     m = MeshTri()
     t = m.t
     t[1, :] += 4
     m1 = MeshTri(np.hstack((m.p, m.p)), t)
 
     assert not m1.is_valid()
     assert m1.remove_duplicate_nodes().is_valid()
+
+
+@pytest.mark.parametrize(
+    "mesh",
+    [
+        MeshTri().refined(3),
+        MeshTet().refined(3),
+        MeshQuad().refined(3),
+        MeshHex().refined(3),
+    ]
+)
+def test_incidence(mesh):
+
+    p2t = mesh.p2t
+    for itr in range(0, 50, 3):
+       assert np.sum((mesh.t == itr).any(axis=0)) == len(p2t[:, itr].data)
+
+    p2f = mesh.p2f
+    for itr in range(0, 50, 3):
+       assert np.sum((mesh.facets == itr).any(axis=0)) == len(p2f[:, itr].data)
```

### Comparing `scikit-fem-9.0.1/tests/test_p_convergence.py` & `scikit_fem-9.1.1/tests/test_p_convergence.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/tests/test_utils.py` & `scikit_fem-9.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-fem-9.0.1/tests/test_visuals.py` & `scikit_fem-9.1.1/tests/test_visuals.py`

 * *Files identical despite different names*

