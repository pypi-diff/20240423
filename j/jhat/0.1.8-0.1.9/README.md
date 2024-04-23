# Comparing `tmp/jhat-0.1.8-py3-none-any.whl.zip` & `tmp/jhat-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 106286 bytes, number of entries: 18
--rw-r--r--  2.0 unx     3406 b- defN 22-Dec-15 17:44 bin/run_st_wcs_align.py
--rw-r--r--  2.0 unx     5313 b- defN 23-Sep-20 13:43 bin/run_st_wcs_align_batch.py
+Zip file size: 109596 bytes, number of entries: 18
+-rw-r--r--  2.0 unx     3653 b- defN 24-Jan-31 23:01 bin/run_st_wcs_align.py
+-rw-r--r--  2.0 unx     5554 b- defN 24-Jan-31 23:01 bin/run_st_wcs_align_batch.py
 -rwxr-xr-x  2.0 unx     3124 b- defN 22-Dec-09 14:45 bin/st_wcs_align
 -rwxr-xr-x  2.0 unx     5059 b- defN 22-Dec-09 14:47 bin/st_wcs_align_batch
 -rw-r--r--  2.0 unx     3502 b- defN 22-Dec-08 23:43 jhat/__init__.py
 -rw-r--r--  2.0 unx    59300 b- defN 23-Sep-27 18:49 jhat/pdastro.py
--rw-r--r--  2.0 unx   100096 b- defN 23-Oct-26 18:20 jhat/simple_jwst_phot.py
+-rw-r--r--  2.0 unx   109775 b- defN 24-Apr-23 17:01 jhat/simple_jwst_phot.py
 -rw-r--r--  2.0 unx   103074 b- defN 23-Sep-13 21:06 jhat/simple_jwst_phot_temp.py
--rw-r--r--  2.0 unx    83391 b- defN 23-Sep-20 13:43 jhat/st_wcs_align.py
--rw-r--r--  2.0 unx    20192 b- defN 23-Dec-02 00:15 jhat/st_wcs_align_batch.py
+-rw-r--r--  2.0 unx    90072 b- defN 24-Apr-23 20:55 jhat/st_wcs_align.py
+-rw-r--r--  2.0 unx    20951 b- defN 24-Jan-31 23:01 jhat/st_wcs_align_batch.py
 -rw-r--r--  2.0 unx    83510 b- defN 23-Sep-13 21:06 jhat/st_wcs_align_temp.py
 -rw-r--r--  2.0 unx      480 b- defN 22-Dec-08 23:43 jhat/test_jhat.py
--rwxr-xr-x  2.0 unx     3392 b- defN 23-Dec-02 00:17 jhat-0.1.8.data/scripts/run_st_wcs_align.py
--rwxr-xr-x  2.0 unx     5300 b- defN 23-Dec-02 00:17 jhat-0.1.8.data/scripts/run_st_wcs_align_batch.py
--rw-r--r--  2.0 unx      471 b- defN 23-Dec-02 00:17 jhat-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-02 00:17 jhat-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Dec-02 00:17 jhat-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1443 b- defN 23-Dec-02 00:17 jhat-0.1.8.dist-info/RECORD
-18 files, 481154 bytes uncompressed, 103956 bytes compressed:  78.4%
+-rwxr-xr-x  2.0 unx     3639 b- defN 24-Apr-23 20:59 jhat-0.1.9.data/scripts/run_st_wcs_align.py
+-rwxr-xr-x  2.0 unx     5541 b- defN 24-Apr-23 20:59 jhat-0.1.9.data/scripts/run_st_wcs_align_batch.py
+-rw-r--r--  2.0 unx      471 b- defN 24-Apr-23 20:59 jhat-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 20:59 jhat-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-23 20:59 jhat-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1443 b- defN 24-Apr-23 20:59 jhat-0.1.9.dist-info/RECORD
+18 files, 499249 bytes uncompressed, 107266 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: jhat/st_wcs_align_temp.py
 Comment: 
 
 Filename: jhat/test_jhat.py
 Comment: 
 
-Filename: jhat-0.1.8.data/scripts/run_st_wcs_align.py
+Filename: jhat-0.1.9.data/scripts/run_st_wcs_align.py
 Comment: 
 
-Filename: jhat-0.1.8.data/scripts/run_st_wcs_align_batch.py
+Filename: jhat-0.1.9.data/scripts/run_st_wcs_align_batch.py
 Comment: 
 
-Filename: jhat-0.1.8.dist-info/METADATA
+Filename: jhat-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: jhat-0.1.8.dist-info/WHEEL
+Filename: jhat-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: jhat-0.1.8.dist-info/top_level.txt
+Filename: jhat-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: jhat-0.1.8.dist-info/RECORD
+Filename: jhat-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bin/run_st_wcs_align.py

```diff
@@ -18,17 +18,21 @@
 
 
 wcs_align.run_all(args.cal_image,
                  telescope = args.telescope,
                  #distortion_file = args.distortion_file,
                  outrootdir = args.outrootdir,
                  outsubdir = args.outsubdir,
+                 distortion_file = args.distortion_file,
                  overwrite = args.overwrite,
+                 photometry_method = args.photometry_method,
+                 find_stars_threshold = args.find_stars_threshold,
+                 sci_xy_catalog=args.sci_xy_catalog,
                  #skip_applydistortions_if_exists=args.skip_applydistortions_if_exists,
-                 use_dq = args.use_dq,
+                 use_dq = not args.skip_use_dq,
                  refcatname = args.refcat,
                  refcat_racol = args.refcat_racol,
                  refcat_deccol = args.refcat_deccol,
                  refcat_magcol = args.refcat_magcol,
                  refcat_magerrcol = args.refcat_magerrcol,
                  refcat_colorcol = args.refcat_colorcol,
                  pmflag = args.refcat_pmflag,
```

## bin/run_st_wcs_align_batch.py

```diff
@@ -73,14 +73,18 @@
 align_batch.align_wcs(ixs_todo,
                     overwrite = args.overwrite,
                     outrootdir= args.outrootdir,
                     outsubdir = args.outsubdir,
                     addfilter2outsubdir = args.addfilter2outsubdir,
                     telescope = args.telescope,
                     #skip_applydistortions_if_exists=args.skip_applydistortions_if_exists,
+                    photometry_method = args.photometry_method,
+                    find_stars_threshold = args.find_stars_threshold,
+                    sci_xy_catalog=args.sci_xy_catalog,
+                    use_dq = not args.skip_use_dq,
                     refcatname = args.refcat,
                     refcat_racol = args.refcat_racol,
                     refcat_deccol = args.refcat_deccol,
                     refcat_magcol = args.refcat_magcol,
                     refcat_magerrcol = args.refcat_magerrcol,
                     refcat_colorcol = args.refcat_colorcol,
                     pmflag = args.refcat_pmflag,
```

## jhat/simple_jwst_phot.py

