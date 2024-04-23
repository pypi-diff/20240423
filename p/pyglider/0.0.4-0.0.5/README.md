# Comparing `tmp/pyglider-0.0.4.tar.gz` & `tmp/pyglider-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglider-0.0.4.tar", last modified: Tue Jun 21 15:04:47 2022, max compression
+gzip compressed data, was "pyglider-0.0.5.tar", last modified: Tue Apr 23 19:43:28 2024, max compression
```

## Comparing `pyglider-0.0.4.tar` & `pyglider-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 jklymak    (501) staff       (20)        0 2022-06-21 15:04:47.555818 pyglider-0.0.4/
--rw-r--r--   0 jklymak    (501) staff       (20)    10272 2022-06-21 14:08:58.000000 pyglider-0.0.4/LICENSE
--rw-r--r--   0 jklymak    (501) staff       (20)      333 2022-06-21 15:04:47.555904 pyglider-0.0.4/PKG-INFO
--rw-r--r--   0 jklymak    (501) staff       (20)     2609 2022-06-07 08:40:26.000000 pyglider-0.0.4/README.md
-drwxr-xr-x   0 jklymak    (501) staff       (20)        0 2022-06-21 15:04:47.554527 pyglider-0.0.4/pyglider/
--rw-r--r--   0 jklymak    (501) staff       (20)       24 2022-05-29 15:57:42.000000 pyglider-0.0.4/pyglider/__init__.py
--rw-r--r--   0 jklymak    (501) staff       (20)      748 2022-06-21 13:18:46.000000 pyglider-0.0.4/pyglider/example_data.py
--rw-r--r--   0 jklymak    (501) staff       (20)    10201 2022-06-16 11:51:28.000000 pyglider-0.0.4/pyglider/ncprocess.py
--rw-r--r--   0 jklymak    (501) staff       (20)    16392 2022-06-07 08:38:08.000000 pyglider-0.0.4/pyglider/seaexplorer.py
--rw-r--r--   0 jklymak    (501) staff       (20)    32532 2022-06-16 11:51:28.000000 pyglider-0.0.4/pyglider/slocum.py
--rw-r--r--   0 jklymak    (501) staff       (20)    22095 2022-06-16 11:51:28.000000 pyglider-0.0.4/pyglider/utils.py
-drwxr-xr-x   0 jklymak    (501) staff       (20)        0 2022-06-21 15:04:47.555551 pyglider-0.0.4/pyglider.egg-info/
--rw-r--r--   0 jklymak    (501) staff       (20)      333 2022-06-21 15:04:47.000000 pyglider-0.0.4/pyglider.egg-info/PKG-INFO
--rw-r--r--   0 jklymak    (501) staff       (20)      351 2022-06-21 15:04:47.000000 pyglider-0.0.4/pyglider.egg-info/SOURCES.txt
--rw-r--r--   0 jklymak    (501) staff       (20)        1 2022-06-21 15:04:47.000000 pyglider-0.0.4/pyglider.egg-info/dependency_links.txt
--rw-r--r--   0 jklymak    (501) staff       (20)      188 2022-06-21 15:04:47.000000 pyglider-0.0.4/pyglider.egg-info/requires.txt
--rw-r--r--   0 jklymak    (501) staff       (20)        9 2022-06-21 15:04:47.000000 pyglider-0.0.4/pyglider.egg-info/top_level.txt
--rw-r--r--   0 jklymak    (501) staff       (20)        1 2022-05-29 19:59:56.000000 pyglider-0.0.4/pyglider.egg-info/zip-safe
--rw-r--r--   0 jklymak    (501) staff       (20)       38 2022-06-21 15:04:47.556121 pyglider-0.0.4/setup.cfg
--rw-r--r--   0 jklymak    (501) staff       (20)      865 2022-06-21 15:04:35.000000 pyglider-0.0.4/setup.py
+drwxr-xr-x   0 jklymak    (501) staff       (20)        0 2024-04-23 19:43:28.748317 pyglider-0.0.5/
+-rw-r--r--   0 jklymak    (501) staff       (20)    10272 2024-03-25 22:44:38.000000 pyglider-0.0.5/LICENSE
+-rw-r--r--   0 jklymak    (501) staff       (20)     1298 2024-04-23 19:43:28.748099 pyglider-0.0.5/PKG-INFO
+-rw-r--r--   0 jklymak    (501) staff       (20)      361 2024-03-25 22:44:38.000000 pyglider-0.0.5/README.md
+drwxr-xr-x   0 jklymak    (501) staff       (20)        0 2024-04-23 19:43:28.745406 pyglider-0.0.5/pyglider/
+-rw-r--r--   0 jklymak    (501) staff       (20)       24 2024-03-25 22:44:38.000000 pyglider-0.0.5/pyglider/__init__.py
+-rw-r--r--   0 jklymak    (501) staff       (20)       21 2024-04-23 19:18:32.000000 pyglider-0.0.5/pyglider/_version.py
+-rw-r--r--   0 jklymak    (501) staff       (20)      748 2024-03-25 22:44:38.000000 pyglider-0.0.5/pyglider/example_data.py
+-rw-r--r--   0 jklymak    (501) staff       (20)    10740 2024-04-23 19:03:22.000000 pyglider-0.0.5/pyglider/ncprocess.py
+-rw-r--r--   0 jklymak    (501) staff       (20)    20335 2024-04-23 19:03:22.000000 pyglider-0.0.5/pyglider/seaexplorer.py
+-rw-r--r--   0 jklymak    (501) staff       (20)    38284 2024-04-23 19:03:22.000000 pyglider-0.0.5/pyglider/slocum.py
+-rw-r--r--   0 jklymak    (501) staff       (20)    22952 2024-04-23 19:03:22.000000 pyglider-0.0.5/pyglider/utils.py
+drwxr-xr-x   0 jklymak    (501) staff       (20)        0 2024-04-23 19:43:28.747343 pyglider-0.0.5/pyglider.egg-info/
+-rw-r--r--   0 jklymak    (501) staff       (20)     1298 2024-04-23 19:43:28.000000 pyglider-0.0.5/pyglider.egg-info/PKG-INFO
+-rw-r--r--   0 jklymak    (501) staff       (20)      446 2024-04-23 19:43:28.000000 pyglider-0.0.5/pyglider.egg-info/SOURCES.txt
+-rw-r--r--   0 jklymak    (501) staff       (20)        1 2024-04-23 19:43:28.000000 pyglider-0.0.5/pyglider.egg-info/dependency_links.txt
+-rw-r--r--   0 jklymak    (501) staff       (20)      222 2024-04-23 19:43:28.000000 pyglider-0.0.5/pyglider.egg-info/requires.txt
+-rw-r--r--   0 jklymak    (501) staff       (20)        9 2024-04-23 19:43:28.000000 pyglider-0.0.5/pyglider.egg-info/top_level.txt
+-rw-r--r--   0 jklymak    (501) staff       (20)        1 2024-03-25 22:47:15.000000 pyglider-0.0.5/pyglider.egg-info/zip-safe
+-rw-r--r--   0 jklymak    (501) staff       (20)      706 2024-04-23 19:43:23.000000 pyglider-0.0.5/pyproject.toml
+-rw-r--r--   0 jklymak    (501) staff       (20)       38 2024-04-23 19:43:28.748361 pyglider-0.0.5/setup.cfg
+-rw-r--r--   0 jklymak    (501) staff       (20)      919 2024-04-23 19:16:31.000000 pyglider-0.0.5/setup.py
+drwxr-xr-x   0 jklymak    (501) staff       (20)        0 2024-04-23 19:43:28.747078 pyglider-0.0.5/tests/
+-rw-r--r--   0 jklymak    (501) staff       (20)    11854 2024-04-23 19:03:22.000000 pyglider-0.0.5/tests/test_pyglider.py
+-rw-r--r--   0 jklymak    (501) staff       (20)     6189 2024-04-23 19:03:22.000000 pyglider-0.0.5/tests/test_seaexplorer.py
+-rw-r--r--   0 jklymak    (501) staff       (20)     1222 2024-03-25 22:44:38.000000 pyglider-0.0.5/tests/test_utils.py
```

### Comparing `pyglider-0.0.4/LICENSE` & `pyglider-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglider-0.0.4/pyglider/example_data.py` & `pyglider-0.0.5/pyglider/example_data.py`

 * *Files identical despite different names*

### Comparing `pyglider-0.0.4/pyglider/ncprocess.py` & `pyglider-0.0.5/pyglider/ncprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,20 @@
                 profile_meta = deployment['profile_variables']
                 if 'water_velocity_eastward' in dss.keys():
                     dss['u'] = dss.water_velocity_eastward.mean()
                     dss['u'].attrs = profile_meta['u']
 
                     dss['v'] = dss.water_velocity_northward.mean()
                     dss['v'].attrs = profile_meta['v']
+                elif 'u' in profile_meta:
+                    dss['u'] = profile_meta['u'].get('_FillValue', np.NaN)
+                    dss['u'].attrs = profile_meta['u']
+
+                    dss['v'] = profile_meta['v'].get('_FillValue', np.NaN)
+                    dss['v'].attrs = profile_meta['v']
 
                 dss['profile_id'] = np.array(p*1.0)
                 dss['profile_id'].attrs = profile_meta['profile_id']
                 dss['profile_time'] = dss.time.mean()
                 dss['profile_time'].attrs = profile_meta['profile_time']
                 dss['profile_lon'] = dss.longitude.mean()
                 dss['profile_lon'].attrs = profile_meta['profile_lon']
@@ -107,25 +113,27 @@
                 to_fill = ['temperature', 'pressure', 'conductivity',
                            'salinity', 'density', 'lon', 'lat', 'depth']
                 for name in to_fill:
                     dss[name].attrs['ancillary_variables'] = name + '_qc'
 
                 # outname = outdir + '/' + utils.get_file_id(dss) + '.nc'
                 _log.info('Writing %s', outname)
-                if 'units' in dss.profile_time.attrs:
-                    dss.profile_time.attrs.pop('units')
-                timeunits = 'seconds since 1970-01-01T00:00:00Z'
-                dss.to_netcdf(outname, encoding={'time': {'units': timeunits}})
+                timeunits = 'nanoseconds since 1970-01-01T00:00:00Z'
+                timecalendar = 'gregorian'
+                dss.to_netcdf(outname, encoding={'time': {'units': timeunits,
+                                                          'calendar': timecalendar},
+                                                          'profile_time':
+                                                         {'units': timeunits}})
 
                 # add traj_strlen using bare ntcdf to make IOOS happy
                 with netCDF4.Dataset(outname, 'r+') as nc:
                     nc.renameDimension('string%d' % trajlen, 'traj_strlen')
 
 
