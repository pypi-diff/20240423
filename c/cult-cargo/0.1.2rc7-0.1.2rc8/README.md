# Comparing `tmp/cult_cargo-0.1.2rc7.tar.gz` & `tmp/cult_cargo-0.1.2rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cult_cargo-0.1.2rc7.tar", max compression
+gzip compressed data, was "cult_cargo-0.1.2rc8.tar", max compression
```

## Comparing `cult_cargo-0.1.2rc7.tar` & `cult_cargo-0.1.2rc8.tar`

### file list

```diff
@@ -1,73 +1,76 @@
--rw-r--r--   0        0        0     1134 2024-03-27 11:26:45.712549 cult_cargo-0.1.2rc7/LICENSE
--rw-r--r--   0        0        0     1339 2024-03-27 11:26:45.712549 cult_cargo-0.1.2rc7/README.md
--rw-r--r--   0        0        0        0 2024-03-27 11:26:45.712549 cult_cargo-0.1.2rc7/cultcargo/__init__.py
--rw-r--r--   0        0        0      895 2024-03-27 11:26:45.712549 cult_cargo-0.1.2rc7/cultcargo/aimfast.yml
--rw-r--r--   0        0        0     3599 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/bdsf.yml
--rw-r--r--   0        0        0      963 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/breizorro.yml
--rwxr-xr-x   0        0        0    16892 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/builder/build_cargo.py
--rw-r--r--   0        0        0     4814 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/builder/cargo-manifest.yml
--rw-r--r--   0        0        0      647 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/casa-concat.yml
--rw-r--r--   0        0        0     1117 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/casa-flag.yml
--rw-r--r--   0        0        0      552 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/crystalball.yml
--rw-r--r--   0        0        0     1336 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/cubical.yml
--rw-r--r--   0        0        0     1081 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/fitstool.yml
--rw-r--r--   0        0        0        0 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/cubical/__init__.py
--rw-r--r--   0        0        0     1013 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/cubical/make_stimela_schema.py
--rw-r--r--   0        0        0    23866 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/cubical/schema.yaml
--rw-r--r--   0        0        0     6990 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/cubical/schema_JONES_TEMPLATE.yaml
--rw-r--r--   0        0        0       87 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/cult-cargo-base.yml
--rw-r--r--   0        0        0      727 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/cgopts.yml
--rw-r--r--   0        0        0     3082 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/clean.yaml
--rw-r--r--   0        0        0     1021 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/degrid.yaml
--rw-r--r--   0        0        0      939 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/dist.yml
--rw-r--r--   0        0        0     2620 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/fastim.yaml
--rw-r--r--   0        0        0      919 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/forward.yaml
--rw-r--r--   0        0        0     2427 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/fwdbwd.yaml
--rw-r--r--   0        0        0     2784 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/grid.yaml
--rw-r--r--   0        0        0      331 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/gridding.yml
--rw-r--r--   0        0        0     2620 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/init.yaml
--rw-r--r--   0        0        0     2432 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/init_ims.yaml
--rw-r--r--   0        0        0      990 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/model2comps.yaml
--rw-r--r--   0        0        0      388 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/out.yml
--rw-r--r--   0        0        0      480 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/pdopts.yml
--rw-r--r--   0        0        0      461 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/pmopts.yml
--rw-r--r--   0        0        0      752 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/restore.yaml
--rw-r--r--   0        0        0     1798 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/spotless.yaml
--rw-r--r--   0        0        0     1320 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/uncabbedcabs.yml
--rw-r--r--   0        0        0      868 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/sync_config.py
--rw-r--r--   0        0        0     1276 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/quartical/__init__.py
--rw-r--r--   0        0        0    14764 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/quartical/argument_schema.yaml
--rw-r--r--   0        0        0     6381 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/quartical/config_classes.py
--rw-r--r--   0        0        0     2206 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/quartical/converters.py
--rw-r--r--   0        0        0     1375 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/quartical/external.py
--rw-r--r--   0        0        0     2533 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/quartical/gain_schema.yaml
--rw-r--r--   0        0        0     4080 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/wsclean/__init__.py
--rw-r--r--   0        0        0     4357 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/genesis/wsclean/wsclean-base.yml
--rw-r--r--   0        0        0      161 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/images/Dockerfile.generic.pip
--rw-r--r--   0        0        0      290 2024-03-27 11:26:45.716549 cult_cargo-0.1.2rc7/cultcargo/images/base-cult/Dockerfile
--rw-r--r--   0        0        0      181 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/images/casa/Dockerfile
--rw-r--r--   0        0        0      637 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/images/casa/Dockerfile.base
--rw-r--r--   0        0        0      163 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/images/casa6/Dockerfile
--rw-r--r--   0        0        0      889 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/images/python-astro/Dockerfile
--rw-r--r--   0        0        0      186 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/images/tricolour/Dockerfile
--rw-r--r--   0        0        0      737 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/images/wsclean/Dockerfile.build
--rw-r--r--   0        0        0      873 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/images/wsclean/Dockerfile.build.2x
--rw-r--r--   0        0        0       68 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/images/wsclean/Dockerfile.kern7
--rw-r--r--   0        0        0     1413 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/mosaic-queen.yml
--rw-r--r--   0        0        0      847 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/msutils.yml
--rw-r--r--   0        0        0      848 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/pfb-clean.yml
--rw-r--r--   0        0        0     2890 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/quartical.yml
--rw-r--r--   0        0        0        0 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/recipes/__init__.py
--rw-r--r--   0        0        0     1868 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/rfinder.yml
--rw-r--r--   0        0        0     5949 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/shadems.yml
--rw-r--r--   0        0        0      807 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/smops.yml
--rw-r--r--   0        0        0      787 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/spimple-spifit.yml
--rw-r--r--   0        0        0      211 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/stimela.conf
--rw-r--r--   0        0        0      590 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/taql.yml
--rw-r--r--   0        0        0      540 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/tigger.yml
--rw-r--r--   0        0        0      995 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/tricolour.yml
--rw-r--r--   0        0        0     3867 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/utils.py
--rw-r--r--   0        0        0     2803 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/cultcargo/wsclean.yml
--rw-r--r--   0        0        0      891 2024-03-27 11:26:45.720549 cult_cargo-0.1.2rc7/pyproject.toml
--rw-r--r--   0        0        0     1990 1970-01-01 00:00:00.000000 cult_cargo-0.1.2rc7/PKG-INFO
+-rw-r--r--   0        0        0     1134 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/LICENSE
+-rw-r--r--   0        0        0     1810 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/cultcargo/__init__.py
+-rw-r--r--   0        0        0      895 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/cultcargo/aimfast.yml
+-rw-r--r--   0        0        0     3599 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/cultcargo/bdsf.yml
+-rw-r--r--   0        0        0      963 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/cultcargo/breizorro.yml
+-rwxr-xr-x   0        0        0    17743 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/cultcargo/builder/build_cargo.py
+-rw-r--r--   0        0        0     5551 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/cultcargo/builder/cargo-manifest.yml
+-rw-r--r--   0        0        0      647 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/cultcargo/casa-concat.yml
+-rw-r--r--   0        0        0     1117 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/cultcargo/casa-flag.yml
+-rw-r--r--   0        0        0      552 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/cultcargo/crystalball.yml
+-rw-r--r--   0        0        0     1336 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/cultcargo/cubical.yml
+-rw-r--r--   0        0        0     1081 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/cultcargo/fitstool.yml
+-rw-r--r--   0        0        0        0 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/cultcargo/genesis/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/cultcargo/genesis/cubical/__init__.py
+-rw-r--r--   0        0        0     1013 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/cultcargo/genesis/cubical/make_stimela_schema.py
+-rw-r--r--   0        0        0    23866 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/cultcargo/genesis/cubical/schema.yaml
+-rw-r--r--   0        0        0     6990 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/cultcargo/genesis/cubical/schema_JONES_TEMPLATE.yaml
+-rw-r--r--   0        0        0       87 2024-04-18 10:31:50.400425 cult_cargo-0.1.2rc8/cultcargo/genesis/cult-cargo-base.yml
+-rw-r--r--   0        0        0      727 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/cgopts.yml
+-rw-r--r--   0        0        0     3082 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/clean.yaml
+-rw-r--r--   0        0        0     1021 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/degrid.yaml
+-rw-r--r--   0        0        0      939 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/dist.yml
+-rw-r--r--   0        0        0     2620 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/fastim.yaml
+-rw-r--r--   0        0        0      919 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/forward.yaml
+-rw-r--r--   0        0        0     2427 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/fwdbwd.yaml
+-rw-r--r--   0        0        0     2784 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/grid.yaml
+-rw-r--r--   0        0        0      331 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/gridding.yml
+-rw-r--r--   0        0        0     2620 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/init.yaml
+-rw-r--r--   0        0        0     2432 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/init_ims.yaml
+-rw-r--r--   0        0        0      990 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/model2comps.yaml
+-rw-r--r--   0        0        0      388 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/out.yml
+-rw-r--r--   0        0        0      480 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/pdopts.yml
+-rw-r--r--   0        0        0      461 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/pmopts.yml
+-rw-r--r--   0        0        0      752 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/restore.yaml
+-rw-r--r--   0        0        0     1798 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/spotless.yaml
+-rw-r--r--   0        0        0     1320 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/uncabbedcabs.yml
+-rw-r--r--   0        0        0      868 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/sync_config.py
+-rw-r--r--   0        0        0     1276 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/quartical/__init__.py
+-rw-r--r--   0        0        0    14764 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/quartical/argument_schema.yaml
+-rw-r--r--   0        0        0     6381 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/quartical/config_classes.py
+-rw-r--r--   0        0        0     2206 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/quartical/converters.py
+-rw-r--r--   0        0        0     1375 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/quartical/external.py
+-rw-r--r--   0        0        0     2533 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/quartical/gain_schema.yaml
+-rw-r--r--   0        0        0     4080 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/wsclean/__init__.py
+-rw-r--r--   0        0        0     4396 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/genesis/wsclean/wsclean-base.yml
+-rw-r--r--   0        0        0      161 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/images/Dockerfile.generic.pip
+-rw-r--r--   0        0        0      290 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/images/base-cult/Dockerfile
+-rw-r--r--   0        0        0      181 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/images/casa/Dockerfile
+-rw-r--r--   0        0        0      637 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/images/casa/Dockerfile.base
+-rw-r--r--   0        0        0      163 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/images/casa6/Dockerfile
+-rw-r--r--   0        0        0     1143 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/images/ddfacet/Dockerfile
+-rw-r--r--   0        0        0      974 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/images/ddfacet/apt.sources.list
+-rw-r--r--   0        0        0      167 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/images/killms/Dockerfile
+-rw-r--r--   0        0        0     1075 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/images/python-astro/Dockerfile
+-rw-r--r--   0        0        0      186 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/images/tricolour/Dockerfile
+-rw-r--r--   0        0        0      737 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/images/wsclean/Dockerfile.build
+-rw-r--r--   0        0        0      873 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/images/wsclean/Dockerfile.build.2x
+-rw-r--r--   0        0        0       68 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/images/wsclean/Dockerfile.kern7
+-rw-r--r--   0        0        0     1413 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/mosaic-queen.yml
+-rw-r--r--   0        0        0      847 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/msutils.yml
+-rw-r--r--   0        0        0      848 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/pfb-clean.yml
+-rw-r--r--   0        0        0     2890 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/quartical.yml
+-rw-r--r--   0        0        0        0 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/recipes/__init__.py
+-rw-r--r--   0        0        0     1868 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/rfinder.yml
+-rw-r--r--   0        0        0     5949 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/shadems.yml
+-rw-r--r--   0        0        0      807 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/smops.yml
+-rw-r--r--   0        0        0      787 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/spimple-spifit.yml
+-rw-r--r--   0        0        0      211 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/stimela.conf
+-rw-r--r--   0        0        0      590 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/taql.yml
+-rw-r--r--   0        0        0      540 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/tigger.yml
+-rw-r--r--   0        0        0      995 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/tricolour.yml
+-rw-r--r--   0        0        0     3867 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/utils.py
+-rw-r--r--   0        0        0     2803 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/cultcargo/wsclean.yml
+-rw-r--r--   0        0        0      909 2024-04-18 10:31:50.404425 cult_cargo-0.1.2rc8/pyproject.toml
+-rw-r--r--   0        0        0     2498 1970-01-01 00:00:00.000000 cult_cargo-0.1.2rc8/PKG-INFO
```

### Comparing `cult_cargo-0.1.2rc7/LICENSE` & `cult_cargo-0.1.2rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/README.md` & `cult_cargo-0.1.2rc8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -45,7 +45,18 @@
 This makes the ``build-cargo.py`` script available. The script is preconfigured to read ``cultcargo/builder/cargo-manifest.yml``, which describes the images that must be built.
 
 ``build-cargo.py -a`` will build and push all images, or specify an image name to build a particular one. Use ``-b`` to build but not push, or ``-p`` for push-only. Use ``-l`` to list available images.
 
 The ``cultcargo`` folder contains YaML files with cab definitions.
 
 If you would like to maintain your own image collection, write your own manifest and Dockerfiles following the cult-cargo example, and use the ``build-cargo.py`` script to build your images.
