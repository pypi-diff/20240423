# Comparing `tmp/light_curve-0.9.0.tar.gz` & `tmp/light_curve-0.9.1.tar.gz`

## Comparing `light_curve-0.9.0.tar` & `light_curve-0.9.1.tar`

### file list

```diff
@@ -1,110 +1,112 @@
--rw-r--r--   0        0        0     1680 1970-01-01 00:00:00.000000 light_curve-0.9.0/Cargo.toml
--rw-r--r--   0     1001      127       91 2024-03-06 13:19:46.000000 light_curve-0.9.0/.gitignore
--rw-r--r--   0     1001      127    75073 2024-03-06 13:19:46.000000 light_curve-0.9.0/.readme/benchplot.png
--rw-r--r--   0     1001      127    27741 2024-03-06 13:19:46.000000 light_curve-0.9.0/README.md
--rw-r--r--   0     1001      127      271 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/__init__.py
--rw-r--r--   0     1001      127      445 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_ext.py
--rw-r--r--   0     1001      127     1112 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/__init__.py
--rw-r--r--   0     1001      127      259 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/dataclass_field.py
--rw-r--r--   0     1001      127        0 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/__init__.py
--rw-r--r--   0     1001      127     5564 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/_base.py
--rw-r--r--   0     1001      127     1485 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/_base_meta.py
--rw-r--r--   0     1001      127      391 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/_lstsq.py
--rw-r--r--   0     1001      127      522 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/adnormal.py
--rw-r--r--   0     1001      127      276 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/amplitude.py
--rw-r--r--   0     1001      127      453 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/beyondnstd.py
--rw-r--r--   0     1001      127     1337 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/bins.py
--rw-r--r--   0     1001      127      826 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/color_of_median.py
--rw-r--r--   0     1001      127      409 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/cusum.py
--rw-r--r--   0     1001      127      373 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/eta.py
--rw-r--r--   0     1001      127      426 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/etae.py
--rw-r--r--   0     1001      127      409 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/excvar.py
--rw-r--r--   0     1001      127     1395 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/extractor.py
--rw-r--r--   0     1001      127     2172 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/flux_n_not_det_before_fd.py
--rw-r--r--   0     1001      127      720 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/intpercrange.py
--rw-r--r--   0     1001      127      520 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/kurtosis.py
--rw-r--r--   0     1001      127      662 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/linfit.py
--rw-r--r--   0     1001      127      499 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/lintrend.py
--rw-r--r--   0     1001      127     2267 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/magnitude_n_not_det_before_fd.py
--rw-r--r--   0     1001      127      967 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/magnpratio.py
--rw-r--r--   0     1001      127      415 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/maxslope.py
--rw-r--r--   0     1001      127      261 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/mean.py
--rw-r--r--   0     1001      127      297 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/meanvar.py
--rw-r--r--   0     1001      127      326 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/medabsdev.py
--rw-r--r--   0     1001      127      578 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/medbufrperc.py
--rw-r--r--   0     1001      127      267 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/median.py
--rw-r--r--   0     1001      127     2685 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/otsusplit.py
--rw-r--r--   0     1001      127      829 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/pdiffmperc.py
--rw-r--r--   0     1001      127      353 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/percampl.py
--rw-r--r--   0     1001      127       23 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/rainbow/__init__.py
--rw-r--r--   0     1001      127     1948 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/rainbow/_bands.py
--rw-r--r--   0     1001      127    13086 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/rainbow/_base.py
--rw-r--r--   0     1001      127     2470 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/rainbow/_parameters.py
--rw-r--r--   0     1001      127     2802 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/rainbow/_scaler.py
--rw-r--r--   0     1001      127     5902 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/rainbow/bolometric.py
--rw-r--r--   0     1001      127     6498 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/rainbow/generic.py
--rw-r--r--   0     1001      127     5206 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/rainbow/temperature.py
--rw-r--r--   0     1001      127        0 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/rainbow.py
--rw-r--r--   0     1001      127      421 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/redchi2.py
--rw-r--r--   0     1001      127      747 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/roms.py
--rw-r--r--   0     1001      127      420 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/skew.py
--rw-r--r--   0     1001      127      294 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/stdev.py
--rw-r--r--   0     1001      127      463 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/stetsonk.py
--rw-r--r--   0     1001      127      309 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/features/weightmean.py
--rw-r--r--   0     1001      127      896 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/minuit_lsq.py
--rw-r--r--   0     1001      127      596 2024-03-06 13:19:46.000000 light_curve-0.9.0/light_curve/light_curve_py/warnings.py
--rw-r--r--   0     1001      127     1395 2024-03-06 13:19:46.000000 light_curve-0.9.0/src/check.rs
--rw-r--r--   0     1001      127     2245 2024-03-06 13:19:46.000000 light_curve-0.9.0/src/cont_array.rs
--rw-r--r--   0     1001      127    50832 2024-03-06 13:19:46.000000 light_curve-0.9.0/src/dmdt.rs
--rw-r--r--   0     1001      127     1504 2024-03-06 13:19:46.000000 light_curve-0.9.0/src/errors.rs
--rw-r--r--   0     1001      127    65118 2024-03-06 13:19:46.000000 light_curve-0.9.0/src/features.rs
--rw-r--r--   0     1001      127     3478 2024-03-06 13:19:46.000000 light_curve-0.9.0/src/lib.rs
--rw-r--r--   0     1001      127     4269 2024-03-06 13:19:46.000000 light_curve-0.9.0/src/ln_prior.rs
--rw-r--r--   0     1001      127     3600 2024-03-06 13:19:46.000000 light_curve-0.9.0/src/np_array.rs
--rw-r--r--   0     1001      127     4450 2024-03-06 13:19:46.000000 light_curve-0.9.0/src/transform.rs
--rw-r--r--   0     1001      127        0 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/__init__.py
--rw-r--r--   0     1001      127      719 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/conftest.py
--rw-r--r--   0     1001      127        0 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_ext/__init__.py
--rw-r--r--   0     1001      127    12272 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_ext/test_dmdt.py
--rw-r--r--   0     1001      127    10826 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_ext/test_feature.py
--rw-r--r--   0     1001      127      786 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_ext/test_ln_prior.py
--rw-r--r--   0     1001      127        0 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/__init__.py
--rw-r--r--   0     1001      127      304 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_adnormal.py
--rw-r--r--   0     1001      127      289 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_amplitude.py
--rw-r--r--   0     1001      127      526 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_beyondnstd.py
--rw-r--r--   0     1001      127     2079 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_bins.py
--rw-r--r--   0     1001      127      610 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_color_of_median.py
--rw-r--r--   0     1001      127      302 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_cusum.py
--rw-r--r--   0     1001      127      311 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_eta.py
--rw-r--r--   0     1001      127      562 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_etae.py
--rw-r--r--   0     1001      127      359 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_excvar.py
--rw-r--r--   0     1001      127     1915 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_extractor.py
--rw-r--r--   0     1001      127      487 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_intpercrange.py
--rw-r--r--   0     1001      127      497 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_kurtosis.py
--rw-r--r--   0     1001      127      702 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_linfit.py
--rw-r--r--   0     1001      127      939 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_lintrend.py
--rw-r--r--   0     1001      127      688 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_magnpratio.py
--rw-r--r--   0     1001      127      297 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_maxslope.py
--rw-r--r--   0     1001      127      450 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_mean.py
--rw-r--r--   0     1001      127      326 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_meanvar.py
--rw-r--r--   0     1001      127      335 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_medabsdev.py
--rw-r--r--   0     1001      127      317 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_medbufrperc.py
--rw-r--r--   0     1001      127      509 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_median.py
--rw-r--r--   0     1001      127     1687 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_n_not_det_before_fd.py
--rw-r--r--   0     1001      127     1307 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_otsusplit.py
--rw-r--r--   0     1001      127      345 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_pdiffmperc.py
--rw-r--r--   0     1001      127      321 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_percampl.py
--rw-r--r--   0     1001      127     5482 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_rainbow.py
--rw-r--r--   0     1001      127      650 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_redchi2.py
--rw-r--r--   0     1001      127     2456 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_roms.py
--rw-r--r--   0     1001      127      302 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_skew.py
--rw-r--r--   0     1001      127      348 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_stdev.py
--rw-r--r--   0     1001      127      673 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_stetsonk.py
--rw-r--r--   0     1001      127      351 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/features/test_weightmean.py
--rw-r--r--   0     1001      127      964 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/test_call.py
--rw-r--r--   0     1001      127     3299 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/light_curve_py/test_single_band.py
--rw-r--r--   0     1001      127    23998 2024-03-06 13:19:46.000000 light_curve-0.9.0/tests/test_w_bench.py
--rw-r--r--   0     1001      127    63700 2024-03-06 13:19:46.000000 light_curve-0.9.0/Cargo.lock
--rw-r--r--   0     1001      127     7149 2024-03-06 13:19:46.000000 light_curve-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    29689 1970-01-01 00:00:00.000000 light_curve-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 light_curve-0.9.1/Cargo.toml
+-rw-r--r--   0     1001      127       91 2024-04-23 13:18:26.000000 light_curve-0.9.1/.gitignore
+-rw-r--r--   0     1001      127    75073 2024-04-23 13:18:26.000000 light_curve-0.9.1/.readme/benchplot.png
+-rw-r--r--   0     1001      127    27873 2024-04-23 13:18:26.000000 light_curve-0.9.1/README.md
+-rw-r--r--   0     1001      127      271 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/__init__.py
+-rw-r--r--   0     1001      127      445 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_ext.py
+-rw-r--r--   0     1001      127     1144 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/__init__.py
+-rw-r--r--   0     1001      127      259 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/dataclass_field.py
+-rw-r--r--   0     1001      127        0 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/__init__.py
+-rw-r--r--   0     1001      127     5564 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/_base.py
+-rw-r--r--   0     1001      127     1485 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/_base_meta.py
+-rw-r--r--   0     1001      127      391 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/_lstsq.py
+-rw-r--r--   0     1001      127      522 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/adnormal.py
+-rw-r--r--   0     1001      127      276 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/amplitude.py
+-rw-r--r--   0     1001      127      453 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/beyondnstd.py
+-rw-r--r--   0     1001      127     1337 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/bins.py
+-rw-r--r--   0     1001      127      826 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/color_of_median.py
+-rw-r--r--   0     1001      127      409 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/cusum.py
+-rw-r--r--   0     1001      127      373 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/eta.py
+-rw-r--r--   0     1001      127      426 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/etae.py
+-rw-r--r--   0     1001      127      409 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/excvar.py
+-rw-r--r--   0     1001      127     1395 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/extractor.py
+-rw-r--r--   0     1001      127     2172 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/flux_n_not_det_before_fd.py
+-rw-r--r--   0     1001      127      720 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/intpercrange.py
+-rw-r--r--   0     1001      127      520 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/kurtosis.py
+-rw-r--r--   0     1001      127      662 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/linfit.py
+-rw-r--r--   0     1001      127      499 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/lintrend.py
+-rw-r--r--   0     1001      127     2267 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/magnitude_n_not_det_before_fd.py
+-rw-r--r--   0     1001      127      967 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/magnpratio.py
+-rw-r--r--   0     1001      127      415 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/maxslope.py
+-rw-r--r--   0     1001      127      261 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/mean.py
+-rw-r--r--   0     1001      127      297 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/meanvar.py
+-rw-r--r--   0     1001      127      326 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/medabsdev.py
+-rw-r--r--   0     1001      127      578 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/medbufrperc.py
+-rw-r--r--   0     1001      127      267 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/median.py
+-rw-r--r--   0     1001      127     2685 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/otsusplit.py
+-rw-r--r--   0     1001      127      829 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/pdiffmperc.py
+-rw-r--r--   0     1001      127      353 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/percampl.py
+-rw-r--r--   0     1001      127     1056 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/ptp_var.py
+-rw-r--r--   0     1001      127       23 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/rainbow/__init__.py
+-rw-r--r--   0     1001      127     1948 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/rainbow/_bands.py
+-rw-r--r--   0     1001      127    13086 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/rainbow/_base.py
+-rw-r--r--   0     1001      127     2470 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/rainbow/_parameters.py
+-rw-r--r--   0     1001      127     2802 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/rainbow/_scaler.py
+-rw-r--r--   0     1001      127     5902 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/rainbow/bolometric.py
+-rw-r--r--   0     1001      127     6498 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/rainbow/generic.py
+-rw-r--r--   0     1001      127     5206 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/rainbow/temperature.py
+-rw-r--r--   0     1001      127        0 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/rainbow.py
+-rw-r--r--   0     1001      127      421 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/redchi2.py
+-rw-r--r--   0     1001      127      747 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/roms.py
+-rw-r--r--   0     1001      127      420 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/skew.py
+-rw-r--r--   0     1001      127      294 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/stdev.py
+-rw-r--r--   0     1001      127      463 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/stetsonk.py
+-rw-r--r--   0     1001      127      309 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/features/weightmean.py
+-rw-r--r--   0     1001      127      896 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/minuit_lsq.py
+-rw-r--r--   0     1001      127      596 2024-04-23 13:18:26.000000 light_curve-0.9.1/light_curve/light_curve_py/warnings.py
+-rw-r--r--   0     1001      127     1395 2024-04-23 13:18:26.000000 light_curve-0.9.1/src/check.rs
+-rw-r--r--   0     1001      127     2245 2024-04-23 13:18:26.000000 light_curve-0.9.1/src/cont_array.rs
+-rw-r--r--   0     1001      127    52550 2024-04-23 13:18:26.000000 light_curve-0.9.1/src/dmdt.rs
+-rw-r--r--   0     1001      127     1504 2024-04-23 13:18:26.000000 light_curve-0.9.1/src/errors.rs
+-rw-r--r--   0     1001      127    66058 2024-04-23 13:18:26.000000 light_curve-0.9.1/src/features.rs
+-rw-r--r--   0     1001      127     3484 2024-04-23 13:18:26.000000 light_curve-0.9.1/src/lib.rs
+-rw-r--r--   0     1001      127     4313 2024-04-23 13:18:26.000000 light_curve-0.9.1/src/ln_prior.rs
+-rw-r--r--   0     1001      127     3636 2024-04-23 13:18:26.000000 light_curve-0.9.1/src/np_array.rs
+-rw-r--r--   0     1001      127     4570 2024-04-23 13:18:26.000000 light_curve-0.9.1/src/transform.rs
+-rw-r--r--   0     1001      127        0 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/__init__.py
+-rw-r--r--   0     1001      127      719 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/conftest.py
+-rw-r--r--   0     1001      127        0 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_ext/__init__.py
+-rw-r--r--   0     1001      127    12272 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_ext/test_dmdt.py
+-rw-r--r--   0     1001      127    10826 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_ext/test_feature.py
+-rw-r--r--   0     1001      127      786 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_ext/test_ln_prior.py
+-rw-r--r--   0     1001      127        0 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/__init__.py
+-rw-r--r--   0     1001      127      304 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_adnormal.py
+-rw-r--r--   0     1001      127      289 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_amplitude.py
+-rw-r--r--   0     1001      127      526 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_beyondnstd.py
+-rw-r--r--   0     1001      127     2079 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_bins.py
+-rw-r--r--   0     1001      127      610 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_color_of_median.py
+-rw-r--r--   0     1001      127      302 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_cusum.py
+-rw-r--r--   0     1001      127      311 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_eta.py
+-rw-r--r--   0     1001      127      562 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_etae.py
+-rw-r--r--   0     1001      127      359 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_excvar.py
+-rw-r--r--   0     1001      127     1915 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_extractor.py
+-rw-r--r--   0     1001      127      487 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_intpercrange.py
+-rw-r--r--   0     1001      127      497 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_kurtosis.py
+-rw-r--r--   0     1001      127      702 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_linfit.py
+-rw-r--r--   0     1001      127      939 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_lintrend.py
+-rw-r--r--   0     1001      127      688 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_magnpratio.py
+-rw-r--r--   0     1001      127      297 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_maxslope.py
+-rw-r--r--   0     1001      127      450 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_mean.py
+-rw-r--r--   0     1001      127      326 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_meanvar.py
+-rw-r--r--   0     1001      127      335 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_medabsdev.py
+-rw-r--r--   0     1001      127      317 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_medbufrperc.py
+-rw-r--r--   0     1001      127      509 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_median.py
+-rw-r--r--   0     1001      127     1687 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_n_not_det_before_fd.py
+-rw-r--r--   0     1001      127     1307 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_otsusplit.py
+-rw-r--r--   0     1001      127      345 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_pdiffmperc.py
+-rw-r--r--   0     1001      127      321 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_percampl.py
+-rw-r--r--   0     1001      127      963 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_ptp_var.py
+-rw-r--r--   0     1001      127     5482 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_rainbow.py
+-rw-r--r--   0     1001      127      650 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_redchi2.py
+-rw-r--r--   0     1001      127     2456 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_roms.py
+-rw-r--r--   0     1001      127      302 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_skew.py
+-rw-r--r--   0     1001      127      348 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_stdev.py
+-rw-r--r--   0     1001      127      673 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_stetsonk.py
+-rw-r--r--   0     1001      127      351 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/features/test_weightmean.py
+-rw-r--r--   0     1001      127      964 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/test_call.py
+-rw-r--r--   0     1001      127     3299 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/light_curve_py/test_single_band.py
+-rw-r--r--   0     1001      127    23998 2024-04-23 13:18:26.000000 light_curve-0.9.1/tests/test_w_bench.py
+-rw-r--r--   0     1001      127    66746 2024-04-23 13:18:26.000000 light_curve-0.9.1/Cargo.lock
+-rw-r--r--   0     1001      127     7149 2024-04-23 13:18:26.000000 light_curve-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    29821 1970-01-01 00:00:00.000000 light_curve-0.9.1/PKG-INFO
```