-def make_gridfiles(inname, outdir, deploymentyaml, dz=1):
+def make_gridfiles(inname, outdir, deploymentyaml, *, fnamesuffix='', dz=1):
     """
     Turn a timeseries netCDF file into a vertically gridded netCDF.
 
     Parameters
     ----------
     inname : str or Path
         netcdf file to break into profiles
@@ -152,15 +160,15 @@
     except FileExistsError:
         pass
 
     with open(deploymentyaml) as fin:
         deployment = yaml.safe_load(fin)
     profile_meta = deployment['profile_variables']
 
-    ds = xr.open_dataset(inname)
+    ds = xr.open_dataset(inname, decode_times=True)
     _log.info(f'Working on: {inname}')
     _log.debug(str(ds))
     _log.debug(str(ds.time[0]))
     _log.debug(str(ds.time[-1]))
 
     profiles = np.unique(ds.profile_index)
     profiles = [p for p in profiles if (~np.isnan(p) and not (p % 1)
@@ -171,25 +179,26 @@
     _log.info(f'Nprofiles {Nprofiles}')
     depth_bins = np.arange(0, 1100.1, dz)
     depths = depth_bins[:-1] + 0.5
 
     dsout = xr.Dataset(
         coords={'depth': ('depth', depths),
                 'profile': ('time', profiles)})
+    print('Booo', ds.time, ds.temperature)
     ds['time_1970'] = ds.temperature.copy()
-    ds['time_1970'].values = ds.time.values.astype(np.float64)/1e9
+    ds['time_1970'].values = ds.time.values.astype(np.float64)
     for td in ('time_1970', 'longitude', 'latitude'):
         good = np.where(~np.isnan(ds[td]) & (ds['profile_index'] % 1 == 0))[0]
         dat, xedges, binnumber = stats.binned_statistic(
                 ds['profile_index'].values[good],
                 ds[td].values[good], statistic='mean',
                 bins=[profile_bins])
         if td == 'time_1970':
             td = 'time'
-            dat = dat.astype('timedelta64[s]') + np.datetime64('1970-01-01T00:00:00')
+            dat = dat.astype('timedelta64[ns]') + np.datetime64('1970-01-01T00:00:00')
         _log.info(f'{td} {len(dat)}')
         dsout[td] = (('time'), dat, ds[td].attrs)
     ds.drop('time_1970')
     good = np.where(~np.isnan(ds['time']) & (ds['profile_index'] % 1 == 0))[0]
     _log.info(f'Done times! {len(dat)}')
     dsout['profile_time_start'] = (
         ('time'), dat, profile_meta['profile_time_start'])
@@ -235,18 +244,18 @@
         dsout['u'].attrs = profile_meta['u']
         dsout['v'] = dsout.water_velocity_northward.mean(axis=0)
         dsout['v'].attrs = profile_meta['v']
         dsout = dsout.drop(['water_velocity_eastward',
                             'water_velocity_northward'])
     dsout.attrs = ds.attrs
 
-    outname = outdir + '/' + ds.attrs['deployment_name'] + '_grid.nc'
+    outname = outdir + '/' + ds.attrs['deployment_name'] + '_grid' + fnamesuffix + '.nc'
     _log.info('Writing %s', outname)
-    timeunits = 'seconds since 1970-01-01T00:00:00Z'
-    dsout.to_netcdf(outname, encoding={'time': {'units': timeunits}})
+    # timeunits = 'nanoseconds since 1970-01-01T00:00:00Z'
+    dsout.to_netcdf(outname)
     _log.info('Done gridding')
 
     return outname
 
 
 # aliases
 extract_L0timeseries_profiles = extract_timeseries_profiles
```

### Comparing `pyglider-0.0.4/pyglider/seaexplorer.py` & `pyglider-0.0.5/pyglider/seaexplorer.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,47 +5,47 @@
 import glob
 import logging
 import numpy as np
 import os
 import xarray as xr
 import yaml
 import pyglider.utils as utils
-import pandas as pd
-
+import datetime
+import polars as pl
 
 _log = logging.getLogger(__name__)
 
 
 def _outputname(f, outdir):
     fnout = os.path.basename(f)
     fns = fnout.split('.')
     fns = fns[:5]
     fns[4] = '%04d' % int(fns[4])
     fns[1] = '%04d' % int(fns[1])
     fnout = ''
     for ff in fns:
         fnout += ff.lower() + '.'
     filenum = int(fns[4])
-    return outdir + fnout + 'nc', filenum
+    return outdir + fnout + 'parquet', filenum
 
 
 def _needsupdating(ftype, fin, fout):
     if not os.path.isfile(fout):
         return True
     return (os.path.getmtime(fin) >= os.path.getmtime(fout))
 
 
 def _sort(ds):
     return ds.sortby('time')
 
 
 def raw_to_rawnc(indir, outdir, deploymentyaml, incremental=True,
-                 min_samples_in_file=5):
+                 min_samples_in_file=5, dropna_subset=None, dropna_thresh=1):
     """
-    Convert seaexplorer text files to raw netcdf files.
+    Convert seaexplorer text files to raw parquet files.
 
     Parameters
     ----------
     indir : str
         Directory with the raw files are kept.  Recommend naming this
         directory "raw"
 
@@ -59,116 +59,159 @@
         If *True* (default), only netcdf files that are older than the
         binary files are re-parsed.
 
     min_samples_in_file : int
         Minimum number of samples in a raw file to trigger writing a netcdf
         file. Defaults to 5
 
+    dropna_subset : list of strings, default None
+        If more values than *dropna_thresh* of the variables listed here are
+        empty (NaN), then drop this line of data.  Useful for raw payload files
+        that are heavily oversampled.  Get the variable names from the raw text
+        file.  See `pandas.DataFrame.dropna`.
+
+    dropna_thresh : integer, default 1
+        Number of variables listed in dropna_subset that can be empty before
+        the line is dropped.
+
+
     Returns
     -------
     status : bool
         *True* success.
 
     Notes
     -----
 
     This process can be slow for many files.
 
+    For the *dropna* functionality, list one variable for each of the sensors
+    that is *not* over-sampled.  For instance, we had an AROD, GPCTD, and
+    FLBBCD and the AROD was grossly oversampled, whereas the other two were not,
+    but were not sampled synchronously.  In that case we chose:
+    `dropna_subset=['GPCTD_TEMPERATURE', 'FLBBCD_CHL_COUNT']` to keep all
+    rows where either of these were good, and dropped all other rows.
+
     """
     # Create out directory for netcdfs if it does not exist
     try:
         os.mkdir(outdir)
     except FileExistsError:
         pass
 
     for ftype in ['gli', 'pld1']:
+        goodfiles = []
+        badfiles = []
         for rawsub in ['raw', 'sub']:
             _log.info(f'Reading in raw files matching *{ftype}.{rawsub}*')
             d = indir + f'*.{ftype}.{rawsub}.*'
+
             files = glob.glob(d)
             fnum = np.zeros(len(files))
             # these files don't sort properly, but we can sort them here.
             for n, f in enumerate(files):
                 p = os.path.basename(f).split('.')
                 fnum[n] = p[4]
             inds = np.argsort(fnum)
             files = [files[ind] for ind in inds]
             _log.info(f'found {files}')
 
             if len(files) == 0:
                 # If no files of this type found, try the next type
                 continue
 
-            badfiles = []
-            goodfiles = []
             for ind, f in enumerate(files):
                 # output name:
                 fnout, filenum = _outputname(f, outdir)
                 _log.info(f'{f} to {fnout}')
                 if not incremental or _needsupdating(ftype, f, fnout):
                     _log.info(f'Doing: {f} to {fnout}')
-                    out = pd.read_csv(f, header=0, delimiter=';',
-                                      parse_dates=True, index_col=0,
-                                      dayfirst=True)
+                    # Try to read the file with polars. If the file is corrupted (rare), file read will fail and file
+                    # is appended to badfiles
+                    try:
+                        out = pl.read_csv(f, separator=';')
+                    except Exception as e:
+                        _log.warning(f'Exception reading {f}: {e}')
+                        _log.warning(f'Could not read {f}')
+                        badfiles.append(f)
+                        continue
+                    # Parse the datetime from nav files (called Timestamp) and pld1 files (called PLD_REALTIMECLOCK)
+                    if "Timestamp" in out.columns:
+                        out = out.with_columns(
+                            pl.col("Timestamp").str.strptime(pl.Datetime, format="%d/%m/%Y %H:%M:%S"))
+                        out = out.rename({"Timestamp": "time"})
+                    else:
+                        out = out.with_columns(
+                            pl.col("PLD_REALTIMECLOCK").str.strptime(pl.Datetime, format="%d/%m/%Y %H:%M:%S.%3f"))
+                        out = out.rename({"PLD_REALTIMECLOCK": "time"})
+                    for col_name in out.columns:
+                        if "time" not in col_name.lower():
+                            out = out.with_columns(pl.col(col_name).cast(pl.Float64))
                     # If AD2CP data present, convert timestamps to datetime
                     if 'AD2CP_TIME' in out.columns:
                         # Set datestamps with date 00000 to None
-                        out.loc[out.AD2CP_TIME.str[:6] == '000000',
-                                'AD2CP_TIME'] = None
-                        out['AD2CP_TIME'] = pd.to_datetime(out.AD2CP_TIME)
-                    with out.to_xarray() as outx:
-                        key = list(outx.coords.keys())[0]
-                        outx = outx.rename({key: 'time'})
-                        outx['fnum'] = ('time',
-                                        int(filenum)*np.ones(len(outx['time'])))
-                        if ftype == 'gli':
-                            outx.to_netcdf(fnout[:-3] + '.nc', 'w')
+                        out = out.with_columns(
+                            pl.col('AD2CP_TIME').str.strptime(pl.Datetime, format="%m%d%y %H:%M:%S", strict=False))
+
+                    # subsetting for heavily oversampled raw data:
+                    if rawsub == 'raw' and dropna_subset is not None:
+                        # This check is the polars equivalent of pandas dropna. See docstring note on dropna
+                        out = out.with_columns(out.select(pl.col(dropna_subset).is_null().cast(pl.Int64))
+                                              .sum(axis=1).alias("null_count")).filter(
+                            pl.col("null_count") <= dropna_thresh) \
+                            .drop("null_count")
+
+                    if ftype == 'gli':
+                        out = out.with_columns([(pl.col("NavState") * 0 + int(filenum)).alias("fnum")])
+                        out.write_parquet(fnout)
+                        goodfiles.append(f)
+                    else:
+                        if out.select("time").shape[0] > min_samples_in_file:
+                            out.write_parquet(fnout)
                             goodfiles.append(f)
                         else:
-                            if outx.indexes["time"].size > min_samples_in_file:
-                                outx.to_netcdf(f'{fnout[:-3]}.nc', 'w',
-                                               unlimited_dims=['time'])
-                                goodfiles.append(f)
-                            else:
-                                _log.warning('Number of sensor data points'
-                                             'too small. Skipping nc write')
-                                badfiles.append(f)
-            if len(badfiles) > 0:
-                _log.warning('Some files could not be parsed:')
-                for fn in badfiles:
-                    _log.warning('%s', fn)
-            if not goodfiles:
-                _log.warning(f'No valid unprocessed seaexplorer files found in'
-                             f'{indir}')
-                return False
-    _log.info('All raw files converted to nc')
+                            _log.warning('Number of sensor data points'
+                                         'too small. Skipping parquet write')
+                            badfiles.append(f)
+    if len(badfiles) > 0:
+        _log.warning('Some files could not be parsed:')
+        for fn in badfiles:
+            _log.warning('%s', fn)
+    if not goodfiles:
+        _log.warning(f'No valid unprocessed seaexplorer files found in'f'{indir}')
+        return False
+    _log.info('All raw files converted to parquet')
     return True
 
 
-def drop_rogue_1970(ds):
+def drop_pre_1971_samples(df):
     """
     If dates greater than 1971, 1, 1 are observed, drop any dates before
     1971-01-01, from the datset and return it. This function removes 1970
     timestamps caused by a SeaExplorer rebooting during a mission. If all dates
     are < 1971-01-01, no action is taken
 
     Parameters:
-        ds: xarray.DataSet
-            dataset to check for pre-1971 dates
+        df: polars.DataFrame
+            dataframe to check for pre-1971 dates
     Returns:
-        ds: xarray.DataSet
+        df: polars.DataFrame
     """
-    dt_1971 = np.datetime64("1971-01-01")
+    dt_1971 = datetime.datetime(1971, 1, 1)
     # If all dates before or after 1971-01-01, return the dataset
-    if (ds.time > dt_1971).all() or (ds.time < dt_1971).all():
-        return ds
-    return ds.where(ds.time > dt_1971, drop=True)
+    pre_1971 = df.filter(pl.col("time") < dt_1971)
+    if len(pre_1971) == len(df):
+        return pre_1971
+    post_1971 = df.filter(pl.col("time") > dt_1971)
+    if len(post_1971) == len(df):
+        return post_1971
+    return df.filter(pl.col("time") > dt_1971)
 
 
-def merge_rawnc(indir, outdir, deploymentyaml, incremental=False, kind='raw'):
+def merge_parquet(indir, outdir, deploymentyaml, incremental=False, kind='raw'):
     """
     Merge all the raw netcdf files in indir.  These are meant to be
     the raw flight and science files from the slocum.
 
     Parameters
     ----------
     indir : str