+
+## Using cult-cargo as a standalone image repository
+
+You don't even need to run stimela (or indeed install anything) to take advantage of the images packaged with cult-cargo. Take a look at the image repository on https://quay.io/organization/stimela2 to see what's available.
+
+For example, if you want to run a wsclean image, just do:
+
+```
+$ singularity build wsclean-3.3.sif docker:quay.io/stimela2/wsclean:3.3-cc0.1.2
+$ singularity exec wsclean-3.3.sif wsclean 
+```
```

### Comparing `cult_cargo-0.1.2rc7/cultcargo/aimfast.yml` & `cult_cargo-0.1.2rc8/cultcargo/aimfast.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/bdsf.yml` & `cult_cargo-0.1.2rc8/cultcargo/bdsf.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/breizorro.yml` & `cult_cargo-0.1.2rc8/cultcargo/breizorro.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/builder/build_cargo.py` & `cult_cargo-0.1.2rc8/cultcargo/builder/build_cargo.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,18 +65,20 @@
                 default=DEFAULT_MANIFEST,
                 help=f'Cargo manifest. Default is {DEFAULT_MANIFEST}.')
 @click.option('-l', '--list', 'do_list', is_flag=True, help='List only, do not push or build. Returns error if images are missing.')
 @click.option('-b', '--build', is_flag=True, help='Build only, do not push.')
 @click.option('-p', '--push', is_flag=True, help='Push only, do not build.')
 @click.option('-r', '--rebuild', is_flag=True, help='Ignore docker image caches (i.e. rebuild).')
 @click.option('-a', '--all', is_flag=True, help='Build and/or push all images in manifest.')