### Comparing `light_curve-0.9.0/Cargo.toml` & `light_curve-0.9.1/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "light-curve-python"
-version = "0.9.0"
+version = "0.9.1"
 authors = ["Konstantin Malanchev <hombit@gmail.com>", "Anastasia Lavrukhina <lavrukhina.ad@gmail.com>"]
 description = "Feature extractor from noisy time series"
 readme = "README.md"
 repository = "https://github.com/light-curve/light-curve-python"
 license = "GPL-3.0-or-later"
 edition = "2021"
 rust-version = "1.67"
@@ -14,15 +14,15 @@
 crate-type = ["cdylib"]
 
 [profile.release]
 lto = true
 codegen-units = 1
 
 [features]
-default = ["ceres-source", "fftw-source", "gsl", "mimalloc"]
+default = ["abi3", "ceres-source", "fftw-source", "gsl", "mimalloc"]
 abi3 = ["pyo3/abi3-py38"]
 ceres-source = ["light-curve-feature/ceres-source"]
 ceres-system = ["light-curve-feature/ceres-system"]
 fftw-source = ["light-curve-feature/fftw-source"]
 fftw-system = ["light-curve-feature/fftw-system"]
 fftw-mkl = ["light-curve-feature/fftw-mkl"]
 gsl = ["light-curve-feature/gsl"]
@@ -31,24 +31,24 @@
 [dependencies]
 const_format = "0.2.32"
 conv = "0.3.3"
 enum-iterator = "2.0.0"
 enumflags2 = { version = "0.7.7", features = ["serde"] }
 itertools = "0.12.1"
 macro_const = "0.1.0"
-mimalloc = { version = "0.1.39", features = ["local_dynamic_tls"], optional=true }
+mimalloc = { version = "0.1.39", features = ["local_dynamic_tls"], optional = true }
 ndarray = { version = "0.15.3", features = ["rayon"] }
-numpy = "0.19.0"
+numpy = "0.21.0"
 num_cpus = "1.13.0"
 num-traits = "0.2"
 once_cell = "1"
-pyo3 = {version = "0.19.2", features = ["extension-module", "multiple-pymethods"]}
+pyo3 = { version = "0.21.2", features = ["extension-module", "multiple-pymethods", "gil-refs"] }
 rand = "0.8.5"
 rand_xoshiro = "0.6.0"
-rayon = "1.8.1"
+rayon = "1.10.0"
 serde = { version = "1", features = ["derive"] }
 serde-pickle = "1"
 serde_json = "1"
 thiserror = "1.0.50"
 unzip3 = "1.0.0"
 
 [dependencies.light-curve-dmdt]
```

### Comparing `light_curve-0.9.0/.readme/benchplot.png` & `light_curve-0.9.1/.readme/benchplot.png`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/README.md` & `light_curve-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 python3 -mpip install 'light-curve[full]'
 ```
 
 `full` extras would install the package with all optional Python dependencies required by experimental features.
 We also provide `light-curve-python` package which is just an "alias" to the main `light-curve[full]` package.
 
 Minimum supported Python version is 3.8.