@@ -189,154 +232,186 @@
         Only add new files....
     """
 
     with open(deploymentyaml) as fin:
         deployment = yaml.safe_load(fin)
     metadata = deployment['metadata']
     id = metadata['glider_name']
-    outgli = outdir + '/' + id + '-rawgli.nc'
-    outpld = outdir + '/' + id + '-' + kind + 'pld.nc'
+    outgli = outdir + '/' + id + '-rawgli.parquet'
+    outpld = outdir + '/' + id + '-' + kind + 'pld.parquet'
 
-    _log.info('Opening *.gli.sub.*.nc multi-file dataset from %s', indir)
-    files = sorted(glob.glob(indir+'/*.gli.sub.*.nc'))
+    _log.info('Opening *.gli.sub.*.parquet multi-file dataset from %s', indir)
+    files = sorted(glob.glob(indir + '/*.gli.sub.*.parquet'))
     if not files:
-        _log.warning(f'No *gli*.nc files found in {indir}')
+        _log.warning(f'No *gli*.parquet files found in {indir}')
         return False
-    with xr.open_dataset(files[0]) as gli:
-        for fil in files[1:]:
-            try:
-                with xr.open_dataset(fil) as gli2:
-                    gli = xr.concat([gli, gli2], dim='time')
-            except:
-                pass
-        gli = drop_rogue_1970(gli)
-        gli.to_netcdf(outgli)
+    gli = pl.read_parquet(indir + '/*.gli.sub.*.parquet')
+    gli = drop_pre_1971_samples(gli)
+    gli.write_parquet(outgli)
     _log.info(f'Done writing {outgli}')
 
-    _log.info('Opening *.pld.sub.*.nc multi-file dataset')
-    files = sorted(glob.glob(indir+'/*.pld1.'+kind+'.*.nc'))
+    _log.info('Opening *.pld.sub.*.parquet multi-file dataset')
+    files = sorted(glob.glob(indir + '/*.pld1.' + kind + '.*.parquet'))
     if not files:
-        _log.warning(f'No *{kind}*.nc files found in {indir}')
+        _log.warning(f'No *{kind}*.parquet files found in {indir}')
         return False
-    with xr.open_dataset(files[0]) as pld:
-        for fil in files[1:]:
-            try:
-                with xr.open_dataset(fil) as pld2:
-                    pld = xr.concat([pld, pld2], dim='time')
-            except:
-                pass
-        pld = drop_rogue_1970(pld)
-        pld.to_netcdf(outpld)
+    pld = pl.read_parquet(indir + '/*.pld1.' + kind + '.*.parquet')
+    pld = drop_pre_1971_samples(pld)
+    pld.write_parquet(outpld)
+
     _log.info(f'Done writing {outpld}')
     _log.info('Done merge_rawnc')
     return True
 
 
 def _interp_gli_to_pld(gli, ds, val, indctd):
     gli_ind = ~np.isnan(val)
-    valout = np.interp(ds['time'],
-                       gli['time'][gli_ind],
-                       val[gli_ind])
+    # switch for if we are comparing two polars dataframes or a polars dataframe and a xarray dataset
+    if type(ds) is pl.DataFrame:
+        valout = np.interp(ds["time"],
+                           gli.filter(gli_ind)["time"],
+                           val[gli_ind])
+    else:
+        valout = np.interp(ds['time'].astype(int),
+                           np.array(gli.filter(gli_ind)["time"].to_numpy().astype('datetime64[ns]')).astype(int),
+                           val[gli_ind])
     return valout
 
 
 def _interp_pld_to_pld(pld, ds, val, indctd):
     pld_ind = np.where(~np.isnan(val))[0]
     if len(pld_ind) != len(indctd):
         val = np.interp(ds['time'],
                         pld['time'][pld_ind],
                         val[pld_ind])
     else:
         val = val[indctd]
     return val
 
 
+def _remove_fill_values(df, fill_value=9999):
+    """
+    For input dataframe df, this function converts all Float values equaling fill_values to null. Columns of other
+    datatypes are not affected.
+    """
+    df = df.with_columns(
+        pl.when(pl.col(pl.Float64) == fill_value)
+        .then(None)
+        .otherwise(pl.col(pl.Float64))
+        .name.keep()
+    )
+    return df
+
+
 def raw_to_timeseries(indir, outdir, deploymentyaml, kind='raw',
-                      profile_filt_time=100, profile_min_time=300):
+                      profile_filt_time=100, profile_min_time=300, maxgap=300, interpolate=False, fnamesuffix=''):
     """
     A little different than above, for the 4-file version of the data set.
     """
 
     with open(deploymentyaml) as fin:
         deployment = yaml.safe_load(fin)
     metadata = deployment['metadata']
     ncvar = deployment['netcdf_variables']
     device_data = deployment['glider_devices']
     id = metadata['glider_name']
     _log.info(f'Opening combined nav file {indir}/{id}-rawgli.nc')
-    gli = xr.open_dataset(f'{indir}/{id}-rawgli.nc')
-    _log.info(f'Opening combined payload file {indir}/{id}-{kind}pld.nc')
-    sensor = xr.open_dataset(f'{indir}/{id}-{kind}pld.nc')
+    gli = pl.read_parquet(f'{indir}/{id}-rawgli.parquet')
+    _log.info(f'Opening combined payload file {indir}/{id}-{kind}pld.parquet')
+    sensor = pl.read_parquet(f'{indir}/{id}-{kind}pld.parquet')
+    sensor = _remove_fill_values(sensor)
 
     # build a new data set based on info in `deploymentyaml.`
     # We will use ctd as the interpolant
     ds = xr.Dataset()
     attr = {}
     name = 'time'
     for atts in ncvar[name].keys():
         if atts != 'coordinates':
             attr[atts] = ncvar[name][atts]
 
-    # If present, use the timebase specified in ncva: timebase in the
-    # deployment yaml. Otherwise, the ctd will be our timebase.
-    # It oversamples the nav data, but mildly undersamples the optics and
-    # oxygen....
-    if 'timebase' in ncvar:
-        indctd = np.where(~np.isnan(sensor[ncvar['timebase']['source']]))[0]
-    elif 'GPCTD_TEMPERATURE' in list(sensor.variables):
-        _log.warning('No timebase specified. Using GPCTD_TEMPERATURE as time'
-                     'base')
-        indctd = np.where(~np.isnan(sensor.GPCTD_TEMPERATURE))[0]
-    elif 'LEGATO_TEMPERATURE' in list(sensor.variables):
-        _log.warning('No timebase specified. Using LEGATO_TEMPERATURE as time'
-                     'base')
-        indctd = np.where(~np.isnan(sensor.LEGATO_TEMPERATURE))[0]
-    else:
-        _log.warning('No gpctd or legato data found. Using NAV_DEPTH as time'
-                     'base')
-        indctd = np.where(~np.isnan(sensor.NAV_DEPTH))[0]
-    ds['time'] = (('time'), sensor['time'].values[indctd], attr)
+    # If present, use the timebase specified in ncvar: timebase in the
+    # deployment yaml.
+    if 'timebase' not in ncvar:
+        raise ValueError("Must specify timebase:source in netcdf_variables section of deployment yaml")
+    if ncvar['timebase']['source'] not in sensor.columns:
+        raise ValueError(f"timebase source: {ncvar['timebase']['source']} not found in pld1 columns")
+    vals = sensor.select([ncvar['timebase']['source']]).to_numpy()[:, 0]
+    indctd = np.where(~np.isnan(vals))[0]
+    ds['time'] = (('time'), sensor.select('time').to_numpy()[indctd, 0].astype('datetime64[ns]'), attr)
     thenames = list(ncvar.keys())
-    for i in ['time', 'timebase', 'keep_variables']:
+    # Check yaml to see if interpolate has been set to True
+    if "interpolate" in thenames:
+        if ncvar["interpolate"]:
+            interpolate = True
+    for i in ['time', 'timebase', 'keep_variables', 'interpolate']:
         if i in thenames:
             thenames.remove(i)
     for name in thenames:
         _log.info('interpolating ' + name)
-        if not('method' in ncvar[name].keys()):
+        if not ('method' in ncvar[name].keys()):
             # variables that are in the data set or can be interpolated from it
             if 'conversion' in ncvar[name].keys():
                 convert = getattr(utils, ncvar[name]['conversion'])
             else:
                 convert = utils._passthrough
             sensorname = ncvar[name]['source']
-            if sensorname in list(sensor.variables):
+            if sensorname in list(sensor.columns):
                 _log.debug('sensorname %s', sensorname)
-                val = convert(sensor[sensorname])
+                val = convert(sensor.select(sensorname).to_numpy()[:, 0])
                 if 'coarsen' in ncvar[name]:
-                    # smooth oxygen data as originally perscribed
+                    # coarsen oxygen data as originally perscribed
                     coarsen_time = ncvar[name]['coarsen']
-                    sensor_sub = sensor.coarsen(time=coarsen_time,
-                                                boundary='trim').mean()
-                    val2 = sensor_sub[sensorname]
-                    val = _interp_gli_to_pld(sensor_sub, sensor, val2, indctd)
-                val = val[indctd]
+                    # create a boolean mask of coarsened timesteps. Use this mask to create an array of samples to keep
+                    coarse_ints = np.arange(0, len(sensor) / coarsen_time, 1 / coarsen_time).astype(int)
+                    sensor_sub = sensor.with_columns(pl.lit(coarse_ints).alias("coarse_ints"))
+                    # Subsample the variable data keeping only the samples from the coarsened timeseries
+                    sensor_sub_grouped = sensor_sub.with_columns(
+                        pl.col('time').to_physical()
+                    ).group_by(
+                        pl.col('coarse_ints'),
+                        maintain_order=True
+                    ).mean().with_columns(
+                        pl.col('time').cast(pl.Datetime('ms'))
+                    )[:-1, :]
+                    val2 = sensor_sub_grouped.select(sensorname).to_numpy()[:, 0]
+                    val = _interp_gli_to_pld(sensor_sub_grouped, sensor, val2, indctd)
+                if interpolate and not np.isnan(val).all():
+                    time_original = sensor.select('time').to_numpy()[:, 0]
+                    time_var = time_original[np.where(~np.isnan(val))[0]]
+                    var_non_nan = val[np.where(~np.isnan(val))[0]]
+                    time_timebase = sensor.select('time').to_numpy()[indctd, 0]
+                    if val.dtype == "<M8[us]":
+                        # for datetime, must convert to numerical, interpolate, then convert back
+                        us_since_1970 = (var_non_nan - np.datetime64("1970-01-01")).astype(int)
+                        val_int = np.interp(time_timebase.astype(float), time_var.astype(float), us_since_1970)
+                        val_us = val_int.astype("timedelta64[us]")
+                        val = np.datetime64("1970-01-01") + val_us
+                    else:
+                        val = np.interp(time_timebase.astype(float), time_var.astype(float), var_non_nan)
+
+                    # interpolate only over those gaps that are smaller than 'maxgap'
+                    tg_ind = utils.find_gaps(time_var.astype(float),time_timebase.astype(float),maxgap)
+                    val[tg_ind] = np.nan
+                else:
+                    val = val[indctd]
 
                 ncvar['method'] = 'linear fill'
             else:
-                val = gli[sensorname]
+                val = gli.select(sensorname).to_numpy()[:, 0]
                 val = convert(val)
                 # Values from the glider netcdf must be interpolated to match
                 # the sensor netcdf
                 val = _interp_gli_to_pld(gli, ds, val, indctd)
 
             # make the attributes:
             ncvar[name].pop('coordinates', None)
             attrs = ncvar[name]
             attrs = utils.fill_required_attrs(attrs)
-            ds[name] = (('time'), val.data, attrs)
+            ds[name] = (('time'), val, attrs)
 
     # fix lon and lat to be linearly interpolated between fixes
     good = np.where(np.abs(np.diff(ds.longitude)) +
                     np.abs(np.diff(ds.latitude)) > 0)[0] + 1
     ds['longitude'].values = np.interp(ds.time, ds.time[good],
                                        ds.longitude[good])
     ds['latitude'].values = np.interp(ds.time, ds.time[good],
@@ -356,102 +431,73 @@
     ds = utils.get_glider_depth(ds)
     ds = utils.get_distance_over_ground(ds)
     #    ds = utils.get_profiles(ds)
     ds = utils.get_profiles_new(ds, filt_time=profile_filt_time,
                                 profile_min_time=profile_min_time)
     ds = utils.get_derived_eos_raw(ds)
 
+    # somehow this comes out unsorted:
+    ds = ds.sortby(ds.time)
+    # Drop duplicate timestamps and check how many are removed this way
+    len_before_drop = len(ds.time)
+    if hasattr(ds, "drop_duplicates"):
+        ds = ds.drop_duplicates(dim="time")
+    else:
+        time_diffs = (ds.time.astype(int).diff(dim="time") > 1e-6).values
+        time_diffs_list = list(time_diffs)
+        time_diffs_list.append(True)
+        good = np.array(time_diffs_list)
+        ds = ds.isel(time=good)
+    len_after_drop = len(ds.time)
+    proportion_kept = len_after_drop / len_before_drop
+    loss_str = f"{100 * (1 - proportion_kept)} % samples removed by timestamp deduplication."
+    if proportion_kept < 0.5:
+        raise ValueError(f"{loss_str} Check input data for duplicate timestamps")
+    elif proportion_kept < 0.999:
+        _log.warning(loss_str)
+    else:
+        _log.info(loss_str)
+
     # Correct oxygen if present:
     if 'oxygen_concentration' in ncvar.keys():
         if 'correct_oxygen' in ncvar['oxygen_concentration'].keys():
             ds = utils.oxygen_concentration_correction(ds, ncvar)
         else:
             _log.warning('correct_oxygen not found in oxygen yaml. No'
                          'correction applied')
     ds = ds.assign_coords(longitude=ds.longitude)
     ds = ds.assign_coords(latitude=ds.latitude)
     ds = ds.assign_coords(depth=ds.depth)
     # ds = ds._get_distance_over_ground(ds)
 
     ds = utils.fill_metadata(ds, deployment['metadata'], device_data)
 
-    # somehow this comes out unsorted:
-    ds = ds.sortby(ds.time)
-
     start = ds['time'].values[0]
     end = ds['time'].values[-1]
 
     ds.attrs['deployment_start'] = str(start)
     ds.attrs['deployment_end'] = str(end)
 
     try:
         os.mkdir(outdir)
     except:
         pass
     id0 = ds.attrs['deployment_name']
-    outname = outdir + id0 + '.nc'
+    outname = outdir + id0 + fnamesuffix + '.nc'
     _log.info('writing %s', outname)
     if 'units' in ds.time.attrs.keys():
         ds.time.attrs.pop('units')
     if 'calendar' in ds.time.attrs.keys():
         ds.time.attrs.pop('calendar')
     if 'ad2cp_time' in list(ds):
         if 'units' in ds.ad2cp_time.attrs.keys():
             ds.ad2cp_time.attrs.pop('units')
     ds.to_netcdf(outname, 'w',
-                 encoding={'time': {'units':
-                                    'seconds since 1970-01-01T00:00:00Z'}})
+                 encoding={'time': {'units': 'milliseconds since 1970-01-01T00:00:00Z'}})
     return outname
 
 
-# alias:
+# aliases:
 raw_to_L1timeseries = raw_to_L0timeseries = raw_to_timeseries
+merge_rawnc = merge_parquet
 
-
-def _parse_sensor_config(filename):
-    """
-    Reads the sensor config file of a SeaExplorer and extracts the active
-    sensors and their calibration data.
-
-    Parameters
-    ----------
-    filename: path to seapayload.cfg file
-
-    Returns
-    -------
-
-    Dictionary of devices and their metadata as dictionaries of key_value pairs
-    """
-    # filename =
-    # "/home/callum/Documents/data-flow/data-in/SEA063_M22/2_PLD/configs/seapayload.cfg"
-    file = open(filename, 'r').read().split('\n')
-    devices = []
-    device_id = 'dummy_value'
-    device_dicts = {}
-    dict_for_device = {}
-    for line in file:
-        # Strip trailing whitespace
-        line = line.strip(" ")
-        # Look for key:value pairs
-        if '=' in line and ">" not in line:
-            # Split only on first = or AD2CP will break the parser
-            key, value = line.split("=", 1)
-            # Look for non-empty device declarations
-            if key == "device" and value != "":
-                devices.append(value)
-            else:
-                dict_for_device[key] = value
-        # Look for pattern [devicename]
-        elif line[1:-1] in devices:
-            # add previous device to the device dict
-            device_dicts[device_id] = dict_for_device
-            device_id = line[1:-1]
-            dict_for_device = {}
-    # Append the final device to the dict
-    device_dicts[device_id] = dict_for_device
-
-    active_device_dicts = {k: device_dicts[k] for k in
-                           (device_dicts.keys() & {*devices})}
-    return active_device_dicts
-
-
-__all__ = ['raw_to_rawnc', 'merge_rawnc', 'raw_to_timeseries']
+__all__ = ['raw_to_rawnc', 'merge_parquet', 'raw_to_timeseries']
```

### Comparing `pyglider-0.0.4/pyglider/slocum.py` & `pyglider-0.0.5/pyglider/slocum.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-# -*- coding: utf-8 -*-
 """
 Routines to convert raw slocum dinkum files to netcdf timeseries.
 
 """
 import bitstring
+from datetime import datetime
+try:
+    import dbdreader
+    have_dbdreader = True
+except ImportError:
+    have_dbdreader = True
 import glob
 import logging
 import numpy as np
 import os
 import time
 import xarray as xr
+import xml.etree.ElementTree as ET
 import yaml
+
 import pyglider.utils as utils
-import xml.etree.ElementTree as ET
-from datetime import datetime
 
 
 _log = logging.getLogger(__name__)
 
 
 def binary_to_rawnc(indir, outdir, cacdir,
                     sensorlist, deploymentyaml,
@@ -88,15 +93,15 @@
         deployment_ind_flight = 0
         badfiles = []
         for ind, filen in enumerate(files):
             # sometimes there is no science file for a flight file, so
             # we need to make sure the files match...
             try:
                 fmeta, _ = dbd_get_meta(filen, cachedir=cacdir)
-                path, ext =  os.path.splitext(filen)
+                path, ext = os.path.splitext(filen)
                 fncname = (fmeta['the8x3_filename'] + '.' +
                            fmeta['filename_extension'] + '.nc')
                 fullfncname = outdir + '/' + fncname
 
                 ncfilesexist = os.path.isfile(fullfncname)
                 if incremental and ncfilesexist:
                     ncfilesold = (os.path.getmtime(filen) >=
@@ -105,46 +110,31 @@
                     ncfilesold = True
                 if ncfilesold:
                     fdata, fmeta = dbd_to_dict(
                         filen, cacdir, keys=keys)
                     # need a unique index that increases monotonically, and is
                     # different for each file (we can't use time because it is
                     # not necessarily monotonic):
-                    deployment_ind_flight = (int(fmeta['the8x3_filename']) * 1.0e4)
+                    deployment_ind_flight = (int(fmeta['the8x3_filename']) * 1.0e6)
                     ds, deployment_ind_flight = datameta_to_nc(
                         fdata, fmeta, outdir=outdir, name=fncname,
                         deployment_ind=deployment_ind_flight)
             except Exception as e:
-                badfiles += [filesMain[ind]]
-                _log.warning('Could not do parsing for %s', filesMain[ind])
+                badfiles += [files[ind]]
+                _log.warning('Could not do parsing for %s', files[ind])
                 _log.warning('%s', e)
 
         if len(badfiles) > 0:
             _log.warning('Some files could not be parsed:')
             for fn in badfiles:
                 _log.warning('%s', fn)
 
     _log.info('All done!')
 
 
-def _check_diag_header(diag_tuple):
-    # diagnostic values should be
-    # ['s', 'a', 4660, 123.45600128173828, 123456789.12345] # 4660 is 0x1234
-    ref_tuple = ['s', 'a', 4660, 123.456, 123456789.12345]
-    for i in range(3):
-        if ref_tuple[i] != diag_tuple[i]:
-            _log.warning('character or int failure: %s', diag_tuple)
-            return False
-    if ((abs(ref_tuple[3] - diag_tuple[3]) > .0001) or
-            (abs(ref_tuple[4] - diag_tuple[4]) > .0001)):
-        _log.warning('floating point failure')
-        return False
-    return True
-
-
 def _decode_sensor_info(dfh, meta):
     """
     Helper to decode the sensor list.
 
     dfh must be a filehandle because we want to be able to say where we stopped
     in file.
     """
@@ -315,23 +305,49 @@
     activeSensorList = meta['activeSensorList']
     dfh = open(dinkum_file, 'rb')
     # ------------------------------------------
     # All subsequent lines are in binary format.
     # Grab the seek pos and use that for a bookmark.
     # ------------------------------------------
     # offset for number of characters already read in.
+    _log.debug('reading file from %d', bindatafilepos * 8)
     binaryData = bitstring.BitStream(dfh, offset=bindatafilepos * 8)
     # First there's the s,a,2byte int, 4 byte float, 8 byte double.
-    diag_header = binaryData.readlist(['bits:8', 'bits:8',
-                                       'uint:16', 'float:32', 'float:64'])
+    # sometimes the endianess seems to get swapped.
+    # ref_tuple = ['s', 'a', 4660, 123.456, 123456789.12345]
+    diag_header = binaryData.readlist(['bits:8', 'bits:8'])
     diag_header[0] = chr(int(diag_header[0].hex, 16))
     diag_header[1] = chr(int(diag_header[1].hex, 16))
-    if not _check_diag_header(diag_header):
+    if not (diag_header[0] == 's') and (diag_header[1] == 'a'):
+        _log.warning("character failure: %s != 's', 'a'", diag_header)
         raise ValueError('Diagnostic header check failed.')
 
+    endian = 'be'
+    data = binaryData.read(f'uint{endian}:16')
+    _log.debug('Checking endianness %s == 4660 or 13330', data)
+    if data == 4660:
+        pass
+    elif data == 13330:
+        endian = 'le'
+    else:
+        _log.warning("integer failure: %s != 4660", data)
+        raise ValueError("Diagnostic header check failed.")
+    _log.debug('Endianness is %s', endian)
+
+    data = binaryData.read(f'float{endian}:32')
+    if not np.allclose(data, 123.456):
+        _log.warning("float32 failure: %s != 123.456", data)
+        raise ValueError("Diagnostic header check failed.")
+
+    data = binaryData.read(f'float{endian}:64')
+    if not np.allclose(data, 123456789.12345):
+        _log.warning("float64 failure: %s != 123456789.12345", data)
+        raise ValueError("Diagnostic header check failed.")
+    _log.debug('Diagnostic check passed.  Endian is %s', endian)
+
     nsensors = int(meta['sensors_per_cycle'])
     currentValues = np.zeros(int(meta['sensors_per_cycle'])) + np.NaN
     data = np.zeros((DINKUMCHUNKSIZE, nsensors)) + np.NaN
     # Then there's a data cycle with every sensor marked as updated, giving
     # us our initial values.
     # 01 means updated with 'same value', 10 means updated with a new value,
     # 11 is reserved, 00 is not updated.
@@ -356,28 +372,36 @@
             if code == '00':  # No new value
                 currentValues[i] = np.NaN
             elif code == '01':  # Same value as before.
                 continue
             elif code == '10':  # New value.
                 if int(activeSensorList[i]['bits']) in [4, 8]:
                     currentValues[i] = binaryData.read(
-                        'float:' + str(int(activeSensorList[i]['bits']) * 8))
-                    # print currentValues[i], activeSensorList[i]['name']
+                        f'float{endian}:' +
+                        str(int(activeSensorList[i]['bits']) * 8))
                 elif int(activeSensorList[i]['bits']) in [1, 2]:
                     currentValues[i] = binaryData.read(
-                        'uint:' + str(int(activeSensorList[i]['bits']) * 8))
+                        f'uint{endian}:' +
+                        str(int(activeSensorList[i]['bits']) * 8))
                 else:
                     raise ValueError('Bad bits')
             else:
                 raise ValueError(('Unrecognizable code in data cycle. ',
                                   'Parsing failed'))
         data[ndata] = currentValues
         binaryData.bytealign()
+
         # We've arrived at the next line.
-        d = binaryData.peek('bytes:1').decode('utf-8')
+        try:
+            d = binaryData.peek('bytes:1').decode('utf-8')
+        except bitstring.ReadError:
+            _log.debug('position at end of stream %d',
+                       binaryData.pos + 8 * bindatafilepos)
+            _log.warning('End of file reached without termination char')
+            d = 'X'
         if d == 'd':
             frameCheck = binaryData.read('bytes:1').decode('utf-8')
             ndata += 1
             if ndata % DINKUMCHUNKSIZE == 0:
                 # need to allocate more data!
                 data = np.concatenate(
                     (data, np.NaN + np.zeros((DINKUMCHUNKSIZE, nsensors))),
@@ -611,33 +635,33 @@
     for f in fin:
         with xr.open_dataset(f) as ds:
             if len(ds._ind) < 2:
                 bad = True
             else:
                 bad = False
         if bad:
-            print(ds)
             os.rename(f, f+'.singleton')
             fglider = f
             try:
                 fglider = fglider.replace(scisuffix, glidersuffix)
                 os.rename(fglider, fglider+'.singleton')
             except FileNotFoundError:
                 pass
 
     fin = glob.glob(indir + '/*.' + glidersuffix + '.nc')
     with xr.open_mfdataset(fin, decode_times=False, lock=False) as ds:
-        outnebd = outdir + '/' + id + f'rawdbd.nc'
+        outnebd = outdir + '/' + id + 'rawdbd.nc'
         ds = ds.sortby('time')
         ds['_ind'] = np.arange(len(ds.time))
         ds.to_netcdf(outnebd, 'w')
 
     fin = glob.glob(indir + '/*.' + scisuffix + '.nc')
+
     with xr.open_mfdataset(fin, decode_times=False, lock=False) as ds:
-        outnebd = outdir + '/' + id + f'rawebd.nc'
+        outnebd = outdir + '/' + id + 'rawebd.nc'
         ds = ds.sortby('time')
         ds['_ind'] = np.arange(len(ds.time))
         ds.to_netcdf(outnebd, 'w')
 
 
 def raw_to_timeseries(indir, outdir, deploymentyaml, *,
                       profile_filt_time=100, profile_min_time=300):
@@ -650,15 +674,14 @@
         Directory to put the merged timeseries files.
     profile_filt_time : float
         time in seconds over which to smooth the pressure time series for
         finding up and down profiles (note, doesn't filter the data that is
         saved)
     profile_min_time : float
         minimum time to consider a profile an actual profile (seconds)
-
     Returns
     -------
     outname : string
         name of the new merged netcdf file.
     """
 
     with open(deploymentyaml) as fin:
@@ -668,111 +691,264 @@
     device_data = deployment['glider_devices']
     thenames = list(ncvar.keys())
     thenames.remove('time')
 
     id = metadata['glider_name'] + metadata['glider_serial']
 
     id0 = None
-    prev_profile = 0
-    for mnum in range(0, 1):
-        ebdn = indir + '/' + id + 'rawebd.nc'
-        dbdn = indir + '/' + id + 'rawdbd.nc'
-        _log.debug(f'{ebdn}, {dbdn}')
-        if not os.path.exists(ebdn) or not os.path.exists(dbdn):
+    ebdn = indir + '/' + id + 'rawebd.nc'
+    dbdn = indir + '/' + id + 'rawdbd.nc'
+    _log.debug(f'{ebdn}, {dbdn}')
+    if not os.path.exists(ebdn) or not os.path.exists(dbdn):
+        raise FileNotFoundError('Could not find %s and %s', ebdn, dbdn)
+
+    _log.info('Opening:', ebdn, dbdn)
+    ebd = xr.open_dataset(ebdn, decode_times=False)
+    dbd = xr.open_dataset(dbdn, decode_times=False)
+    _log.debug(f'DBD, {dbd}, {dbd.m_depth}')
+    if len(ebd.time) <= 2:
+        raise RuntimeError('Science file has no data')
+    # build a new data set based on info in `deployment.`
+    # We will use ebd.m_present_time as the interpolant if the
+    # variable is in dbd.
+    ds = xr.Dataset()
+    attr = {}
+    name = 'time'
+    for atts in ncvar[name].keys():
+        if atts != 'coordinates':
+            attr[atts] = ncvar[name][atts]
+    ds[name] = (('time'), ebd[name].values, attr)
+
+    for name in thenames:
+        _log.info('working on %s', name)
+        if 'method' in ncvar[name].keys():
             continue