```diff
@@ -25,14 +25,15 @@
 
 from photutils.detection import DAOStarFinder
 from photutils.background import MMMBackground, MADStdBackgroundRMS, Background2D
 from photutils import CircularAperture, CircularAnnulus, aperture_photometry
 from astropy.visualization import simple_norm
 
 import jwst
+#from stdatamodels.jwst.datamodels import ImageModel
 from jwst.datamodels import ImageModel
 from jwst import datamodels
 from jwst import source_catalog
 from jwst.source_catalog import reference_data
 import astropy.units as u
 import pysiaf
 from astroquery.gaia import Gaia
@@ -75,17 +76,23 @@
     apps = [float(x.split('#')[1]) for x in ee.colnames]
     interp = scipy.interpolate.interp2d(waves,apps,ee_arr)
     filt_wave = waves[np.where(filts==filt.upper())[0][0]]
     return(interp(filt_wave,ap))
 
 def hst_get_zp(filt,zpsys='ab'):
     if zpsys.lower()=='ab':
-        return {'F098M':25.666,'F105W':26.264,'F110W':26.819,'F125W':26.232,'F140W':26.450,'F160W':25.936}[filt]
+        return {'F098M':25.666,'F105W':26.264,'F110W':26.819,
+        'F125W':26.232,'F140W':26.450,'F160W':25.936,'F126N':22.849,'F127M':24.625,
+        'F128N':22.956,'F130N':22.981,'F132N':22.933,'F139M':24.466,'F153M':24.447,
+        'F164N':22.892,'F167N':22.937}[filt]
     elif zpsys.lower()=='vega':
-        return {'F098M':25.090,'F105W':25.603,'F110W':26.042,'F125W':25.312,'F140W':25.353,'F160W':24.662}[filt]
+        return {'F098M':25.090,'F105W':25.603,'F110W':26.042,
+        'F125W':25.312,'F140W':25.353,'F160W':24.662,'F126N':21.908,'F127M':23.643,
+        'F128N':21.898,'F130N':21.985,'F132N':21.915,'F139M':23.366,'F153M':23.171,
+        'F164N':22.892,'F167N':21.550}[filt]
     else:
         print('unknown zpsys')
         return
 
 def get_apcorr_params(fname,ee=70):
     try:
         sc = source_catalog.source_catalog_step.SourceCatalogStep()
@@ -280,14 +287,16 @@
     else:
         print(f'### NO propoer motion correction!!!')
         racol='ra'
         deccol='dec'
     
     df = tb_gaia.to_pandas()
 
+    Table.from_pandas(df).write('Gaia_reference_catalog.txt',format='ascii')
+
     # renames columns from f'phot_{filt}_mean_mag' to f'{filt}'
     if rename_mag_colnames:
         for filt in ['g','bp','rp']:
             df.rename(columns={f'phot_{filt}_mean_mag':f'{filt}'},inplace=True)
                               
     if calc_mag_errors:
         for filt in ['g','bp','rp']:
@@ -515,14 +524,15 @@
         self.imagename = imagename
         self.dm = datamodels.open(self.imagename)
         self.im = fits.open(imagename)
         self.primaryhdr = self.im['PRIMARY'].header
         self.scihdr = self.im['SCI'].header
         #self.sci_wcs = wcs.WCS(self.scihdr)
         self.sci_wcs = self.dm.meta.wcs
+        
         self.sip_wcs = wcs.WCS(self.scihdr)
         try:
             self.err = self.im['ERR'].data
         except:
             self.err = None
         self.pixel_scale = wcs.utils.proj_plane_pixel_scales(self.sip_wcs)[0]  *\
          self.sip_wcs.wcs.cunit[0].to('arcsec')
@@ -612,14 +622,15 @@
         else:
             mask = np.zeros(data_original.shape, dtype='int')
 
         # hijack a few bits for our purposes...
         mask[np.isnan(data)==True] = 8
         mask[np.isfinite(data)==False] = 8
         mask[np.where(data==0)] = 16
+
         #fits.writeto('TEST_mask_delme.fits',mask,overwrite=True,output_verify='ignore')
                
         data[mask>0] = np.nan
 
         return data,mask,DNunits
     
     def get_bool_mask(self, data,  mask=None):
@@ -690,15 +701,15 @@
         fwhm_psf = self.dict_utils[instrument.upper()][filt]['psf fwhm']
         if instrument.upper() == 'MIRI':
             fwhm_psf/=self.pixel_scale
         return(fwhm_psf)
         
         
 
-    def find_stars(self, threshold=3, var_bkg=False, primaryhdr=None, scihdr=None):
+    def find_stars(self, threshold=3, var_bkg=False, primaryhdr=None, scihdr=None,centers=None):
         
         '''
         Parameters
         ----------
         
         threshold : float 
             The absolute image value above which to select sources.
@@ -734,15 +745,15 @@
         full_mask = np.bitwise_or(nan_mask,zero_mask)
         if self.mask is not None: 
              full_mask = np.bitwise_or(full_mask,self.mask)
         bool_mask = np.where(full_mask>0,True,False)
        
         self.data_bkgsub, std = self.calc_bkg(self.data, mask=bool_mask, var_bkg=var_bkg)
 
-        daofind = DAOStarFinder(threshold=threshold * std, fwhm=fwhm_psf, exclude_border=True)
+        daofind = DAOStarFinder(threshold=threshold * std, fwhm=fwhm_psf, exclude_border=True,xycoords=centers)
         self.found_stars = daofind(self.data_bkgsub, mask=bool_mask)
 
         #found_stars = daofind(data_bkgsub)
         if self.verbose:            
             print('')
             print('Number of sources found in the image:', len(self.found_stars))
             print('-------------------------------------')
@@ -783,14 +794,99 @@
         
         return(radii,radius_sky_in,radius_sky_out,radius_for_mag)
 
     def colname(self,basecolname,radius):
         return(f'{basecolname}_{radius:.1f}px')
 
     #def aperture_phot(self, radius=[3.5], sky_in=7, sky_out=10, add_radius_to_colname=False):
+    def psf_phot(self, filt=None, 
+                      primaryhdr=None, scihdr=None):
+        
+        """
+        Aperture photometry routine for HST.
+            
+        Returns
+        -------
+        table_aper : :class:`astropy.table.Table`
+
+        """
+        if primaryhdr is None: primaryhdr=self.primaryhdr
+        if scihdr is None: scihdr=self.scihdr
+
+        # det = primaryhdr['DETECTOR']
+        # if filt is None:
+        #     if det in ['GUIDER1','GUIDER2']:
+        #         filt = 'NA'
+        #     else:
+        #         filt = primaryhdr['FILTER']
+        # if pupil is None: 
+        #     if det in ['GUIDER1','GUIDER2']:
+        #         pupil = 'NA'
+        #     else:
+        #         pupil = primaryhdr['PUPIL']
+
+        # (self.radii_px,
+        #  self.radius_sky_in_px,
+        #  self.radius_sky_out_px,
+        #  self.radius_for_mag_px) = self.get_radii_phot(filt,pupil,
+        #                                                radii_Nfwhm = radii_Nfwhm,
+        #                                                radius_Nfwhm_sky_in = radius_Nfwhm_sky_in, 
+        #                                                radius_Nfwhm_sky_out = radius_Nfwhm_sky_out, 
+        #                                                radius_Nfwhm_for_mag = radius_Nfwhm_for_mag)
+
+        positions = np.transpose((self.found_stars['ycentroid'], self.found_stars['xcentroid']))
+        
+        tic = time.perf_counter()
+    
+        import space_phot
+        if self.pipeline_level==2:
+            obs = space_phot.observation2(self.imagename)
+        else:
+            raise RuntimeError('PSF only set up for level 2 at the moment.')
+            
+        if self.psf_model is None:
+            width = int(3*self.get_fwhm_psf(obs.filter))
+            if width%2==0:
+                width = int(width+1)
+            self.psf_model = space_phot.util.get_jwst_psf_grid(obs,num_psfs=4)
+        obs.fast_psf(self.psf_model,positions,psf_width=width,local_bkg=True)
+        
+        table_aper = obs.psf_result.phot_cal_table
+        print(table_aper.colnames)
+        table_aper['ycentroid'] = obs.psf_result.phot_cal_table['y_fit']
+        table_aper['xcentroid'] = obs.psf_result.phot_cal_table['x_fit']
+        table_aper['y'] = obs.psf_result.phot_cal_table['y_fit']
+        table_aper['x'] = obs.psf_result.phot_cal_table['x_fit']
+        table_aper.remove_column('flux_fit')
+        table_aper.remove_column('flux_err')
+        table_aper.rename_column('fluxerr','flux_err')
+        table_aper.rename_column('magerr','dmag')
+        
+        table_aper['psf_quality'] = np.abs([np.sum(obs.psf_result.resid_arr[i]/obs.psf_result.data_arr[i]) for i in range(len(obs.psf_result.data_arr))])
+        
+        
+            #if rad == self.radius_for_mag_px:
+                #table_aper['mag'] = -2.5 * np.log10(table_aper[self.colname('aper_sum_bkgsub',rad)])
+                #table_aper['dmag'] = 1.086 * (table_aper[self.colname('flux_err',rad)] / 
+                #                              table_aper[self.colname('aper_sum_bkgsub',rad)])      
+
+        #table_aper['x'] = self.found_stars['xcentroid']
+        #table_aper['y'] = self.found_stars['ycentroid']
+        table_aper['sharpness'] = self.found_stars['sharpness']
+        table_aper['roundness1'] = self.found_stars['roundness1']
+        table_aper['roundness2'] = self.found_stars['roundness2']
+        table_aper = table_aper[~np.isnan(table_aper['mag'])]
+        toc = time.perf_counter()
+        if self.verbose:
+            print("Time Elapsed:", toc - tic)
+    
+        self.t = table_aper.to_pandas()
+
+        return table_aper
+    
     def aperture_phot(self, filt=None, pupil=None, 
                       radii_Nfwhm = None,
                       radius_Nfwhm_sky_in = None, 
                       radius_Nfwhm_sky_out = None, 
                       radius_Nfwhm_for_mag =None,
                       primaryhdr=None, scihdr=None):
         
@@ -934,38 +1030,47 @@
         if self.verbose:
             print("Time Elapsed:", toc - tic)
     
         self.t = table_aper.to_pandas()
 
         return table_aper
 
-    def clean_phottable(self,SNR_min=3.0,indices=None):
+    def clean_phottable(self,SNR_min=3.0,indices=None,psf_quality=None):
         # remove nans
         ixs = self.ix_not_null(['mag','dmag'],indices=indices)
         if self.verbose:
             print(f'{len(ixs)} objects left after removing entries with NaNs in mag or dmag column')
         #self.write()
         
         if SNR_min is not None:
             dmag_max = 1.086 * 1.0/SNR_min
             ixs = self.ix_inrange('dmag',None,dmag_max,indices=ixs)
             if self.verbose:
                 print(f'SNR_min cut: {len(ixs)} objects left after removing entries dmag>{dmag_max} (SNR<{SNR_min})')
 
+        if psf_quality is not None:
+            ixs = self.ix_inrange('psf_quality',None,psf_quality,indices=ixs) 
+            if self.verbose:
+                print(f'PSF cut: {len(ixs)} objects left after removing entries psf_q>{psf_quality}')
         return(ixs)
 
     def xy_to_radec(self,xcol='x',ycol='y',racol='ra',deccol='dec',indices=None,
                     xshift=0.0,yshift=0.0):
         ixs = self.getindices(indices=indices)
 
         image_model = ImageModel(self.im)
         
-        coord = self.sci_wcs.pixel_to_world(self.t.loc[ixs,xcol]+xshift, self.t.loc[ixs,ycol]+yshift)
-        self.t.loc[ixs,racol] = coord.ra.degree
-        self.t.loc[ixs,deccol] = coord.dec.degree
+        #try:
+        #    coord = self.sci_wcs.pixel_to_world(self.t.loc[ixs,xcol]+xshift, self.t.loc[ixs,ycol]+yshift)
+        #except:
+        #    coord = self.sip_wcs.pixel_to_world(self.t.loc[ixs,xcol]+xshift, self.t.loc[ixs,ycol]+yshift)
+        detector_to_world = image_model.meta.wcs.get_transform('detector','world')
+        (self.t.loc[ixs,racol],self.t.loc[ixs,deccol]) = detector_to_world(self.t.loc[ixs,xcol], self.t.loc[ixs,ycol])
+        #self.t.loc[ixs,racol] = coord.ra.degree
+        #self.t.loc[ixs,deccol] = coord.dec.degree
 
     def radec_to_xy(self,racol='ra',deccol='dec',xcol='x',ycol='y',indices=None):
         ixs = self.getindices(indices=indices)
 
         image_model = ImageModel(self.im)
         world_to_detector = image_model.meta.wcs.get_transform('world', 'detector')
         (self.t.loc[ixs,xcol], self.t.loc[ixs,ycol]) = world_to_detector(self.t.loc[ixs,racol],self.t.loc[ixs,deccol])
@@ -1384,16 +1489,18 @@
         return(photfilename)
                     
     def get_radecinfo_image(self,im=None,nx=None,ny=None):
         if im is None: im=self.im
         image_model = ImageModel(im)
         if nx is None: nx = int(im['SCI'].header['NAXIS1'])
         if ny is None: ny = int(im['SCI'].header['NAXIS2'])
-                
-        ra0,dec0 = image_model.meta.wcs(nx/2.0-1,ny/2.0-1)
+        
+        detector_to_world = self.sci_wcs.get_transform('detector','world')
+        ra0,dec0 = detector_to_world(nx/2.0-1,ny/2.0-1)
+        #ra0,dec0 = image_model.meta.wcs(nx/2.0-1,ny/2.0-1)
         coord0 = SkyCoord(ra0,dec0,unit=(u.deg, u.deg), frame='icrs')
         radius_deg = []
         for x in [0,nx-1]:        
             for y in [0,ny-1]:     
                 ra,dec = image_model.meta.wcs(x,y)
                 radius_deg.append(coord0.separation(SkyCoord(ra,dec,unit=(u.deg, u.deg), frame='icrs')).deg)
         radius_deg = np.amax(radius_deg)
@@ -1408,22 +1515,27 @@
                  outsubdir=None,
                  overwrite=False,                
                  load_photcat_if_exists=False,
                  use_dq = False,
                  DNunits=False, 
                  SNR_min=3.0,
                  do_photometry_flag=True,
+                 photometry_method='aperture',
+                 find_stars_threshold = 3.0,
+                 psf_model=None,
+                 sci_xy_catalog=None,
                  photcat_loaded = False,
                  Nbright4match=None,
                  xshift=0.0,# added to the x coordinate before calculating ra,dec. This can be used to correct for large shifts before matching!
                  yshift=0.0, # added to the y coordinate before calculating ra,dec. This can be used to correct for large shifts before matching!
                  ee_radius=70):
         if self.verbose:
             print(f'\n### Doing photometry on {imagename}')
         self.ee_radius = ee_radius
+        self.psf_model = psf_model
         
         # get the photfilename. photfilename='auto' removes fits from image name and replaces it with phot.txt
         self.photfilename = self.get_photfilename(photfilename,outrootdir=outrootdir,outsubdir=outsubdir,imagename=imagename)
         print(self.verbose,self.photfilename)
         # Load photcat if wanted
         photcat_loaded = False
         if (self.photfilename is not None):
@@ -1450,22 +1562,33 @@
         # load the image, and prepare it. The data and mask are saved in 
         # self.data and self.mask
         self.load_image(imagename,DNunits=DNunits,use_dq=use_dq)
         # only do the photometry if not reloaded
         if do_photometry_flag:
     
             # find the stars, saved in self.found_stars
-            self.find_stars()
             
+            if sci_xy_catalog is not None:
+                
+                ref = Table.read(sci_xy_catalog,format='ascii')
+                xycoords=np.atleast_2d([ref['x'],ref['y']]).T
+                self.find_stars(centers=xycoords, threshold = find_stars_threshold)
+            else:
+                self.find_stars(threshold = find_stars_threshold)
             #aperture phot, saved in self.t
-            self.aperture_phot()
-             
-        
+            if photometry_method == 'aperture':
+                self.aperture_phot()
+                psf_quality=None
+            elif photometry_method == 'psf':
+                self.psf_phot()
+                psf_quality= 25
+        else:
+            psf_quality=None
         # get the indices of good stars
-        ixs_clean = self.clean_phottable(SNR_min=SNR_min)
+        ixs_clean = self.clean_phottable(SNR_min=SNR_min,psf_quality=psf_quality)
         if self.verbose:
             print(f'{len(ixs_clean)} out of {len(self.getindices())} entries remain in photometry table')
         if len(ixs_clean)<1:
             self.write()
             raise RuntimeError('NO  OBJECTS FOUND IN  IMAGE!!')
         
         #self.write('DELME0.txt',columns=['x','y','mag','dmag'])
@@ -1855,15 +1978,109 @@
         mask[np.where(data==0)] = 16
         #fits.writeto('TEST_mask_delme.fits',mask,overwrite=True,output_verify='ignore')
                
         data[mask>0] = np.nan
 
         return data,mask
 
+    def psf_phot(self, filt=None, 
+                      primaryhdr=None, scihdr=None):
+        
+        """
+        Aperture photometry routine for HST.
+            
+        Returns
+        -------
+        table_aper : :class:`astropy.table.Table`
+
+        """
+        if primaryhdr is None: primaryhdr=self.primaryhdr
+        if scihdr is None: scihdr=self.scihdr
+
+        # det = primaryhdr['DETECTOR']
+        # if filt is None:
+        #     if det in ['GUIDER1','GUIDER2']:
+        #         filt = 'NA'
+        #     else:
+        #         filt = primaryhdr['FILTER']
+        # if pupil is None: 
+        #     if det in ['GUIDER1','GUIDER2']:
+        #         pupil = 'NA'
+        #     else:
+        #         pupil = primaryhdr['PUPIL']
 
+        # (self.radii_px,
+        #  self.radius_sky_in_px,
+        #  self.radius_sky_out_px,
+        #  self.radius_for_mag_px) = self.get_radii_phot(filt,pupil,
+        #                                                radii_Nfwhm = radii_Nfwhm,
+        #                                                radius_Nfwhm_sky_in = radius_Nfwhm_sky_in, 
+        #                                                radius_Nfwhm_sky_out = radius_Nfwhm_sky_out, 
+        #                                                radius_Nfwhm_for_mag = radius_Nfwhm_for_mag)
+
+        positions = np.transpose((self.found_stars['ycentroid'], self.found_stars['xcentroid']))
+        
+        tic = time.perf_counter()
+    
+        import space_phot
+        if self.pipeline_level==2:
+            obs = space_phot.observation2(self.imagename)
+        else:
+            raise RuntimeError('PSF only set up for level 2 at the moment.')
+            
+        if self.psf_model is None:
+
+            self.psf_model = space_phot.util.get_hst_psf_grid(obs,num_psfs=16)
+        obs.fast_psf(self.psf_model,positions,local_bkg=True)
+
+        
+        table_aper = obs.psf_result.phot_cal_table
+        #for i in range(5):
+        import matplotlib.pyplot as plt
+        table_aper['psf_quality'] = np.abs([np.sum(obs.psf_result.resid_arr[i]/obs.psf_result.data_arr[i]) for i in range(len(obs.psf_result.data_arr))])
+        #plt.hist(table_aper['psf_quality'][table_aper['psf_quality']<100])
+        #plt.show()
+        #import matplotlib.pyplot as plt
+        #print(obs.psf_result['local_bkg'][0],obs.psf_result.phot_table[0])
+        #plt.imshow(obs.psf_result['data_arr'][0])
+        #plt.show()
+        #plt.imshow(obs.psf_result['fit_residuals'][0].reshape(5,5))
+        #print(list(obs.psf_result.keys()))
+        #for i in range(5):
+        #   obs.plot_psf_fit(fast_n=i)
+        #   plt.show()
+        #sys.exit()
+        table_aper['ycentroid'] = obs.psf_result.phot_cal_table['y_fit']
+        table_aper['xcentroid'] = obs.psf_result.phot_cal_table['x_fit']
+        table_aper['y'] = obs.psf_result.phot_cal_table['y_fit']
+        table_aper['x'] = obs.psf_result.phot_cal_table['x_fit']
+        table_aper.remove_column('flux_fit')
+        table_aper.remove_column('flux_err')
+        table_aper.rename_column('fluxerr','flux_err')
+        #table_aper.rename_column('flux_cal','flux')
+        table_aper.rename_column('magerr','dmag')
+            #if rad == self.radius_for_mag_px:
+                #table_aper['mag'] = -2.5 * np.log10(table_aper[self.colname('aper_sum_bkgsub',rad)])
+                #table_aper['dmag'] = 1.086 * (table_aper[self.colname('flux_err',rad)] / 
+                #                              table_aper[self.colname('aper_sum_bkgsub',rad)])      
+
+        #table_aper['x'] = self.found_stars['xcentroid']
+        #table_aper['y'] = self.found_stars['ycentroid']
+        table_aper['sharpness'] = self.found_stars['sharpness']
+        table_aper['roundness1'] = self.found_stars['roundness1']
+        table_aper['roundness2'] = self.found_stars['roundness2']
+        table_aper = table_aper[~np.isnan(table_aper['mag'])]
+        toc = time.perf_counter()
+        if self.verbose:
+            print("Time Elapsed:", toc - tic)
+    
+        self.t = table_aper.to_pandas()
+
+        return table_aper
+    
     def aperture_phot(self, filt=None, pupil=None, 
                       radii_Nfwhm = None,
                       radius_Nfwhm_sky_in = None, 
                       radius_Nfwhm_sky_out = None, 
                       radius_Nfwhm_for_mag =None,
                       primaryhdr=None, scihdr=None):
```