-We provide binary wheels via [PyPi](https://pypi.org/project/light-curve/) for a number of platforms and architectures, both for CPython and PyPy.
+We provide binary CPython wheels via [PyPi](https://pypi.org/project/light-curve/) for a number of platforms and architectures.
 We also provide binary wheels for stable CPython ABI, so the package is guaranteed to work with all future CPython3 versions.
 
 ### Support matrix
 
 | Arch \ OS   | Linux glibc | Linux musl                     | macOS                                                          | Windows https://github.com/light-curve/light-curve-python/issues/186 |
 | ----------- |-------------|--------------------------------|----------------------------------------------------------------|----------------------------------------------------------------------|
 | **x86-64**  | wheel (MKL) | wheel (MKL)                    | wheel                                                          | wheel (no Ceres, no GSL)                                             |
@@ -28,14 +28,16 @@
 | **aarch64** | wheel       | wheel                          | wheel                                                          | not tested                                                           |
 | **ppc64le** | wheel       | not tested (no Rust toolchain) | —                                                              | —                                                                    |
 
 - "wheel": binary wheel is available on pypi.org, local building is not required for the platform, the only pre-requirement is a recent `pip` version. For Linux x86-64 we provide binary wheels built with Intel MKL for better periodogram performance, which is not a default build option. For Windows x86-64 we provide wheel with no Ceres and no GSL support, which is not a default build option.
 - "src": the package is confirmed to be built and pass unit tests locally, but testing and package building is not supported by CI. It is required to have the [GNU scientific library (GSL)](https://www.gnu.org/software/gsl/) v2.1+ and the [Rust toolchain](https://rust-lang.org) v1.67+ to install it via `pip install`. `ceres-solver` and `fftw` may be installed locally or built from source, in the later case you would also need C/C++ compiler and `cmake`.
 - "not tested": building from the source code is not tested, please report us building status via issue/PR/email.
 
+We stopped publishing PyPy wheels (https://github.com/light-curve/light-curve-python/issues/345), please feel free to open an issue if you need them.
+
 ## Feature evaluators
 
 Most of the classes implement various feature evaluators useful for light-curve based
 astrophysical source classification and characterisation.
 
 <!-- name: test_feature_evaluators_basic -->
 ```python
```

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/__init__.py` & `light_curve-0.9.1/light_curve/light_curve_py/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .features.meanvar import *
 from .features.medabsdev import *
 from .features.medbufrperc import *
 from .features.median import *
 from .features.otsusplit import *
 from .features.pdiffmperc import *
 from .features.percampl import *
+from .features.ptp_var import *
 from .features.rainbow import *
 from .features.redchi2 import *
 from .features.roms import *
 from .features.skew import *
 from .features.stdev import *
 from .features.stetsonk import *
 from .features.weightmean import *
```

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/_base.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/_base.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/_base_meta.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/_base_meta.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/adnormal.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/adnormal.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/bins.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/bins.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/color_of_median.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/color_of_median.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/extractor.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/extractor.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/flux_n_not_det_before_fd.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/flux_n_not_det_before_fd.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/intpercrange.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/intpercrange.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/kurtosis.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/kurtosis.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/linfit.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/linfit.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/magnitude_n_not_det_before_fd.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/magnitude_n_not_det_before_fd.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/magnpratio.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/magnpratio.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/medbufrperc.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/medbufrperc.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/otsusplit.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/otsusplit.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/pdiffmperc.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/pdiffmperc.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/rainbow/_bands.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/rainbow/_bands.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/rainbow/_base.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/rainbow/_base.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/rainbow/_parameters.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/rainbow/_parameters.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/rainbow/_scaler.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/rainbow/_scaler.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/rainbow/bolometric.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/rainbow/bolometric.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/rainbow/generic.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/rainbow/generic.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/rainbow/temperature.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/rainbow/temperature.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/features/roms.py` & `light_curve-0.9.1/light_curve/light_curve_py/features/roms.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/minuit_lsq.py` & `light_curve-0.9.1/light_curve/light_curve_py/minuit_lsq.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/light_curve/light_curve_py/warnings.py` & `light_curve-0.9.1/light_curve/light_curve_py/warnings.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/src/check.rs` & `light_curve-0.9.1/src/check.rs`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/src/cont_array.rs` & `light_curve-0.9.1/src/cont_array.rs`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/src/dmdt.rs` & `light_curve-0.9.1/src/dmdt.rs`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 use crate::np_array::Arr;
 
 use conv::{ApproxFrom, ApproxInto, ConvAsUtil};
 use enumflags2::{bitflags, BitFlags};
 use light_curve_dmdt as lcdmdt;
 use light_curve_dmdt::{Grid, GridTrait};
 use ndarray::IntoNdProducer;
-use numpy::{Element, IntoPyArray, PyArray1, ToPyArray};
+use numpy::prelude::*;
+use numpy::{Element, PyArray1, PyUntypedArray, ToPyArray};
 use pyo3::prelude::*;
 use pyo3::types::{PyBytes, PyTuple};
 use rand::SeedableRng;
 use rand_xoshiro::Xoshiro256PlusPlus;
 use rayon::prelude::*;
 use serde::{Deserialize, Serialize};
 use std::cell::RefCell;
@@ -50,19 +51,19 @@
 {
     dmdt: lcdmdt::DmDt<T>,
     norm: BitFlags<NormFlag>,
     error_func: ErrorFunction,
     n_jobs: usize,
 }
 
-impl<'a, T> GenericDmDt<T>
+impl<'py, T> GenericDmDt<T>
 where
     T: Element + ndarray::NdFloat + lcdmdt::ErfFloat,
 {
-    fn sigma_to_err2(sigma: Arr<'a, T>) -> ContArray<T> {
+    fn sigma_to_err2(sigma: Arr<'py, T>) -> ContArray<T> {
         let mut a: ContArray<_> = sigma.as_array().into();
         a.0.mapv_inplace(|x| x.powi(2));
         a
     }
 
     fn normalize(&self, a: &mut ndarray::Array2<T>, t: &[T]) {
         if self.norm.contains(NormFlag::Dt) {
@@ -80,28 +81,38 @@
             let max = *a.iter().max_by(|a, b| a.partial_cmp(b).unwrap()).unwrap();
             if !max.is_zero() {
                 a.mapv_inplace(|x| x / max);
             }
         }
     }
 
-    fn py_count_dt(&self, py: Python, t: Arr<'a, T>, sorted: Option<bool>) -> Res<PyObject> {
+    fn py_count_dt(
+        &self,
+        py: Python<'py>,
+        t: Arr<'py, T>,
+        sorted: Option<bool>,
+    ) -> Res<Bound<'py, PyUntypedArray>> {
         self.count_dt(
             ContCowArray::from_view(t.as_array(), true).as_slice(),
             sorted,
         )
-        .map(|a| a.into_pyarray(py).into_py(py))
+        .map(|a| a.into_pyarray_bound(py).as_untyped().clone())
     }
 
     fn count_dt(&self, t: &[T], sorted: Option<bool>) -> Res<ndarray::Array1<T>> {
         check_sorted(t, sorted)?;
         Ok(self.dmdt.dt_points(t).mapv(|x| x.approx_into().unwrap()))
     }
 
-    fn py_count_dt_many(&self, py: Python, t_: Vec<&PyAny>, sorted: Option<bool>) -> Res<PyObject> {
+    fn py_count_dt_many(
+        &self,
+        py: Python<'py>,
+        t_: Vec<Bound<'py, PyAny>>,
+        sorted: Option<bool>,
+    ) -> Res<Bound<'py, PyUntypedArray>> {
         let wrapped_t_ = t_
             .into_iter()
             .enumerate()
             .map(|(i, t)| match t.downcast::<PyArray1<T>>() {
                 Ok(a) => Ok(a.readonly()),
                 Err(_) => Err(Exception::TypeError(format!(
                     "t_[{}] has mismatched dtype with the t_[0] which is {}",
@@ -113,16 +124,17 @@
         let array_t_ = wrapped_t_
             .iter()
             .map(|t| ContCowArray::from_view(t.as_array(), true))
             .collect::<Vec<_>>();
         let typed_t_ = array_t_.iter().map(|t| t.as_slice()).collect();
         Ok(self
             .count_dt_many(typed_t_, sorted)?
-            .into_pyarray(py)
-            .into_py(py))
+            .into_pyarray_bound(py)
+            .as_untyped()
+            .clone())
     }
 
     fn count_dt_many(&self, t_: Vec<&[T]>, sorted: Option<bool>) -> Res<ndarray::Array2<T>> {
         let dt_size = self.dmdt.dt_grid.cell_count();
         let mut result = ndarray::Array2::zeros((t_.len(), dt_size));
 
         rayon::ThreadPoolBuilder::new()
@@ -139,43 +151,44 @@
                     })
             })?;
         Ok(result)
     }
 
     fn py_points(
         &self,
-        py: Python,
-        t: Arr<'a, T>,
-        m: Arr<'a, T>,
+        py: Python<'py>,
+        t: Arr<'py, T>,
+        m: Arr<'py, T>,
         sorted: Option<bool>,
-    ) -> Res<PyObject> {
+    ) -> Res<Bound<'py, PyUntypedArray>> {
         Ok(self
             .points(
                 ContCowArray::from_view(t.as_array(), true).as_slice(),
                 ContCowArray::from_view(m.as_array(), true).as_slice(),
                 sorted,
             )?
-            .into_pyarray(py)
-            .into_py(py))
+            .into_pyarray_bound(py)
+            .as_untyped()
+            .clone())
     }
 
     fn points(&self, t: &[T], m: &[T], sorted: Option<bool>) -> Res<ndarray::Array2<T>> {
         check_sorted(t, sorted)?;
 
         let mut result = self.dmdt.points(t, m).mapv(|x| x.approx_into().unwrap());
         self.normalize(&mut result, t);
         Ok(result)
     }
 
     fn py_points_many(
         &self,
-        py: Python,
-        lcs: Vec<(&PyAny, &PyAny)>,
+        py: Python<'py>,
+        lcs: Vec<(Bound<'py, PyAny>, Bound<'py, PyAny>)>,
         sorted: Option<bool>,
-    ) -> Res<PyObject> {
+    ) -> Res<Bound<'py, PyUntypedArray>> {
         let wrapped_lcs = lcs
             .into_iter()
             .enumerate()
             .map(|(i, (t, m))| {
                 let t = t.downcast::<PyArray1<T>>().map(|a| a.readonly());
                 let m = m.downcast::<PyArray1<T>>().map(|a| a.readonly());
                 match (t, m) {
@@ -199,16 +212,17 @@
             .collect::<Vec<_>>();
         let typed_lcs = array_lcs
             .iter()
             .map(|(t, m)| (t.as_slice(), m.as_slice()))
             .collect();
         Ok(self
             .points_many(typed_lcs, sorted)?
-            .into_pyarray(py)
-            .into_py(py))
+            .into_pyarray_bound(py)
+            .as_untyped()
+            .clone())
     }
 
     fn points_many(&self, lcs: Vec<(&[T], &[T])>, sorted: Option<bool>) -> Res<ndarray::Array3<T>> {
         let dmdt_shape = self.dmdt.shape();
         let mut result = ndarray::Array3::zeros((lcs.len(), dmdt_shape.0, dmdt_shape.1));
 
         rayon::ThreadPoolBuilder::new()
@@ -226,15 +240,15 @@
             })?;
         Ok(result)
     }
 
     #[allow(clippy::too_many_arguments)]
     fn generic_dmdt_points_batches(
         &self,
-        lcs: Vec<(&'a PyAny, &'a PyAny)>,
+        lcs: Vec<(Bound<'py, PyAny>, Bound<'py, PyAny>)>,
         sorted: Option<bool>,
         batch_size: usize,
         yield_index: bool,
         shuffle: bool,
         drop_nobs: DropNObsType,
         random_seed: Option<u64>,
     ) -> Res<GenericDmDtBatches<T, TmLc<T>>> {
@@ -268,30 +282,31 @@
             drop_nobs,
             random_seed,
         )
     }
 
     fn py_gausses(
         &self,
-        py: Python,
-        t: Arr<'a, T>,
-        m: Arr<'a, T>,
-        sigma: Arr<'a, T>,
+        py: Python<'py>,
+        t: Arr<'py, T>,
+        m: Arr<'py, T>,
+        sigma: Arr<'py, T>,
         sorted: Option<bool>,
-    ) -> Res<PyObject> {
+    ) -> Res<Bound<'py, PyUntypedArray>> {
         let err2 = Self::sigma_to_err2(sigma);
         Ok(self
             .gausses(
                 ContCowArray::from_view(t.as_array(), true).as_slice(),
                 ContCowArray::from_view(m.as_array(), true).as_slice(),
                 err2.as_slice(),
                 sorted,
             )?
-            .into_pyarray(py)
-            .into_py(py))
+            .into_pyarray_bound(py)
+            .as_untyped()
+            .clone())
     }
 
     fn gausses(
         &self,
         t: &[T],
         m: &[T],
         err2: &[T],
@@ -305,18 +320,18 @@
         };
         self.normalize(&mut result, t);
         Ok(result)
     }
 
     fn py_gausses_many(
         &self,
-        py: Python,
-        lcs: Vec<(&'a PyAny, &'a PyAny, &'a PyAny)>,
+        py: Python<'py>,
+        lcs: Vec<(Bound<'py, PyAny>, Bound<'py, PyAny>, Bound<'py, PyAny>)>,
         sorted: Option<bool>,
-    ) -> Res<PyObject> {
+    ) -> Res<Bound<'py, PyUntypedArray>> {
         let wrapped_lcs = lcs
             .into_iter()
             .enumerate()
             .map(|(i, (t, m, sigma))| {
                 let t = t.downcast::<PyArray1<T>>().map(|a| a.readonly());
                 let m = m.downcast::<PyArray1<T>>().map(|a| a.readonly());
                 let sigma = sigma.downcast::<PyArray1<T>>().map(|a| a.readonly());
@@ -343,16 +358,17 @@
             .collect::<Vec<_>>();
         let typed_lcs = array_lcs
             .iter()
             .map(|(t, m, err2)| (t.as_slice(), m.as_slice(), err2.as_slice()))
             .collect();
         Ok(self
             .gausses_many(typed_lcs, sorted)?
-            .into_pyarray(py)
-            .into_py(py))
+            .into_pyarray_bound(py)
+            .as_untyped()
+            .clone())
     }
 
     fn gausses_many(
         &self,
         lcs: Vec<(&[T], &[T], &[T])>,
         sorted: Option<bool>,
     ) -> Res<ndarray::Array3<T>> {
@@ -374,15 +390,15 @@
             })?;
         Ok(result)
     }
 
     #[allow(clippy::too_many_arguments)]
     fn generic_dmdt_gausses_batches(
         &self,
-        lcs: Vec<(&'a PyAny, &'a PyAny, &'a PyAny)>,
+        lcs: Vec<(Bound<PyAny>, Bound<PyAny>, Bound<PyAny>)>,
         sorted: Option<bool>,
         batch_size: usize,
         yield_index: bool,
         shuffle: bool,
         drop_nobs: DropNObsType,
         random_seed: Option<u64>,
     ) -> Res<GenericDmDtBatches<T, Tmerr2Lc<T>>> {
@@ -596,15 +612,15 @@
 
         #[pymethods]
         impl $name_iter {
             fn __iter__(slf: PyRef<Self>) -> PyRef<Self> {
                 slf
             }
 
-            fn __next__(mut slf: PyRefMut<Self>) -> Res<Option<PyObject>> {
+            fn __next__(mut slf: PyRefMut<Self>) -> Res<Option<Bound<PyAny>>> {
                 if slf.worker_thread.borrow().is_none() {
                     return Ok(None);
                 }
 
                 let current_range = match slf.dmdt_batches.yield_index {
                     true => Some(slf.range.clone()),
                     false => None,
@@ -623,21 +639,23 @@
                     slf.worker_thread.replace(Some(Self::run_worker_thread(
                         &slf.dmdt_batches,
                         &slf.lcs_order[slf.range.start..slf.range.end],
                         rng,
                     )));
                 }
 
-                let py_array = array.into_pyarray(slf.py()).into_py(slf.py());
+                let py_array = array.into_pyarray_bound(slf.py()).into_any();
                 match current_range {
                     Some(range) => {
-                        let py_index =
-                            PyArray1::from_slice(slf.py(), &slf.lcs_order[range.start..range.end])
-                                .into_py(slf.py());
-                        let tuple = PyTuple::new(slf.py(), &[py_index, py_array]).into_py(slf.py());
+                        let py_index = PyArray1::from_slice_bound(
+                            slf.py(),
+                            &slf.lcs_order[range.start..range.end],
+                        )
+                        .into_any();
+                        let tuple = PyTuple::new_bound(slf.py(), &[py_index, py_array]).into_any();
                         Ok(Some(tuple))
                     }
                     None => Ok(Some(py_array)),
                 }
             }
         }
     };
@@ -972,17 +990,17 @@
         *,
         dt_type = "auto",
         dm_type = "auto",
         norm=vec![],
         n_jobs = -1,
         approx_erf = false
     ))]
-    fn __new__<'a>(
-        dt: Arr<'a, f64>,
-        dm: Arr<'a, f64>,
+    fn __new__<'py>(
+        dt: Arr<'py, f64>,
+        dm: Arr<'py, f64>,
         dt_type: &str,
         dm_type: &str,
         norm: Vec<&str>,
         n_jobs: i64,
         approx_erf: bool,
     ) -> Res<Self> {
         let (dt_grid_f32, dt_grid_f64) = Self::grids(dt.as_array(), dt_type)?;
@@ -1056,31 +1074,39 @@
 
     #[getter]
     fn shape(&self) -> (usize, usize) {
         self.dmdt_f64.dmdt.shape()
     }
 
     #[getter]
-    fn dt_grid<'py>(&self, py: Python<'py>) -> &'py PyArray1<f64> {
-        self.dmdt_f64.dmdt.dt_grid.get_borders().to_pyarray(py)
+    fn dt_grid<'py>(&self, py: Python<'py>) -> Bound<'py, PyArray1<f64>> {
+        self.dmdt_f64
+            .dmdt
+            .dt_grid
+            .get_borders()
+            .to_pyarray_bound(py)
     }
 
     #[getter]
     fn min_dt(&self) -> f64 {
         self.dmdt_f64.dmdt.dt_grid.get_start()
     }
 
     #[getter]
     fn max_dt(&self) -> f64 {
         self.dmdt_f64.dmdt.dt_grid.get_end()
     }
 
     #[getter]
-    fn dm_grid<'py>(&self, py: Python<'py>) -> &'py PyArray1<f64> {
-        self.dmdt_f64.dmdt.dm_grid.get_borders().to_pyarray(py)
+    fn dm_grid<'py>(&self, py: Python<'py>) -> Bound<'py, PyArray1<f64>> {
+        self.dmdt_f64
+            .dmdt
+            .dm_grid
+            .get_borders()
+            .to_pyarray_bound(py)
     }
 
     #[getter]
     fn min_dm(&self) -> f64 {
         self.dmdt_f64.dmdt.dm_grid.get_start()
     }
 
@@ -1101,15 +1127,20 @@
     /// sorted : bool or None, optional
     ///     `True` guarantees that `t` is sorted
     ///
     /// Returns
     /// 1d-array of float
     ///
     #[pyo3(signature=(t, *, sorted=None))]
-    fn count_dt(&self, py: Python, t: &PyAny, sorted: Option<bool>) -> Res<PyObject> {
+    fn count_dt<'py>(
+        &self,
+        py: Python<'py>,
+        t: Bound<'py, PyAny>,
+        sorted: Option<bool>,
+    ) -> Res<Bound<'py, PyUntypedArray>> {
         dtype_dispatch!(
             |t| self.dmdt_f32.py_count_dt(py, t, sorted),
             |t| self.dmdt_f64.py_count_dt(py, t, sorted),
             t
         )
     }
 
@@ -1125,15 +1156,20 @@
     /// sorted : bool or None, optional
     ///     `True` guarantees that `t` is sorted
     ///
     /// Returns
     /// 1d-array of float
     ///
     #[pyo3(signature = (t_, sorted=None))]
-    fn count_dt_many(&self, py: Python, t_: Vec<&PyAny>, sorted: Option<bool>) -> Res<PyObject> {
+    fn count_dt_many<'py>(
+        &self,
+        py: Python<'py>,
+        t_: Vec<Bound<'py, PyAny>>,
+        sorted: Option<bool>,
+    ) -> Res<Bound<'py, PyUntypedArray>> {
         if t_.is_empty() {
             Err(Exception::ValueError("t_ is empty".to_owned()))
         } else {
             dtype_dispatch!(
                 |_first_t| self.dmdt_f32.py_count_dt_many(py, t_, sorted),
                 |_first_t| self.dmdt_f64.py_count_dt_many(py, t_, sorted),
                 t_[0]
@@ -1153,15 +1189,21 @@
     ///     `True` guarantees that the light curve is sorted
     ///
     /// Returns
     /// -------
     /// 2d-ndarray of float
     ///
     #[pyo3(signature = (t, m, *, sorted=None))]
-    fn points(&self, py: Python, t: &PyAny, m: &PyAny, sorted: Option<bool>) -> Res<PyObject> {
+    fn points<'py>(
+        &self,
+        py: Python<'py>,
+        t: Bound<'py, PyAny>,
+        m: Bound<'py, PyAny>,
+        sorted: Option<bool>,
+    ) -> Res<Bound<'py, PyUntypedArray>> {
         dtype_dispatch!(
             |t, m| self.dmdt_f32.py_points(py, t, m, sorted),
             |t, m| self.dmdt_f64.py_points(py, t, m, sorted),
             t,
             =m
         )
     }
@@ -1179,20 +1221,20 @@
     ///     `True` guarantees that all light curves is sorted
     ///
     /// Returns
     /// -------
     /// 3d-ndarray of float
     ///
     #[pyo3(signature = (lcs, *, sorted=None))]
-    fn points_many(
+    fn points_many<'py>(
         &self,
-        py: Python,
-        lcs: Vec<(&PyAny, &PyAny)>,
+        py: Python<'py>,
+        lcs: Vec<(Bound<'py, PyAny>, Bound<'py, PyAny>)>,
         sorted: Option<bool>,
-    ) -> Res<PyObject> {
+    ) -> Res<Bound<'py, PyUntypedArray>> {
         if lcs.is_empty() {
             Err(Exception::ValueError("lcs is empty".to_owned()))
         } else {
             dtype_dispatch!(
                 |_first_t| self.dmdt_f32.py_points_many(py, lcs, sorted),
                 |_first_t| self.dmdt_f64.py_points_many(py, lcs, sorted),
                 lcs[0].0
@@ -1248,53 +1290,59 @@
             yield_index=false,
             shuffle=false,
             drop_nobs=DropNObsType::Int(0),
             random_seed=None,
         ),
         text_signature = "(lcs, *, sorted=None, batch_size=1, yield_index=False, shuffle=False, drop_nobs=0, random_seed=None)",
     )]