+        # variables that are in the data set or can be interpolated from it
+        if 'conversion' in ncvar[name].keys():
+            convert = getattr(utils, ncvar[name]['conversion'])
+        else:
+            convert = utils._passthrough
+        sensorname = ncvar[name]['source']
+        _log.info('names: %s %s', name, sensorname)
+        if sensorname in ebd.keys():
+            _log.debug('EBD sensorname %s', sensorname)
+            val = ebd[sensorname]
+            val = utils._zero_screen(val)
+    #        val[val==0] = np.NaN
+            val = convert(val)
+        else:
+            _log.debug('DBD sensorname %s', sensorname)
+            val = convert(dbd[sensorname])
+            val = _dbd2ebd(dbd, ds, val)
+            ncvar['method'] = 'linear fill'
+        # make the attributes:
+        ncvar[name].pop('coordinates', None)
+        attrs = ncvar[name]
+        attrs = utils.fill_required_attrs(attrs)
+        ds[name] = (('time'), val.data, attrs)
+
+    _log.debug(f'HERE, {ds}')
+    _log.debug(f'HERE, {ds.pressure[0:100]}')
+    # some derived variables:
+    # trim bad times...
+
+    ds = utils.get_glider_depth(ds)
+    ds = utils.get_distance_over_ground(ds)
+
+    ds = utils.get_derived_eos_raw(ds)
+    ds = ds.assign_coords(longitude=ds.longitude)
+    ds = ds.assign_coords(latitude=ds.latitude)
+    ds = ds.assign_coords(depth=ds.depth)
+
+    ds['time'] = (ds.time.values.astype('timedelta64[s]') +
+                  np.datetime64('1970-01-01T00:00:00')).astype('datetime64[ns]')
+    ds = utils.fill_metadata(ds, deployment['metadata'], device_data)
+    start = ds['time'].values[0]
+    end = ds['time'].values[-1]
+
+    ds.attrs['deployment_start'] = str(start)
+    ds.attrs['deployment_end'] = str(end)
+    _log.debug(ds.depth.values[:100])
+    _log.debug(ds.depth.values[2000:2100])
+    ds = utils.get_profiles_new(
+        ds, filt_time=profile_filt_time, profile_min_time=profile_min_time)
+    _log.debug(ds.depth.values[:100])
+    _log.debug(ds.depth.values[2000:2100])
+
+    try:
+        os.mkdir(outdir)
+    except:
+        pass
+    outname = (outdir + '/' + ds.attrs['deployment_name'] + '.nc')
+    _log.info('writing %s', outname)
+    ds.to_netcdf(outname, 'w',
+                 encoding={'time': {'units': 'seconds since 1970-01-01T00:00:00Z'}})
+    if id0 is None:
+        id0 = ds.attrs['deployment_name']
 
-        _log.info('Opening:', ebdn, dbdn)
-        ebd = xr.open_dataset(ebdn, decode_times=False)
-        dbd = xr.open_dataset(dbdn, decode_times=False)
-        _log.debug(f'DBD, {dbd}, {dbd.m_depth}')
-        if len(ebd.time) <= 2:
+    return outname
+
+
+def binary_to_timeseries(indir, cachedir, outdir, deploymentyaml, *,
+                         search='*.[D|E]BD', fnamesuffix='',
+                         time_base='sci_water_temp', profile_filt_time=100,
+                         profile_min_time=300, maxgap=300):
+    """
+    Convert directly from binary files to netcdf timeseries file.  Requires
+    dbdreader to be installed.
+
+    Parameters
+    ----------
+    indir : string
+        Directory with binary files from the glider.
+
+    cachedir : string
+        Directory with glider cache files (cac files)
+
+    outdir : string
+        Directory to put the merged timeseries files.
+
+    deploymentyaml : str
+        YAML text file with deployment information for this glider.
+
+    profile_filt_time : float
+        time in seconds over which to smooth the pressure time series for
+        finding up and down profiles (note, doesn't filter the data that is
+        saved)
+
+    profile_min_time : float
+        minimum time to consider a profile an actual profile (seconds)
+
+    Returns
+    -------
+    outname : string
+        name of the new merged netcdf file.
+    """
+
+    if not have_dbdreader:
+        raise ImportError('Cannot import dbdreader')
+
+    with open(deploymentyaml) as fin:
+        deployment = yaml.safe_load(fin)
+    ncvar = deployment['netcdf_variables']
+    device_data = deployment['glider_devices']
+    thenames = list(ncvar.keys())
+    thenames.remove('time')
+
+    # get the dbd file
+    _log.info(f'{indir}/{search}')
+    dbd = dbdreader.MultiDBD(pattern=f'{indir}/{search}',
+                             cacheDir=cachedir)
+
+    # build a new data set based on info in `deployment.`
+    # We will use ebd.m_present_time as the interpolant if the
+    # variable is in dbd.
+    ds = xr.Dataset()
+    attr = {}
+    name = 'time'
+    for atts in ncvar[name].keys():
+        if (atts != 'coordinates') & (atts != 'units') & (atts != 'calendar'):
+            attr[atts] = ncvar[name][atts]
+    sensors = [time_base]
+
+    for nn, name in enumerate(thenames):
+        sensorname = ncvar[name]['source']
+        if not sensorname == time_base:
+            sensors.append(sensorname)
+        else:
+            baseind = nn
+
+    # get the data, with `time_base` as the time source that
+    # all other variables are synced to:
+    data = list(dbd.get_sync(*sensors))
+    # get the time:
+    time = data.pop(0)
+    ds['time'] = (('time'), time, attr)
+    # get the time_base data:
+    basedata = data.pop(0)
+    # slot the time_base variable into the right place in the
+    # data list:
+    data.insert(baseind, basedata)
+
+    for nn, name in enumerate(thenames):
+        _log.info('working on %s', name)
+        if 'method' in ncvar[name].keys():
             continue