## jhat/st_wcs_align.py

```diff
@@ -9,16 +9,20 @@
 import os,re,sys,copy,warnings
 #from jwst.tweakreg import TweakRegStep
 import tweakreg_hack
 import argparse
 import numpy as np
 import matplotlib.pyplot as plt
 from astropy.table import Table
+import astropy.io.fits as fits
 
 from jwst import datamodels
+from jwst.pipeline.calwebb_image2 import Image2Pipeline
+from jwst.assign_wcs import AssignWcsStep
+
 
 from .simple_jwst_phot import jwst_photclass,hst_photclass
 from .pdastro import *
 
 warnings.simplefilter('ignore')
 __all__ = ['st_wcs_align']
 
@@ -57,14 +61,15 @@
         phot.t.loc[phot.ixs_notuse].plot('y','dx',ax=sp[0],ylim=dx_plotlim, **plot_style['do_not_use_data'])
         phot.t.loc[phot.ixs_notuse].plot('x','dy',ax=sp[1],ylim=dy_plotlim, **plot_style['do_not_use_data'])
         phot.t.loc[phot.ixs_notuse].plot('x','y',ax=sp[2],**plot_style['do_not_use_data'])
         phot.t.loc[phot.ixs_notuse].plot('sharpness','mag',ax=sp[3],**plot_style['do_not_use_data'])
         phot.t.loc[phot.ixs_notuse].plot('sharpness','dmag',ax=sp[4],**plot_style['do_not_use_data'])
         phot.t.loc[phot.ixs_notuse].plot('sharpness','roundness1',ax=sp[5],**plot_style['do_not_use_data'])
 
+    
     if phot.ixs_use is not None:
         ixs_cut = AnotB(phot.ixs_use,ixs_good)
         phot.t.loc[ixs_cut].plot('y','dx',ax=sp[0],ylim=dx_plotlim, **plot_style['cut_data'])
         phot.t.loc[ixs_cut].plot('y','dx',ax=sp[0],ylim=dx_plotlim, **plot_style['cut_data'])
         phot.t.loc[ixs_cut].plot('x','dy',ax=sp[1],ylim=dy_plotlim, **plot_style['cut_data'])
         phot.t.loc[ixs_cut].plot('x','y',ax=sp[2],**plot_style['cut_data'])
         phot.t.loc[ixs_cut].plot('sharpness','mag',ax=sp[3],**plot_style['cut_data'])
@@ -109,15 +114,16 @@
     minval = np.min(phot.t.loc[ixs,d_col_rot])
     maxval = np.max(phot.t.loc[ixs,d_col_rot])
     if minval>histolim[0]:histolim[0]=minval
     if maxval<histolim[1]:histolim[1]=maxval
     # add a buffer to the min and max values
     histolim[0]-=0.1*(maxval-minval)
     histolim[1]+=0.1*(maxval-minval)
-        
+
+
     if phot.ixs_notuse is not None:
         phot.t.loc[phot.ixs_notuse].plot(col,d_col_rot,ax=sp[spi[0]],**plot_style['do_not_use_data'])
     phot.t.loc[ixs].plot(col,d_col,ax=sp[spi[0]],ylim=histolim,title=title,**plot_style['cut_data'])
     phot.t.loc[ixs].plot(col,d_col_rot,ax=sp[spi[0]],ylim=histolim,ylabel=f'{d_col} [pixels]',**plot_style['good_data'])
     sp[spi[0]].get_legend().remove()
 
     
@@ -332,14 +338,15 @@
         
     #phot.t.loc[ixs,d_col_rot] = phot.t.loc[ixs,d_col] - f(phot.t.loc[ixs,col],slope,intercept)
     phot.t[d_col_rot] = phot.t[d_col] - f(phot.t[col],slope,intercept)
 
     # get the histogram
     d_rotated = phot.t.loc[ixs,d_col_rot]
     bins = np.arange(np.min(d_rotated),np.max(d_rotated)+binsize,binsize)
+    
     if bin_weights_flag:
         histo = np.histogram(d_rotated,bins=bins,weights=phot.t.loc[ixs,'__weights'])
     else:
         histo = np.histogram(d_rotated,bins=bins)
 
     histotable=pdastroclass()            
     if apply_rolling_gaussian:
@@ -400,15 +407,15 @@
                      spi=spi,
                      histolim = [bincenter4maxval-8,bincenter4maxval+8],
                      title=f'slope:{slope}')
 
 def rotate_d_and_find_binmax(phot,ixs,d_col,col,
                              Naxis_px, # Nx or Ny, depending on col
                              apply_rolling_gaussian=True,
-                             gaussian_sigma_px=0.22,
+                             gaussian_sigma_px=0.022,
                              d_col_rot='d_rot_tmp',
                              binsize=0.02,
                              bin_weights_flag=False,
                              slope_min=-10.0/2048.0, # 
                              slope_max=10.0/2048.0, # 
                              slope_stepsize=1.0/2048,
                              showplots=0,
@@ -575,14 +582,15 @@
                   slope_min=-10.0/2048.0, # 
                   slope_max=10.0/2048.0, # 
                   slope_stepsize=1.0/2048,
                   #This is the first rough cut:  get rid of everything d_rot_bestguess+-Nfwhm*fwhm,
                   Nfwhm=2.0,
                   rough_cut_px_min=None,
                   rough_cut_px_max=None,
+                  gaussian_sigma_px=0.2,
                   Nsigma=3.0,
                   showplots=0,
                   verbose=0,
                   sp=None
                   ):
     if verbose:
         print(f'### Doing histogram cut for {d_col}, slope_min:{slope_min:.6f} slope_max:{slope_max:.6f} slope_stepsize:{slope_stepsize:.6f}')
@@ -600,14 +608,15 @@
                                                         d_col_rot=d_col_rot,
                                                         binsize=binsize,
                                                         bin_weights_flag=bin_weights_flag,
                                                         slope_min=slope_min,
                                                         slope_max=slope_max,
                                                         slope_stepsize=slope_stepsize,
                                                         showplots=showplots,
+                                                        gaussian_sigma_px=gaussian_sigma_px,
                                                         sp=sp,
                                                         verbose=verbose,
                                                         spi=[0,1,2,3,4])
     
     # Using the best dy_rotated, we first remove all entries with dy_rotated outside of dy_bestguess+-Nfwhm*fwhm
     # Note that FWHM ~ 2.355 stdev, so Nfwhm*fwhm should be at least 3*stdev. This is the first ROUGH cut, with 
     # which we just want to remove excessive amounts of outliers. Then a 3-sigma cut is done on the *rotated* dy
@@ -735,14 +744,18 @@
             encircled energy percentage (multiples of 10) for photometry
     rough_cut_px_min : float
             first rough cut: best d_rotated+-rough_cut_pix. This is the lower limit for rough_cut
     rough_cut_px_max : float
             first rough cut: best d_rotated+-rough_cut_pix. This is the upper limit for rough_cut 
     d_rotated_Nsigma : float
             Nsigma for sigma cut of d_rotated. If 0.0, then 3-sigma cut is skipped 
+    gaussian_sigma_px: float
+        Nsigma for rolling gaussian fit to histogram
+    binsize_px: float
+        Bin size in pixels for histogram cuts
     """
     def __init__(self):
         self.verbose=0
         self.outdir = None
         
         self.telescope = None
         
@@ -753,22 +766,26 @@
         self.sip_err = 0.1
         self.sip_degree = 3
         self.sip_points = 128
 
         self.rough_cut_px_min=0.3
         self.rough_cut_px_max=0.8
 
-        self.d_rotated_Nsigma=3.0        
+        self.d_rotated_Nsigma=3.0     
+        self.gaussian_sigma_px=0.2
+        self.binsize_px=0.02
 
     def define_options(self,parser=None,usage=None,conflict_handler='resolve'):
         if parser is None:
             parser = argparse.ArgumentParser(usage=usage,conflict_handler=conflict_handler)
 
         #parser.add_argument('--rate_dir', default=ratedir, help='Directory in which the rate images are located, which will be used to test the distortions. (default=%(default)s)')
         parser.add_argument('cal_image',  help='cal.fits filename or any other image that is at a similar reduction stage.')
+        parser.add_argument('--distortion_file', default=None, help='apply distortion coefficients from given file to image before aligning the image (default=%(default)s)')
+
 
         parser = self.default_options(parser)
         return(parser)
 
     def default_options(self,parser):
 
         # default directory for input images
@@ -791,28 +808,31 @@
 
         parser.add_argument('--skip_if_exists', default=False, action='store_true', help='Skip doing the analysis of a given input image if the cal file already exists, assuming the full analysis has been already done')
 
         parser.add_argument('-v','--verbose', default=0, action='count')
 
         parser.add_argument('--SNR_min', default=None,type=float, help='mininum SNR for object in image to be used for analysis (default=%(default)s)')
 
-        parser.add_argument('--use_dq', default=False, action='store_true', help='use the DQ extensions for masking')
-
+        parser.add_argument('--skip_use_dq', default=False, action='store_true', help='skip using the DQ extensions for masking')
 
         parser.add_argument('--refcat', default='Gaia', help='reference catalog. Can be a filename or Gaia (default=%(default)s)')
         parser.add_argument('--refcat_racol', default=None, help='RA column of reference catalog. If None, then automatically determined (default=%(default)s)')
         parser.add_argument('--refcat_deccol', default=None, help='Dec column of reference catalog. If None, then automatically determined (default=%(default)s)')
         parser.add_argument('--refcat_magcol', default=None, help='mag column of reference catalog. If None and not one of the default refcats like gaia, then 3rd column is used (default=%(default)s)')
         parser.add_argument('--refcat_magerrcol', default=None, help='magerr column of reference catalog. If None, then not used  (default=%(default)s)')
         parser.add_argument('--refcat_colorcol', default=None, help='color column of reference catalog. If None, then not used (default=%(default)s)')
         parser.add_argument('--refcat_pmflag', default=False, action='store_true', help='Apply the proper motion correction (only for catalogs it is applicable, e.g., gaia')
         parser.add_argument('--refcat_pmmedian', default=False, action='store_true', help='Apply the MEDIAN proper motion correction (only for catalogs it is applicable, e.g., gaia')
         parser.add_argument('--photfilename', default='auto', help='photometry output filename. if "auto", the fits in the image filename is substituted with phot.txt (default=%(default)s)')
 #        parser.add_argument('--photfilename', default='auto', help='photometry output filename. if "auto", the fits in the image filename is substituted with phot.txt (default=%(default)s)')
 
+        parser.add_argument('--photometry_method', default='aperture', choices=['aperture','psf'], help='photometry method (default=%(default)s)')
+        parser.add_argument('--find_stars_threshold', default=3.0, type=float, help='Nsigma threshold used for the  photutils find_stars method (default=%(default)s)')
+        parser.add_argument('--sci_xy_catalog', default=None, help='Pass a file with xy positions, which are used instead of the internal photometry x,y positions. The column names need to be called "x" and "y".')
+
         parser.add_argument('--load_photcat_if_exists', default=False, action='store_true', help='If the photometric catalog file already exists, skip recreating it.')
         parser.add_argument('--rematch_refcat', default=False, action='store_true', help='if --load_photcat_if_exists and the photcat already exists, load the photcat, but rematch with refcat')
 
         parser.add_argument('--d2d_max', default=None, type=float, help='maximum distance between source in image and refcat object, in arcsec (default=%(default)s)')
         parser.add_argument('--dmag_max', default=None, type=float, help='maximum uncertainty of sources in image (default=%(default)s)')
         parser.add_argument('--sharpness_lim', default=(None,None), nargs=2, type=float, help='sharpness limits of sources in image (default=%(default)s)')
         parser.add_argument('--roundness1_lim', default=(-0.75,0.75), nargs=2, type=float, help='roundness1 limits of sources in image (default=%(default)s)')
@@ -835,15 +855,18 @@
         parser.add_argument('--sip_degree', default=3, type=int,help='degree for SIP transformation.  (default=%(default)s)')
         parser.add_argument('--sip_points', default=128, type=int,help='npoints for SIP transformation.  (default=%(default)s)')
         parser.add_argument('--ee_radius', default=70, type=int, help='encircled energy percentage (multiples of 10) for photometry.  (default=%(default)s)')
         parser.add_argument('--is_hst', default=False, action='store_true', help='set if your image is from hst not jwst')
         parser.add_argument('--rough_cut_px_min', default=0.3, type=float,help='first rough cut: best d_rotated+-rough_cut_pix. This is the lower limit for rough_cut (default=%(default)s)')
         parser.add_argument('--rough_cut_px_max', default=1.0, type=float,help='first rough cut: best d_rotated+-rough_cut_pix. This is the upper limit for rough_cut (default=%(default)s)')
         parser.add_argument('--d_rotated_Nsigma', default=3.0, type=float,help='Nsigma for sigma cut of d_rotated. If 0.0, then 3-sigma cut is skipped (default=%(default)s)')
-
+        parser.add_argument('--gaussian_sigma_px', default=0.2, type=float,help='Nsigma for rolling gaussian fit to histogram (default=%(default)s)')
+        parser.add_argument('--binsize_px', default=0.02, type=float,help='Histogram binsize (default=%(default)s)')
+        
+        
         return(parser)
     
     def set_telescope(self,telescope=None,imname=None):
         """
         Figuring out which telescope your data come from (HST or JWST).
         Note that if your filename is non-standard, then you MUST set
         """
@@ -1078,15 +1101,15 @@
                                  show_initial_plot=1,
                                  show_histofit_plots=1,
                                  savephottable=1,
                                  outbasename=None,
                                  plots_dxdy_delta_pix_ylim=20,
                                  # histogram cut parameters
                                  histocut_order = 'dxdy', # this can only be 'dxdy' or 'dydx'
-                                 binsize_px = 0.2, # this is the binsize of the dx/dy histograms
+                                 binsize_px = 0.02, # this is the binsize of the dx/dy histograms
                                  bin_weights_flag=False,# If bin_weights_flag is set to True, 
                                                        #then the dx/dy bins are weighted by 
                                                        # the flux of the detection.
                                  slope_min=-10/2048.0, 
                                  slope_Nsteps = 200, # slope_max=-slope_min, slope_stepsize=(slope_max-slope_min)/slope_Nsteps
                                  Nfwhm = 2.5 
                                  ):
@@ -1171,28 +1194,30 @@
                                                 bin_weights_flag=bin_weights_flag,
                                                 slope_min=slope_min,
                                                 slope_max=slope_max,
                                                 slope_stepsize=slope_stepsize,
                                                 Nfwhm=Nfwhm,
                                                 rough_cut_px_min=self.rough_cut_px_min,
                                                 rough_cut_px_max=self.rough_cut_px_max,
+                                                gaussian_sigma_px=self.gaussian_sigma_px,
                                                 Nsigma=self.d_rotated_Nsigma,
                                                 showplots=show_histofit_plots,
                                                 verbose=self.verbose)
 
         # Do the histogram cut on the second dcol (dx or dy, as selected)
         (ixs_cut2,rot_results2) = histogram_cut(phot,ixs_cut1,d_col2,col2,Naxis2_px,
                                                 binsize=binsize_px,
                                                 bin_weights_flag=bin_weights_flag,
                                                 slope_min=slope_min,
                                                 slope_max=slope_max,
                                                 slope_stepsize=slope_stepsize,
                                                 Nfwhm=Nfwhm,
                                                 rough_cut_px_min=self.rough_cut_px_min,
                                                 rough_cut_px_max=self.rough_cut_px_max,
+                                                gaussian_sigma_px=self.gaussian_sigma_px,
                                                 Nsigma=self.d_rotated_Nsigma,
                                                 showplots=show_histofit_plots,
                                                 verbose=self.verbose)
 
 
         if savephottable:
             #print(f'Saving {outbasename}.good.phot.txt')
@@ -1314,20 +1339,28 @@
             #for i in range(len(x1)):
             #    if not 0<x1[i]<old_model['SCI',1].data.shape[1] or not\
             #        0<y1[i]<old_model['SCI',1].data.shape[0]:
             #        x1[i],y1[i] = skycoord_to_pixel(SkyCoord(phot.t[refcat_racol][i],
             #                        phot.t[refcat_deccol][i],unit=u.deg),oldwcs2)
             phot.t[refcat_xcol] = x1
             phot.t[refcat_ycol] = y1
-        else:
+        elif self.telescope.lower()=='hst':
             phot.t[refcat_xcol], phot.t[refcat_ycol] = skycoord_to_pixel(SkyCoord(phot.t[refcat_racol],
                 phot.t[refcat_deccol],unit=u.deg),imwcs)
             sc = pixel_to_skycoord(phot.t['x'],phot.t['y'],imwcs)
             phot.t['ra'] = sc.ra.value
             phot.t['dec'] = sc.dec.value
+        else:
+            image_model = datamodels.ImageModel(outputfits)
+            phot.t[refcat_xcol], phot.t[refcat_ycol] = image_model.meta.wcs.world_to_pixel(SkyCoord(phot.t[refcat_racol],
+                phot.t[refcat_deccol],unit=u.deg))
+            sc = image_model.meta.wcs.pixel_to_world(phot.t['x'],phot.t['y'])
+            phot.t['ra'] = sc.ra.value
+            phot.t['dec'] = sc.dec.value
+            
 
         # recalculate dx, dy
         phot.t['dx'] = phot.t[refcat_xcol] - phot.t['x']
         phot.t['dy'] = phot.t[refcat_ycol] - phot.t['y']
 
         # recalculate the RA, Dec of the image objects
         #detector_to_world = image_model.meta.wcs.get_transform('detector', 'world')
@@ -1356,15 +1389,14 @@
                         rmfile(outfilename)
                 if self.verbose:        
                     print(f'Saving {outfilename}')
                 phot.write(outfilename)
 
         # show or save dxdy post WCS correction
         if showplots>=0 or saveplots:
-            print('should be plotting')
             dxdy_plot(phot, ixs_bestmatch,title='after WCS correction',
                       refcat_mainfilter=phot.refcat_mainfilter,
                       refcat_mainfilter_err=phot.refcat_mainfilter_err,
                       refcat_maincolor=phot.refcat_maincolor)
             if saveplots:
                 outfilename = f'{outbasename}.phot.finalwcs.png'
                 if os.path.isfile(outfilename):
@@ -1372,25 +1404,91 @@
                 if self.verbose:
                     print(f'Saving {outfilename}')
                 plt.savefig(outfilename)
             if showplots>0:
                 plt.show()
             plt.close()
 
+    def apply_distortion_coefficients(self,input_image,distortion_file,outdir=None,
+                                      overwrite=True, skip_if_exists=False):
+        
+        scihdr = fits.getheader(input_image)
+        dummy_filename = f'{scihdr["APERNAME"].lower()}_{scihdr["FILTER"].lower()}_{scihdr["PUPIL"].lower()}.polycoeff.asdf'
+        if dummy_filename != os.path.basename(distortion_file):
+            print(f'\n!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n!!! WARNING! distortion file {os.path.basename(distortion_file)} is not as expected {dummy_filename}!'
+                  f' The image has aperture={scihdr["APERNAME"]}, filter={scihdr["FILTER"]}, and pupil={scihdr["PUPIL"]}, is that consistent with the distortion file???\n'
+                  '!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n')
+
+        print(f'assigning WCS to file {input_image} using distortion file {distortion_file}')
+        step = AssignWcsStep()
+
+        if not os.path.isfile(input_image):
+            raise RuntimeError(f'image {input_image} does not exist')
+
+        if distortion_file.lower() == 'none':
+            print('WARNING!! not applying any distortion file!!')
+        else:
+            if re.search('\.asdf$',distortion_file) is None:
+                raise RuntimeError(f'distortion file {distortion_file} does not have .asdf suffix. asdf format required.')
+            if not os.path.isfile(distortion_file):
+                raise RuntimeError(f'distortion file {distortion_file} does not exist')
+            step.override_distortion = distortion_file
 
+        step.save_results = True
+ 
+        if outdir is None:
+            outdir=os.path.dirname(input_image)
+        if self.verbose: print(f'Setting output directory for assignwcsstep.fits file to {outdir}')
+        
+        assignwcsfilename = re.sub('\_[a-zA-Z0-9]+\.fits$','_assignwcsstep.fits',os.path.basename(input_image))
+        if assignwcsfilename == os.path.basename(input_image):
+            raise RuntimeError('Could not get assignwcsstep filename from {os.path.basename(input_image)}!')
+        assignwcsfilename = f'{outdir}/{assignwcsfilename}'
+
+        
+        
+        step.output_dir = outdir
+        if not os.path.isdir(outdir):
+            makepath(outdir)
+
+        if os.path.isfile(assignwcsfilename):
+            if skip_if_exists:
+                # return False means that rate2cal did not run
+                print(f'Image {assignwcsfilename} already exists, skipping recreating it...')
+                return(False,assignwcsfilename)
+            else:
+                if overwrite:
+                    print(f'WARNING! {assignwcsfilename} exists, deleting it since "overwrite" is set!')
+                    # make sure cal frame is deleted
+                    rmfile(assignwcsfilename)
+                else:
+                    raise RuntimeError(f'Image {assignwcsfilename} already exists! exiting. If you want to overwrite or skip, you can use "overwrite" or "skip_if_exists"')
+                
+        print(f'Creating {assignwcsfilename}')
+        step.run(input_image)
+        
+        #make sure the image got created
+        if not os.path.isfile(assignwcsfilename):
+            raise RuntimeError(f'Image {assignwcsfilename} did not get created!!')
+        else:
+            print(f'distortions {distortion_file} applied to {assignwcsfilename}!!')
+        return(True,assignwcsfilename)
 
     def run_all(self,input_image,
                 telescope=None,
-                #distortion_file=None,
                 outrootdir = None,
                 outsubdir = None,
                 overwrite = False,
+                distortion_file = None,
                 skip_if_exists = False,
                 #skip_applydistortions_if_exists = False,
                 use_dq=False,
+                photometry_method='aperture',
+                find_stars_threshold = 3.0,
+                sci_xy_catalog=None,
                 # refcat parameters
                 refcatname = 'Gaia',
                 refcat_racol='auto',
                 refcat_deccol='auto',
                 refcat_magcol = None,
                 refcat_magerrcol = None,
                 refcat_colorcol = None,
@@ -1416,35 +1514,51 @@
                 Nfwhm = 2.5,
                 xshift=0.0,# added to the x coordinate before calculating ra,dec. This can be used to correct for large shifts before matching!
                 yshift=0.0, # added to the y coordinate before calculating ra,dec. This can be used to correct for large shifts before matching!
                 iterate_with_xyshifts = False,
                 showplots=0,
                 saveplots=0,
                 savephottable=0,
-                ee_radius=70                ):
+                psf_model=None,
+                ee_radius=70,
+                **kwargs):
+        
+        for k in kwargs.keys():
+            if k in self.__dict__.keys():
+                self.__dict__[k] = kwargs[k]
             
         # set self.outbasename based on option
         self.set_outbasename(outrootdir=outrootdir,outsubdir=outsubdir,inputname=input_image)
         
         # set the telescope
         self.set_telescope(telescope=telescope,imname=input_image)
-            
+        
+        if distortion_file is not None:
+            runflag,assignwcs_filename = self.apply_distortion_coefficients(input_image,distortion_file,outdir=os.path.dirname(self.outbasename))
+            input_image = assignwcs_filename
+        else:
+            assignwcs_filename = None
+        
         # do the photometry
         self.phot.verbose = self.verbose
         photfilename = f'{self.outbasename}.phot.txt'
         (photfilename_4check,photcat_loaded) = self.phot.run_phot(input_image,
                                                                   use_dq=use_dq,
                                                                   photfilename=photfilename,
                                                                   load_photcat_if_exists=load_photcat_if_exists,
                                                                   overwrite=overwrite,
                                                                   Nbright4match=Nbright4match,
                                                                   SNR_min=SNR_min,
                                                                   xshift=xshift,
                                                                   yshift=yshift,
-                                                                  ee_radius=ee_radius)
+                                                                  ee_radius=ee_radius,
+                                                                  sci_xy_catalog=sci_xy_catalog,
+                                                                  psf_model=psf_model,
+                                                                  photometry_method=photometry_method,
+                                                                  find_stars_threshold = find_stars_threshold)
         if (photfilename!=photfilename_4check):
             raise RuntimeError(f'BUG!!! {photfilename}!={photfilename_4check}')
             
         # make the initial cut on the image photometry catalog on magnitudes, sharpness, roundness etc
         ixs_use = self.phot.initial_cut_photcat(dmag_max = dmag_max,
                                                 sharpness_lim = sharpness_lim, # sharpness limits
                                                 roundness1_lim = roundness1_lim, # roundness1 limits 
@@ -1479,15 +1593,16 @@
                                                      histocut_order=histocut_order,
                                                      slope_min=slope_min, 
                                                      slope_Nsteps = slope_Nsteps, # slope_max=-slope_min, slope_stepsize=(slope_max-slope_min)/slope_Nsteps
                                                      Nfwhm = Nfwhm,
                                                      show_initial_plot=showplots,
                                                      show_histofit_plots=showplots,
                                                      savephottable=savephottable,
-                                                     outbasename=self.outbasename
+                                                     outbasename=self.outbasename,
+                                                     binsize_px=self.binsize_px
                                                      )     
         
         # If iterate with x/yshift
         if iterate_with_xyshifts:
             # get the median of dx and dy of the best matched objects from the first iteration!
             dx_median = self.phot.t.loc[ixs_bestmatch,'dx'].median()
             dy_median = self.phot.t.loc[ixs_bestmatch,'dy'].median()
@@ -1516,22 +1631,26 @@
                                                          histocut_order=histocut_order,
                                                          slope_min=slope_min, 
                                                          slope_Nsteps = slope_Nsteps, # slope_max=-slope_min, slope_stepsize=(slope_max-slope_min)/slope_Nsteps
                                                          Nfwhm = Nfwhm,
                                                          show_initial_plot=0,
                                                          show_histofit_plots=showplots,
                                                          savephottable=savephottable,
-                                                         outbasename=self.outbasename
+                                                         outbasename=self.outbasename,
+                                                         binsize_px=self.binsize_px
                                                          )     
 
         jhatfits = f'{self.outbasename}_jhat.fits'
         (runflag,jhatfits) = self.run_align2refcat(input_image,
                                                    outputfits=jhatfits,
                                                    ixs=ixs_bestmatch,
                                                    overwrite=overwrite,skip_if_exists=skip_if_exists)
+        if assignwcs_filename is not None:
+            rmfile(assignwcs_filename)
+        
         #if self.telescope.lower()=='jwst':
         self.update_phottable_final_wcs(jhatfits,
                                             ixs_bestmatch = ixs_bestmatch,
                                             showplots=showplots,
                                             saveplots=saveplots,
                                             savephottable=savephottable,
                                             overwrite=overwrite
```