-    fn points_batches(
+    fn points_batches<'py>(
         &self,
-        py: Python,
-        lcs: Vec<(&PyAny, &PyAny)>,
+        py: Python<'py>,
+        lcs: Vec<(Bound<'py, PyAny>, Bound<'py, PyAny>)>,
         sorted: Option<bool>,
         batch_size: usize,
         yield_index: bool,
         shuffle: bool,
         drop_nobs: DropNObsType,
         random_seed: Option<u64>,
-    ) -> Res<PyObject> {
+    ) -> Res<Bound<'py, PyAny>> {
         if lcs.is_empty() {
             Err(Exception::ValueError("lcs is empty".to_owned()))
         } else {
             dtype_dispatch!(
-                |_first_t| Ok(DmDtPointsBatchesF32 {
-                    dmdt_batches: Arc::new(self.dmdt_f32.generic_dmdt_points_batches(
-                        lcs,
-                        sorted,
-                        batch_size,
-                        yield_index,
-                        shuffle,
-                        drop_nobs,
-                        random_seed,
-                    )?),
-                }
-                .into_py(py)),
-                |_first_t| Ok(DmDtPointsBatchesF64 {
-                    dmdt_batches: Arc::new(self.dmdt_f64.generic_dmdt_points_batches(
-                        lcs,
-                        sorted,
-                        batch_size,
-                        yield_index,
-                        shuffle,
-                        drop_nobs,
-                        random_seed,
-                    )?),
-                }
-                .into_py(py)),
+                |_first_t| Ok(Bound::new(
+                    py,
+                    DmDtPointsBatchesF32 {
+                        dmdt_batches: Arc::new(self.dmdt_f32.generic_dmdt_points_batches(
+                            lcs,
+                            sorted,
+                            batch_size,
+                            yield_index,
+                            shuffle,
+                            drop_nobs,
+                            random_seed,
+                        )?),
+                    }
+                )?
+                .into_any()),
+                |_first_t| Ok(Bound::new(
+                    py,
+                    DmDtPointsBatchesF64 {
+                        dmdt_batches: Arc::new(self.dmdt_f64.generic_dmdt_points_batches(
+                            lcs,
+                            sorted,
+                            batch_size,
+                            yield_index,
+                            shuffle,
+                            drop_nobs,
+                            random_seed,
+                        )?),
+                    }
+                )?
+                .into_any()),
                 lcs[0].0
             )
         }
     }
 
     /// Produces smeared dmdt-map from light curve
     ///
@@ -1310,22 +1358,22 @@
     ///     `True` guarantees that the light curve is sorted
     ///
     /// Returns
     /// -------
     /// 2d-array of float
     ///
     #[pyo3(signature = (t, m, sigma, *, sorted=None))]
-    fn gausses(
+    fn gausses<'py>(
         &self,
-        py: Python,
-        t: &PyAny,
-        m: &PyAny,
-        sigma: &PyAny,
+        py: Python<'py>,
+        t: Bound<'py, PyAny>,
+        m: Bound<'py, PyAny>,
+        sigma: Bound<'py, PyAny>,
         sorted: Option<bool>,
-    ) -> Res<PyObject> {
+    ) -> Res<Bound<'py, PyUntypedArray>> {
         dtype_dispatch!(
             |t, m, sigma| self.dmdt_f32.py_gausses(py, t, m, sigma, sorted),
             |t, m, sigma| self.dmdt_f64.py_gausses(py, t, m, sigma, sorted),
             t,
             =m,
             =sigma
         )
@@ -1344,20 +1392,20 @@
     ///     `True` guarantees that all light curves are sorted
     ///
     /// Returns
     /// -------
     /// 3d-ndarray of float
     ///
     #[pyo3(signature = (lcs, *, sorted=None))]
-    fn gausses_many(
+    fn gausses_many<'py>(
         &self,
-        py: Python,
-        lcs: Vec<(&PyAny, &PyAny, &PyAny)>,
+        py: Python<'py>,
+        lcs: Vec<(Bound<'py, PyAny>, Bound<'py, PyAny>, Bound<'py, PyAny>)>,
         sorted: Option<bool>,
-    ) -> Res<PyObject> {
+    ) -> Res<Bound<'py, PyUntypedArray>> {
         if lcs.is_empty() {
             Err(Exception::ValueError("lcs is empty".to_owned()))
         } else {
             dtype_dispatch!(
                 |_first_t| self.dmdt_f32.py_gausses_many(py, lcs, sorted),
                 |_first_t| self.dmdt_f64.py_gausses_many(py, lcs, sorted),
                 lcs[0].0
@@ -1409,89 +1457,98 @@
             yield_index=false,
             shuffle=false,
             drop_nobs=DropNObsType::Int(0),
             random_seed=None,
         ),
         text_signature = "($self, lcs, *, sorted=None, batch_size=1, yield_index=False, shuffle=False, drop_nobs=0, random_seed=None)"
     )]
-    fn gausses_batches(
+    fn gausses_batches<'py>(
         &self,
-        py: Python,
-        lcs: Vec<(&PyAny, &PyAny, &PyAny)>,
+        py: Python<'py>,
+        lcs: Vec<(Bound<'py, PyAny>, Bound<'py, PyAny>, Bound<'py, PyAny>)>,
         sorted: Option<bool>,
         batch_size: usize,
         yield_index: bool,
         shuffle: bool,
         drop_nobs: DropNObsType,
         random_seed: Option<u64>,
-    ) -> Res<PyObject> {
+    ) -> Res<Bound<'py, PyAny>> {
         if lcs.is_empty() {
             Err(Exception::ValueError("lcs is empty".to_owned()))
         } else {
             dtype_dispatch!(
-                |_first_t| Ok(DmDtGaussesBatchesF32 {
-                    dmdt_batches: Arc::new(self.dmdt_f32.generic_dmdt_gausses_batches(
-                        lcs,
-                        sorted,
-                        batch_size,
-                        yield_index,
-                        shuffle,
-                        drop_nobs,
-                        random_seed,
-                    )?),
-                }
-                .into_py(py)),
-                |_first_t| Ok(DmDtGaussesBatchesF64 {
-                    dmdt_batches: Arc::new(self.dmdt_f64.generic_dmdt_gausses_batches(
-                        lcs,
-                        sorted,
-                        batch_size,
-                        yield_index,
-                        shuffle,
-                        drop_nobs,
-                        random_seed,
-                    )?),
-                }
-                .into_py(py)),
+                |_first_t| Ok(Bound::new(
+                    py,
+                    DmDtGaussesBatchesF32 {
+                        dmdt_batches: Arc::new(self.dmdt_f32.generic_dmdt_gausses_batches(
+                            lcs,
+                            sorted,
+                            batch_size,
+                            yield_index,
+                            shuffle,
+                            drop_nobs,
+                            random_seed,
+                        )?),
+                    }
+                )?
+                .into_any()),
+                |_first_t| Ok(Bound::new(
+                    py,
+                    DmDtGaussesBatchesF64 {
+                        dmdt_batches: Arc::new(self.dmdt_f64.generic_dmdt_gausses_batches(
+                            lcs,
+                            sorted,
+                            batch_size,
+                            yield_index,
+                            shuffle,
+                            drop_nobs,
+                            random_seed,
+                        )?),
+                    }
+                )?
+                .into_any()),
                 lcs[0].0
             )
         }
     }
 
     /// Used by pickle.load / pickle.loads
-    fn __setstate__(&mut self, state: &PyBytes) -> Res<()> {
+    fn __setstate__(&mut self, state: Bound<PyBytes>) -> Res<()> {
         *self = serde_pickle::from_slice(state.as_bytes(), serde_pickle::DeOptions::new())
             .map_err(|err| {
                 Exception::UnpicklingError(format!(
                     r#"Error happened on the Rust side when deserializing DmDt: "{err}""#
                 ))
             })?;
         Ok(())
     }
 
     /// Used by pickle.dump / pickle.dumps
-    fn __getstate__<'py>(&self, py: Python<'py>) -> Res<&'py PyBytes> {
+    fn __getstate__<'py>(&self, py: Python<'py>) -> Res<Bound<'py, PyBytes>> {
         let vec_bytes =
             serde_pickle::to_vec(&self, serde_pickle::SerOptions::new()).map_err(|err| {
                 Exception::PicklingError(format!(
                     r#"Error happened on the Rust side when serializing DmDt: "{err}""#
                 ))
             })?;
-        Ok(PyBytes::new(py, &vec_bytes))
+        Ok(PyBytes::new_bound(py, &vec_bytes))
     }
 
     /// Used by pickle.dump / pickle.dumps
-    fn __getnewargs__<'py>(&self, py: Python<'py>) -> (&'py PyArray1<f64>, &'py PyArray1<f64>) {
-        let a = ndarray::array![1.0, 2.0].to_pyarray(py);
-        (a, a)
+    fn __getnewargs__<'py>(
+        &self,
+        py: Python<'py>,
+    ) -> (Bound<'py, PyArray1<f64>>, Bound<'py, PyArray1<f64>>) {
+        let a = ndarray::array![1.0, 2.0].to_pyarray_bound(py);
+        (a.clone(), a)
     }
 
     /// Used by copy.copy
     fn __copy__(&self) -> Self {
         self.clone()
     }
 
     /// Used by copy.deepcopy
-    fn __deepcopy__(&self, _memo: &PyAny) -> Self {
+    fn __deepcopy__(&self, _memo: Bound<PyAny>) -> Self {
         self.clone()
     }
 }
```

### Comparing `light_curve-0.9.0/src/errors.rs` & `light_curve-0.9.1/src/errors.rs`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/src/features.rs` & `light_curve-0.9.1/src/features.rs`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 use const_format::formatcp;
 use conv::ConvUtil;
 use itertools::Itertools;
 use light_curve_feature::{self as lcf, prelude::*, DataSample};
 use macro_const::macro_const;
 use ndarray::IntoNdProducer;
-use numpy::{IntoPyArray, PyArray1};
+use numpy::prelude::*;
+use numpy::{PyArray1, PyUntypedArray};
 use once_cell::sync::OnceCell;
 use pyo3::exceptions::{PyNotImplementedError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::{PyBool, PyBytes, PyTuple};
 use rayon::prelude::*;
 use serde::{Deserialize, Serialize};
 use std::collections::HashMap;
@@ -29,14 +30,20 @@
 // __new__ is called. Thus we implement __getnewargs__ (or __getnewargs_ex__ when constructor has
 // keyword-only arguments) for such classes. Despite the "standard" way we return some default
 // arguments from this method and de-facto re-create the underlying Rust objects during
 // __setstate__, which could reduce performance of deserialising. We also make this method static
 // to use it in tests, which is also a bit weird thing to do. We use pickle as a serialization
 // format for it, so all Rust object internals can be inspected from Python.
 
+type PyLcs<'py> = Vec<(
+    Bound<'py, PyAny>,
+    Bound<'py, PyAny>,
+    Option<Bound<'py, PyAny>>,
+)>;
+
 const ATTRIBUTES_DOC: &str = r#"Attributes
 ----------
 names : list of str
     Feature names
 descriptions : list of str
     Feature descriptions"#;
 