-        # build a new data set based on info in `deployment.`
-        # We will use ebd.m_present_time as the interpolant if the
-        # variable is in dbd.
-        ds = xr.Dataset()
-        attr = {}
-        name = 'time'
-        for atts in ncvar[name].keys():
-            if atts != 'coordinates':
-                attr[atts] = ncvar[name][atts]
-        ds[name] = (('time'), ebd[name].values, attr)
-
-        for name in thenames:
-            _log.info('working on %s', name)
-            if 'method' in ncvar[name].keys():
-                continue
-            # variables that are in the data set or can be interpolated from it
-            if 'conversion' in ncvar[name].keys():
-                convert = getattr(utils, ncvar[name]['conversion'])
-            else:
-                convert = utils._passthrough
-            sensorname = ncvar[name]['source']
-            _log.info('names: %s %s', name, sensorname)
-            if sensorname in ebd.keys():
-                _log.debug('EBD sensorname %s', sensorname)
-                val = ebd[sensorname]
-                val = utils._zero_screen(val)
-        #        val[val==0] = np.NaN
-                val = convert(val)
-            else:
-                _log.debug('DBD sensorname %s', sensorname)
-                val = convert(dbd[sensorname])
-                val = _dbd2ebd(dbd, ds, val)
-                ncvar['method'] = 'linear fill'
-            # make the attributes:
-            ncvar[name].pop('coordinates', None)
-            attrs = ncvar[name]
-            attrs = utils.fill_required_attrs(attrs)
-            ds[name] = (('time'), val.data, attrs)
-
-        _log.debug(f'HERE, {ds}')
-        _log.debug(f'HERE, {ds.pressure[0:100]}')
-        # some derived variables:
-        # trim bad times...
-        #ds = ds.sel(time=slice(1e8, None))
-
-        ds = utils.get_glider_depth(ds)
-
-        ds = utils.get_distance_over_ground(ds)
-
-        # ds = utils.get_profiles(ds)
-        # ds['profile_index'] = ds.profile_index + prev_profile
-
-        #ind = np.where(np.isfinite(ds.profile_index))[0]
-        #prev_profile = ds.profile_index.values[ind][-1]
-        ds = utils.get_derived_eos_raw(ds)
-        ds = ds.assign_coords(longitude=ds.longitude)
-        ds = ds.assign_coords(latitude=ds.latitude)
-        ds = ds.assign_coords(depth=ds.depth)
-
-        #ds = ds._get_distance_over_ground(ds)
-        ds['time'] = ds.time.values.astype('timedelta64[s]') + np.datetime64('1970-01-01T00:00:00')
-        ds = utils.fill_metadata(ds, deployment['metadata'], device_data)
-        start = ds['time'].values[0]
-        end = ds['time'].values[-1]
-
-        ds.attrs['deployment_start'] = str(start)
-        ds.attrs['deployment_end'] = str(end)
-        _log.debug(ds.depth.values[:100])
-        _log.debug(ds.depth.values[2000:2100])
-        ds = utils.get_profiles_new(
-            ds, filt_time=profile_filt_time, profile_min_time=profile_min_time)
-        _log.debug(ds.depth.values[:100])
-        _log.debug(ds.depth.values[2000:2100])
+        # variables that are in the data set or can be interpolated from it
+        if 'conversion' in ncvar[name].keys():
+            convert = getattr(utils, ncvar[name]['conversion'])
+        else:
+            convert = utils._passthrough
 
-        try:
-            os.mkdir(outdir)
-        except:
-            pass
-        outname = (outdir + '/' + ds.attrs['deployment_name'] + '.nc')
-        _log.info('writing %s', outname)
-        ds.to_netcdf(outname, 'w', encoding={'time': {'units': 'seconds since 1970-01-01T00:00:00Z'}})
-        if id0 is None:
-            id0 = ds.attrs['deployment_name']
+        sensorname = ncvar[name]['source']
+        _log.info('names: %s %s', name, sensorname)
+        if sensorname in dbd.parameterNames['sci']:
+            _log.debug('Sci sensorname %s', sensorname)
+            val = data[nn]
+
+            # interpolate only over those gaps that are smaller than 'maxgap'
+            _t, _ = dbd.get(ncvar[name]['source'])
+            tg_ind = utils.find_gaps(_t,time,maxgap)
+            val[tg_ind] = np.nan
+
+            val = utils._zero_screen(val)
+            val = convert(val)
+        elif sensorname in dbd.parameterNames['eng']:
+            _log.debug('Eng sensorname %s', sensorname)
+            val = data[nn]
+            val = convert(val)
+            ncvar['method'] = 'linear fill'
+        else:
+            ValueError(f'{sensorname} not in science or eng parameter names')
+
+        # make the attributes:
+        ncvar[name].pop('coordinates', None)
+        attrs = ncvar[name]
+        attrs = utils.fill_required_attrs(attrs)
+        ds[name] = (('time'), val, attrs)
+
+    _log.info(f'Getting glider depths, {ds}')
+    _log.debug(f'HERE, {ds.pressure[0:100]}')
+
+    ds = utils.get_glider_depth(ds)
+    ds = utils.get_distance_over_ground(ds)
+
+    ds = utils.get_derived_eos_raw(ds)
+    ds = ds.assign_coords(longitude=ds.longitude)
+    ds = ds.assign_coords(latitude=ds.latitude)
+    ds = ds.assign_coords(depth=ds.depth)
+
+    # screen out-of-range times; these won't convert:
+    ds['time'] = ds.time.where((ds.time>0) & (ds.time<6.4e9), np.NaN)
+    ds['time'] = (('time'), (ds.time.values.astype('timedelta64[s]') +
+                  np.datetime64('1970-01-01T00:00:00')).astype('datetime64[ns]'), attr)
+
+    ds = utils.fill_metadata(ds, deployment['metadata'], device_data)
+    start = ds['time'].values[0]
+    end = ds['time'].values[-1]
+    _log.debug('Long')
+    _log.debug(ds.longitude.values[-2000:])
+    ds.attrs['deployment_start'] = str(start)
+    ds.attrs['deployment_end'] = str(end)
+    _log.debug(ds.depth.values[:100])
+    _log.debug(ds.depth.values[2000:2100])
+
+    ds = utils.get_profiles_new(
+        ds, filt_time=profile_filt_time, profile_min_time=profile_min_time)
+    _log.debug(ds.depth.values[:100])
+    _log.debug(ds.depth.values[2000:2100])
+
+    try:
+        os.mkdir(outdir)
+    except:
+        pass
+    outname = (outdir + '/' + ds.attrs['deployment_name'] + fnamesuffix + '.nc')
+    _log.info('writing %s', outname)
+    ds.to_netcdf(outname, 'w',
+                 encoding={'time': {'units': 'seconds since 1970-01-01T00:00:00Z'}})
 
     return outname
 
 
 # alias:
 raw_to_L1timeseries = raw_to_L0timeseries = raw_to_timeseries
 
@@ -869,46 +1045,46 @@
     gps = [''] * 10000
     amph = [''] * 10000
     ntimes = 0
     for fn in files:
         found_time = False
 
         with open(fn, 'r') as fin:
-            for l in fin:
-                if 'Curr Time:' in l:
-                    times[ntimes] = l
+            for ll in fin:
+                if 'Curr Time:' in ll:
+                    times[ntimes] = ll
                     ntimes += 1
-                    found_time=True
-                if found_time and 'GPS Location' in l:
-                    gps[ntimes - 1] = l
-                if found_time and "sensor:m_coulomb_amphr_total" in l:
-                    amph[ntimes-1] = l
+                    found_time = True
+                if found_time and 'GPS Location' in ll:
+                    gps[ntimes - 1] = ll
+                if found_time and "sensor:m_coulomb_amphr_total" in ll:
+                    amph[ntimes-1] = ll
     amph = amph[:ntimes]
     gps = gps[:ntimes]
     times = times[:ntimes]
 
     # now parse them
-    out = xr.Dataset(coords={'time': ('surfacing', np.zeros(ntimes, dtype='datetime64[s]'))})
+    out = xr.Dataset(
+        coords={'time': ('surfacing', np.zeros(ntimes, dtype='datetime64[ns]'))})
     out['ampH'] = ('surfacing', np.zeros(ntimes) * np.NaN)
     out['lon'] = ('surfacing', np.zeros(ntimes) * np.NaN)
     out['lat'] = ('surfacing', np.zeros(ntimes) * np.NaN)
 
     for i in range(ntimes):
         timestring = times[i][11:-13]
-        out['time'][i] = np.datetime64(datetime.strptime(timestring, '%a %b %d %H:%M:%S %Y'))
         try:
+            out['time'][i] = np.datetime64(
+                datetime.strptime(timestring, '%a %b %d %H:%M:%S %Y'), 'ns')
             st = amph[i].index('=')
             en = amph[i][st:].index(' ') + st
             out['ampH'][i] = float(amph[i][(st+1):en])
-
-            #        GPS Location:  4912.737 N -12357.253 E measured    110.757 secs ago
             sp = gps[i].split(' ')
             out['lat'][i] = utils.nmea2deg(float(sp[3]))
             out['lon'][i] = utils.nmea2deg(float(sp[5]))
         except:
             pass
 
     return out
 
 
 __all__ = ['binary_to_rawnc', 'merge_rawnc', 'raw_to_timeseries',
-           'parse_glider_state', 'parse_logfiles']
+           'parse_gliderState', 'parse_logfiles']
```

### Comparing `pyglider-0.0.4/pyglider/utils.py` & `pyglider-0.0.5/pyglider/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,18 +26,19 @@
     ds : `.xarray.Dataset`
         With ``distance_over_ground`` key.
     """
     good = ~np.isnan(ds.latitude + ds.longitude)
     dist = gsw.distance(ds.longitude[good].values, ds.latitude[good].values)/1000
     dist = np.roll(np.append(dist, 0), 1)
     dist = np.cumsum(dist)
+    dist = np.interp(ds.time, ds.time[good], dist)
     attr = {'long_name': 'distance over ground flown since mission start',
-     'method': 'get_distance_over_ground',
-     'units': 'km',
-     'sources': 'latitude longitude'}
+            'method': 'get_distance_over_ground',
+            'units': 'km',
+            'sources': 'latitude longitude'}
     ds['distance_over_ground'] = (('time'), dist, attr)
     return ds
 
 
 def get_glider_depth(ds):
     """
     Get glider depth from pressure sensor.
@@ -53,41 +54,43 @@
     ds : `.xarray.Dataset`
         With ``depth`` key.
 
     """
     good = np.where(~np.isnan(ds.pressure))[0]
     ds['depth'] = ds.pressure * 0.
     ds['depth'].values = -gsw.z_from_p(ds.pressure.values,
-            ds.latitude.values)
+                                       ds.latitude.values)
     # now we really want to know where it is, so interpolate:
     if len(good) > 0:
-        ds['depth'].values = np.interp(np.arange(len(ds.depth)),
-                                good, ds['depth'].values[good])
+        ds['depth'].values = np.interp(
+            np.arange(len(ds.depth)), good, ds['depth'].values[good])
 
     attr = {'source': 'pressure', 'long_name': 'glider depth',
             'standard_name': 'depth', 'units': 'm',
             'comment': 'from science pressure and interpolated',
+            'instrument': 'instrument_ctd',
             'observation_type': 'calulated',
             'accuracy': '1', 'precision': '2', 'resolution': '0.02',
+            'platform': 'platform',
             'valid_min': '0', 'valid_max': '2000',
             'reference_datum': 'surface', 'positive': 'down'}
     ds['depth'].attrs = attr
     return ds
 
 
-def get_profiles(ds, min_dp = 10.0, inversion=3., filt_length=7,
+def get_profiles(ds, min_dp=10.0, inversion=3., filt_length=7,
                  min_nsamples=14):
     """
     Not currently used...
 
     make two variables: profile_direction and profile_index; this version
     is good for lots of data.  Less good for sparse data
     """
-    profile = ds.pressure.values * 0
-    direction = ds.pressure.values * 0
+    profile = ds.pressure.values * np.NaN
+    direction = ds.pressure.values * np.NaN
     pronum = 1
     lastpronum = 0
 
     good = np.where(~np.isnan(ds.pressure))[0]
     p = np.convolve(ds.pressure.values[good],
                     np.ones(filt_length) / filt_length, 'same')
     dpall = np.diff(p)
@@ -101,70 +104,73 @@
             direction[inds] = np.sign(dp)
             profile[inds] = pronum
             lastpronum = pronum
             pronum += 1
         else:
             profile[good[inflect[n]]:good[inflect[n+1]]] = lastpronum + 0.5
 
-    attrs = collections.OrderedDict([('long_name', 'profile index'),
-             ('units', '1'),
-             ('comment',
-              'N = inside profile N, N + 0.5 = between profiles N and N + 1'),
-             ('sources', 'time pressure'),
-             ('method', 'get_profiles'),
-             ('min_dp', min_dp),
-             ('filt_length', filt_length),
-             ('min_nsamples', min_nsamples)])
+    attrs = collections.OrderedDict([
+        ('long_name', 'profile index'),
+        ('units', '1'),
+        ('comment',
+         'N = inside profile N, N + 0.5 = between profiles N and N + 1'),
+        ('sources', 'time pressure'),
+        ('method', 'get_profiles'),
+        ('min_dp', min_dp),
+        ('filt_length', filt_length),
+        ('min_nsamples', min_nsamples)])
     ds['profile_index'] = (('time'), profile, attrs)
 
-
-    attrs = collections.OrderedDict([('long_name', 'glider vertical speed direction'),
-             ('units', '1'),
-             ('comment',
-              '-1 = ascending, 0 = inflecting or stalled, 1 = descending'),
-             ('sources', 'time pressure'),
-             ('method', 'get_profiles')])
+    attrs = collections.OrderedDict([
+        ('long_name', 'glider vertical speed direction'),
+        ('units', '1'),
+        ('comment',
+         '-1 = ascending, 0 = inflecting or stalled, 1 = descending'),
+        ('sources', 'time pressure'),
+        ('method', 'get_profiles')])
     ds['profile_direction'] = (('time'), direction, attrs)
     return ds
 
 
-def get_profiles_new(ds, min_dp = 10.0, filt_time=100, profile_min_time=300):
+def get_profiles_new(ds, min_dp=10.0, filt_time=100, profile_min_time=300):
     """
     Find profiles in a glider timeseries:
 
     Parameters
     ----------
     ds : `xarray.Dataset`
         Must have *time* coordinate and *pressure* as a variable
     min_dp : float, default=10.0
         Minimum distance a profile must transit to be considered a profile, in dbar.
     filt_time : float, default=100
         Approximate length of time filter, in seconds.  Note that the filter