## jhat/st_wcs_align_batch.py

```diff
@@ -201,15 +201,19 @@
                   outrootdir=None, 
                   outsubdir=None,
                   addfilter2outsubdir=False,
                   overwrite = False,
                   skip_if_exists = False,
                   telescope = None,
                   #skip_applydistortions_if_exists = False,
+                  photometry_method = 'aperture',
+                  find_stars_threshold = 3.0,
+                  sci_xy_catalog=None,
                   # refcat parameters
+                  use_dq=False,
                   refcatname = 'Gaia',
                   refcat_racol='auto',
                   refcat_deccol='auto',
                   refcat_magcol = None,
                   refcat_magerrcol = None,
                   refcat_colorcol = None,
                   pmflag = False,
@@ -267,14 +271,18 @@
                                        #distortion_file=distfile,  
                                        telescope = telescope,
                                        outrootdir = outrootdir,
                                        outsubdir = outsubdir_filter,
                                        overwrite = overwrite,
                                        skip_if_exists = skip_if_exists,
                                        #skip_applydistortions_if_exists=skip_applydistortions_if_exists,
+                                       photometry_method = photometry_method,
+                                       find_stars_threshold = find_stars_threshold,
+                                       sci_xy_catalog=sci_xy_catalog,
+                                       use_dq = use_dq,
                                        refcatname = refcatname,
                                        refcat_racol = refcat_racol,
                                        refcat_deccol = refcat_deccol,
                                        refcat_magcol=refcat_magcol,
                                        refcat_magerrcol=refcat_magerrcol,
                                        refcat_colorcol=refcat_colorcol,
                                        pmflag = pmflag,
@@ -306,14 +314,18 @@
                                            #distortion_file=distfile,                     
                                            telescope = telescope,
                                            outrootdir = outrootdir,
                                            outsubdir = outsubdir_filter,
                                            overwrite = overwrite,
                                            skip_if_exists = skip_if_exists,
                                            #skip_applydistortions_if_exists=skip_applydistortions_if_exists,
+                                           photometry_method = photometry_method,
+                                           find_stars_threshold = find_stars_threshold,
+                                           sci_xy_catalog=sci_xy_catalog,
+                                           use_dq = use_dq,
                                            refcatname = refcatname,
                                            refcat_racol = refcat_racol,
                                            refcat_deccol = refcat_deccol,
                                            refcat_magcol=refcat_magcol,
                                            refcat_magerrcol=refcat_magerrcol,
                                            refcat_colorcol=refcat_colorcol,
                                            pmflag = pmflag,
```