@@ -175,15 +182,15 @@
                 .into(),
         })
     }
 
     fn with_py_transform(
         fe_f32: lcf::Feature<f32>,
         fe_f64: lcf::Feature<f64>,
-        transform: Option<&PyAny>,
+        transform: Option<Bound<PyAny>>,
         default_transformer: StockTransformer,
     ) -> Res<Self> {
         let transform = parse_transform(transform, default_transformer)?;
         match transform {
             Some(transform) => Self::with_transform((fe_f32, fe_f64), transform.into()),
             None => Ok(Self {
                 feature_evaluator_f32: fe_f32,
@@ -274,25 +281,25 @@
             None => lcf::TimeSeries::new_without_weight(t, m),
         };
 
         Ok(ts)
     }
 
     #[allow(clippy::too_many_arguments)]
-    fn call_impl<T>(
+    fn call_impl<'py, T>(
         feature_evaluator: &lcf::Feature<T>,
-        py: Python,
-        t: Arr<T>,
-        m: Arr<T>,
-        sigma: Option<Arr<T>>,
+        py: Python<'py>,
+        t: Arr<'py, T>,
+        m: Arr<'py, T>,
+        sigma: Option<Arr<'py, T>>,
         sorted: Option<bool>,
         check: bool,
         is_t_required: bool,
         fill_value: Option<T>,
-    ) -> Res<PyObject>
+    ) -> Res<Bound<'py, PyUntypedArray>>
     where
         T: lcf::Float + numpy::Element,
     {
         let mut ts = Self::ts_from_numpy(
             feature_evaluator,
             &t,
             &m,
@@ -304,41 +311,42 @@
 
         let result = match fill_value {
             Some(x) => feature_evaluator.eval_or_fill(&mut ts, x),
             None => feature_evaluator
                 .eval(&mut ts)
                 .map_err(|e| Exception::ValueError(e.to_string()))?,
         };
-        let array = PyArray1::from_vec(py, result);
-        Ok(array.into_py(py))
+        let array = PyArray1::from_vec_bound(py, result);
+        Ok(array.as_untyped().clone())
     }
 
     #[allow(clippy::too_many_arguments)]
-    fn py_many<'a, T>(
+    fn py_many<'py, T>(
         &self,
         feature_evaluator: &lcf::Feature<T>,
-        py: Python,
-        lcs: Vec<(&'a PyAny, &'a PyAny, Option<&'a PyAny>)>,
+        py: Python<'py>,
+        lcs: PyLcs<'py>,
         sorted: Option<bool>,
         check: bool,
         fill_value: Option<T>,
         n_jobs: i64,
-    ) -> Res<PyObject>
+    ) -> Res<Bound<'py, PyUntypedArray>>
     where
         T: lcf::Float + numpy::Element,
     {
         let wrapped_lcs = lcs
             .into_iter()
             .enumerate()
             .map(|(i, (t, m, sigma))| {
                 let t = t.downcast::<PyArray1<T>>().map(|a| a.readonly());
                 let m = m.downcast::<PyArray1<T>>().map(|a| a.readonly());
-                let sigma = sigma
-                    .map(|a| a.downcast::<PyArray1<T>>().map(|a| a.readonly()))
-                    .transpose();
+                let sigma = match &sigma {
+                    Some(sigma) => sigma.downcast::<PyArray1<T>>().map(|a| Some(a.readonly())),
+                    None => Ok(None),
+                };
 
                 match (t, m, sigma) {
                     (Ok(t), Ok(m), Ok(sigma)) => Ok((t, m, sigma)),
                     _ => Err(Exception::TypeError(format!(
                         "lcs[{}] elements have mismatched dtype with the lc[0][0] which is {}",
                         i,
                         std::any::type_name::<T>()
@@ -351,16 +359,17 @@
             wrapped_lcs,
             sorted,
             check,
             self.is_t_required(sorted),
             fill_value,
             n_jobs,
         )?
-        .into_pyarray(py)
-        .into_py(py))
+        .into_pyarray_bound(py)
+        .as_untyped()
+        .clone())
     }
 
     fn many_impl<T>(
         feature_evaluator: &lcf::Feature<T>,
         lcs: Vec<PyLightCurve<T>>,
         sorted: Option<bool>,
         check: bool,
@@ -431,24 +440,24 @@
         m,
         sigma = None,
         *,
         sorted = None,
         check = true,
         fill_value = None
     ))]
-    fn __call__(
+    fn __call__<'py>(
         &self,
-        py: Python,
-        t: &PyAny,
-        m: &PyAny,
-        sigma: Option<&PyAny>,
+        py: Python<'py>,
+        t: Bound<'py, PyAny>,
+        m: Bound<'py, PyAny>,
+        sigma: Option<Bound<'py, PyAny>>,
         sorted: Option<bool>,
         check: bool,
         fill_value: Option<f64>,
-    ) -> Res<PyObject> {
+    ) -> Res<Bound<'py, PyUntypedArray>> {
         if let Some(sigma) = sigma {
             dtype_dispatch!(
                 |t, m, sigma| {
                     Self::call_impl(
                         &self.feature_evaluator_f32,
                         py,
                         t,
@@ -509,23 +518,23 @@
                 =m,
             )
         }
     }
 
     #[doc = METHOD_MANY_DOC!()]
     #[pyo3(signature = (lcs, *, sorted=None, check=true, fill_value=None, n_jobs=-1))]
-    fn many(
+    fn many<'py>(
         &self,
-        py: Python,
-        lcs: Vec<(&PyAny, &PyAny, Option<&PyAny>)>,
+        py: Python<'py>,
+        lcs: PyLcs<'py>,
         sorted: Option<bool>,
         check: bool,
         fill_value: Option<f64>,
         n_jobs: i64,
-    ) -> Res<PyObject> {
+    ) -> Res<Bound<'py, PyUntypedArray>> {
         if lcs.is_empty() {
             Err(Exception::ValueError("lcs is empty".to_string()))
         } else {
             dtype_dispatch!(
                 |_first_t| {
                     self.py_many(
                         &self.feature_evaluator_f32,
@@ -567,67 +576,66 @@
     /// Feature descriptions
     #[getter]
     fn descriptions(&self) -> Vec<&str> {
         self.feature_evaluator_f64.get_descriptions()
     }
 
     /// Used by pickle.load / pickle.loads
-    fn __setstate__(&mut self, state: &PyBytes) -> Res<()> {
+    fn __setstate__(&mut self, state: Bound<PyBytes>) -> Res<()> {
         *self = serde_pickle::from_slice(state.as_bytes(), serde_pickle::DeOptions::new())
             .map_err(|err| {
                 Exception::UnpicklingError(format!(
                     r#"Error happened on the Rust side when deserializing _FeatureEvaluator: "{err}""#
                 ))
             })?;
         Ok(())
     }
 
     /// Used by pickle.dump / pickle.dumps
-    fn __getstate__<'py>(&self, py: Python<'py>) -> Res<&'py PyBytes> {
+    fn __getstate__<'py>(&self, py: Python<'py>) -> Res<Bound<'py, PyBytes>> {
         let vec_bytes =
             serde_pickle::to_vec(&self, serde_pickle::SerOptions::new()).map_err(|err| {
                 Exception::PicklingError(format!(
                     r#"Error happened on the Rust side when serializing _FeatureEvaluator: "{err}""#
                 ))
             })?;
-        Ok(PyBytes::new(py, &vec_bytes))
+        Ok(PyBytes::new_bound(py, &vec_bytes))
     }
 
     /// Used by copy.copy
     fn __copy__(&self) -> Self {
         self.clone()
     }
 
     /// Used by copy.deepcopy
-    fn __deepcopy__(&self, _memo: &PyAny) -> Self {
+    fn __deepcopy__(&self, _memo: Bound<PyAny>) -> Self {
         self.clone()
     }
 }
 
 #[pyclass(extends = PyFeatureEvaluator, module="light_curve.light_curve_ext")]
 pub struct Extractor {}
 
 #[pymethods]
 impl Extractor {
     #[new]
     #[pyo3(signature = (*features, transform=None))]
     fn __new__(
-        features: &PyTuple,
-        transform: Option<&PyAny>,
+        features: Bound<PyTuple>,
+        transform: Option<Bound<PyAny>>,
     ) -> PyResult<(Self, PyFeatureEvaluator)> {
         if transform.is_some() {
             return Err(Exception::NotImplementedError(
                 "transform is not implemented for Extractor, transform individual features instead"
                     .to_string(),
             )
             .into());
         }
-        let evals_iter = features.iter().map(|arg| {
-            arg.downcast::<PyCell<PyFeatureEvaluator>>().map(|fe| {
-                let fe = fe.borrow();
+        let evals_iter = features.iter_borrowed().map(|arg| {
+            arg.extract::<PyFeatureEvaluator>().map(|fe| {
                 (
                     fe.feature_evaluator_f32.clone(),
                     fe.feature_evaluator_f64.clone(),
                 )
             })
         });
         let (evals_f32, evals_f64) =
@@ -690,15 +698,15 @@
 
         impl_stock_transform!($name, $default_transform);
 
         #[pymethods]
         impl $name {
             #[new]
             #[pyo3(signature=(*, transform=None))]
-            fn __new__(transform: Option<&PyAny>) -> Res<PyClassInitializer<Self>> {
+            fn __new__(transform: Option<Bound<PyAny>>) -> Res<PyClassInitializer<Self>> {
                 let base = PyFeatureEvaluator::with_py_transform(
                     <$eval>::new().into(),
                     <$eval>::new().into(),
                     transform,
                     Self::DEFAULT_TRANSFORMER,
                 )?;
                 Ok(PyClassInitializer::from(base).add_subclass(Self {}))
@@ -816,33 +824,33 @@
             where
                 T: lcf::Float + numpy::Element,
             {
                 let params = ContCowArray::from_view(params.as_array(), true);
                 t.as_array().mapv(|x| <$eval>::f(x, params.as_slice()))
             }
 
-            fn default_lmsder_iterations() -> u16 {
+            fn default_lmsder_iterations() -> Option<u16> {
                 #[cfg(feature = "gsl")]
                 {
-                    lcf::LmsderCurveFit::default_niterations()
+                    lcf::LmsderCurveFit::default_niterations().into()
                 }
                 #[cfg(not(feature = "gsl"))]
                 {
-                    0
+                    None
                 }
             }
 
-            fn default_ceres_iterations() -> u16 {
+            fn default_ceres_iterations() -> Option<u16> {
                 #[cfg(any(feature = "ceres-source", feature = "ceres-system"))]
                 {
-                    lcf::CeresCurveFit::default_niterations()
+                    lcf::CeresCurveFit::default_niterations().into()
                 }
                 #[cfg(not(any(feature = "ceres-source", feature = "ceres-system")))]
                 {
-                    0
+                    None
                 }
             }
         }
 
         #[allow(clippy::too_many_arguments)]
         #[pymethods]
         impl $name {
@@ -858,43 +866,47 @@
                 bounds = None,
                 ln_prior = None,
                 transform = None,
             ))]
             fn __new__(
                 algorithm: &str,
                 mcmc_niter: Option<u32>,
-                lmsder_niter: Option<u16>,
-                ceres_niter: Option<u16>,
+                // The first Option is for Python's None, the second is for compile-time None from
+                // Self::default_lmsder_iterations()
+                lmsder_niter: Option<Option<u16>>,
+                // The first Option is for Python's None, the second is for compile-time None from
+                // Self::default_ceres_iterations()
+                ceres_niter: Option<Option<u16>>,
                 ceres_loss_reg: Option<f64>,
                 init: Option<Vec<Option<f64>>>,
                 bounds: Option<Vec<(Option<f64>, Option<f64>)>>,
                 ln_prior: Option<FitLnPrior<'_>>,
-                transform: Option<&PyAny>,
+                transform: Option<Bound<PyAny>>,
             ) -> PyResult<(Self, PyFeatureEvaluator)> {
                 let mcmc_niter = mcmc_niter.unwrap_or_else(lcf::McmcCurveFit::default_niterations);
 
                 #[cfg(feature = "gsl")]
                 let lmsder_fit: lcf::CurveFitAlgorithm = lcf::LmsderCurveFit::new(
-                    lmsder_niter.unwrap_or_else(lcf::LmsderCurveFit::default_niterations),
+                    lmsder_niter.unwrap_or_else(Self::default_lmsder_iterations).expect("logical error: default lmsder_niter is None but GSL is enabled"),
                 )
                 .into();
                 #[cfg(not(feature = "gsl"))]
-                if lmsder_niter.is_some() {
+                if lmsder_niter.flatten().is_some() {
                     return Err(PyValueError::new_err(
                         "Compiled without GSL support, lmsder_niter is not supported",
                     ));
                 }
 
                 #[cfg(any(feature = "ceres-source", feature = "ceres-system"))]
                 let ceres_fit: lcf::CurveFitAlgorithm = lcf::CeresCurveFit::new(
-                    ceres_niter.unwrap_or_else(lcf::CeresCurveFit::default_niterations),
+                    ceres_niter.unwrap_or_else(Self::default_ceres_iterations).expect("logical error: default ceres_niter is None but Ceres is enabled"),
                     ceres_loss_reg.or_else(lcf::CeresCurveFit::default_loss_factor),
                 ).into();
                 #[cfg(not(any(feature = "ceres-source", feature = "ceres-system")))]
-                if ceres_niter.is_some() || ceres_loss_reg.is_some() {
+                if ceres_niter.flatten().is_some() || ceres_loss_reg.is_some() {
                     return Err(PyValueError::new_err(
                         "Compiled without Ceres support, ceres_niter and ceres_loss_reg are not supported",
                     ));
                 }
 
                 let init_bounds = match (init, bounds) {
                     (Some(init), Some(bounds)) => Some((init, bounds)),
@@ -999,21 +1011,21 @@
             #[staticmethod]
             fn __getnewargs__() -> (&'static str,) {
                 ("mcmc",)
             }
 
             #[doc = FIT_METHOD_MODEL_DOC!()]
             #[staticmethod]
-            fn model(
-                py: Python,
-                t: &PyAny,
-                params: &PyAny,
-            ) -> Res<PyObject> {
+            fn model<'py>(
+                py: Python<'py>,
+                t: Bound<'py, PyAny>,
+                params: Bound<'py, PyAny>,
+            ) -> Res<Bound<'py, PyUntypedArray>> {
                 dtype_dispatch!({
-                    |t, params| Ok(Self::model_impl(t, params).into_pyarray(py).into_py(py))
+                    |t, params| Ok(Self::model_impl(t, params).into_pyarray_bound(py).as_untyped().clone())
                 }(t, !=params))
             }
 
             #[classattr]
             fn supported_algorithms() -> [&'static str; N_ALGO_CURVE_FIT] {
                 return SUPPORTED_ALGORITHMS_CURVE_FIT;
             }
@@ -1138,15 +1150,15 @@
 
 impl_stock_transform!(BeyondNStd, StockTransformer::Identity);
 
 #[pymethods]
 impl BeyondNStd {
     #[new]
     #[pyo3(signature = (nstd=lcf::BeyondNStd::default_nstd(), *, transform=None))]
-    fn __new__(nstd: f64, transform: Option<&PyAny>) -> Res<PyClassInitializer<Self>> {
+    fn __new__(nstd: f64, transform: Option<Bound<PyAny>>) -> Res<PyClassInitializer<Self>> {
         Ok(
             PyClassInitializer::from(PyFeatureEvaluator::with_py_transform(
                 lcf::BeyondNStd::new(nstd as f32).into(),
                 lcf::BeyondNStd::new(nstd).into(),
                 transform,
                 Self::DEFAULT_TRANSFORMER,
             )?)
@@ -1198,31 +1210,30 @@
 pub struct Bins {}
 
 #[pymethods]
 impl Bins {
     #[new]
     #[pyo3(signature = (features, *, window, offset, transform = None))]
     fn __new__(
-        py: Python,
-        features: PyObject,
+        features: Bound<PyAny>,
         window: f64,
         offset: f64,
-        transform: Option<&PyAny>,
+        transform: Option<Bound<PyAny>>,
     ) -> PyResult<(Self, PyFeatureEvaluator)> {
         if transform.is_some() {
             return Err(Exception::NotImplementedError(
                 "transform is not supported by Bins, apply transformations to individual features"
                     .to_string(),
             )
             .into());
         }
         let mut eval_f32 = lcf::Bins::default();
         let mut eval_f64 = lcf::Bins::default();
-        for x in features.extract::<&PyAny>(py)?.iter()? {
-            let py_feature = x?.downcast::<PyCell<PyFeatureEvaluator>>()?.borrow();
+        for x in features.iter()? {
+            let py_feature = x?.downcast::<PyFeatureEvaluator>()?.borrow();
             eval_f32.add_feature(py_feature.feature_evaluator_f32.clone());
             eval_f64.add_feature(py_feature.feature_evaluator_f64.clone());
         }
 
         eval_f32.set_window(window as f32);
         eval_f64.set_window(window);
 
@@ -1244,17 +1255,17 @@
         Err(PyNotImplementedError::new_err(
             "use __getnewargs_ex__ instead",
         ))
     }
 
     /// Required by pickle.load / pickle.loads
     #[staticmethod]
-    fn __getnewargs_ex__(py: Python) -> ((&PyTuple,), HashMap<&'static str, f64>) {
+    fn __getnewargs_ex__(py: Python) -> ((Bound<PyTuple>,), HashMap<&'static str, f64>) {
         (
-            (PyTuple::empty(py),),
+            (PyTuple::empty_bound(py),),
             [
                 ("window", lcf::Bins::<_, Feature<_>>::default_window()),
                 ("offset", lcf::Bins::<_, Feature<_>>::default_offset()),
             ]
             .into(),
         )
     }
@@ -1299,15 +1310,15 @@
 
 impl_stock_transform!(InterPercentileRange, StockTransformer::Identity);
 
 #[pymethods]
 impl InterPercentileRange {
     #[new]
     #[pyo3(signature = (quantile=lcf::InterPercentileRange::default_quantile(), *, transform = None))]
-    fn __new__(quantile: f32, transform: Option<&PyAny>) -> Res<PyClassInitializer<Self>> {
+    fn __new__(quantile: f32, transform: Option<Bound<PyAny>>) -> Res<PyClassInitializer<Self>> {
         Ok(
             PyClassInitializer::from(PyFeatureEvaluator::with_py_transform(
                 lcf::InterPercentileRange::new(quantile).into(),
                 lcf::InterPercentileRange::new(quantile).into(),
                 transform,
                 Self::DEFAULT_TRANSFORMER,
             )?)
@@ -1374,15 +1385,15 @@
         quantile_denominator=lcf::MagnitudePercentageRatio::default_quantile_denominator(),
         *,
         transform=None,
     ))]
     fn __new__(
         quantile_numerator: f32,
         quantile_denominator: f32,
-        transform: Option<&PyAny>,
+        transform: Option<Bound<PyAny>>,
     ) -> Res<PyClassInitializer<Self>> {
         if !(0.0..0.5).contains(&quantile_numerator) {
             return Err(Exception::ValueError(
                 "quantile_numerator must be between 0.0 and 0.5".to_string(),
             ));
         }
         if !(0.0..0.5).contains(&quantile_denominator) {
@@ -1455,15 +1466,15 @@
 
 impl_stock_transform!(MedianBufferRangePercentage, StockTransformer::Identity);
 
 #[pymethods]
 impl MedianBufferRangePercentage {
     #[new]
     #[pyo3(signature = (quantile=lcf::MedianBufferRangePercentage::<f64>::default_quantile(), *, transform = None))]
-    fn __new__(quantile: f64, transform: Option<&PyAny>) -> Res<PyClassInitializer<Self>> {
+    fn __new__(quantile: f64, transform: Option<Bound<PyAny>>) -> Res<PyClassInitializer<Self>> {
         Ok(
             PyClassInitializer::from(PyFeatureEvaluator::with_py_transform(
                 lcf::MedianBufferRangePercentage::new(quantile as f32).into(),
                 lcf::MedianBufferRangePercentage::new(quantile).into(),
                 transform,
                 Self::DEFAULT_TRANSFORMER,
             )?)
@@ -1510,15 +1521,15 @@
     StockTransformer::ClippedLg
 );
 
 #[pymethods]
 impl PercentDifferenceMagnitudePercentile {
     #[new]
     #[pyo3(signature = (quantile=lcf::PercentDifferenceMagnitudePercentile::default_quantile(), *, transform = None))]
-    fn __new__(quantile: f32, transform: Option<&PyAny>) -> Res<PyClassInitializer<Self>> {
+    fn __new__(quantile: f32, transform: Option<Bound<PyAny>>) -> Res<PyClassInitializer<Self>> {
         if !(0.0..0.5).contains(&quantile) {
             return Err(Exception::ValueError(
                 "quantile must be between 0.0 and 0.5".to_string(),
             ));
         }
         Ok(
             PyClassInitializer::from(PyFeatureEvaluator::with_py_transform(
@@ -1568,21 +1579,20 @@
 pub struct Periodogram {
     eval_f32: LcfPeriodogram<f32>,
     eval_f64: LcfPeriodogram<f64>,
 }
 
 impl Periodogram {
     fn create_evals(
-        py: Python,
         peaks: Option<usize>,
         resolution: Option<f32>,
         max_freq_factor: Option<f32>,
         nyquist: Option<NyquistArgumentOfPeriodogram>,
         fast: Option<bool>,
-        features: Option<PyObject>,
+        features: Option<Bound<PyAny>>,
     ) -> PyResult<(LcfPeriodogram<f32>, LcfPeriodogram<f64>)> {
         let mut eval_f32 = match peaks {
             Some(peaks) => lcf::Periodogram::new(peaks),
             None => lcf::Periodogram::default(),
         };
         let mut eval_f64 = match peaks {
             Some(peaks) => lcf::Periodogram::new(peaks),
@@ -1620,39 +1630,39 @@
                 eval_f64.set_periodogram_algorithm(lcf::PeriodogramPowerFft::new().into());
             } else {
                 eval_f32.set_periodogram_algorithm(lcf::PeriodogramPowerDirect {}.into());
                 eval_f64.set_periodogram_algorithm(lcf::PeriodogramPowerDirect {}.into());
             }
         }
         if let Some(features) = features {
-            for x in features.extract::<&PyAny>(py)?.iter()? {
-                let py_feature = x?.downcast::<PyCell<PyFeatureEvaluator>>()?.borrow();
+            for x in features.iter()? {
+                let py_feature = x?.downcast::<PyFeatureEvaluator>()?.borrow();
                 eval_f32.add_feature(py_feature.feature_evaluator_f32.clone());
                 eval_f64.add_feature(py_feature.feature_evaluator_f64.clone());
             }
         }
         Ok((eval_f32, eval_f64))
     }
 
-    fn freq_power_impl<T>(
+    fn freq_power_impl<'py, T>(
         eval: &lcf::Periodogram<T, lcf::Feature<T>>,
-        py: Python,
+        py: Python<'py>,
         t: Arr<T>,
         m: Arr<T>,
-    ) -> (PyObject, PyObject)
+    ) -> (Bound<'py, PyUntypedArray>, Bound<'py, PyUntypedArray>)
     where
         T: lcf::Float + numpy::Element,
     {
         let t: DataSample<_> = t.as_array().into();
         let m: DataSample<_> = m.as_array().into();
         let mut ts = lcf::TimeSeries::new_without_weight(t, m);
         let (freq, power) = eval.freq_power(&mut ts);
-        let freq = PyArray1::from_vec(py, freq);
-        let power = PyArray1::from_vec(py, power);
-        (freq.into_py(py), power.into_py(py))
+        let freq = PyArray1::from_vec_bound(py, freq);
+        let power = PyArray1::from_vec_bound(py, power);
+        (freq.as_untyped().clone(), power.as_untyped().clone())
     }
 }
 
 #[pymethods]
 impl Periodogram {
     #[allow(clippy::too_many_arguments)]
     #[new]
@@ -1663,51 +1673,48 @@
         max_freq_factor = LcfPeriodogram::<f64>::default_max_freq_factor(),
         nyquist = NyquistArgumentOfPeriodogram::String("average"),
         fast = true,
         features = None,
         transform = None,
     ))]
     fn __new__(
-        py: Python,
         peaks: Option<usize>,
         resolution: Option<f32>,
         max_freq_factor: Option<f32>,
         nyquist: Option<NyquistArgumentOfPeriodogram>,
         fast: Option<bool>,
-        features: Option<PyObject>,
-        transform: Option<&PyAny>,
+        features: Option<Bound<PyAny>>,
+        transform: Option<Bound<PyAny>>,
     ) -> PyResult<(Self, PyFeatureEvaluator)> {
         if transform.is_some() {
             return Err(PyNotImplementedError::new_err(
                 "transform is not supported by Periodogram, peak-related features are not transformed, but you still may apply transformation for the underlying features",
             ));
         }
-        let (eval_f32, eval_f64) = Self::create_evals(
-            py,
-            peaks,
-            resolution,
-            max_freq_factor,
-            nyquist,
-            fast,
-            features,
-        )?;
+        let (eval_f32, eval_f64) =
+            Self::create_evals(peaks, resolution, max_freq_factor, nyquist, fast, features)?;
         Ok((
             Self {
                 eval_f32: eval_f32.clone(),
                 eval_f64: eval_f64.clone(),
             },
             PyFeatureEvaluator {
                 feature_evaluator_f32: eval_f32.into(),
                 feature_evaluator_f64: eval_f64.into(),
             },
         ))
     }
 
     /// Angular frequencies and periodogram values
-    fn freq_power(&self, py: Python, t: &PyAny, m: &PyAny) -> Res<(PyObject, PyObject)> {
+    fn freq_power<'py>(
+        &self,
+        py: Python<'py>,
+        t: Bound<PyAny>,
+        m: Bound<PyAny>,
+    ) -> Res<(Bound<'py, PyUntypedArray>, Bound<'py, PyUntypedArray>)> {
         dtype_dispatch!(
             |t, m| Ok(Self::freq_power_impl(&self.eval_f32, py, t, m)),
             |t, m| Ok(Self::freq_power_impl(&self.eval_f64, py, t, m)),
             t,
             =m
         )
     }
@@ -1839,15 +1846,15 @@
 #[pyclass(extends = PyFeatureEvaluator, module="light_curve.light_curve_ext")]
 pub struct OtsuSplit {}
 
 #[pymethods]
 impl OtsuSplit {
     #[new]
     #[pyo3(signature = (*, transform=None))]
-    fn __new__(transform: Option<&PyAny>) -> Res<(Self, PyFeatureEvaluator)> {
+    fn __new__(transform: Option<Bound<PyAny>>) -> Res<(Self, PyFeatureEvaluator)> {
         if transform.is_some() {
             return Err(Exception::NotImplementedError(
                 "OtsuSplit does not support transformations yet".to_string(),
             ));
         }
         Ok((
             Self {},
@@ -1855,15 +1862,15 @@
                 feature_evaluator_f32: lcf::OtsuSplit::new().into(),
                 feature_evaluator_f64: lcf::OtsuSplit::new().into(),
             },
         ))
     }
 
     #[staticmethod]
-    fn threshold(m: &PyAny) -> Res<f64> {
+    fn threshold(m: Bound<PyAny>) -> Res<f64> {
         dtype_dispatch!({ Self::threshold_impl }(m))
     }
 
     #[classattr]
     fn __doc__() -> String {
         format!(
             "{}{}",
```

### Comparing `light_curve-0.9.0/src/lib.rs` & `light_curve-0.9.1/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ///
 /// The module provides a collection of features to be extracted from unevenly separated
 /// time-series. This module if based on Rust crates `light-curve-feature` & `light-curve-dmdt`.
 ///
 /// dm-lg(dt) maps generator is represented by `DmDt` class, while all other classes are
 /// feature extractors
 #[pymodule]
-fn light_curve(py: Python, m: &PyModule) -> PyResult<()> {
+fn light_curve(py: Python, m: Bound<PyModule>) -> PyResult<()> {
     m.add("__version__", env!("CARGO_PKG_VERSION"))?;
 
     m.add(
         "_built_with_ceres",
         cfg!(any(feature = "ceres-source", feature = "ceres-system")),
     )?;
     m.add("_built_with_gsl", cfg!(feature = "gsl"))?;
```

### Comparing `light_curve-0.9.0/src/ln_prior.rs` & `light_curve-0.9.1/src/ln_prior.rs`

 * *Files 10% similar despite different names*

```diff
@@ -18,42 +18,42 @@
 impl LnPrior1D {
     #[new]
     fn __new__() -> Self {
         Self(lcf::LnPrior1D::none())
     }
 
     /// Used by pickle.load / pickle.loads
-    fn __setstate__(&mut self, state: &PyBytes) -> Res<()> {
+    fn __setstate__(&mut self, state: Bound<PyBytes>) -> Res<()> {
         *self = serde_pickle::from_slice(state.as_bytes(), serde_pickle::DeOptions::new())
             .map_err(|err| {
                 Exception::UnpicklingError(format!(
                     r#"Error happened on the Rust side when deserializing LnPrior1D: "{err}""#
                 ))
             })?;
         Ok(())
     }
 
     /// Used by pickle.dump / pickle.dumps
-    fn __getstate__<'py>(&self, py: Python<'py>) -> Res<&'py PyBytes> {
+    fn __getstate__<'py>(&self, py: Python<'py>) -> Res<Bound<'py, PyBytes>> {
         let vec_bytes =
             serde_pickle::to_vec(&self, serde_pickle::SerOptions::new()).map_err(|err| {
                 Exception::PicklingError(format!(
                     r#"Error happened on the Rust side when serializing LnPrior1D: "{err}""#
                 ))
             })?;
-        Ok(PyBytes::new(py, &vec_bytes))
+        Ok(PyBytes::new_bound(py, &vec_bytes))
     }
 
     /// Used by copy.copy
     fn __copy__(&self) -> Self {
         self.clone()
     }
 
     /// Used by copy.deepcopy
-    fn __deepcopy__(&self, _memo: &PyAny) -> Self {
+    fn __deepcopy__(&self, _memo: Bound<PyAny>) -> Self {
         self.clone()
     }
 }
 
 /// "None" prior, its logarithm is zero
 ///
 /// Returns
@@ -144,19 +144,19 @@
     let priors = mix
         .into_iter()
         .map(|(weight, py_ln_prior)| (weight, py_ln_prior.0))
         .collect();
     LnPrior1D(lcf::LnPrior1D::mix(priors))
 }
 
-pub fn register_ln_prior_submodule(py: Python, parent_module: &PyModule) -> PyResult<()> {
-    let m = PyModule::new(py, "ln_prior")?;
+pub fn register_ln_prior_submodule(py: Python, parent_module: Bound<PyModule>) -> PyResult<()> {
+    let m = PyModule::new_bound(py, "ln_prior")?;
     m.add_class::<LnPrior1D>()?;
-    m.add_function(wrap_pyfunction!(none, m)?)?;
-    m.add_function(wrap_pyfunction!(log_normal, m)?)?;
-    m.add_function(wrap_pyfunction!(log_uniform, m)?)?;
-    m.add_function(wrap_pyfunction!(normal, m)?)?;
-    m.add_function(wrap_pyfunction!(uniform, m)?)?;
-    m.add_function(wrap_pyfunction!(mix, m)?)?;
-    parent_module.add_submodule(m)?;
+    m.add_function(wrap_pyfunction!(none, &m)?)?;
+    m.add_function(wrap_pyfunction!(log_normal, &m)?)?;
+    m.add_function(wrap_pyfunction!(log_uniform, &m)?)?;
+    m.add_function(wrap_pyfunction!(normal, &m)?)?;
+    m.add_function(wrap_pyfunction!(uniform, &m)?)?;
+    m.add_function(wrap_pyfunction!(mix, &m)?)?;
+    parent_module.add_submodule(&m)?;
     Ok(())
 }
```

### Comparing `light_curve-0.9.0/src/np_array.rs` & `light_curve-0.9.1/src/np_array.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use crate::errors::{Exception, Res};
 
+use numpy::prelude::*;
 use numpy::{Element, PyArray1, PyReadonlyArray1};
 use pyo3::prelude::*;
 
 pub(crate) type Arr<'a, T> = PyReadonlyArray1<'a, T>;
 
 pub(crate) trait DType {
     fn dtype_name() -> &'static str;
@@ -19,21 +20,21 @@
     fn dtype_name() -> &'static str {
         "float64"
     }
 }
 
 pub(crate) fn extract_matched_array<'py, T>(
     y_name: &'static str,
-    y: &'py PyAny,
+    y: Bound<'py, PyAny>,
     x_name: &'static str,
     x: &Arr<'py, T>,
     check_size: bool,
 ) -> Res<Arr<'py, T>>
 where
-    T: Element + DType,
+    T: Element + DType + 'py,
 {
     if let Ok(y) = y.downcast::<PyArray1<T>>() {
         let y = y.readonly();
         if check_size {
             if y.len() == x.len() {
                 Ok(y)
             } else {
```

### Comparing `light_curve-0.9.0/src/transform.rs` & `light_curve-0.9.1/src/transform.rs`

 * *Files 10% similar despite different names*

```diff
@@ -101,40 +101,42 @@
                 SqrtTransformer::default().into(),
             ),
         }
     }
 }
 
 pub(crate) fn parse_transform(
-    option: Option<&PyAny>,
+    option: Option<Bound<PyAny>>,
     default: StockTransformer,
 ) -> Res<Option<StockTransformer>> {
     match option {
         None => Ok(None),
         Some(py_any) => {
             if let Ok(py_bool) = py_any.downcast::<PyBool>() {
                 if py_bool.is_true() {
                     Ok(Some(default))
                 } else {
                     Ok(None)
                 }
             } else if let Ok(py_str) = py_any.downcast::<PyString>() {
-                let s = py_str.to_str()?;
+                // py_str.to_str() is Python 3.10+ only
+                let cow_string = py_str.to_cow()?;
+                let s = cow_string.as_ref();
                 if let Ok(stock_transformer) = s.try_into() {
                     Ok(Some(stock_transformer))
                 } else if s == "default" {
                     Ok(Some(default))
                 } else {
                     Err(Exception::ValueError(format!(
                         "Unknown transformation: {}",
                         s
                     )))
                 }
             } else {
                 Err(Exception::ValueError(format!(
                     "transform must be None, a bool or a str, not {}",
-                    py_any.get_type().name()?
+                    py_any.get_type().qualname()?
                 )))
             }
         }
     }
 }
```

### Comparing `light_curve-0.9.0/tests/conftest.py` & `light_curve-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_ext/test_dmdt.py` & `light_curve-0.9.1/tests/light_curve_ext/test_dmdt.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_ext/test_feature.py` & `light_curve-0.9.1/tests/light_curve_ext/test_feature.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_ext/test_ln_prior.py` & `light_curve-0.9.1/tests/light_curve_ext/test_ln_prior.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_py/features/test_beyondnstd.py` & `light_curve-0.9.1/tests/light_curve_py/features/test_beyondnstd.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_py/features/test_bins.py` & `light_curve-0.9.1/tests/light_curve_py/features/test_bins.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_py/features/test_color_of_median.py` & `light_curve-0.9.1/tests/light_curve_py/features/test_color_of_median.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_py/features/test_etae.py` & `light_curve-0.9.1/tests/light_curve_py/features/test_etae.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_py/features/test_extractor.py` & `light_curve-0.9.1/tests/light_curve_py/features/test_extractor.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_py/features/test_linfit.py` & `light_curve-0.9.1/tests/light_curve_py/features/test_linfit.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_py/features/test_lintrend.py` & `light_curve-0.9.1/tests/light_curve_py/features/test_lintrend.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_py/features/test_magnpratio.py` & `light_curve-0.9.1/tests/light_curve_py/features/test_magnpratio.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_py/features/test_n_not_det_before_fd.py` & `light_curve-0.9.1/tests/light_curve_py/features/test_n_not_det_before_fd.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_py/features/test_otsusplit.py` & `light_curve-0.9.1/tests/light_curve_py/features/test_otsusplit.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_py/features/test_rainbow.py` & `light_curve-0.9.1/tests/light_curve_py/features/test_rainbow.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_py/features/test_redchi2.py` & `light_curve-0.9.1/tests/light_curve_py/features/test_redchi2.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_py/features/test_roms.py` & `light_curve-0.9.1/tests/light_curve_py/features/test_roms.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_py/features/test_stetsonk.py` & `light_curve-0.9.1/tests/light_curve_py/features/test_stetsonk.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_py/test_call.py` & `light_curve-0.9.1/tests/light_curve_py/test_call.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/light_curve_py/test_single_band.py` & `light_curve-0.9.1/tests/light_curve_py/test_single_band.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/tests/test_w_bench.py` & `light_curve-0.9.1/tests/test_w_bench.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/Cargo.lock` & `light_curve-0.9.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -55,19 +55,19 @@
 checksum = "ca972c2ea5f742bfce5687b9aef75506a764f61d37f8f649047846a9686ddb66"
 dependencies = [
  "memchr 0.1.11",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
- "memchr 2.7.1",
+ "memchr 2.7.2",
 ]
 
 [[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
@@ -79,56 +79,56 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.80"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ad32ce52e4161730f7098c077cd2ed6229b5804ccf99e5366be1ab72a98b4e1"
+checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base16ct"
-version = "0.1.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "349a06037c7bf932dd7e7d1f653678b2038b9ad46a74102f1fc7bd7872678cce"
+checksum = "4c7f02d4ea65f2c1853089ffd8d2787bdbc63de2f0d29dedbcf8ccdfa0ccd4cf"
 
 [[package]]
 name = "base64"
-version = "0.13.1"
+version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
+checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
 name = "base64"
-version = "0.21.7"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
+checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
 
 [[package]]
 name = "base64ct"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c3c1a368f70d6cf7302d78f8f7093da241fb8e8807c05cc9e51a125895a6d5b"
 
@@ -136,32 +136,32 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.3"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ea184aa71bb362a1157c896979544cc23974e08fd265f29ea96b59f0b4a555b"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
@@ -184,19 +184,21 @@
  "cc",
  "libc",
  "pkg-config",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.88"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02f341c093d19155a6e41631ce5971aac4e9a868262212153124c15fa22d1cdc"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 dependencies = [
+ "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "ceres-solver"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c2449161c41ba9cf1a0dfbe6872791b18773eccb49aed955bacc428586e6d68"
@@ -241,24 +243,24 @@
 dependencies = [
  "num",
  "time 0.1.45",
 ]
 
 [[package]]
 name = "chrono"
-version = "0.4.34"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bc015644b92d5890fab7489e49d21f879d5c990186827d42ec511919404f38b"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "wasm-bindgen",
- "windows-targets 0.52.3",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "cipher"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
@@ -428,85 +430,85 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "darling"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
+checksum = "54e36fcd13ed84ffdfda6f5be89b31287cbb80c439841fe69e04841435464391"
 dependencies = [
  "darling_core",
  "darling_macro",
 ]
 
 [[package]]
 name = "darling_core"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "109c1ca6e6b7f82cc233a97004ea8ed7ca123a9af07a8230878fcfda9b158bf0"
+checksum = "9c2cf1c23a687a1feeb728783b993c4e1ad83d99f351801977dd809b48d0a70f"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim",
- "syn 1.0.109",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "darling_macro"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4aab4dbc9f7611d8b55048a3a16d2d010c2c8334e46304b40ac1cc14bf3b48e"
+checksum = "a668eda54683121533a393014d8692171709ff57a7d61f187b6e782719f8933f"
 dependencies = [
  "darling_core",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "deranged"
 version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
 dependencies = [
  "powerfmt",
 ]
 
 [[package]]
 name = "derive_builder"
-version = "0.11.2"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d07adf7be193b71cc36b193d0f5fe60b918a3a9db4dad0449f57bcfd519704a3"
+checksum = "0350b5cb0331628a5916d6c5c0b72e97393b8b6b03b47a9284f4e7f5a405ffd7"
 dependencies = [
  "derive_builder_macro",
 ]
 
 [[package]]
 name = "derive_builder_core"
-version = "0.11.2"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f91d4cfa921f1c05904dc3c57b4a32c38aed3340cce209f3a6fd1478babafc4"
+checksum = "d48cda787f839151732d396ac69e3473923d54312c070ee21e9effcaa8ca0b1d"
 dependencies = [
  "darling",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "derive_builder_macro"
-version = "0.11.2"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f0314b72bed045f3a68671b3c86328386762c93f82d98c65c3cb5e5f573dd68"
+checksum = "206868b8242f27cecce124c19fd88157fbd0dd334df2587f36417bafbc85097b"
 dependencies = [
  "derive_builder_core",
- "syn 1.0.109",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
@@ -514,84 +516,85 @@
  "block-buffer",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
 name = "directories"
-version = "4.0.1"
+version = "5.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f51c5d4ddabd36886dd3e1438cb358cdcb0d7c499cb99cb4ac2e38e18b5cb210"
+checksum = "9a49173b84e034382284f27f1af4dcbbd231ffa358c0fe316541a7337f376a35"
 dependencies = [
  "dirs-sys",
 ]
 
 [[package]]
 name = "dirs-sys"
-version = "0.3.7"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b1d1d91c932ef41c0f2663aa8b0ca0342d444d842c06914aa0a7e352d0bada6"
+checksum = "520f05a5cbd335fae5a99ff7a6ab8627577660ee5cfd6a94a6a929b52ff0321c"
 dependencies = [
  "libc",
+ "option-ext",
  "redox_users",
- "winapi 0.3.9",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "dyn-clone"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "emcee"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d903b65b48e77869a8ca98db3f4cbe0756892d69dafdcc6255580dfa6b5745f9"
 dependencies = [
  "error-chain",
  "rand 0.3.23",
 ]
 
 [[package]]
 name = "enum-iterator"
-version = "2.0.0"
+version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "600536cfe9e2da0820aa498e570f6b2b9223eec3ce2f835c8ae4861304fa4794"
+checksum = "2e0b48d2b80ff6b002339547442496ea29d66a8c66ce8e1a6bd8c58b9cec7cf3"
 dependencies = [
  "enum-iterator-derive",
 ]
 
 [[package]]
 name = "enum-iterator-derive"
-version = "1.3.0"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03cdc46ec28bd728e67540c528013c6a10eb69a02eb31078a1bda695438cbfb8"
+checksum = "c19cbb53d33b57ac4df1f0af6b92c38c107cded663c4aea9fae1189dcfc17cf5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.51",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "enum_dispatch"
-version = "0.3.12"
+version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f33313078bb8d4d05a2733a94ac4c2d8a0df9a2b84424ebf4f33bfc224a890e"
+checksum = "aa18ce2bc66555b3218614519ac839ddb759a7d6720732f979ef8d13be147ecd"
 dependencies = [
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.51",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "enumflags2"
 version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3278c9d5fb675e0a51dabcf4c0d355f692b064171535ba72361be1528a9d8e8d"
@@ -604,25 +607,31 @@
 name = "enumflags2_derive"
 version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c785274071b1b420972453b306eeca06acf4633829db4223b58a2a8c5953bc4"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.51",
+ "syn 2.0.60",
 ]
 
 [[package]]
+name = "equivalent"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
+
+[[package]]
 name = "errno"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
  "libc",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "error-chain"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9435d864e017c3c6afeac1654189b06cdb491cf2ff73dbf0d73b0f292f42ff8"
@@ -632,15 +641,15 @@
 
 [[package]]
 name = "fftw"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5ca544f4c7f2c162c493d084893ec81b9dc3c17e43098d6c3e0c6f9a4173c5d2"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "fftw-sys",
  "lazy_static 1.4.0",
  "ndarray",
  "num-complex",
  "num-traits",
  "thiserror",
 ]
@@ -675,15 +684,15 @@
 version = "0.2.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ee447700ac8aa0b2f2bd7bc4462ad686ba06baa6727ac149a2d6277f0d240fd"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "flate2"
 version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
@@ -738,17 +747,17 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
@@ -772,18 +781,30 @@
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
+name = "hashbrown"
+version = "0.14.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+
+[[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
 name = "hermit-abi"
-version = "0.3.8"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "379dada1584ad501b383485dd706b8afb7a70fcbc7f4da7d780638a5a6124a60"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "hmac"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
@@ -832,22 +853,32 @@
 [[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
- "hashbrown",
+ "hashbrown 0.12.3",
+]
+
+[[package]]
+name = "indexmap"
+version = "2.2.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
+dependencies = [
+ "equivalent",
+ "hashbrown 0.14.3",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.9"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "inout"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0c10553d664a4d0bcff9f4215d0aac67a639cc68ef660840afe309b807bc9f5"
 dependencies = [
@@ -904,23 +935,32 @@
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
+
+[[package]]
+name = "jobserver"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
+dependencies = [
+ "libc",
+]
 
 [[package]]
 name = "js-sys"
-version = "0.3.68"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "406cda4b368d531c842222cf9d2600a9a4acce8d29423695379c6868a143a9ee"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "kernel32-sys"
 version = "0.2.2"
@@ -963,21 +1003,20 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "libredox"
-version = "0.0.1"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85c833ca1e66078851dba29046874e38f08b2c883700aa29a03ddd3b23814ee8"
+checksum = "c0ff37bd590ca25063e35af745c343cb7a0271906fb7b37e4813e8f79f00268d"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "libc",
- "redox_syscall",
 ]
 
 [[package]]
 name = "light-curve-dmdt"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f8af1536df1cbb9ec6c25d01e9a844c045fa7930e0e3a67068557972835e0187"
@@ -1019,15 +1058,15 @@
  "thiserror",
  "thread_local 1.1.8",
  "unzip3",
 ]
 
 [[package]]
 name = "light-curve-python"
-version = "0.9.0"
+version = "0.9.1"
 dependencies = [
  "const_format",
  "conv",
  "enum-iterator",
  "enumflags2",
  "itertools 0.12.1",
  "light-curve-dmdt",
@@ -1073,17 +1112,17 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "macro_const"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0a3ce974efca8c8fafc305ad68708850b8b5842f73546e32f95719640518de6a"
 
@@ -1104,23 +1143,23 @@
 checksum = "d8b629fb514376c675b98c1421e80b151d3817ac42d7c667717d282761418d20"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mimalloc"
 version = "0.1.39"
@@ -1156,15 +1195,15 @@
 
 [[package]]
 name = "ndarray-stats"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af5a8477ac96877b5bd1fd67e0c28736c12943aba24eda92b127e036b0c8f400"
 dependencies = [
- "indexmap",
+ "indexmap 1.9.3",
  "itertools 0.10.5",
  "ndarray",
  "noisy_float",
  "num-integer",
  "num-traits",
  "rand 0.8.5",
 ]
@@ -1252,17 +1291,17 @@
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "numpy"
-version = "0.19.0"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "437213adf41bbccf4aeae535fbfcdad0f6fed241e1ae182ebe97fa1f3ce19389"
+checksum = "ec170733ca37175f5d75a5bea5911d6ff45d2cd52849ce98b685394e4f2f37f4"
 dependencies = [
  "libc",
  "ndarray",
  "num-complex",
  "num-integer",
  "num-traits",
  "pyo3",
@@ -1271,45 +1310,45 @@
 
 [[package]]
 name = "object"
 version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
- "memchr 2.7.1",
+ "memchr 2.7.2",
 ]
 
 [[package]]
 name = "oci-spec"
-version = "0.5.8"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98135224dd4faeb24c05a2fac911ed53ea6b09ecb09d7cada1cb79963ab2ee34"
+checksum = "e423c4f827362c0d8d8da4b1f571270f389ebde73bcd3240a3d23c6d6f61d0f0"
 dependencies = [
  "derive_builder",
  "getset",
  "serde",
  "serde_json",
  "thiserror",
 ]
 
 [[package]]
 name = "ocipkg"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60cf01280832705a4e4c4d046d9e67a54b900297c69191457a8fc6d198ddefa2"
+checksum = "9bb3293021f06540803301af45e7ab81693d50e89a7398a3420bdab139e7ba5e"
 dependencies = [
  "base16ct",
- "base64 0.13.1",
- "chrono 0.4.34",
+ "base64 0.22.0",
+ "chrono 0.4.38",
  "directories",
  "flate2",
  "lazy_static 1.4.0",
  "log",
  "oci-spec",
- "regex 1.10.3",
+ "regex 1.10.4",
  "serde",
  "serde_json",
  "sha2",
  "tar",
  "thiserror",
  "toml",
  "ureq",
@@ -1321,14 +1360,20 @@
 [[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
+name = "option-ext"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
+
+[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
@@ -1385,14 +1430,20 @@
 [[package]]
 name = "pkg-config"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "powerfmt"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
 
 [[package]]
 name = "ppv-lite86"
@@ -1422,87 +1473,90 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e681a6cfdc4adcc93b4d3cf993749a4552018ee0a9b65fc0ccfad74352c72a38"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "inventory",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "076c73d0bc438f7a4ef6fdd0c3bb4732149136abd952b110ac93e4edb13a6ba5"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e53cee42e77ebe256066ba8aa77eff722b3bb91f3419177cf4cd0f304d3284d9"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfeb4c99597e136528c6dd7d5e3de5434d1ceaf487436a3f03b2d56b6fc9efd1"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "947dc12175c254889edc0c02e399476c2f652b4b9ebd123aa655c224de259536"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
+ "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.3.23"
@@ -1584,17 +1638,17 @@
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4963ed1bc86e4f3ee217022bd855b297cef07fb9eac5dfa1f788b220b49b3bd"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -1622,17 +1676,17 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "redox_users"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a18479200779601e498ada4e8c1e1f50e3ee19deb0259c25825a98b5603b2cb4"
+checksum = "bd283d9651eeda4b2a83a43c1c91b266c40fd76ecd39a50a8c630ae69dc72891"
 dependencies = [
  "getrandom",
  "libredox",
  "thiserror",
 ]
 
 [[package]]
@@ -1646,60 +1700,60 @@
  "regex-syntax 0.3.9",
  "thread_local 0.2.7",
  "utf8-ranges",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
- "aho-corasick 1.1.2",
- "memchr 2.7.1",
+ "aho-corasick 1.1.3",
+ "memchr 2.7.2",
  "regex-automata",
- "regex-syntax 0.8.2",
+ "regex-syntax 0.8.3",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bb987efffd3c6d0d8f5f89510bb458559eab11e4f869acb20bf845e016259cd"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
- "aho-corasick 1.1.2",
- "memchr 2.7.1",
- "regex-syntax 0.8.2",
+ "aho-corasick 1.1.3",
+ "memchr 2.7.2",
+ "regex-syntax 0.8.3",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9ec002c35e86791825ed294b50008eea9ddfc8def4420124fbc6b08db834957"
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "ring"
 version = "0.17.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c17fa4cb658e3583423e915b9f3acc01cceaee1860e33d59ebae66adc3a2dc0d"
 dependencies = [
  "cc",
  "cfg-if",
  "getrandom",
  "libc",
  "spin",
  "untrusted",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
@@ -1708,50 +1762,50 @@
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.38.31"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.22.2"
+version = "0.22.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e87c9956bd9807afa1f77e0f7594af32566e830e088a5576d27c5b6f30f49d41"
+checksum = "bf4ef73721ac7bcd79b2b315da7779d8fc09718c6b3d2d1b2d94850eb8c18432"
 dependencies = [
  "log",
  "ring",
  "rustls-pki-types",
  "rustls-webpki",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.3.1"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ede67b28608b4c60685c7d54122d4400d90f62b40caee7700e700380a390fa8"
+checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
 
 [[package]]
 name = "rustls-webpki"
-version = "0.102.2"
+version = "0.102.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
+checksum = "f3bce581c0dd41bce533ce695a1437fa16a7ab5ac3ccfa99fe1a620a7885eabf"
 dependencies = [
  "ring",
  "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
@@ -1803,17 +1857,17 @@
 name = "scratch"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3cf7c11c38cb994f3d40e8a8cde3bbd1f72a435e4c49e85d6553d8312306152"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-pickle"
 version = "1.1.1"
@@ -1825,21 +1879,21 @@
  "num-bigint",
  "num-traits",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.51",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "serde_derive_internals"
 version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85bf8229e7920a9f636479437026331ce11aa132b4dde37d121944a44d6e5f3c"
@@ -1847,24 +1901,33 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "serde_spanned"
+version = "0.6.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eb3622f419d1296904700073ea6cc23ad690adbd66f13ea683df73298736f0c1"
+dependencies = [
+ "serde",
+]
+
+[[package]]
 name = "sha1"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3bf829a2d51ab4a5ddf1352d8470c140cadc8301b2ae1789db023f01cedd6ba"
 dependencies = [
  "cfg-if",
  "cpufeatures",
@@ -1880,17 +1943,17 @@
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 
@@ -1915,17 +1978,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.51"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ab617d94515e94ae53b8406c628598680aa0c9587474ecbe58188f7b345d66c"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1952,30 +2015,30 @@
 checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.57"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e45bcbe8ed29775f228095caf2cd67af7a4ccf756ebff23a306bf3e8b47b24b"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.57"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a953cb265bef375dae3de6663da4d3804eee9682ea80d8e2542529b73c531c81"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.51",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "thread-id"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9539db560102d1cef46b8b78ce737ff0bb64e7e18d35b2a5688f7d097d0ff03"
@@ -2012,17 +2075,17 @@
  "libc",
  "wasi 0.10.0+wasi-snapshot-preview1",
  "winapi 0.3.9",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.34"
+version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8248b6521bb14bc45b4067159b9b6ad792e2d6d754d6c41fb50e29fefe38749"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
 dependencies = [
  "deranged",
  "num-conv",
  "powerfmt",
  "serde",
  "time-core",
 ]
@@ -2046,19 +2109,44 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "toml"
-version = "0.5.11"
+version = "0.8.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
+checksum = "e9dd1545e8208b4a5af1aa9bbd0b4cf7e9ea08fabc5d0a5c67fcaafa17433aa3"
 dependencies = [
  "serde",
+ "serde_spanned",
+ "toml_datetime",
+ "toml_edit",
+]
+
+[[package]]
+name = "toml_datetime"
+version = "0.6.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
+dependencies = [
+ "serde",
+]
+
+[[package]]
+name = "toml_edit"
+version = "0.22.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d3328d4f68a705b2a4498da1d580585d39a6510f98318a2cec3018a7ec61ddef"
+dependencies = [
+ "indexmap 2.2.6",
+ "serde",
+ "serde_spanned",
+ "toml_datetime",
+ "winnow",
 ]
 
 [[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
@@ -2094,17 +2182,17 @@
 name = "unicode-xid"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "untrusted"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
 
@@ -2148,32 +2236,32 @@
 name = "utf8-ranges"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1ca13c08c41c9c3e04224ed9ff80461d97e121589ff27c753a16cb10830ae0f"
 
 [[package]]
 name = "uuid"
-version = "1.7.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f00cc9702ca12d3c81455259621e676d0f7251cec66a21e98fe2e9a37db93b2a"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d71d857dc86794ca4c280d616f7da00d2dbfd8cd788846559a6813e6aa4b54ee"
+checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
 name = "wasi"
@@ -2185,65 +2273,65 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1e124130aee3fb58c5bdd6b639a0509486b0338acaaae0c84a5124b0f588b7f"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c9e7e1900c352b609c8488ad12639a311045f40a35491fb69ba8c12f758af70b"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.51",
+ "syn 2.0.60",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b30af9e2d358182b5c7449424f017eba305ed32a7010509ede96cdc4696c46ed"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "642f325be6301eb8107a83d12a8ac6c1e1c54345a7ef1a9261962dfefda09e66"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.51",
+ "syn 2.0.60",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f186bd2dcf04330886ce82d6f33dd75a7bfcf69ecf5763b89fcde53b6ac9838"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "webpki-roots"
 version = "0.26.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b3de34ae270483955a94f4b21bdaaeb83d508bb84a01435f393818edb0012009"
 dependencies = [
@@ -2295,24 +2383,33 @@
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.3",
+ "windows-targets 0.52.5",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.3",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -2324,110 +2421,126 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d380ba1dc7187569a8a9e91ed34b8ccfc33123bbacb8c0aed2d1ad7f3ef2dc5f"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.3",
- "windows_aarch64_msvc 0.52.3",
- "windows_i686_gnu 0.52.3",
- "windows_i686_msvc 0.52.3",
- "windows_x86_64_gnu 0.52.3",
- "windows_x86_64_gnullvm 0.52.3",
- "windows_x86_64_msvc 0.52.3",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68e5dcfb9413f53afd9c8f86e56a7b4d86d9a2fa26090ea2dc9e40fba56c6ec6"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8dab469ebbc45798319e69eebf92308e541ce46760b49b18c6b3fe5e8965b30f"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.3"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a4e9b6a7cac734a8b4138a4e1044eac3404d8326b6c0f939276560687a033fb"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28b0ec9c422ca95ff34a78755cfa6ad4a51371da2a5ace67500cf7ca5f232c58"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "704131571ba93e89d7cd43482277d6632589b18ecf4468f591fbae0a8b101614"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42079295511643151e98d61c38c0acc444e52dd42ab456f7ccfd5152e8ecf21c"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0770833d60a970638e989b3fa9fd2bb1aaadcf88963d1659fd7d9990196ed2d6"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
+
+[[package]]
+name = "winnow"
+version = "0.6.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f0c976aaaa0e1f90dbb21e9587cdaf1d9679a1cde8875c0d6bd83ab96a208352"
+dependencies = [
+ "memchr 2.7.2",
+]
 
 [[package]]
 name = "xattr"
 version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8da84f1a25939b27f6820d92aed108f83ff920fdf11a7b19366c27c4cda81d4f"
 dependencies = [
@@ -2454,15 +2567,15 @@
  "constant_time_eq",
  "crc32fast",
  "crossbeam-utils",
  "flate2",
  "hmac",
  "pbkdf2",
  "sha1",
- "time 0.3.34",
+ "time 0.3.36",
  "zstd",
 ]
 
 [[package]]
 name = "zstd"
 version = "0.11.2+zstd.1.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2479,14 +2592,14 @@
 dependencies = [
  "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.9+zstd.1.5.5"
+version = "2.0.10+zstd.1.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e16efa8a874a0481a574084d34cc26fdb3b99627480f785888deb6386506656"
+checksum = "c253a4914af5bafc8fa8c86ee400827e83cf6ec01195ec1f1ed8441bf00d65aa"
 dependencies = [
  "cc",
  "pkg-config",
 ]
```

### Comparing `light_curve-0.9.0/pyproject.toml` & `light_curve-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `light_curve-0.9.0/PKG-INFO` & `light_curve-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: light-curve
-Version: 0.9.0
+Version: 0.9.1
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -55,15 +55,15 @@
 python3 -mpip install 'light-curve[full]'
 ```
 
 `full` extras would install the package with all optional Python dependencies required by experimental features.
 We also provide `light-curve-python` package which is just an "alias" to the main `light-curve[full]` package.
 
 Minimum supported Python version is 3.8.
-We provide binary wheels via [PyPi](https://pypi.org/project/light-curve/) for a number of platforms and architectures, both for CPython and PyPy.
+We provide binary CPython wheels via [PyPi](https://pypi.org/project/light-curve/) for a number of platforms and architectures.
 We also provide binary wheels for stable CPython ABI, so the package is guaranteed to work with all future CPython3 versions.
 
 ### Support matrix
 
 | Arch \ OS   | Linux glibc | Linux musl                     | macOS                                                          | Windows https://github.com/light-curve/light-curve-python/issues/186 |
 | ----------- |-------------|--------------------------------|----------------------------------------------------------------|----------------------------------------------------------------------|
 | **x86-64**  | wheel (MKL) | wheel (MKL)                    | wheel                                                          | wheel (no Ceres, no GSL)                                             |
@@ -71,14 +71,16 @@
 | **aarch64** | wheel       | wheel                          | wheel                                                          | not tested                                                           |
 | **ppc64le** | wheel       | not tested (no Rust toolchain) | —                                                              | —                                                                    |
 
 - "wheel": binary wheel is available on pypi.org, local building is not required for the platform, the only pre-requirement is a recent `pip` version. For Linux x86-64 we provide binary wheels built with Intel MKL for better periodogram performance, which is not a default build option. For Windows x86-64 we provide wheel with no Ceres and no GSL support, which is not a default build option.
 - "src": the package is confirmed to be built and pass unit tests locally, but testing and package building is not supported by CI. It is required to have the [GNU scientific library (GSL)](https://www.gnu.org/software/gsl/) v2.1+ and the [Rust toolchain](https://rust-lang.org) v1.67+ to install it via `pip install`. `ceres-solver` and `fftw` may be installed locally or built from source, in the later case you would also need C/C++ compiler and `cmake`.
 - "not tested": building from the source code is not tested, please report us building status via issue/PR/email.
 
+We stopped publishing PyPy wheels (https://github.com/light-curve/light-curve-python/issues/345), please feel free to open an issue if you need them.
+
 ## Feature evaluators
 
 Most of the classes implement various feature evaluators useful for light-curve based
 astrophysical source classification and characterisation.
 
 <!-- name: test_feature_evaluators_basic -->
 ```python
```