-        is really implemented by sample, so the number of samples is ``filt_time / dt``
+        is really implemented by sample, so the number of samples is
+        ``filt_time / dt``
         where *dt* is the median time between samples in the time series.
     profile_min_time : float, default=300
         Minimum time length of profile in s.
     """
 
     profile = ds.pressure.values * 0
     direction = ds.pressure.values * 0
     pronum = 1
 
     good = np.where(np.isfinite(ds.pressure))[0]
-    #dt = float(np.median(np.diff(ds.time.values[good[:200000]])))
-    dt = float(np.median(np.diff(ds.time.values[good[:200000]]).astype(np.float64)) * 1e-9)
+    dt = float(np.median(
+        np.diff(ds.time.values[good[:200000]]).astype(np.float64)) * 1e-9)
     _log.info(f'dt, {dt}')
-    filt_length = int(filt_time /  dt)
+    filt_length = int(filt_time / dt)
 
     min_nsamples = int(profile_min_time / dt)
     _log.info('Filt Len  %d, dt %f, min_n %d', filt_length, dt, min_nsamples)
-
-    p = np.convolve(ds.pressure.values[good],
-                    np.ones(filt_length) / filt_length, 'same')
-    _log.info('ffilt, {filt_length}')
+    if filt_length > 1:
+        p = np.convolve(ds.pressure.values[good],
+                        np.ones(filt_length) / filt_length, 'same')
+    else:
+        p = ds.pressure.values[good]
     decim = int(filt_length / 3)
     if decim < 2:
         decim = 2
     # why?  because argrelextrema doesn't like repeated values, so smooth
     # then decimate to get fewer values:
     pp = p[::decim]
     maxs = argrelextrema(pp, np.greater)[0]
@@ -177,61 +183,65 @@
         mins = np.concatenate((mins, good[[-1]]))
 
     _log.debug(f'mins: {len(mins)} {mins} , maxs: {len(maxs)} {maxs}')
 
     pronum = 0
     p = ds.pressure
     nmin = 0
-    nmax=0
+    nmax = 0
     while (nmin < len(mins)) and (nmax < len(maxs)):
-        nmax = np.where(maxs>mins[nmin])[0]
+        nmax = np.where(maxs > mins[nmin])[0]
         if len(nmax) >= 1:
             nmax = nmax[0]
         else:
             break
         _log.debug(nmax)
         ins = range(int(mins[nmin]), int(maxs[nmax]+1))
         _log.debug(f'{pronum}, {ins}, {len(p)}, {mins[nmin]}, {maxs[nmax]}')
         _log.debug(f'Down, {ins}, {p[ins[0]].values},{p[ins[-1]].values}')
-        if (len(ins) > min_nsamples and np.nanmax(p[ins]) - np.nanmin(p[ins]) > min_dp):
+        if ((len(ins) > min_nsamples) and
+                (np.nanmax(p[ins]) - np.nanmin(p[ins]) > min_dp)):
             profile[ins] = pronum
             direction[ins] = +1
             pronum += 1
-        nmin = np.where(mins>maxs[nmax])[0]
+        nmin = np.where(mins > maxs[nmax])[0]
         if len(nmin) >= 1:
             nmin = nmin[0]
         else:
             break
         ins = range(maxs[nmax], mins[nmin])
         _log.debug(f'{pronum}, {ins}, {len(p)}, {mins[nmin]}, {maxs[nmax]}')
         _log.debug(f'Up, {ins}, {p[ins[0]].values}, {p[ins[-1]].values}')
-        if (len(ins) > min_nsamples and np.nanmax(p[ins]) - np.nanmin(p[ins]) > min_dp):
+        if ((len(ins) > min_nsamples) and
+                (np.nanmax(p[ins]) - np.nanmin(p[ins]) > min_dp)):
             # up
             profile[ins] = pronum
             direction[ins] = -1
             pronum += 1
 
     _log.debug('Doing this...')
-    attrs = collections.OrderedDict([('long_name', 'profile index'),
-             ('units', '1'),
-             ('comment',
-              'N = inside profile N, N + 0.5 = between profiles N and N + 1'),
-             ('sources', 'time pressure'),
-             ('method', 'get_profiles_new'),
-             ('min_dp', min_dp),
-             ('filt_length', filt_length),
-             ('min_nsamples', min_nsamples)])
+    attrs = collections.OrderedDict([
+        ('long_name', 'profile index'),
+        ('units', '1'),
+        ('comment',
+         'N = inside profile N, N + 0.5 = between profiles N and N + 1'),
+        ('sources', 'time pressure'),
+        ('method', 'get_profiles_new'),
+        ('min_dp', min_dp),
+        ('filt_length', filt_length),
+        ('min_nsamples', min_nsamples)])
     ds['profile_index'] = (('time'), profile, attrs)
 
-    attrs = collections.OrderedDict([('long_name', 'glider vertical speed direction'),
-             ('units', '1'),
-             ('comment',
-              '-1 = ascending, 0 = inflecting or stalled, 1 = descending'),
-             ('sources', 'time pressure'),
-             ('method', 'get_profiles_new')])
+    attrs = collections.OrderedDict([
+        ('long_name', 'glider vertical speed direction'),
+        ('units', '1'),
+        ('comment',
+         '-1 = ascending, 0 = inflecting or stalled, 1 = descending'),
+        ('sources', 'time pressure'),
+        ('method', 'get_profiles_new')])
     ds['profile_direction'] = (('time'), direction, attrs)
     return ds
 
 
 def get_derived_eos_raw(ds):
     """
     Calculate salinity, potential density, density, and potential temperature
@@ -249,109 +259,112 @@
         as new variables.
 
     Notes
     -----
     Thermodynamic variables derived from the Gibbs seawater toolbox ``import gsw``.
 
     - *salinity*::
-
         gsw.conversions.SP_from_C(r, ds.temperature, ds.pressure)
-
     - *potential_density*::
-
-        sa = gsw.SA_from_SP(ds['salinity'], ds['pressure'], ds['longitude'], ds['latitude'])
+        sa = gsw.SA_from_SP(ds['salinity'], ds['pressure'],
+                            ds['longitude'], ds['latitude'])
         ct = gsw.CT_from_t(sa, ds['temperature'], ds['pressure'])
-        ds['potential_density'] = (('time'), 1000 + gsw.density.sigma0(sa, ct).values)
+        ds['potential_density'] = (('time'),
+                1000 + gsw.density.sigma0(sa, ct).values)
     - *density*::
-
         ds['density'] = (('time'), gsw.density.rho(
             ds.salinity, ds.temperature, ds.pressure).values)
     - *potential_temperature*::
-
         ds['potential_temperature'] = (('time'), gsw.conversions.pt0_from_t(
             ds.salinity, ds.temperature, ds.pressure).values)
 
     """
 
-    # GPCTD and slocum ctd require a scale factor of 10 for conductivity. Legato does not
+    # GPCTD and slocum ctd require a scale factor of 10 for conductivity.
+    # Legato does not
     if 'S m' in ds.conductivity.units:
         r = 10 * ds.conductivity
     elif 'mS cm' in ds.conductivity.units:
         r = ds.conductivity
     else:
-        raise ValueError("Could not parse conductivity units in yaml. Expected 'S m-1' or 'mS cm-1'. "
+        raise ValueError("Could not parse conductivity units in yaml. "
+                         "Expected 'S m-1' or 'mS cm-1'. "
                          "Check yaml entry netcdf_variables: conductivity: units")
-    ds['salinity'] = (('time'),
-                      gsw.conversions.SP_from_C(r, ds.temperature, ds.pressure).values)
-    attrs = collections.OrderedDict([('long_name', 'water salinity'),
-             ('standard_name', 'sea_water_practical_salinity'),
-             ('units', '1e-3'),
-             ('comment', 'raw, uncorrected salinity'),
-             ('sources', 'conductivity temperature pressure'),
-             ('method', 'get_derived_eos_raw'),
-             ('observation_type', 'calulated'),
-             ('instrument', 'instrument_ctd'),
-             ('valid_max', '40.0'),
-             ('valid_min', '0.0'),
-             ('accuracy', '0.01'),
-             ('precision', '0.01'),
-             ('resolution', '0.001')
-             ])
+    ds['salinity'] = (
+        ('time'), gsw.conversions.SP_from_C(r, ds.temperature, ds.pressure).values)
+    attrs = collections.OrderedDict([
+        ('long_name', 'water salinity'),
+        ('standard_name', 'sea_water_practical_salinity'),
+        ('units', '1e-3'),
+        ('comment', 'raw, uncorrected salinity'),
+        ('sources', 'conductivity temperature pressure'),
+        ('method', 'get_derived_eos_raw'),
+        ('observation_type', 'calulated'),
+        ('instrument', 'instrument_ctd'),
+        ('valid_max', '40.0'),
+        ('valid_min', '0.0'),
+        ('accuracy', '0.01'),
+        ('precision', '0.01'),
+        ('resolution', '0.001')])
     attrs = fill_required_attrs(attrs)
     ds['salinity'].attrs = attrs
-    sa = gsw.SA_from_SP(ds['salinity'], ds['pressure'], ds['longitude'], ds['latitude'])
+    sa = gsw.SA_from_SP(ds['salinity'], ds['pressure'], ds['longitude'],
+                        ds['latitude'])
     ct = gsw.CT_from_t(sa, ds['temperature'], ds['pressure'])
     ds['potential_density'] = (('time'), 1000 + gsw.density.sigma0(sa, ct).values)
-    attrs = collections.OrderedDict([('long_name', 'water potential density'),
-             ('standard_name', 'sea_water_potential_density'),
-             ('units', 'kg m-3'),
-             ('comment', 'raw, uncorrected salinity'),
-             ('sources', 'salinity temperature pressure'),
-             ('method', 'get_derived_eos_raw'),
-             ('observation_type', 'calulated'),
-             ('instrument', 'instrument_ctd'),
-              ('accuracy', '0.01'),
-              ('precision', '0.01'),
-              ('resolution', '0.001')
-             ])
+    attrs = collections.OrderedDict([
+        ('long_name', 'water potential density'),
+        ('standard_name', 'sea_water_potential_density'),
+        ('units', 'kg m-3'),
+        ('comment', 'raw, uncorrected salinity'),
+        ('sources', 'salinity temperature pressure'),
+        ('method', 'get_derived_eos_raw'),
+        ('observation_type', 'calulated'),
+        ('instrument', 'instrument_ctd'),
+        ('accuracy', '0.01'),
+        ('precision', '0.01'),
+        ('resolution', '0.001')
+        ])
     attrs = fill_required_attrs(attrs)
     ds['potential_density'].attrs = attrs
 
     ds['density'] = (('time'), gsw.density.rho(
             ds.salinity, ds.temperature, ds.pressure).values)
-    attrs = collections.OrderedDict([('long_name', 'Density'),
-             ('standard_name', 'sea_water_density'),
-             ('units', 'kg m-3'),
-             ('comment', 'raw, uncorrected salinity'),
-             ('observation_type', 'calulated'),
-             ('sources', 'salinity temperature pressure'),
-             ('instrument', 'instrument_ctd'),
-             ('method', 'get_derived_eos_raw'),
-              ('valid_min', '1000.0'),
-              ('valid_max', '1040.0'),
-               ('accuracy', '0.01'),
-               ('precision', '0.01'),
-               ('resolution', '0.001')
-             ])
+    attrs = collections.OrderedDict([
+        ('long_name', 'Density'),
+        ('standard_name', 'sea_water_density'),
+        ('units', 'kg m-3'),
+        ('comment', 'raw, uncorrected salinity'),
+        ('observation_type', 'calulated'),
+        ('sources', 'salinity temperature pressure'),
+        ('instrument', 'instrument_ctd'),
+        ('method', 'get_derived_eos_raw'),
+        ('valid_min', '1000.0'),
+        ('valid_max', '1040.0'),
+        ('accuracy', '0.01'),
+        ('precision', '0.01'),
+        ('resolution', '0.001')
+        ])
     attrs = fill_required_attrs(attrs)
     ds['density'].attrs = attrs
     ds['potential_temperature'] = (('time'), gsw.conversions.pt0_from_t(
             ds.salinity, ds.temperature, ds.pressure).values)
-    attrs = collections.OrderedDict([('long_name', 'water potential temperature'),
-             ('standard_name', 'sea_water_potential_temperature'),
-             ('units', 'Celsius'),
-             ('comment', 'raw, uncorrected salinity'),
-             ('sources', 'salinity temperature pressure'),
-             ('observation_type', 'calulated'),
-             ('method', 'get_derived_eos_raw'),
-              ('instrument', 'instrument_ctd'),
-           ('accuracy', '0.002'),
-           ('precision', '0.001'),
-           ('resolution', '0.0001')
-             ])
+    attrs = collections.OrderedDict([
+        ('long_name', 'water potential temperature'),
+        ('standard_name', 'sea_water_potential_temperature'),
+        ('units', 'Celsius'),
+        ('comment', 'raw, uncorrected salinity'),
+        ('sources', 'salinity temperature pressure'),
+        ('observation_type', 'calulated'),
+        ('method', 'get_derived_eos_raw'),
+        ('instrument', 'instrument_ctd'),
+        ('accuracy', '0.002'),
+        ('precision', '0.001'),
+        ('resolution', '0.0001')
+    ])
     attrs = fill_required_attrs(attrs)
     ds['potential_temperature'].attrs = attrs
 
     return ds
 
 
 def _time_to_datetime64(time):
@@ -368,15 +381,15 @@
         'comment': " ",
         'accuracy': " ",
         'precision': " ",
         'platform':  "platform",
         'resolution': " ",
         'ancillary_variables': " "}
     for k in required.keys():
-        if not k in attrs.keys():
+        if not (k in attrs.keys()):
             attrs[k] = required[k]
     return attrs
 
 
 def get_file_id(ds):
     """
     Make a file id for a Dataset