## Comparing `jhat-0.1.8.data/scripts/run_st_wcs_align.py` & `jhat-0.1.9.data/scripts/run_st_wcs_align.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,21 @@
 
 
 wcs_align.run_all(args.cal_image,
                  telescope = args.telescope,
                  #distortion_file = args.distortion_file,
                  outrootdir = args.outrootdir,
                  outsubdir = args.outsubdir,
+                 distortion_file = args.distortion_file,
                  overwrite = args.overwrite,
+                 photometry_method = args.photometry_method,
+                 find_stars_threshold = args.find_stars_threshold,
+                 sci_xy_catalog=args.sci_xy_catalog,
                  #skip_applydistortions_if_exists=args.skip_applydistortions_if_exists,
-                 use_dq = args.use_dq,
+                 use_dq = not args.skip_use_dq,
                  refcatname = args.refcat,
                  refcat_racol = args.refcat_racol,
                  refcat_deccol = args.refcat_deccol,
                  refcat_magcol = args.refcat_magcol,
                  refcat_magerrcol = args.refcat_magerrcol,
                  refcat_colorcol = args.refcat_colorcol,
                  pmflag = args.refcat_pmflag,
```

## Comparing `jhat-0.1.8.data/scripts/run_st_wcs_align_batch.py` & `jhat-0.1.9.data/scripts/run_st_wcs_align_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,18 @@
 align_batch.align_wcs(ixs_todo,
                     overwrite = args.overwrite,
                     outrootdir= args.outrootdir,
                     outsubdir = args.outsubdir,
                     addfilter2outsubdir = args.addfilter2outsubdir,
                     telescope = args.telescope,
                     #skip_applydistortions_if_exists=args.skip_applydistortions_if_exists,
+                    photometry_method = args.photometry_method,
+                    find_stars_threshold = args.find_stars_threshold,
+                    sci_xy_catalog=args.sci_xy_catalog,
+                    use_dq = not args.skip_use_dq,
                     refcatname = args.refcat,
                     refcat_racol = args.refcat_racol,
                     refcat_deccol = args.refcat_deccol,
                     refcat_magcol = args.refcat_magcol,
                     refcat_magerrcol = args.refcat_magerrcol,
                     refcat_colorcol = args.refcat_colorcol,
                     pmflag = args.refcat_pmflag,
```

## Comparing `jhat-0.1.8.dist-info/RECORD` & `jhat-0.1.9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-bin/run_st_wcs_align.py,sha256=CGM_5dPSDR8ltVdD-YXi4RJ7N5YbdqL0LPFACMDT9hc,3406
-bin/run_st_wcs_align_batch.py,sha256=M3ot__TVa7xaGrhx_qcan4wfv52Q02DlxYGCcluJuPM,5313
+bin/run_st_wcs_align.py,sha256=IvwlrooZmWZ3tqAlvTHnf2bjLGo22BiF8-mX-C8Mlo0,3653
+bin/run_st_wcs_align_batch.py,sha256=nB_zjdZcH-TCbXErgi8cV-90Nn-4hTu7Y5OxD_HnKpQ,5554
 bin/st_wcs_align,sha256=iQCWenevrh7-aei8Lj6xy81UtXioHsN9o8FqVLXblPI,3124
 bin/st_wcs_align_batch,sha256=4oFo2Y-4N_Dz6igObjsCe-rkUr5qOaFwIhyPDNP_qVE,5059
 jhat/__init__.py,sha256=1ldZLh2uImIXe-OIpYYKr3SGzlj2zJbH5nWyj_8pjWw,3502
 jhat/pdastro.py,sha256=9LlLeF0fsrW11-qQJsd8EGR_RgOZgXcRVSp10nbUe2Q,59300
-jhat/simple_jwst_phot.py,sha256=HHjo0rG68AgSghE5Tj2PGEoz2PJ6WdjhH0wy6ZIxAR4,100096
+jhat/simple_jwst_phot.py,sha256=BskcE7ghqE8rDTeDV3bjAUyxQ1Q_1bmwTnmOCjfTVo8,109775
 jhat/simple_jwst_phot_temp.py,sha256=hMf3Bm66j_aZrv3w7dBYYhBI2cHQxY6qjSgEJKyhl7k,103074
-jhat/st_wcs_align.py,sha256=fLCCQRqwCrtRA-ZHqQBP8iTl66mkBMv_KSZqqfRfkVs,83391
-jhat/st_wcs_align_batch.py,sha256=E3pyqFUacekJzwGQebIfgtDiojGLHK6BoddGGmXEP-E,20192
+jhat/st_wcs_align.py,sha256=dlAdCEj7NDT984Dcve98Y8nPjcBFSp8s9iBXeTkG_7A,90072
+jhat/st_wcs_align_batch.py,sha256=Y2MP10OEOsg1afnONsVYdiXfyhrtzRsIQz94mWNo3Ks,20951
 jhat/st_wcs_align_temp.py,sha256=eqF1Ih4WSyEKiP0eCu_VFHp6Iz1ypy5LFY40fQT8j2s,83510
 jhat/test_jhat.py,sha256=gjZE-iogZj-KDnLzKKeqAuaFishf69uUjHNMTqjWKTI,480
-jhat-0.1.8.data/scripts/run_st_wcs_align.py,sha256=ADzGVN26KqT8cCOaYW1j65Y-BIY5CqJWAwhGcN_-TnI,3392
-jhat-0.1.8.data/scripts/run_st_wcs_align_batch.py,sha256=aQP8SvafrvCaH5Doay8LqWiizeoVEjTC9b6h22IjGXA,5300
-jhat-0.1.8.dist-info/METADATA,sha256=5OBrDxa5ysk3cS2SjDsfi1sbk9RkA1nx-GpPNKf5jZA,471
-jhat-0.1.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-jhat-0.1.8.dist-info/top_level.txt,sha256=vzk1Odzduniwh8nqkRvjd5qpRf5LIw701hBBYY0lrXM,9
-jhat-0.1.8.dist-info/RECORD,,
+jhat-0.1.9.data/scripts/run_st_wcs_align.py,sha256=_ep5tIA0vPIqxsMYQmPPAzPacAbtad7wwkka5eNrL0E,3639
+jhat-0.1.9.data/scripts/run_st_wcs_align_batch.py,sha256=Op6B5kfD8NbqRUo8dskMl1HRuQbLeUqcF12evn1EYoA,5541
+jhat-0.1.9.dist-info/METADATA,sha256=pHGP5qt1lMKPCgRAIwWZcryY50Lg0LPgDj4TBxffC5E,471
+jhat-0.1.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+jhat-0.1.9.dist-info/top_level.txt,sha256=vzk1Odzduniwh8nqkRvjd5qpRf5LIw701hBBYY0lrXM,9
+jhat-0.1.9.dist-info/RECORD,,
```