+@click.option('-E', '--experimental', is_flag=True, help='Enable experimental versions.')
 @click.option('-v', '--verbose', is_flag=True, help='Be verbose.')
-@click.option('-b', '--boring', is_flag=True, help='Be boring -- no progress bar.')
+@click.option('--boring', is_flag=True, help='Be boring -- no progress bar.')
 @click.argument('imagenames', type=str, nargs=-1)
-def build_cargo(manifest: str, do_list=False, build=False, push=False, all=False, rebuild=False, boring=False, verbose=False, imagenames: List[str] = []):
+def build_cargo(manifest: str, do_list=False, build=False, push=False, all=False, rebuild=False, boring=False,
+                experimental=False, verbose=False, imagenames: List[str] = []):
     if not (build or push or do_list):
         build = push = True
 
     with Progress(
             TimeElapsedColumn(),
             SpinnerColumn(),
             "{task.description}",
@@ -248,14 +250,28 @@
 
                 version_info = image_info.versions[version]
                 version_vars = image_vars.copy()
                 version_vars.update(**version_info)
                 version_vars["VERSION"] = version
                 version_vars["IMAGE_VERSION"] = image_version
 
+                is_exp = version_info.get('experimental')
+                exp_deps = version_info.get('experimental_dependencies', [])
+
+                if is_exp or exp_deps:
+                    if not experimental:
+                        print(f"[bold]{image}:{image_version}[/bold] is experimental and -E switch not given, skipping")
+                        continue
+                    # check dependencies
+                    print(f"[bold]{image}:{image_version}[/bold] is experimental")
+                    for dep in exp_deps:
+                        if not os.path.exists(dep):
+                            print(f"  [red]ERROR: dependency {dep} doesn't exist[/red]")
+                            return 1
+
                 dockerfile = version_info.get('dockerfile') or image_info.dockerfile or 'Dockerfile'
                 dockerfile = dockerfile.format(**version_vars)
                 full_image = f"{registry}/{image}:{image_version}"
                 remote_image_exists = True
 
                 # find Dockerfile for this image
                 dockerpath = os.path.join(path, dockerfile)
@@ -291,15 +307,15 @@
                         print(f"Pulling {full_image} from registry")
                         run(f"docker pull {full_image}")
                     # substitute Dockerfile and build
                     content = open(dockerpath, "rt").read().format(**version_vars)
                     if verbose:
                         print(f"Dockerfile:", style="bold")
                         print(f"{content}", style="dim", highlight=True)
-                    run(f"docker build {no_cache} -t {full_image} -", cwd=build_dir, input=content)
+                    run(f"docker build {no_cache} -t {full_image} -f- {build_dir}", cwd=build_dir, input=content)
                     # is this the latest version that needs to be tagged
                     if image_version == tag_latest.get(image):
                         run(f"docker tag {registry}/{image}:{image_version} {registry}/{image}:{BUNDLE_VERSION}")
 
                 # go push
                 if push:
                     if remote_image_exists:
@@ -313,15 +329,15 @@
                         elif current_release:
                             if not candidate_release:
                                 print(f"  [red]Image exists and package released: won't push.[/red]")
                                 continue
                             else:
                                 print(f"  Image exists, but package is a release candidate: ok to push.")
                         else:
-                            print(f"  Image exists, but package unreleased, ok push.")
+                            print(f"  Image exists, but package unreleased, ok to push.")
                     run(f"docker push {full_image}", cwd=path)
                     if image_version == tag_latest.get(image):
                         run(f"docker push {registry}/{image}:{BUNDLE_VERSION}")
             progress.update(progress_task, description=
                 f"image [bold]{image}[/bold] [{i_image}/{len(imagenames)}]: tagging latest version")
 
             # # apply :latest tag to images
```

### Comparing `cult_cargo-0.1.2rc7/cultcargo/builder/cargo-manifest.yml` & `cult_cargo-0.1.2rc8/cultcargo/builder/cargo-manifest.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 metadata:
   # name of python package
   PACKAGE: cult-cargo
   # its repository
   GITHUB_REPOSITORY: caracal-pipeline/cult-cargo
   # registry to use. Use module::filename.yml::variable format to pull from a config file inside a python module
   REGISTRY: cultcargo.genesis::cult-cargo-base.yml::vars.cult-cargo.images.registry
-  # image bundle ersion. Use module::filename.yml::variable format to pull from a config file inside a python module
+  # image bundle version. Use module::filename.yml::variable format to pull from a config file inside a python module
   BUNDLE_VERSION: cultcargo.genesis::cult-cargo-base.yml::vars.cult-cargo.images.version
   # prefix to be removed from image version when comparing to python package version
   BUNDLE_VERSION_PREFIX: cc
   # path to images. Use module::filename to refer to content of module
   BASE_IMAGE_PATH: cultcargo::images
 
 assign:
@@ -50,14 +50,15 @@
         tag: v3.2
       '3.3':
         dockerfile: Dockerfile.build
         tag: v3.3
 
   python-astro:
     versions:
+      '3.10': {}
       '3.9': {}
       '3.8': {}
 
   casa:
     assign:
       url: https://casa.nrao.edu/download/distro/casa/release/el7
     versions:
@@ -153,14 +154,33 @@
         package: git+https://github.com/ratt-ru/CubiCal
 
   pfb-clean:
     versions:
       latest:
         package: git+https://github.com/ratt-ru/pfb-clean@awskube
 
+  ddfacet:
+    assign:
+      # base image for generic Python-based packages
+      base_python_image: python-astro:3.10
+      # corresponding python binary
+      python: python3.10
+    versions:
+      # experimental branch, Oleg only
+      useapp-meerklass:
+        experimental_dependencies:
+          - /home/oms/projects/cult-cargo/cultcargo/images/ddfacet/DDFacet-useapp-meerklass
+          - /home/oms/projects/cult-cargo/cultcargo/images/ddfacet/killMS-useapp-meerklass
+        pre_install: |
+          ADD DDFacet-useapp-meerklass DDFacet-branch
+          ADD killMS-useapp-meerklass killMS-branch
+        package: -e ./DDFacet-branch ./killMS-branch
+      '0.8':
+        package: DDFacet==0.8.0.0 killMS==3.2.0
+
   mosaic-queen:
     assign:
       pre_install: RUN apt update && apt install -y montage && rm -rf /var/lib/apt/lists/* && rm -rf /var/cache/apt/archives
     versions:
       '1.1.1':
         package: mosaic-queen==1.1.1
       latest:
```

### Comparing `cult_cargo-0.1.2rc7/cultcargo/casa-concat.yml` & `cult_cargo-0.1.2rc8/cultcargo/casa-concat.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/casa-flag.yml` & `cult_cargo-0.1.2rc8/cultcargo/casa-flag.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/crystalball.yml` & `cult_cargo-0.1.2rc8/cultcargo/crystalball.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/cubical.yml` & `cult_cargo-0.1.2rc8/cultcargo/cubical.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/fitstool.yml` & `cult_cargo-0.1.2rc8/cultcargo/fitstool.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/cubical/make_stimela_schema.py` & `cult_cargo-0.1.2rc8/cultcargo/genesis/cubical/make_stimela_schema.py`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/cubical/schema.yaml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/cubical/schema.yaml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/cubical/schema_JONES_TEMPLATE.yaml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/cubical/schema_JONES_TEMPLATE.yaml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/cgopts.yml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/cgopts.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/clean.yaml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/clean.yaml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/degrid.yaml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/degrid.yaml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/dist.yml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/dist.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/fastim.yaml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/fastim.yaml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/forward.yaml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/forward.yaml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/fwdbwd.yaml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/fwdbwd.yaml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/grid.yaml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/grid.yaml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/init.yaml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/init.yaml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/init_ims.yaml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/init_ims.yaml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/model2comps.yaml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/model2comps.yaml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/restore.yaml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/restore.yaml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/spotless.yaml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/spotless.yaml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/latest/uncabbedcabs.yml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/latest/uncabbedcabs.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/pfb-clean/sync_config.py` & `cult_cargo-0.1.2rc8/cultcargo/genesis/pfb-clean/sync_config.py`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/quartical/__init__.py` & `cult_cargo-0.1.2rc8/cultcargo/genesis/quartical/__init__.py`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/quartical/argument_schema.yaml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/quartical/argument_schema.yaml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/quartical/config_classes.py` & `cult_cargo-0.1.2rc8/cultcargo/genesis/quartical/config_classes.py`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/quartical/converters.py` & `cult_cargo-0.1.2rc8/cultcargo/genesis/quartical/converters.py`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/quartical/external.py` & `cult_cargo-0.1.2rc8/cultcargo/genesis/quartical/external.py`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/quartical/gain_schema.yaml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/quartical/gain_schema.yaml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/wsclean/__init__.py` & `cult_cargo-0.1.2rc8/cultcargo/genesis/wsclean/__init__.py`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/genesis/wsclean/wsclean-base.yml` & `cult_cargo-0.1.2rc8/cultcargo/genesis/wsclean/wsclean-base.yml`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,16 @@
           dtype: int
         parallel-gridding:
           dtype: int
         parallel-reordering:
           dtype: int
         no-reorder:
           dtype: bool
+        reorder:
+          dtype: bool
         predict:
           dtype: bool
         no-update-model-required:
           dtype: bool
         continue:
           dtype: bool
         subtract-model:
```

### Comparing `cult_cargo-0.1.2rc7/cultcargo/images/casa/Dockerfile.base` & `cult_cargo-0.1.2rc8/cultcargo/images/casa/Dockerfile.base`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/images/python-astro/Dockerfile` & `cult_cargo-0.1.2rc8/cultcargo/images/python-astro/Dockerfile`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 FROM {REGISTRY}/base-cult:base-{BUNDLE_VERSION}
 
 ENV DEBIAN_FRONTEND=noninteractive
 
+RUN apt-add-repository -y ppa:deadsnakes/ppa
+
 RUN apt-get update && apt-get install apt-utils && \
-    apt-get install -y casacore-data casacore-tools python{VERSION}-dev \
-    python3-pip python3-pytest python3-matplotlib \
+    apt-get install -y casacore-data casacore-tools python{VERSION}-dev python{VERSION}-distutils \
+    python3-pip python3-pytest python3-matplotlib curl\
     && rm -rf /var/lib/apt/lists/* \
     && rm -rf /var/cache/apt/archives 
 
 RUN update-alternatives --install /usr/bin/python python /usr/bin/python{VERSION} 1
 
-# upgrade pip
+# needed to upgrade pip properly -- sometimes it gets stuck and is unable to upgrade itself
+RUN curl -sS https://bootstrap.pypa.io/get-pip.py | python{VERSION}
+
 RUN python{VERSION} -mpip install --no-cache-dir -U pip setuptools wheel 
 
 # add useful astro stuff
 RUN python{VERSION} -mpip install --no-cache-dir \
     python-casacore astropy astroplan regions astro-tigger-lsm \
     owlcat dask-ms scipy omegaconf bdsf msutils
 
 # add stimela -- useful for scabha.schema_utils
-RUN python{VERSION} -mpip install --no-cache-dir git+https://github.com/caracal-pipeline/stimela@2.0rc12
+RUN python{VERSION} -mpip install --no-cache-dir "stimela>=2.0rc17"
 
 CMD /usr/bin/python{VERSION}
```

### Comparing `cult_cargo-0.1.2rc7/cultcargo/images/wsclean/Dockerfile.build` & `cult_cargo-0.1.2rc8/cultcargo/images/wsclean/Dockerfile.build`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/images/wsclean/Dockerfile.build.2x` & `cult_cargo-0.1.2rc8/cultcargo/images/wsclean/Dockerfile.build.2x`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/mosaic-queen.yml` & `cult_cargo-0.1.2rc8/cultcargo/mosaic-queen.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/msutils.yml` & `cult_cargo-0.1.2rc8/cultcargo/msutils.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/pfb-clean.yml` & `cult_cargo-0.1.2rc8/cultcargo/pfb-clean.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/quartical.yml` & `cult_cargo-0.1.2rc8/cultcargo/quartical.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/rfinder.yml` & `cult_cargo-0.1.2rc8/cultcargo/rfinder.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/shadems.yml` & `cult_cargo-0.1.2rc8/cultcargo/shadems.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/smops.yml` & `cult_cargo-0.1.2rc8/cultcargo/smops.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/spimple-spifit.yml` & `cult_cargo-0.1.2rc8/cultcargo/spimple-spifit.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/taql.yml` & `cult_cargo-0.1.2rc8/cultcargo/taql.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/tigger.yml` & `cult_cargo-0.1.2rc8/cultcargo/tigger.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/tricolour.yml` & `cult_cargo-0.1.2rc8/cultcargo/tricolour.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/utils.py` & `cult_cargo-0.1.2rc8/cultcargo/utils.py`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/cultcargo/wsclean.yml` & `cult_cargo-0.1.2rc8/cultcargo/wsclean.yml`

 * *Files identical despite different names*

### Comparing `cult_cargo-0.1.2rc7/pyproject.toml` & `cult_cargo-0.1.2rc8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "cult-cargo"
-version = "0.1.2rc7"
+version = "0.1.2rc8"
 description = "Curated cargo of standard radio astronomy packages for stimela 2.0"
 authors = ["Oleg Smirnov, Sphesihle Makhathini"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "cultcargo"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 stimela = "^2.0rc17"
+requests = "^2.0"
 
 [tool.poetry.scripts]
 build-cargo = "cultcargo.builder.build_cargo:driver"
 
 [tool.poetry.group.builder]
 optional = true
```

### Comparing `cult_cargo-0.1.2rc7/PKG-INFO` & `cult_cargo-0.1.2rc8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: cult-cargo
-Version: 0.1.2rc7
+Version: 0.1.2rc8
 Summary: Curated cargo of standard radio astronomy packages for stimela 2.0
 License: MIT
 Author: Oleg Smirnov, Sphesihle Makhathini
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: requests (>=2.0,<3.0)
 Requires-Dist: stimela (>=2.0rc17,<3.0)
 Description-Content-Type: text/markdown
 
 # cult-cargo
 Curated Stimela2 cargo for popular radio astronomy software.
 
 ## Regular userland install
@@ -63,7 +64,18 @@
 
 ``build-cargo.py -a`` will build and push all images, or specify an image name to build a particular one. Use ``-b`` to build but not push, or ``-p`` for push-only. Use ``-l`` to list available images.
 
 The ``cultcargo`` folder contains YaML files with cab definitions.
 
 If you would like to maintain your own image collection, write your own manifest and Dockerfiles following the cult-cargo example, and use the ``build-cargo.py`` script to build your images.
 
+## Using cult-cargo as a standalone image repository
+
+You don't even need to run stimela (or indeed install anything) to take advantage of the images packaged with cult-cargo. Take a look at the image repository on https://quay.io/organization/stimela2 to see what's available.
+
+For example, if you want to run a wsclean image, just do:
+
+```
+$ singularity build wsclean-3.3.sif docker:quay.io/stimela2/wsclean:3.3-cc0.1.2
+$ singularity exec wsclean-3.3.sif wsclean 
+```
+
```