@@ -391,21 +404,21 @@
     ------
     id : string
         Id = *glider_name* + *glider_serial* + "YYYYMMDDTHHMM"
 
     """
 
     _log.debug(ds.time)
-    if not ds.time.dtype=='datetime64[ns]':
+    if not ds.time.dtype == 'datetime64[ns]':
         dt = _time_to_datetime64(ds.time.values[0])
     else:
         dt = ds.time.values[0].astype('datetime64[s]')
     _log.debug(f'dt, {dt}')
     id = (ds.attrs['glider_name'] + ds.attrs['glider_serial'] + '-' +
-                      dt.item().strftime('%Y%m%dT%H%M'))
+          dt.item().strftime('%Y%m%dT%H%M'))
     return id
 
 
 def fill_metadata(ds, metadata, sensor_data):
     """
     Add metadata to a Dataset
 
@@ -447,25 +460,26 @@
     ds.attrs['deployment_name'] = metadata['deployment_name']
     ds.attrs['title'] = ds.attrs['id']
 
     dt = ds.time.values
     ds.attrs['time_coverage_start'] = '%s' % dt[0]
     ds.attrs['time_coverage_end'] = '%s' % dt[-1]
 
-    ds.attrs['processing_level'] = 'Level 0 (L0) processed data timeseries; no corrections or data screening'
+    ds.attrs['processing_level'] = ('Level 0 (L0) processed data timeseries; '
+                                    'no corrections or data screening')
 
     for k, v in sensor_data.items():
         ds.attrs[k] = str(v)
     ds.attrs = collections.OrderedDict(sorted(ds.attrs.items()))
 
     return ds
 
 
 def _zero_screen(val):
-    val[val==0] = np.NaN
+    val[val == 0] = np.NaN
     return val
 
 
 def nmea2deg(nmea):
     """
     Convert a NMEA float to a decimal degree float.  e.g. -12640.3232 = -126.6721
     """
@@ -492,29 +506,35 @@
     -------
     ds : `xarray.Dataset`
         With *oxygen_concentration* corrected for the salinity effect.
     """
 
     oxy_yaml = ncvar['oxygen_concentration']
     if 'reference_salinity' not in oxy_yaml.keys():
-        _log.warning('No reference_salinity found in oxygen deployment yaml. Assuming reference salinity of 0 psu')
+        _log.warning('No reference_salinity found in oxygen deployment yaml. '
+                     'Assuming reference salinity of 0 psu')
         ref_sal = 0
     else:
         ref_sal = float(oxy_yaml['reference_salinity'])
     _log.info(f'Correcting oxygen using reference salinity {ref_sal} PSU')
     ds_oxy = ds.oxygen_concentration[~np.isnan(ds.oxygen_concentration)]
     # Match the nearest temperature and salinity values from their timestamps
-    ds_temp = ds.potential_temperature[~np.isnan(ds.potential_temperature)].reindex(time=ds_oxy.time, method="nearest")
-    ds_sal = ds.salinity[~np.isnan(ds.salinity)].reindex(time=ds_oxy.time, method="nearest")
+    ds_temp = ds.potential_temperature[~np.isnan(ds.potential_temperature)].reindex(
+        time=ds_oxy.time, method="nearest")
+    ds_sal = ds.salinity[~np.isnan(ds.salinity)].reindex(
+        time=ds_oxy.time, method="nearest")
     o2_sol = gsw.O2sol_SP_pt(ds_sal, ds_temp)
     o2_sat = ds_oxy / gsw.O2sol_SP_pt(ds_sal*0 + ref_sal, ds_temp)
-    ds['oxygen_concentration'].values[~np.isnan(ds.oxygen_concentration)] = o2_sat * o2_sol
-    ds['oxygen_concentration'].attrs['oxygen_concentration_QC:RTQC_methodology'] =\
-        f'oxygen concentration corrected for salinity using gsw.O2sol_SP_pt with salinity and potential temperature ' \
-        f'from dataset. Original oxygen concentration assumed to have been calculated using salinity = {ref_sal} PSU'
+    ds['oxygen_concentration'].values[~np.isnan(ds.oxygen_concentration)] = (
+        o2_sat * o2_sol)
+    ds['oxygen_concentration'].attrs['oxygen_concentration_QC:RTQC_methodology'] = (
+        f'oxygen concentration corrected for salinity using gsw.O2sol_SP_pt with'
+        f'salinity and potential temperature from dataset. Original oxygen '
+        f'concentration assumed to have been calculated using salinity = '
+        f'{ref_sal} PSU')
     return ds
 
 
 def bar2dbar(val):
     """
     convert val bar to dbar
     """
@@ -544,86 +564,108 @@
         ind = np.where(~np.isnan(data[:, j]))[0]
         if (len(ind) > 0 and len(ind) < (ind[-1] - ind[0])
                 and len(ind) > (ind[-1] - ind[0]) * 0.05):
             int = np.arange(ind[0], ind[-1])
             data[:, j][ind[0]:ind[-1]] = np.interp(int, ind, data[ind, j])
     return data
 
+def find_gaps(sample_time, timebase, maxgap):
+    """
+    Return an index into *timebase* where True are times in gaps of *sample_time* larger
+    than maxgap.
+    """
+    # figure out which sample each time in time base belongs to:
+    time_index = np.searchsorted(sample_time, timebase, side='right')
+    time_index = np.clip(time_index, 0, len(sample_time)-1)
+    
+    # figure out the space between sample pairs
+    dt = np.concatenate(([0], np.diff(sample_time)))
+    # get the gap size for each timebase data point:
+    ddt = dt[time_index]
+    
+    # get the indices of timebase that are too large and account for the 
+    # degenerate case when a timebase point falls directly on a sample time. 
+    index = ~np.logical_or((ddt <= maxgap),(np.isin(timebase,sample_time)))
+      
+    return index
 
 def _parse_gliderxml_pos(fname):
     """
     DEPRECATED: use slocum.parse_gliderState instead
 
     returns lon, lat, timestr
     """
 
     xmln = fname
     from bs4 import BeautifulSoup
     with open(xmln, 'r') as fin:
-        y=BeautifulSoup(fin, features="xml")
+        y = BeautifulSoup(fin, features="xml")
         time = None
         lon = None
         lat = None
         for a in y.find_all('valid_location'):
             try:
                 dtime = np.datetime64(a.time.text)
                 if dtime > np.datetime64('2019-07-19'):
-                    #print(dtime, float(a.lat.text), float(a.lon.text))
-                    #print(np.array(dtime))
                     if time is not None:
                         time = np.append(time, dtime)
                         lat = np.append(lat, float(a.lat.text))
                         lon = np.append(lon, float(a.lon.text))
                     else:
                         time = np.array(dtime)
                         lat = np.array(float(a.lat.text))
                         lon = np.array(float(a.lon.text))
             except:
                 pass
         lon = nmea2deg(lon)
         lat = nmea2deg(lat)
     return lon, lat, time
 
+
 def _parse_gliderxml_surfacedatetime(fname):
     """
     DEPRECATED: use slocum.parse_gliderState instead
 
     returns lon, lat, timestr
     """
 
     xmln = fname
     from bs4 import BeautifulSoup
     with open(xmln, 'r') as fin:
-        y=BeautifulSoup(fin, features="xml")
+        y = BeautifulSoup(fin, features="xml")
         time = None
         for a in y.find_all('report'):
             _log.debug(a)
             if a.text is not None:
                 try:
                     time = np.append(time, np.datetime64(a.text))
                 except:
                     pass
     return time
 
 
-def example_gridplot(filename, outname, toplot=['potential_temperature', 'salinity', 'oxygen_concentration'],
+def example_gridplot(filename, outname,
+                     toplot=['potential_temperature', 'salinity',
+                             'oxygen_concentration'],
                      pdenlevels=np.arange(10, 30, 0.5), dpi=200, ylim=None):
     """
     Smoketest for plotting the netcdf files.
     """
 
     import matplotlib.pyplot as plt
 
     ntoplot = len(toplot)
     with xr.open_dataset(filename) as ds:
-        fig, axs =  plt.subplots(nrows=ntoplot, constrained_layout=True, figsize=(7, 3*ntoplot),
-                                 sharex=True, sharey=True)
+        fig, axs = plt.subplots(nrows=ntoplot, constrained_layout=True,
+                                figsize=(7, 3*ntoplot),
+                                sharex=True, sharey=True)
         for ax, vname in zip(axs, toplot):
             ds[vname].plot.pcolormesh(ax=ax)
             (ds['potential_density']-1000).plot.contour(ax=ax, levels=pdenlevels)
             if ylim:
                 ax.set_ylim(ylim)
         fig.savefig(outname, dpi=dpi)
 
+
 __all__ = ['get_distance_over_ground', 'get_glider_depth', 'get_profiles_new',
-'get_derived_eos_raw', "get_glider_id", "fill_metadata", "nmea2deg",
-"gappy_fill_vertical", "oxygen_concentration_correction"]
+           'get_derived_eos_raw', "fill_metadata", "nmea2deg",
+           "gappy_fill_vertical", "oxygen_concentration_correction"]
```

