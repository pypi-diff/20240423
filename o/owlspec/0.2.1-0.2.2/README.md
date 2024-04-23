# Comparing `tmp/owlspec-0.2.1.tar.gz` & `tmp/owlspec-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owlspec-0.2.1.tar", last modified: Mon Apr 22 13:47:43 2024, max compression
+gzip compressed data, was "owlspec-0.2.2.tar", last modified: Tue Apr 23 21:47:44 2024, max compression
```

## Comparing `owlspec-0.2.1.tar` & `owlspec-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 13:47:43.467621 owlspec-0.2.1/
--rw-rw-rw-   0        0        0     1089 2024-04-20 00:47:16.000000 owlspec-0.2.1/LICENSE
--rw-rw-rw-   0        0        0    15742 2024-04-22 13:47:43.467621 owlspec-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    15236 2024-04-20 17:21:16.000000 owlspec-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 13:47:43.325900 owlspec-0.2.1/owlspec/
--rw-rw-rw-   0        0        0      313 2024-04-20 15:14:45.000000 owlspec-0.2.1/owlspec/__init__.py
--rw-rw-rw-   0        0        0     8238 2024-04-20 15:19:49.000000 owlspec-0.2.1/owlspec/emission_line.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:47:43.389011 owlspec-0.2.1/owlspec/emitter/
--rw-rw-rw-   0        0        0       65 2024-04-20 15:11:09.000000 owlspec-0.2.1/owlspec/emitter/__init__.py
--rw-rw-rw-   0        0        0     5561 2024-04-20 15:14:23.000000 owlspec-0.2.1/owlspec/emitter/level.py
--rw-rw-rw-   0        0        0     4328 2024-04-20 15:14:19.000000 owlspec-0.2.1/owlspec/emitter/transition.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:47:43.404660 owlspec-0.2.1/owlspec/nist_levels/
--rw-rw-rw-   0        0        0      694 2024-04-20 00:47:16.000000 owlspec-0.2.1/owlspec/nist_levels/__init__.py
--rw-rw-rw-   0        0        0     5230 2024-04-20 00:47:16.000000 owlspec-0.2.1/owlspec/nist_levels/core.py
--rw-rw-rw-   0        0        0    10043 2024-04-20 15:11:11.000000 owlspec-0.2.1/owlspec/spectrum.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:47:43.455072 owlspec-0.2.1/owlspec/stark/
--rw-rw-rw-   0        0        0       39 2022-05-12 14:02:58.000000 owlspec-0.2.1/owlspec/stark/__init__.py
--rw-rw-rw-   0        0        0     8133 2023-11-24 23:39:14.000000 owlspec-0.2.1/owlspec/stark/gigosos_he_loader.py
--rw-rw-rw-   0        0        0     7066 2023-11-24 23:40:20.000000 owlspec-0.2.1/owlspec/stark/gigosos_loader.py
--rw-rw-rw-   0        0        0     3105 2024-04-20 00:47:16.000000 owlspec-0.2.1/owlspec/stark/griem.py
--rw-rw-rw-   0        0        0     3386 2023-11-24 21:43:57.000000 owlspec-0.2.1/owlspec/stark/stark.py
--rw-rw-rw-   0        0        0     6606 2024-04-20 15:11:07.000000 owlspec-0.2.1/owlspec/util.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:47:43.467621 owlspec-0.2.1/owlspec/vdW/
--rw-rw-rw-   0        0        0       37 2022-05-12 14:06:55.000000 owlspec-0.2.1/owlspec/vdW/__init__.py
--rw-rw-rw-   0        0        0     4518 2024-04-20 15:11:10.000000 owlspec-0.2.1/owlspec/vdW/vdW.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:47:43.357648 owlspec-0.2.1/owlspec.egg-info/
--rw-rw-rw-   0        0        0    15742 2024-04-22 13:47:43.000000 owlspec-0.2.1/owlspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2024-04-22 13:47:43.000000 owlspec-0.2.1/owlspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 13:47:43.000000 owlspec-0.2.1/owlspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2024-04-22 13:47:43.000000 owlspec-0.2.1/owlspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-22 13:47:43.000000 owlspec-0.2.1/owlspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 13:47:43.467621 owlspec-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      920 2024-04-22 03:55:48.000000 owlspec-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:47:44.106662 owlspec-0.2.2/
+-rw-rw-rw-   0        0        0     1089 2024-04-19 19:45:30.000000 owlspec-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0    15742 2024-04-23 21:47:44.106662 owlspec-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    15236 2024-04-23 21:44:09.000000 owlspec-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 21:47:44.075288 owlspec-0.2.2/owlspec/
+-rw-rw-rw-   0        0        0      323 2024-04-23 21:44:09.000000 owlspec-0.2.2/owlspec/__init__.py
+-rw-rw-rw-   0        0        0     8427 2024-04-23 21:44:09.000000 owlspec-0.2.2/owlspec/emission_line.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:47:44.095531 owlspec-0.2.2/owlspec/emitter/
+-rw-rw-rw-   0        0        0       68 2024-04-19 19:45:30.000000 owlspec-0.2.2/owlspec/emitter/__init__.py
+-rw-rw-rw-   0        0        0     5561 2024-04-19 20:27:41.000000 owlspec-0.2.2/owlspec/emitter/level.py
+-rw-rw-rw-   0        0        0     4328 2024-04-23 21:44:09.000000 owlspec-0.2.2/owlspec/emitter/transition.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:47:44.095531 owlspec-0.2.2/owlspec/nist_levels/
+-rw-rw-rw-   0        0        0      694 2024-04-19 22:49:41.000000 owlspec-0.2.2/owlspec/nist_levels/__init__.py
+-rw-rw-rw-   0        0        0     5230 2024-04-19 19:50:47.000000 owlspec-0.2.2/owlspec/nist_levels/core.py
+-rw-rw-rw-   0        0        0    10392 2024-04-23 21:44:09.000000 owlspec-0.2.2/owlspec/spectrum.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:47:44.105153 owlspec-0.2.2/owlspec/stark/
+-rw-rw-rw-   0        0        0       41 2024-04-19 19:45:30.000000 owlspec-0.2.2/owlspec/stark/__init__.py
+-rw-rw-rw-   0        0        0     8360 2024-04-19 19:45:30.000000 owlspec-0.2.2/owlspec/stark/gigosos_he_loader.py
+-rw-rw-rw-   0        0        0     7268 2024-04-19 19:45:30.000000 owlspec-0.2.2/owlspec/stark/gigosos_loader.py
+-rw-rw-rw-   0        0        0     3105 2024-04-19 20:31:25.000000 owlspec-0.2.2/owlspec/stark/griem.py
+-rw-rw-rw-   0        0        0     3474 2024-04-19 19:45:30.000000 owlspec-0.2.2/owlspec/stark/stark.py
+-rw-rw-rw-   0        0        0     6606 2024-04-19 21:17:52.000000 owlspec-0.2.2/owlspec/util.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:47:44.106662 owlspec-0.2.2/owlspec/vdW/
+-rw-rw-rw-   0        0        0       39 2024-04-19 19:45:30.000000 owlspec-0.2.2/owlspec/vdW/__init__.py
+-rw-rw-rw-   0        0        0     4650 2024-04-23 21:44:09.000000 owlspec-0.2.2/owlspec/vdW/vdW.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:47:44.095531 owlspec-0.2.2/owlspec.egg-info/
+-rw-rw-rw-   0        0        0    15742 2024-04-23 21:47:43.000000 owlspec-0.2.2/owlspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2024-04-23 21:47:43.000000 owlspec-0.2.2/owlspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 21:47:43.000000 owlspec-0.2.2/owlspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-04-23 21:47:43.000000 owlspec-0.2.2/owlspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 21:47:43.000000 owlspec-0.2.2/owlspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 21:47:44.106662 owlspec-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      920 2024-04-23 21:45:27.000000 owlspec-0.2.2/setup.py
```

### Comparing `owlspec-0.2.1/LICENSE` & `owlspec-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `owlspec-0.2.1/PKG-INFO` & `owlspec-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owlspec
-Version: 0.2.1
+Version: 0.2.2
 Summary: Library for optical emission spectroscopy of low-temperature plasmas.
 Home-page: https://github.com/mimurrayy/owl
 Author: Julian Held
 Author-email: julian.held@umn.edu
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `owlspec-0.2.1/README.md` & `owlspec-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `owlspec-0.2.1/owlspec/emission_line.py` & `owlspec-0.2.2/owlspec/emission_line.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-#!/bin/python3
-import numpy as np
-from scipy.signal import fftconvolve as convolve
-from scipy import constants as const
-from scipy import interpolate
-from .util import zeeman, parse_spectroscopic_name, doppler_thompson,\
-                        doppler_maxwell, gauss_function, psd_voigt
-from . import stark
-from . import vdW
-import mendeleev 
-
-class emission_line():
-    def __init__(self, transition, wl, instr_func = None, w = None, mu = 0.0,
-                 T = None, Eb = None, gamma = None, B = None, ne = None, 
-                                Te = None, side = False, N = None, pert = None):
-        
-        """  Class to calculate the shape of an emission line based on the 
-        physical situation. Providing information on densities and temperatures
-        automatically switches on different broadening mechanisms.
-
-        Supported broadening mechanisms: Doppler, Stark, Zeeman, van der Waals
-        and instrumental broadening. Stark broadening is only supported for
-        some transitions: H-alpha to gamma, He 447.1 nm, He 492.2 nm, O 777 nm,
-        Ar 810.369 nm and Ar 738.398 nm.
-
-        <transition>: An owl.emitter.transition object for the specific line.
-        <wl>: Center wavelength in nm. Does not need to be the theoretical wl
-              of the transition. Use to move simulation relative to measurement.
-        <instr_func>: Instrumental function of the spectrometer. Must be a 
-                      function that take parameters x and xc (wavelength axis 
-                      and central position) and return the profile as a 
-                      numpy array.
-        <w>: Width of the instrumental function in nm. Only if instr_func=None.
-        <mu>: Shape parameter of the instrumental fucntion. 0=Gauss, 1=Lorentz.
-        Use together with w or use instr_func instead. Only if instr_func=None.
-        <T>: Emitter temperature in Kelvin. Used for vdW and Doppler broadening.
-        <Eb>: Surface binding energy in eV to calculate Doppler broadening of 
-              sputtered particles.
-        <gamma>: Thermalization degree of sputtered particles (used with Eb).
-        <B>: Magnetic field strength for Zeeman splitting. Units of Tesla.
-        <ne>: Electron density for Stark broadening. Units of m^-3. 
-        <Te>: Electron temperature for stark broadening. Units of Kelvin.
-              Has only minor impact on the results and can usually be guessed.
-        <side>: Used for Zeeman and together with gamma. To be updated.
-        <N>: Neutral density for van der Waals broadening. Units of m^-3.
-             This is the density of species sourrounding the emitter.
-        <pert>: Perturber species for vdW and Stark boradening. This is the ion
-                or atom species surrounding the emitter particles. In case vdW 
-                we look up the polarizability of the element. For Stark we only 
-                need the mass. Specify like emitter species, e.g. 'Ar I'.  
-        """
-
-        self.wl = wl
-        self.transition = transition
-        self.instr = instr_func
-        self.w = w
-        self.mu = mu
-        particle = transition.particle
-        self.m  = particle.m
-        self.Ei = particle.Ei
-        self.T  = T
-        self.Eb = Eb
-        self.gamma = gamma
-        self.B  = B
-        self.ne = ne
-        self.Te = Te
-        self.N  = N
-        self.pert = pert
-        self.side = side # symmetric version of Thompson?
-        self.profiles = dict.fromkeys(['Doppler', 'Zeeman', 'Stark', 'vdW', 'instrument'])
-
-        if pert:          
-            self.pert_name, self.pert_charge = parse_spectroscopic_name(pert)
-            self.pert = mendeleev.element(self.pert_name)
-            self.pert.charge = self.pert_charge
-            self.pert.m = self.pert.mass
-            self.pert.Ei = self.pert.ionenergies[1]
-            if T:
-                self.pert.T = T
-            elif Te:
-                self.pert.T = Te*const.eV/const.k
-
-
-
-    def get_profile(self, x, A = 1, instr_func = None, w = None, mu = None,
-            shift = False, wl=None, T = None, Eb = None, gamma = None, B = None,
-            N = None, ne = None, Te = None, pert = None):
-
-        if instr_func == None and self.instr:
-            instr_func = self.instr
-        if w == None and self.w:
-            w = self.w
-        if mu == None and self.mu:
-            mu = self.mu
-        if wl == None and self.wl:
-            wl = self.wl
-        if T == None and self.T:
-            T = self.T
-        if Eb == None and self.Eb:
-            Eb = self.Eb
-        if gamma == None and self.gamma:
-            gamma = self.gamma
-        if B == None and self.B:
-            B = self.B
-        if ne == None and self.ne:
-            ne = self.ne
-        if Te == None and self.Te:
-            Te = self.Te
-        if N == None and self.N:
-            N = self.N
-        if pert == None and self.pert:
-            pert = self.pert
-        
-        elif pert:
-            self.pert_name, self.pert_charge = parse_spectroscopic_name(pert)
-            self.pert = mendeleev.element(self.pert_name)
-            self.pert.charge = self.pert_charge
-            self.pert.m = self.pert.mass
-            self.pert.Ei = self.pert.ionenergies[1]
-            if T:
-                self.pert.T = T
-            elif Te:
-                self.pert.T = Te*const.eV/const.k
-            pert = self.pert
-
-        self.profiles = dict.fromkeys(['x', 'y', 'Doppler', 'Zeeman', 'Stark', 'vdW', 'instrument'])
-        orig_x = np.copy(x)
-        s = 0 # lineshift in nm
-        fine_x = interpolate.make_interp_spline(np.linspace(0,1,len(x)), x)
-        x = fine_x(np.linspace(0,1,len(x)*50)) # upsample x axis
-        self.profiles['x'] = x
-
-        resolution = abs((x[-1]-x[0])/(len(x)-1))
-        middle_wl = x[int(len(x)/2)-1]
-        components = []
-
-        if T:
-            if Eb and gamma:
-                thompson = doppler_thompson(x, middle_wl, Eb, self.m, self.side)
-                maxwell = doppler_maxwell(x, middle_wl, T, self.m)
-                doppler = gamma*maxwell + (1-gamma)*thompson
-                self.profiles['Doppler'] = doppler/np.max(doppler)
-                components.append(doppler)
-            else:
-                maxwell = doppler_maxwell(x, middle_wl, T, self.m)
-                self.profiles['Doppler'] = maxwell/np.max(maxwell)
-                components.append(maxwell)
-        if Eb and not T:
-            thompson = doppler_thompson(x, middle_wl, Eb, self.m, self.side)
-            self.profiles['Doppler'] = thompson/np.max(thompson)
-            components.append(thompson)
-        if B:
-            t = self.transition
-            zeeman_pattern = zeeman(x, middle_wl, B, t.upperJ, t.lowerJ, t.upperG, t.lowerG)/resolution
-            self.profiles['Zeeman'] = zeeman_pattern/np.max(zeeman_pattern)
-            components.append(zeeman_pattern)
-        if ne:
-            this_stark = stark.stark(self.transition)
-            stark_profile = this_stark.get_profile(x, ne, Te, pert)
-            self.profiles['Stark'] = stark_profile/np.max(stark_profile)
-            components.append(stark_profile)
-        if N:
-            this_vdW = vdW.vdW(self.transition, pert=pert)
-            vdW_profile = this_vdW.get_profile(x, T, N)
-            self.profiles['vdW'] = vdW_profile/np.max(vdW_profile)
-            components.append(vdW_profile)
-            if shift:
-                s = s + this_vdW.get_shift(x, N, T)
-
-        # We let the instrumental profile determine center position.
-        # ALL other components are shifted to the middle!
-        if instr_func:
-            instrumental_profile = instr_func(x, wl+s)
-        elif w:   
-            instrumental_profile = psd_voigt(x, wl+s, w, mu)
-        else:
-            instrumental_profile = gauss_function(x, wl+s, x[1]-x[0])
-        
-        self.profiles['instrument'] = instrumental_profile/np.max(instrumental_profile)
-
-        profile = instrumental_profile
-        for component in components:
-            profile = convolve(profile, component, mode='same') * resolution
-
-        y = A*profile
-        self.profiles['y'] = y
-        lowres_y = np.interp(orig_x, x, y)
-        # normalize intensity to A
-        y = A*lowres_y/np.sum(lowres_y)/resolution
+#!/bin/python3
+import numpy as np
+from scipy.signal import fftconvolve as convolve
+from scipy import constants as const
+from scipy import interpolate
+from .util import zeeman, parse_spectroscopic_name, doppler_thompson,\
+                        doppler_maxwell, gauss_function, psd_voigt
+from . import stark
+from . import vdW
+import mendeleev 
+
+class emission_line():
+    def __init__(self, transition, wl, instr_func = None, w = None, mu = 0.0,
+                 T = None, Eb = None, gamma = None, B = None, ne = None, 
+                                Te = None, side = False, N = None, pert = None):
+        
+        """  Class to calculate the shape of an emission line based on the 
+        physical situation. Providing information on densities and temperatures
+        automatically switches on different broadening mechanisms.
+
+        Supported broadening mechanisms: Doppler, Stark, Zeeman, van der Waals
+        and instrumental broadening. Stark broadening is only supported for
+        some transitions: H-alpha to gamma, He 447.1 nm, He 492.2 nm, O 777 nm,
+        Ar 810.369 nm and Ar 738.398 nm.
+
+        <transition>: An owl.emitter.transition object for the specific line.
+        <wl>: Center wavelength in nm. Does not need to be the theoretical wl
+              of the transition. Use to move simulation relative to measurement.
+        <instr_func>: Instrumental function of the spectrometer. Must be a 
+                      function that take parameters x and xc (wavelength axis 
+                      and central position) and return the profile as a 
+                      numpy array.
+        <w>: Width of the instrumental function in nm. Only if instr_func=None.
+        <mu>: Shape parameter of the instrumental fucntion. 0=Gauss, 1=Lorentz.
+        Use together with w or use instr_func instead. Only if instr_func=None.
+        <T>: Emitter temperature in Kelvin. Used for vdW and Doppler broadening.
+        <Eb>: Surface binding energy in eV to calculate Doppler broadening of 
+              sputtered particles.
+        <gamma>: Thermalization degree of sputtered particles (used with Eb).
+        <B>: Magnetic field strength for Zeeman splitting. Units of Tesla.
+        <ne>: Electron density for Stark broadening. Units of m^-3. 
+        <Te>: Electron temperature for stark broadening. Units of Kelvin.
+              Has only minor impact on the results and can usually be guessed.
+        <side>: Used for Zeeman and together with gamma. To be updated.
+        <N>: Neutral density for van der Waals broadening. Units of m^-3.
+             This is the density of species sourrounding the emitter.
+        <pert>: Perturber species for vdW and Stark boradening. This is the ion
+                or atom species surrounding the emitter particles. In case vdW 
+                we look up the polarizability of the element. For Stark we only 
+                need the mass. Specify like emitter species, e.g. 'Ar I'.  
+        """
+
+        self.wl = wl
+        self.transition = transition
+        self.instr = instr_func
+        self.w = w
+        self.mu = mu
+        particle = transition.particle
+        self.m  = particle.m
+        self.Ei = particle.Ei
+        self.T  = T
+        self.Eb = Eb
+        self.gamma = gamma
+        self.B  = B
+        self.ne = ne
+        self.Te = Te
+        self.N  = N
+        self.pert = pert
+        self.side = side # symmetric version of Thompson?
+        self.profiles = dict.fromkeys(['Doppler', 'Zeeman', 'Stark', 'vdW', 'instrument'])
+
+        if pert:          
+            self.pert_name, self.pert_charge = parse_spectroscopic_name(pert)
+            self.pert = mendeleev.element(self.pert_name)
+            self.pert.charge = self.pert_charge
+            self.pert.m = self.pert.mass
+            self.pert.Ei = self.pert.ionenergies[1]
+            if T:
+                self.pert.T = T
+            elif Te:
+                self.pert.T = Te*const.eV/const.k
+
+
+
+    def get_profile(self, x, A = 1, instr_func = None, w = None, mu = None,
+            shift = False, wl=None, T = None, Eb = None, gamma = None, B = None,
+            N = None, ne = None, Te = None, pert = None):
+
+        if instr_func == None and self.instr:
+            instr_func = self.instr
+        if w == None and self.w:
+            w = self.w
+        if mu == None and self.mu:
+            mu = self.mu
+        if wl == None and self.wl:
+            wl = self.wl
+        if T == None and self.T:
+            T = self.T
+        if Eb == None and self.Eb:
+            Eb = self.Eb
+        if gamma == None and self.gamma:
+            gamma = self.gamma
+        if B == None and self.B:
+            B = self.B
+        if ne == None and self.ne:
+            ne = self.ne
+        if Te == None and self.Te:
+            Te = self.Te
+        if N == None and self.N:
+            N = self.N
+        if pert == None and self.pert:
+            pert = self.pert
+        
+        elif pert:
+            self.pert_name, self.pert_charge = parse_spectroscopic_name(pert)
+            self.pert = mendeleev.element(self.pert_name)
+            self.pert.charge = self.pert_charge
+            self.pert.m = self.pert.mass
+            self.pert.Ei = self.pert.ionenergies[1]
+            if T:
+                self.pert.T = T
+            elif Te:
+                self.pert.T = Te*const.eV/const.k
+            pert = self.pert
+
+        self.profiles = dict.fromkeys(['x', 'y', 'Doppler', 'Zeeman', 'Stark', 'vdW', 'instrument'])
+        orig_x = np.copy(x)
+        s = 0 # lineshift in nm
+        fine_x = interpolate.make_interp_spline(np.linspace(0,1,len(x)), x)
+        x = fine_x(np.linspace(0,1,len(x)*50)) # upsample x axis
+        self.profiles['x'] = x
+
+        resolution = abs((x[-1]-x[0])/(len(x)-1))
+        middle_wl = x[int(len(x)/2)-1]
+        components = []
+
+        if T:
+            if Eb and gamma:
+                thompson = doppler_thompson(x, middle_wl, Eb, self.m, self.side)
+                maxwell = doppler_maxwell(x, middle_wl, T, self.m)
+                doppler = gamma*maxwell + (1-gamma)*thompson
+                self.profiles['Doppler'] = doppler/np.max(doppler)
+                components.append(doppler)
+            else:
+                maxwell = doppler_maxwell(x, middle_wl, T, self.m)
+                self.profiles['Doppler'] = maxwell/np.max(maxwell)
+                components.append(maxwell)
+        if Eb and not T:
+            thompson = doppler_thompson(x, middle_wl, Eb, self.m, self.side)
+            self.profiles['Doppler'] = thompson/np.max(thompson)
+            components.append(thompson)
+        if B:
+            t = self.transition
+            zeeman_pattern = zeeman(x, middle_wl, B, t.upperJ, t.lowerJ, t.upperG, t.lowerG)/resolution
+            self.profiles['Zeeman'] = zeeman_pattern/np.max(zeeman_pattern)
+            components.append(zeeman_pattern)
+        if ne:
+            this_stark = stark.stark(self.transition)
+            stark_profile = this_stark.get_profile(x, ne, Te, pert)
+            self.profiles['Stark'] = stark_profile/np.max(stark_profile)
+            components.append(stark_profile)
+        if N:
+            this_vdW = vdW.vdW(self.transition, pert=pert)
+            vdW_profile = this_vdW.get_profile(x, T, N)
+            self.profiles['vdW'] = vdW_profile/np.max(vdW_profile)
+            components.append(vdW_profile)
+            if shift:
+                s = s + this_vdW.get_shift(x, N, T)
+
+        # We let the instrumental profile determine center position.
+        # ALL other components are shifted to the middle!
+        if instr_func:
+            instrumental_profile = instr_func(x, wl+s)
+        elif w:   
+            instrumental_profile = psd_voigt(x, wl+s, w, mu)
+        else:
+            instrumental_profile = gauss_function(x, wl+s, x[1]-x[0])
+        
+        self.profiles['instrument'] = instrumental_profile/np.max(instrumental_profile)
+
+        profile = instrumental_profile
+        for component in components:
+            profile = convolve(profile, component, mode='same') * resolution
+
+        y = A*profile
+        self.profiles['y'] = y
+        lowres_y = np.interp(orig_x, x, y)
+        # normalize intensity to A
+        y = A*lowres_y/np.sum(lowres_y)/resolution
         return y
```

### Comparing `owlspec-0.2.1/owlspec/emitter/level.py` & `owlspec-0.2.2/owlspec/emitter/level.py`

 * *Files identical despite different names*

### Comparing `owlspec-0.2.1/owlspec/emitter/transition.py` & `owlspec-0.2.2/owlspec/emitter/transition.py`

 * *Files identical despite different names*

### Comparing `owlspec-0.2.1/owlspec/nist_levels/__init__.py` & `owlspec-0.2.2/owlspec/nist_levels/__init__.py`

 * *Files identical despite different names*

### Comparing `owlspec-0.2.1/owlspec/nist_levels/core.py` & `owlspec-0.2.2/owlspec/nist_levels/core.py`

 * *Files identical despite different names*

### Comparing `owlspec-0.2.1/owlspec/spectrum.py` & `owlspec-0.2.2/owlspec/spectrum.py`

 * *Files 8% similar despite different names*

```diff
@@ -168,15 +168,17 @@
             wl =  line['Observed']
             if not np.ma.is_masked(rel_int) and not np.ma.is_masked(wl):
                 rel_int = str(rel_int) # is byte type initally
                 wl =  str(wl)
                 rel_int = re.sub(r'[^\d.]+', '', rel_int)
                 wl = re.sub(r'[^\d.]+', '', wl) # removes non-number chars
                 try: # conversion to float can still fail...
-                    rel_int = float(rel_int)
+                    rel_int = str(line['Rel.'])
+                    rel_int = re.sub(r'[^\d.]+', '', rel_int)
+                    rel_int =  float(rel_int)
                     wl = float(wl)
                     if min_Aik > 0:
                         with warnings.catch_warnings(): # ignore masked element warning
                             warnings.simplefilter("ignore", category=UserWarning)
                             Aik =  float(line['Aki'])
                     else:
                         Aik = 1
@@ -215,15 +217,20 @@
                 wl = re.sub(r'[^\d.]+', '', wl) # removes non-number chars
                 # left/right strips non-number chars (preserves the 'e' in 5e7 
                 Aik = re.sub(r'(^[^\d.]+)|([^\d.]+$)', '', Aik) 
                 
                 if min_int > 0:
                     with warnings.catch_warnings(): # ignore masked element warning
                         warnings.simplefilter("ignore", category=UserWarning)
-                        rel_int =  float(line['Rel.'])
+                        rel_int = str(line['Rel.'])
+                        rel_int = re.sub(r'[^\d.]+', '', rel_int)
+                        if len(rel_int) > 0:
+                            rel_int = float(rel_int)
+                        else:
+                            rel_int = 0
                 else:
                     rel_int = 1
 
                 try: # conversion to float can still fail...
                     wl = float(wl)
                     Aik = float(Aik)
                     gi = line['gi   gk'].split('-')[1]
```

### Comparing `owlspec-0.2.1/owlspec/stark/gigosos_he_loader.py` & `owlspec-0.2.2/owlspec/stark/gigosos_he_loader.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,227 +1,227 @@
-#!/usr/bin/python3
-
-import numpy as np
-from scipy import constants as const
-from ..util import interpol
-import os
-import sys
-from platformdirs import user_data_dir
-import requests
-from pathlib import Path
-import tarfile
-from io import BytesIO
-data_folder447 = os.path.join(user_data_dir("owl-OES", "owl-OES"), "Gigosos2009He")
-data_folder492 = os.path.join(user_data_dir("owl-OES", "owl-OES"), "Lara2012He")
-
-            
-class gigosos_he_loader():
-    def __init__(self, transition):
-        self.transition = transition
-
-
-    def download_profiles(redownload = False):
-        if os.path.exists(data_folder447+"/table06.txt") and \
-           os.path.exists(data_folder492+"/table06.txt") and redownload==False:
-            return
-        print("Downloading Stark broadening data tables for helium.")
-        URL447 = "https://cdsarc.u-strasbg.fr/ftp/J/A+A/503/293/tab.tar.gz"
-        URL492 = "http://cdsarc.u-strasbg.fr/ftp/J/A+A/542/A75/tab.tar.gz"
-        try:
-            response = requests.get(URL447)
-            zip_file447 = response.content
-            response = requests.get(URL492)
-            zip_file492 = response.content
-        except:
-            print("ERROR: could not download helium Stark broadening tables")
-            
-        try:
-            Path(data_folder447).mkdir(parents=True, exist_ok=True)
-            Path(data_folder492).mkdir(parents=True, exist_ok=True)
-            with tarfile.open(name=None, fileobj=BytesIO(zip_file447)) as zip_ref:
-                zip_ref.extractall(data_folder447)
-            with tarfile.open(name=None, fileobj=BytesIO(zip_file492)) as zip_ref:
-                zip_ref.extractall(data_folder492)
-        except:
-            print("ERROR: could now save helium Stark broadening tables to disk")
-            
-
-    def load(self, ne, Te, pert):
-        if pert:
-           emitter_m = self.transition.particle.m
-           reduced_m = (emitter_m * pert.m)/(emitter_m + pert.m)
-           mu = reduced_m * Te/pert.T
-        else:
-           mu = 1
-
-        return self.load_stark_profile(ne, mu, Te*const.eV/const.k)
-
-
-    def closest(self,val,array):
-        return array[np.argmin(np.abs(array-val))]
-
-
-    def slightly_smaller(self,val,array):
-        array = array[array < val]
-        return array[np.argmin(np.abs(array-val))]
-
-
-    def slightly_bigger(self,val,array):
-        array = array[array > val]
-        return array[np.argmin(np.abs(array-val))]
-
-
-    def mirror_profile(self,profile):
-        return np.append(np.array(profile[::-1]), profile)
-
-
-    def mirror_x(self,x):
-        return np.append(np.array(x[::-1])*-1, x)
-
-
-    def closest_ne(self,ne):
-        if round(self.transition.wl,0) == 447:
-            ne_stock = 10**np.linspace(21,24,10)
-        if round(self.transition.wl,0) == 492:
-            ne_stock = 10**np.linspace(20,24,13)
-        if ne in ne_stock:
-            ne_low = ne_high = ne
-        else:
-            ne_low  = self.slightly_smaller(ne,ne_stock)
-            ne_high = self.slightly_bigger(ne,ne_stock)
-        return ne_low,ne_high
-
-
-    def closest_mu(self,mu):
-        if round(self.transition.wl,0) == 447:
-            mu_stock = np.array([0.8, 2, 4])
-        if round(self.transition.wl,0) == 492:
-            mu_stock = np.array([0.8, 2, 4, 10])
-        if mu in mu_stock:
-            mu_low = mu_high = mu
-        elif mu < mu_stock[0]:
-            mu_low = mu_high = mu_stock[0]
-        elif mu > mu_stock[-1]:
-            mu_low = mu_high = mu_stock[-1]
-        else:
-            mu_low  = self.slightly_smaller(mu,mu_stock)
-            mu_high = self.slightly_bigger(mu,mu_stock)
-        return mu_low,mu_high
-
-
-    def get_T_stock(self, ne):
-        if round(self.transition.wl,0) == 447:
-            ne_stock = 10**np.linspace(21,24,10) # prevent rounding errors
-            if ne <= ne_stock[4]:
-                T_stock = np.array([5000, 10000, 20000, 40000])
-            if ne > ne_stock[4] and ne < ne_stock[8]:
-                T_stock = np.array([10000, 20000, 40000])
-            if ne >= ne_stock[8]:
-                T_stock = np.array([20000, 40000])
-                
-        if round(self.transition.wl,0) == 492:
-            if ne <= 1e22:
-                T_stock = np.array([5000, 10000, 20000, 40000])
-            if ne > 1e22 and ne <= 1e23:
-                T_stock = np.array([10000, 20000, 30000, 40000])
-            if ne > 1e23 and ne < 1e24:
-                T_stock = np.array([20000, 30000, 40000])
-            if ne == 1e24:
-                T_stock = np.array([30000, 40000])
-                
-        return T_stock
-
-
-    def closest_T(self,T,ne):
-        T_stock = self.get_T_stock(ne)
-        if T in T_stock:
-            T_low = T_high = T
-        elif T < T_stock[0]:
-            T_low = T_high = T_stock[0]
-        elif T > T_stock[-1]:
-            T_low = T_high = T_stock[-1]
-        else:
-            T_low  = self.slightly_smaller(T,T_stock)
-            T_high = self.slightly_bigger(T,T_stock)
-        return T_low,T_high
-
-
-    def load_file(self,ne):
-        if round(self.transition.wl,0) == 447:
-            folder = data_folder447
-            filename = "table"
-            table_num = str(int(round((np.log10((ne/1e20))*3-1)))).zfill(2)
-        if round(self.transition.wl,0) == 492:
-            folder = data_folder492
-            folder = os.path.join(folder,"He492")
-            filename = "table"
-            table_num = str(int(round((np.log10((ne/1e20))*3+4)))).zfill(2)
-
-        filename = filename + table_num + ".txt"
-        try:
-            table = np.loadtxt(os.path.join(folder,filename)).T
-        except:
-            raise SystemExit('Error: Could not find Stark broadening data tables.')
-        return table
-
-
-    def interpolate_stark_profile(self, x, low_y, high_y, low_val, high_val, val):
-        "Creates profile for arbitrary T/mu. Arrays must use same x!"
-        if high_val != low_val:
-            low_y = np.array(low_y)
-            high_y = np.array(high_y)
-            mix_factor = ((val - low_val)/(high_val - low_val))#**(1.5)
-            return x,(mix_factor * high_y + (1-mix_factor) * low_y)
-        else:
-            return x,high_y
-
-    def interpolate_stark_profile_ne(self,low_x, high_x, low_y, high_y, low_val, high_val, val):
-        "Creates profile for arbitrary ne. X can be interpolated"
-        low_y = interpol(low_x, low_y, high_x) # all to high_x
-        if high_val != low_val:
-            low_y = np.array(low_y)
-            high_y = np.array(high_y)
-            mix_factor = ((val - low_val)/(high_val - low_val))
-            return high_x,(mix_factor * high_y + (1-mix_factor) * low_y)
-        else:
-            return high_x,high_y
-
-
-    def load_stark_profile(self,ne_, mu_, T_):
-        if round(self.transition.wl,0) == 447:
-            mu_stock = np.array([0.8, 2, 4])
-        if round(self.transition.wl,0) == 492:
-            mu_stock = np.array([0.8, 2, 4, 10])
-
-        x = None
-        profiles_ne = []
-        vals_ne = []
-        for ne in self.closest_ne(ne_):
-            table = self.load_file(ne)
-            profiles_mu = []
-            vals_mu = []
-            for mu in self.closest_mu(mu_):
-                T_stock = self.get_T_stock(ne)
-                T_low,T_high = self.closest_T(T_,ne)
-                pos_low = (list(T_stock).index(T_low)+1) + (len(T_stock) * list(mu_stock).index(mu))
-                pos_high = (list(T_stock).index(T_high)+1) + (len(T_stock) * list(mu_stock).index(mu))
-                _,y_low = table[0], table[pos_low]
-                high_x,y_high = table[0], table[pos_high]
-                x,y = self.interpolate_stark_profile(high_x,y_low,y_high,T_low,T_high,T_)
-                profiles_mu.append((x,y))
-                vals_mu.append(mu)
-
-            x,y = self.interpolate_stark_profile(
-                profiles_mu[1][0],profiles_mu[0][1],
-                profiles_mu[1][1],vals_mu[0],vals_mu[1],mu_)
-
-            profiles_ne.append((x,y))
-            vals_ne.append(ne)
-
-        x,y = self.interpolate_stark_profile_ne(
-            profiles_ne[0][0],profiles_ne[1][0],profiles_ne[0][1],
-            profiles_ne[1][1],vals_ne[0],vals_ne[1],ne_)
-
-        return x,y
-
-
-
+#!/usr/bin/python3
+
+import numpy as np
+from scipy import constants as const
+from ..util import interpol
+import os
+import sys
+from platformdirs import user_data_dir
+import requests
+from pathlib import Path
+import tarfile
+from io import BytesIO
+data_folder447 = os.path.join(user_data_dir("owl-OES", "owl-OES"), "Gigosos2009He")
+data_folder492 = os.path.join(user_data_dir("owl-OES", "owl-OES"), "Lara2012He")
+
+            
+class gigosos_he_loader():
+    def __init__(self, transition):
+        self.transition = transition
+
+
+    def download_profiles(redownload = False):
+        if os.path.exists(data_folder447+"/table06.txt") and \
+           os.path.exists(data_folder492+"/table06.txt") and redownload==False:
+            return
+        print("Downloading Stark broadening data tables for helium.")
+        URL447 = "https://cdsarc.u-strasbg.fr/ftp/J/A+A/503/293/tab.tar.gz"
+        URL492 = "http://cdsarc.u-strasbg.fr/ftp/J/A+A/542/A75/tab.tar.gz"
+        try:
+            response = requests.get(URL447)
+            zip_file447 = response.content
+            response = requests.get(URL492)
+            zip_file492 = response.content
+        except:
+            print("ERROR: could not download helium Stark broadening tables")
+            
+        try:
+            Path(data_folder447).mkdir(parents=True, exist_ok=True)
+            Path(data_folder492).mkdir(parents=True, exist_ok=True)
+            with tarfile.open(name=None, fileobj=BytesIO(zip_file447)) as zip_ref:
+                zip_ref.extractall(data_folder447)
+            with tarfile.open(name=None, fileobj=BytesIO(zip_file492)) as zip_ref:
+                zip_ref.extractall(data_folder492)
+        except:
+            print("ERROR: could now save helium Stark broadening tables to disk")
+            
+
+    def load(self, ne, Te, pert):
+        if pert:
+           emitter_m = self.transition.particle.m
+           reduced_m = (emitter_m * pert.m)/(emitter_m + pert.m)
+           mu = reduced_m * Te/pert.T
+        else:
+           mu = 1
+
+        return self.load_stark_profile(ne, mu, Te*const.eV/const.k)
+
+
+    def closest(self,val,array):
+        return array[np.argmin(np.abs(array-val))]
+
+
+    def slightly_smaller(self,val,array):
+        array = array[array < val]
+        return array[np.argmin(np.abs(array-val))]
+
+
+    def slightly_bigger(self,val,array):
+        array = array[array > val]
+        return array[np.argmin(np.abs(array-val))]
+
+
+    def mirror_profile(self,profile):
+        return np.append(np.array(profile[::-1]), profile)
+
+
+    def mirror_x(self,x):
+        return np.append(np.array(x[::-1])*-1, x)
+
+
+    def closest_ne(self,ne):
+        if round(self.transition.wl,0) == 447:
+            ne_stock = 10**np.linspace(21,24,10)
+        if round(self.transition.wl,0) == 492:
+            ne_stock = 10**np.linspace(20,24,13)
+        if ne in ne_stock:
+            ne_low = ne_high = ne
+        else:
+            ne_low  = self.slightly_smaller(ne,ne_stock)
+            ne_high = self.slightly_bigger(ne,ne_stock)
+        return ne_low,ne_high
+
+
+    def closest_mu(self,mu):
+        if round(self.transition.wl,0) == 447:
+            mu_stock = np.array([0.8, 2, 4])
+        if round(self.transition.wl,0) == 492:
+            mu_stock = np.array([0.8, 2, 4, 10])
+        if mu in mu_stock:
+            mu_low = mu_high = mu
+        elif mu < mu_stock[0]:
+            mu_low = mu_high = mu_stock[0]
+        elif mu > mu_stock[-1]:
+            mu_low = mu_high = mu_stock[-1]
+        else:
+            mu_low  = self.slightly_smaller(mu,mu_stock)
+            mu_high = self.slightly_bigger(mu,mu_stock)
+        return mu_low,mu_high
+
+
+    def get_T_stock(self, ne):
+        if round(self.transition.wl,0) == 447:
+            ne_stock = 10**np.linspace(21,24,10) # prevent rounding errors
+            if ne <= ne_stock[4]:
+                T_stock = np.array([5000, 10000, 20000, 40000])
+            if ne > ne_stock[4] and ne < ne_stock[8]:
+                T_stock = np.array([10000, 20000, 40000])
+            if ne >= ne_stock[8]:
+                T_stock = np.array([20000, 40000])
+                
+        if round(self.transition.wl,0) == 492:
+            if ne <= 1e22:
+                T_stock = np.array([5000, 10000, 20000, 40000])
+            if ne > 1e22 and ne <= 1e23:
+                T_stock = np.array([10000, 20000, 30000, 40000])
+            if ne > 1e23 and ne < 1e24:
+                T_stock = np.array([20000, 30000, 40000])
+            if ne == 1e24:
+                T_stock = np.array([30000, 40000])
+                
+        return T_stock
+
+
+    def closest_T(self,T,ne):
+        T_stock = self.get_T_stock(ne)
+        if T in T_stock:
+            T_low = T_high = T
+        elif T < T_stock[0]:
+            T_low = T_high = T_stock[0]
+        elif T > T_stock[-1]:
+            T_low = T_high = T_stock[-1]
+        else:
+            T_low  = self.slightly_smaller(T,T_stock)
+            T_high = self.slightly_bigger(T,T_stock)
+        return T_low,T_high
+
+
+    def load_file(self,ne):
+        if round(self.transition.wl,0) == 447:
+            folder = data_folder447
+            filename = "table"
+            table_num = str(int(round((np.log10((ne/1e20))*3-1)))).zfill(2)
+        if round(self.transition.wl,0) == 492:
+            folder = data_folder492
+            folder = os.path.join(folder,"He492")
+            filename = "table"
+            table_num = str(int(round((np.log10((ne/1e20))*3+4)))).zfill(2)
+
+        filename = filename + table_num + ".txt"
+        try:
+            table = np.loadtxt(os.path.join(folder,filename)).T
+        except:
+            raise SystemExit('Error: Could not find Stark broadening data tables.')
+        return table
+
+
+    def interpolate_stark_profile(self, x, low_y, high_y, low_val, high_val, val):
+        "Creates profile for arbitrary T/mu. Arrays must use same x!"
+        if high_val != low_val:
+            low_y = np.array(low_y)
+            high_y = np.array(high_y)
+            mix_factor = ((val - low_val)/(high_val - low_val))#**(1.5)
+            return x,(mix_factor * high_y + (1-mix_factor) * low_y)
+        else:
+            return x,high_y
+
+    def interpolate_stark_profile_ne(self,low_x, high_x, low_y, high_y, low_val, high_val, val):
+        "Creates profile for arbitrary ne. X can be interpolated"
+        low_y = interpol(low_x, low_y, high_x) # all to high_x
+        if high_val != low_val:
+            low_y = np.array(low_y)
+            high_y = np.array(high_y)
+            mix_factor = ((val - low_val)/(high_val - low_val))
+            return high_x,(mix_factor * high_y + (1-mix_factor) * low_y)
+        else:
+            return high_x,high_y
+
+
+    def load_stark_profile(self,ne_, mu_, T_):
+        if round(self.transition.wl,0) == 447:
+            mu_stock = np.array([0.8, 2, 4])
+        if round(self.transition.wl,0) == 492:
+            mu_stock = np.array([0.8, 2, 4, 10])
+
+        x = None
+        profiles_ne = []
+        vals_ne = []
+        for ne in self.closest_ne(ne_):
+            table = self.load_file(ne)
+            profiles_mu = []
+            vals_mu = []
+            for mu in self.closest_mu(mu_):
+                T_stock = self.get_T_stock(ne)
+                T_low,T_high = self.closest_T(T_,ne)
+                pos_low = (list(T_stock).index(T_low)+1) + (len(T_stock) * list(mu_stock).index(mu))
+                pos_high = (list(T_stock).index(T_high)+1) + (len(T_stock) * list(mu_stock).index(mu))
+                _,y_low = table[0], table[pos_low]
+                high_x,y_high = table[0], table[pos_high]
+                x,y = self.interpolate_stark_profile(high_x,y_low,y_high,T_low,T_high,T_)
+                profiles_mu.append((x,y))
+                vals_mu.append(mu)
+
+            x,y = self.interpolate_stark_profile(
+                profiles_mu[1][0],profiles_mu[0][1],
+                profiles_mu[1][1],vals_mu[0],vals_mu[1],mu_)
+
+            profiles_ne.append((x,y))
+            vals_ne.append(ne)
+
+        x,y = self.interpolate_stark_profile_ne(
+            profiles_ne[0][0],profiles_ne[1][0],profiles_ne[0][1],
+            profiles_ne[1][1],vals_ne[0],vals_ne[1],ne_)
+
+        return x,y
+
+
+
```

### Comparing `owlspec-0.2.1/owlspec/stark/gigosos_loader.py` & `owlspec-0.2.2/owlspec/stark/gigosos_loader.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-#!/usr/bin/python3
-
-import numpy as np
-from scipy import constants as const
-from ..util import interpol
-import os
-from platformdirs import user_data_dir
-import requests
-from pathlib import Path
-from zipfile import ZipFile
-from io import BytesIO
-data_folder = os.path.join(user_data_dir("owl-OES", "owl-OES"), "Gigosos2003H")
-
-class gigosos_loader():
-    def __init__(self, transition):
-        self.transition = transition
-        
-        
-    def download_profiles(redownload = False):
-        if os.path.exists(data_folder+"/HalphaProfiles.zip") and redownload==False:
-            return
-        print("Downloading Stark broadening data tables for hydrogen.")
-        URL = "https://ars.els-cdn.com/content/image/1-s2.0-S0584854703000971-mmc1.zip"
-        try:
-            response = requests.get(URL)
-            zip_file = response.content
-        except:
-            print("ERROR: could not download hydrogen Stark broadening tables")
-            
-        try:
-            Path(data_folder).mkdir(parents=True, exist_ok=True)
-            with ZipFile(BytesIO(zip_file)) as zip_ref:
-                zip_ref.extractall(data_folder)
-        except:
-            print("ERROR: could now save hydrogen Stark broadening tables to disk")
-
-
-    def load(self, ne, Te, pert):
-        r0 = (3/(4 * np.pi * ne))**(1/3)
-        rD = ((const.epsilon_0 * const.eV * Te)/(ne * const.e**2))**(1/2)
-        rho = r0/rD
-        if pert:
-           emitter_m = self.transition.particle.m
-           reduced_m = (emitter_m * pert.m)/(emitter_m + pert.m)
-           mu = reduced_m * Te/pert.T
-        else:
-           mu = 1
-        return self.load_stark_profile(ne, mu, rho)
-
-
-    def closest(self,val,array):
-        return array[np.argmin(np.abs(array-val))]
-
-
-    def slightly_smaller(self,val,array):
-        array = array[array < val]
-        return array[np.argmin(np.abs(array-val))]
-
-
-    def slightly_bigger(self,val,array):
-        array = array[array > val]
-        return array[np.argmin(np.abs(array-val))]
-
-
-    def mirror_profile(self,profile):
-        return np.append(np.array(profile[::-1]), profile)
-
-
-    def mirror_x(self,x):
-        return np.append(np.array(x[::-1])*-1, x)
-
-
-    def closest_ne(self,ne):
-        ne_stock = 10**np.linspace(20,25,16)
-        if ne in ne_stock:
-            ne_low = ne_high = ne
-        else:
-            ne_low  = self.slightly_smaller(ne,ne_stock)
-            ne_high = self.slightly_bigger(ne,ne_stock)
-        return ne_low,ne_high
-
-
-    def closest_mu(self,mu):
-        mu_stock = np.array([0.50, 0.80, 0.90, 1.00, 1.25, 1.5, 1.75, 2.00,
-            2.50, 3.00, 4.00, 5.00, 6.00, 7.00, 8.00, 9.00, 10.0])
-        if mu in mu_stock:
-            mu_low = mu_high = mu
-        elif mu < mu_stock[0]:
-            mu_low = mu_high = mu_stock[0]
-        elif mu > mu_stock[-1]:
-            mu_low = mu_high = mu_stock[-1]
-        else:
-            mu_low  = self.slightly_smaller(mu,mu_stock)
-            mu_high = self.slightly_bigger(mu,mu_stock)
-        return mu_low,mu_high
-
-
-    def closest_rho(self,rho):
-        rho_stock = np.linspace(0.1,0.6,11)
-        if rho in rho_stock:
-            rho_low = rho_high = rho
-        elif rho < rho_stock[0]:
-            rho_low = rho_high = rho_stock[0]
-        elif rho > rho_stock[-1]:
-            rho_low = rho_high = rho_stock[-1]
-        else:
-            rho_low  = self.slightly_smaller(rho,rho_stock)
-            rho_high = self.slightly_bigger(rho,rho_stock)
-        return rho_low,rho_high
-
-
-    def rho_to_T(self,rho,ne):
-        r0 = (3/(4 * np.pi * ne))**(1/3)
-        T = ((ne*const.e**2)/(const.epsilon_0 * const.k))*(r0/rho)**2
-        T = T*0.9999944 # Gigosos temperature calculations are strange...
-        return T
-
-
-    def load_file(self,ne,mu,rho,prefix,datazip):        
-        ne_name = str(int(round(np.log10(ne)*100,0)))
-        T = str(int(round(self.rho_to_T(rho,ne),0)))
-        T_name = str(T).zfill(7)
-        mu_name = str(int(mu*100)).zfill(4)
-        filename = prefix + ne_name + "t" + T_name + "m" + mu_name + ".dlp"
-        try:
-            datafile = datazip.open(filename)
-            x,y = np.loadtxt(datafile).T
-        except:
-            raise SystemExit('Error: Could not find Stark broadening data tables.')
-        return x,y
-
-
-    def interpolate_stark_profile(self,low_x, high_x, low_y, high_y, low_val, high_val, val):
-        "Creates profile for arbitrary ne. Arrays must use same x!"
-        low_y = interpol(low_x, low_y, high_x) # all to high_x
-        if high_val != low_val:
-            low_y = np.array(low_y)
-            high_y = np.array(high_y)
-            mix_factor = ((val - low_val)/(high_val - low_val))#**(1.5)
-            return high_x,(mix_factor * high_y + (1-mix_factor) * low_y)
-        else:
-            return high_x,high_y
-
-
-    def interpolate_stark_profile_ne(self,low_x, high_x, low_y, high_y, low_val, high_val, val):
-        "Creates profile for arbitrary ne. Arrays must use same x!"
-        low_y = interpol(low_x, low_y, high_x) # all to high_x
-        if high_val != low_val:
-            low_y = np.array(low_y)
-            high_y = np.array(high_y)
-            mix_factor = ((val - low_val)/(high_val - low_val))
-            return high_x,(mix_factor * high_y + (1-mix_factor) * low_y)
-        else:
-            return high_x,high_y
-
-
-    def load_stark_profile(self,ne_, mu_, rho_):
-        
-        folder = data_folder
-        ele = self.transition.emitter.symbol
-        if ele == "H" and round(self.transition.wl,0) == 656.0:
-            datazip = os.path.join(folder,"HalphaProfiles.zip")
-            prefix = "BAn"
-        if ele == "H" and round(self.transition.wl,0) == 486.0:
-            datazip = os.path.join(folder,"HbetaProfiles.zip")
-            prefix = "BBn"
-        if ele == "H" and round(self.transition.wl,0) == 434.0:
-            datazip = os.path.join(folder,"HgammaProfiles.zip")
-            prefix = "BGn"
-        datazip = ZipFile(datazip, 'r')
-        
-        x = None
-        profiles_ne = []
-        vals_ne = []
-        for ne in self.closest_ne(ne_):
-            profiles_mu = []
-            vals_mu = []
-            for mu in self.closest_mu(mu_):
-                rho_low,rho_high = self.closest_rho(rho_)
-                low_x,y_low = self.load_file(ne,mu,rho_low,prefix,datazip)
-                high_x,y_high = self.load_file(ne,mu,rho_high,prefix,datazip)
-                x,y = self.interpolate_stark_profile(low_x,high_x,y_low,y_high,rho_low,rho_high,rho_)
-                profiles_mu.append((x,y))
-                vals_mu.append(mu)
-            x,y = self.interpolate_stark_profile(
-                profiles_mu[0][0],profiles_mu[1][0],profiles_mu[0][1],
-                profiles_mu[1][1],vals_mu[0],vals_mu[1],mu_)
-
-            profiles_ne.append((x,y))
-            vals_ne.append(ne)
-
-        x,y = self.interpolate_stark_profile_ne(
-            profiles_ne[0][0],profiles_ne[1][0],profiles_ne[0][1],
-            profiles_ne[1][1],vals_ne[0],vals_ne[1],ne_)
-
-        y = self.mirror_profile(y)/1e9
-        x = self.mirror_x(x)*1e9
-
-        return x,y
-
-
-
+#!/usr/bin/python3
+
+import numpy as np
+from scipy import constants as const
+from ..util import interpol
+import os
+from platformdirs import user_data_dir
+import requests
+from pathlib import Path
+from zipfile import ZipFile
+from io import BytesIO
+data_folder = os.path.join(user_data_dir("owl-OES", "owl-OES"), "Gigosos2003H")
+
+class gigosos_loader():
+    def __init__(self, transition):
+        self.transition = transition
+        
+        
+    def download_profiles(redownload = False):
+        if os.path.exists(data_folder+"/HalphaProfiles.zip") and redownload==False:
+            return
+        print("Downloading Stark broadening data tables for hydrogen.")
+        URL = "https://ars.els-cdn.com/content/image/1-s2.0-S0584854703000971-mmc1.zip"
+        try:
+            response = requests.get(URL)
+            zip_file = response.content
+        except:
+            print("ERROR: could not download hydrogen Stark broadening tables")
+            
+        try:
+            Path(data_folder).mkdir(parents=True, exist_ok=True)
+            with ZipFile(BytesIO(zip_file)) as zip_ref:
+                zip_ref.extractall(data_folder)
+        except:
+            print("ERROR: could now save hydrogen Stark broadening tables to disk")
+
+
+    def load(self, ne, Te, pert):
+        r0 = (3/(4 * np.pi * ne))**(1/3)
+        rD = ((const.epsilon_0 * const.eV * Te)/(ne * const.e**2))**(1/2)
+        rho = r0/rD
+        if pert:
+           emitter_m = self.transition.particle.m
+           reduced_m = (emitter_m * pert.m)/(emitter_m + pert.m)
+           mu = reduced_m * Te/pert.T
+        else:
+           mu = 1
+        return self.load_stark_profile(ne, mu, rho)
+
+
+    def closest(self,val,array):
+        return array[np.argmin(np.abs(array-val))]
+
+
+    def slightly_smaller(self,val,array):
+        array = array[array < val]
+        return array[np.argmin(np.abs(array-val))]
+
+
+    def slightly_bigger(self,val,array):
+        array = array[array > val]
+        return array[np.argmin(np.abs(array-val))]
+
+
+    def mirror_profile(self,profile):
+        return np.append(np.array(profile[::-1]), profile)
+
+
+    def mirror_x(self,x):
+        return np.append(np.array(x[::-1])*-1, x)
+
+
+    def closest_ne(self,ne):
+        ne_stock = 10**np.linspace(20,25,16)
+        if ne in ne_stock:
+            ne_low = ne_high = ne
+        else:
+            ne_low  = self.slightly_smaller(ne,ne_stock)
+            ne_high = self.slightly_bigger(ne,ne_stock)
+        return ne_low,ne_high
+
+
+    def closest_mu(self,mu):
+        mu_stock = np.array([0.50, 0.80, 0.90, 1.00, 1.25, 1.5, 1.75, 2.00,
+            2.50, 3.00, 4.00, 5.00, 6.00, 7.00, 8.00, 9.00, 10.0])
+        if mu in mu_stock:
+            mu_low = mu_high = mu
+        elif mu < mu_stock[0]:
+            mu_low = mu_high = mu_stock[0]
+        elif mu > mu_stock[-1]:
+            mu_low = mu_high = mu_stock[-1]
+        else:
+            mu_low  = self.slightly_smaller(mu,mu_stock)
+            mu_high = self.slightly_bigger(mu,mu_stock)
+        return mu_low,mu_high
+
+
+    def closest_rho(self,rho):
+        rho_stock = np.linspace(0.1,0.6,11)
+        if rho in rho_stock:
+            rho_low = rho_high = rho
+        elif rho < rho_stock[0]:
+            rho_low = rho_high = rho_stock[0]
+        elif rho > rho_stock[-1]:
+            rho_low = rho_high = rho_stock[-1]
+        else:
+            rho_low  = self.slightly_smaller(rho,rho_stock)
+            rho_high = self.slightly_bigger(rho,rho_stock)
+        return rho_low,rho_high
+
+
+    def rho_to_T(self,rho,ne):
+        r0 = (3/(4 * np.pi * ne))**(1/3)
+        T = ((ne*const.e**2)/(const.epsilon_0 * const.k))*(r0/rho)**2
+        T = T*0.9999944 # Gigosos temperature calculations are strange...
+        return T
+
+
+    def load_file(self,ne,mu,rho,prefix,datazip):        
+        ne_name = str(int(round(np.log10(ne)*100,0)))
+        T = str(int(round(self.rho_to_T(rho,ne),0)))
+        T_name = str(T).zfill(7)
+        mu_name = str(int(mu*100)).zfill(4)
+        filename = prefix + ne_name + "t" + T_name + "m" + mu_name + ".dlp"
+        try:
+            datafile = datazip.open(filename)
+            x,y = np.loadtxt(datafile).T
+        except:
+            raise SystemExit('Error: Could not find Stark broadening data tables.')
+        return x,y
+
+
+    def interpolate_stark_profile(self,low_x, high_x, low_y, high_y, low_val, high_val, val):
+        "Creates profile for arbitrary ne. Arrays must use same x!"
+        low_y = interpol(low_x, low_y, high_x) # all to high_x
+        if high_val != low_val:
+            low_y = np.array(low_y)
+            high_y = np.array(high_y)
+            mix_factor = ((val - low_val)/(high_val - low_val))#**(1.5)
+            return high_x,(mix_factor * high_y + (1-mix_factor) * low_y)
+        else:
+            return high_x,high_y
+
+
+    def interpolate_stark_profile_ne(self,low_x, high_x, low_y, high_y, low_val, high_val, val):
+        "Creates profile for arbitrary ne. Arrays must use same x!"
+        low_y = interpol(low_x, low_y, high_x) # all to high_x
+        if high_val != low_val:
+            low_y = np.array(low_y)
+            high_y = np.array(high_y)
+            mix_factor = ((val - low_val)/(high_val - low_val))
+            return high_x,(mix_factor * high_y + (1-mix_factor) * low_y)
+        else:
+            return high_x,high_y
+
+
+    def load_stark_profile(self,ne_, mu_, rho_):
+        
+        folder = data_folder
+        ele = self.transition.emitter.symbol
+        if ele == "H" and round(self.transition.wl,0) == 656.0:
+            datazip = os.path.join(folder,"HalphaProfiles.zip")
+            prefix = "BAn"
+        if ele == "H" and round(self.transition.wl,0) == 486.0:
+            datazip = os.path.join(folder,"HbetaProfiles.zip")
+            prefix = "BBn"
+        if ele == "H" and round(self.transition.wl,0) == 434.0:
+            datazip = os.path.join(folder,"HgammaProfiles.zip")
+            prefix = "BGn"
+        datazip = ZipFile(datazip, 'r')
+        
+        x = None
+        profiles_ne = []
+        vals_ne = []
+        for ne in self.closest_ne(ne_):
+            profiles_mu = []
+            vals_mu = []
+            for mu in self.closest_mu(mu_):
+                rho_low,rho_high = self.closest_rho(rho_)
+                low_x,y_low = self.load_file(ne,mu,rho_low,prefix,datazip)
+                high_x,y_high = self.load_file(ne,mu,rho_high,prefix,datazip)
+                x,y = self.interpolate_stark_profile(low_x,high_x,y_low,y_high,rho_low,rho_high,rho_)
+                profiles_mu.append((x,y))
+                vals_mu.append(mu)
+            x,y = self.interpolate_stark_profile(
+                profiles_mu[0][0],profiles_mu[1][0],profiles_mu[0][1],
+                profiles_mu[1][1],vals_mu[0],vals_mu[1],mu_)
+
+            profiles_ne.append((x,y))
+            vals_ne.append(ne)
+
+        x,y = self.interpolate_stark_profile_ne(
+            profiles_ne[0][0],profiles_ne[1][0],profiles_ne[0][1],
+            profiles_ne[1][1],vals_ne[0],vals_ne[1],ne_)
+
+        y = self.mirror_profile(y)/1e9
+        x = self.mirror_x(x)*1e9
+
+        return x,y
+
+
+
```

### Comparing `owlspec-0.2.1/owlspec/stark/griem.py` & `owlspec-0.2.2/owlspec/stark/griem.py`

 * *Files identical despite different names*

### Comparing `owlspec-0.2.1/owlspec/stark/stark.py` & `owlspec-0.2.2/owlspec/stark/stark.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-#!/usr/bin/python
-
-import numpy as np
-from ..util import interpol, lorentz_function
-from .gigosos_loader import gigosos_loader
-from .gigosos_he_loader import gigosos_he_loader
-from .griem import griem
-
-class stark():
-    def __init__(self, transition, ion_pert = None):
-        self.transition = transition
-        self.fast = False
-        self.pert = ion_pert
-
-
-    def get_profile(self,x, ne, Te=None, pert=None):
-        middle_wl = x[int(len(x)/2)]
-        ele = self.transition.emitter.symbol
-
-        ################ Hydrogen ########
-        if ele == "H":
-            if round(self.transition.wl,0) == 656:
-                # Gigosos et al, Spectrochimica Acta Part B 58 (2003) 1489–1504
-                if self.fast or not Te:
-                    w = ((ne/1e23)**(0.67965)) * 1.098
-                    return lorentz_function(x,middle_wl,w)
-                else:
-                    this_loader = gigosos_loader(self.transition)
-                    gigosos_x,y = this_loader.load(ne, Te, pert)
-                    gigosos_x = gigosos_x + middle_wl # to nm
-                    y = interpol(gigosos_x,y,x)
-                    return y
-
-            if round(self.transition.wl, 0) == 486:
-                # Gigosos et al, Spectrochimica Acta Part B 58 (2003) 1489–1504
-                if self.fast or not Te:
-                    w = ((ne/1e23)**(0.68116)) * 4.8
-                    return lorentz_function(x,middle_wl,w)
-                else:
-                    this_loader = gigosos_loader(self.transition)
-                    gigosos_x,y = this_loader.load(ne, Te, pert)
-                    gigosos_x = gigosos_x + middle_wl # to nm
-                    y = interpol(gigosos_x,y,x)
-                    return y
-
-        ################ Helium ##########
-        if ele == "He":
-            if round(self.transition.wl,0) == 447:
-                # Gigosos et al, A&A 503, 293–299 (2009)
-                # doi: 10.1051/0004-6361/200912243
-                this_loader = gigosos_he_loader(self.transition)
-                gigosos_x,y = this_loader.load(ne, Te, pert)
-                gigosos_x = gigosos_x + middle_wl # to nm
-                y = interpol(gigosos_x,y,x)
-                return y
-
-            if round(self.transition.wl, 0) == 492:
-                # Lara et al, A&A 542, A75 (2012)
-                # doi: 10.1051/0004-6361/201219123
-                this_loader = gigosos_he_loader(self.transition)
-                gigosos_x,y = this_loader.load(ne, Te, pert)
-                gigosos_x = gigosos_x + middle_wl # to nm
-                y = interpol(gigosos_x,y,x)
-                return y
-
-        ################ Others: Griem ##########
-        if ele == "O" or "Ar":
-            this_griem = griem(self.transition)
-            w,d = this_griem.get_width_shift(ne, Te)
-            # shift is ignored for now
-            return lorentz_function(x,middle_wl,w)
-
-
-    def get_width(self, ne, Te=None, pert=None):
-        ele = self.transition.element
-        if ele == "O" or ele == "Ar":
-            this_griem = griem(self.transition)
-            w,d = this_griem.get_width_shift(ne, Te)
-            return w
-
-    def get_shift(self, ne, Te=None, pert=None):
-        ele = self.transition.element
-        if ele == "O" or ele == "Ar" :
-            this_griem = griem(self.transition)
-            w,d = this_griem.get_width_shift(ne, Te)
-            return d
-
-
+#!/usr/bin/python
+
+import numpy as np
+from ..util import interpol, lorentz_function
+from .gigosos_loader import gigosos_loader
+from .gigosos_he_loader import gigosos_he_loader
+from .griem import griem
+
+class stark():
+    def __init__(self, transition, ion_pert = None):
+        self.transition = transition
+        self.fast = False
+        self.pert = ion_pert
+
+
+    def get_profile(self,x, ne, Te=None, pert=None):
+        middle_wl = x[int(len(x)/2)]
+        ele = self.transition.emitter.symbol
+
+        ################ Hydrogen ########
+        if ele == "H":
+            if round(self.transition.wl,0) == 656:
+                # Gigosos et al, Spectrochimica Acta Part B 58 (2003) 1489–1504
+                if self.fast or not Te:
+                    w = ((ne/1e23)**(0.67965)) * 1.098
+                    return lorentz_function(x,middle_wl,w)
+                else:
+                    this_loader = gigosos_loader(self.transition)
+                    gigosos_x,y = this_loader.load(ne, Te, pert)
+                    gigosos_x = gigosos_x + middle_wl # to nm
+                    y = interpol(gigosos_x,y,x)
+                    return y
+
+            if round(self.transition.wl, 0) == 486:
+                # Gigosos et al, Spectrochimica Acta Part B 58 (2003) 1489–1504
+                if self.fast or not Te:
+                    w = ((ne/1e23)**(0.68116)) * 4.8
+                    return lorentz_function(x,middle_wl,w)
+                else:
+                    this_loader = gigosos_loader(self.transition)
+                    gigosos_x,y = this_loader.load(ne, Te, pert)
+                    gigosos_x = gigosos_x + middle_wl # to nm
+                    y = interpol(gigosos_x,y,x)
+                    return y
+
+        ################ Helium ##########
+        if ele == "He":
+            if round(self.transition.wl,0) == 447:
+                # Gigosos et al, A&A 503, 293–299 (2009)
+                # doi: 10.1051/0004-6361/200912243
+                this_loader = gigosos_he_loader(self.transition)
+                gigosos_x,y = this_loader.load(ne, Te, pert)
+                gigosos_x = gigosos_x + middle_wl # to nm
+                y = interpol(gigosos_x,y,x)
+                return y
+
+            if round(self.transition.wl, 0) == 492:
+                # Lara et al, A&A 542, A75 (2012)
+                # doi: 10.1051/0004-6361/201219123
+                this_loader = gigosos_he_loader(self.transition)
+                gigosos_x,y = this_loader.load(ne, Te, pert)
+                gigosos_x = gigosos_x + middle_wl # to nm
+                y = interpol(gigosos_x,y,x)
+                return y
+
+        ################ Others: Griem ##########
+        if ele == "O" or "Ar":
+            this_griem = griem(self.transition)
+            w,d = this_griem.get_width_shift(ne, Te)
+            # shift is ignored for now
+            return lorentz_function(x,middle_wl,w)
+
+
+    def get_width(self, ne, Te=None, pert=None):
+        ele = self.transition.element
+        if ele == "O" or ele == "Ar":
+            this_griem = griem(self.transition)
+            w,d = this_griem.get_width_shift(ne, Te)
+            return w
+
+    def get_shift(self, ne, Te=None, pert=None):
+        ele = self.transition.element
+        if ele == "O" or ele == "Ar" :
+            this_griem = griem(self.transition)
+            w,d = this_griem.get_width_shift(ne, Te)
+            return d
+
+
```

### Comparing `owlspec-0.2.1/owlspec/util.py` & `owlspec-0.2.2/owlspec/util.py`

 * *Files identical despite different names*

### Comparing `owlspec-0.2.1/owlspec/vdW/vdW.py` & `owlspec-0.2.2/owlspec/vdW/vdW.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-#!/usr/bin/python
-
-import numpy as np
-from ..util import *
-from scipy import constants as const
-
-class vdW():
-    def __init__(self, transition, pert):
-        self.transition = transition
-        self.pert = pert
-
-
-    def get_profile(self,x, T, n):
-        middle_wl = x[int(len(x)/2)] - 0.5*abs((x[-1]-x[0])/(len(x)-1))
-        if not T:
-            print("""Need to provide a gas temperture (in Kelvin).
-            Assuming 300 K""")
-            T = 300
-
-        if self.transition.emitter.symbol == "H":
-            return self.hydrogen_profile(x,T,n)
-        w = self.get_width(self.transition, n, T)
-        y = lorentz_function(x,middle_wl,w)
-
-        return y/max(y)
-
-
-    def get_width(self, transition, n, T):
-        """
-        Interface for get_width2 using the transition properties.
-        Energies in eV, alpha in m^2,
-        lambda in nm, n in m^-3, T in K, m in amu.
-        """
-        
-        xc = self.transition.wl
-        m1 = self.transition.particle.m
-        m2 = self.pert.m
-        Eion = self.transition.particle.Ei
-        Eu = self.transition.upperE
-        El = self.transition.lowerE
-        lu = self.transition.upperl
-        ll = self.transition.lowerl
-        alpha = self.pert.dipole_polarizability*const.value('Bohr radius')**3
-                
-        return self.get_width2(xc,m1,m2,T,n,Eion,Eu,El,lu,ll,alpha)
-
-
-    def get_shift(self,x, n, T):
-        w = self.get_width(self.transition, n, T)
-        s = w*0.28 # citation needed
-        return s
-
-    
-    def get_width2(self,xc,m1,m2,T,n,Eion,Eu,El,lu,ll,alpha):
-        """
-        Energies in eV, alpha in m^2,
-        lambda in nm, n in m^-3, T in K, m in amu.
-        From: N. Konjevic & / Physics Reports 316 (1999) 339}401
-        """
-        mu = m1*m2/(m1+m2)
-
-        ### upper
-        EH = 13.59844
-        nj = np.sqrt(EH/(Eion-Eu))
-        Ru2 = 0.5*(nj**2) * (5 * (nj**2) + 1 - 3*lu * (lu + 1))
-
-        ### lower
-        nj = np.sqrt(EH/(Eion-El))
-        Rl2 = 0.5*(nj**2) * (5 * (nj**2) + 1 - 3*ll * (ll + 1))
-
-        R = np.sqrt(Ru2 - Rl2)
-        alpha = alpha*1e6 # to cm^3
-        n = n/1e6 # to cm^-3
-        xc = xc/1e7 # to cm
-        w = 8.18e-12 * (xc**2 ) * ((alpha * R**2)**(2/5)) * ((T/mu)**(3/10))*n
-        return w*1e7 # to nm
-
-
-    def hydrogen_profile(self,x,T,n):
-        """ Data from NIST: J. Phys. Chem. Ref. Data, Vol. 38, No. 3, 2009"""
-        middle_wl = x[int(len(x)/2)] - 0.5*abs((x[-1]-x[0])/(len(x)-1))
-        xc = self.transition.wl
-        m1 = self.transition.particle.m
-        m2 = self.pert.m
-        Eion = self.transition.particle.Ei
-        a = self.pert.dipole_polarizability*const.value('Bohr radius')**3
-
-        if round(self.transition.wl, 0) == 656:
-            H = self.transition.particle
-            #[Aik*gi, wl, Eu, El, lu, ll]
-            components = [
-            [2.2448e-01*4, 656.2724, 12.087507, 10.19881, 1, 0],
-            [2.2449e-01*2, 656.2771, 12.08749, 10.19881, 1, 0],
-
-            [4.2097e-02*2, 656.2909, 12.087495, 10.19885, 0, 1],
-            [2.1046e-02*2, 656.2752, 12.087495, 10.198806, 0, 1],
-
-            [6.4651e-01*6, 656.2852, 12.08751, 10.19885, 0, 1],
-            [5.3877e-01*4, 656.2701, 12.087507, 10.198806, 2, 1],
-            [1.0775e-01*4, 656.2868, 12.087507, 10.19885, 2, 1]]
-
-            y = np.zeros(len(x))
-            for comp in components:
-                Aik = comp[0]
-                wl = comp[1]     
-                w = self.get_width2(xc,m1,m2,T,n,Eion,*comp[2:],a)
-                y = y + Aik*lorentz_function(x,wl-656.280+middle_wl,w)
-
-
-        if round(self.transition.wl, 0) == 486:
-            H = self.transition.particle
-            #[Aik*gi, wl, Eu, El, lu, ll]
-            components = [
-            [1.7188e+07*4, 486.1278624, 12.74853800, 10.19880606, 2, 1],
-            [2.0625e+07*6, 486.1361516, 12.74853989, 10.19885143, 2, 1],
-            [3.4375e+06*4, 486.1365118, 12.74853800, 10.19885143, 2, 1],
-
-            [9.6680e+06*4, 486.1286949, 12.74853801, 10.19881044, 1, 0],
-            [9.6683e+06*2, 486.1297761, 12.74853234, 10.19881044, 1, 0],
-
-            [8.5941e+05*2, 486.1288370, 12.74853289, 10.19880606, 0, 1],
-            [1.7190e+06*2, 486.1374864, 12.74853289, 10.19885143, 0, 1]]
-
-            y = np.zeros(len(x))
-            for comp in components:
-                Aik = comp[0]
-                wl = comp[1]
-                w = self.get_width2(xc,m1,m2,T,n,Eion,*comp[2:],a)
-                y = y + Aik*lorentz_function(x,wl-486.133+middle_wl,w)
-
-
-        return y/max(y)
+#!/usr/bin/python
+
+import numpy as np
+from ..util import *
+from scipy import constants as const
+
+class vdW():
+    def __init__(self, transition, pert):
+        self.transition = transition
+        self.pert = pert
+
+
+    def get_profile(self,x, T, n):
+        middle_wl = x[int(len(x)/2)] - 0.5*abs((x[-1]-x[0])/(len(x)-1))
+        if not T:
+            print("""Need to provide a gas temperture (in Kelvin).
+            Assuming 300 K""")
+            T = 300
+
+        if self.transition.emitter.symbol == "H":
+            return self.hydrogen_profile(x,T,n)
+        w = self.get_width(self.transition, n, T)
+        y = lorentz_function(x,middle_wl,w)
+
+        return y/max(y)
+
+
+    def get_width(self, transition, n, T):
+        """
+        Interface for get_width2 using the transition properties.
+        Energies in eV, alpha in m^2,
+        lambda in nm, n in m^-3, T in K, m in amu.
+        """
+        
+        xc = self.transition.wl
+        m1 = self.transition.particle.m
+        m2 = self.pert.m
+        Eion = self.transition.particle.Ei
+        Eu = self.transition.upperE
+        El = self.transition.lowerE
+        lu = self.transition.upperl
+        ll = self.transition.lowerl
+        alpha = self.pert.dipole_polarizability*const.value('Bohr radius')**3
+                
+        return self.get_width2(xc,m1,m2,T,n,Eion,Eu,El,lu,ll,alpha)
+
+
+    def get_shift(self,x, n, T):
+        w = self.get_width(self.transition, n, T)
+        s = w*0.28 # citation needed
+        return s
+
+    
+    def get_width2(self,xc,m1,m2,T,n,Eion,Eu,El,lu,ll,alpha):
+        """
+        Energies in eV, alpha in m^2,
+        lambda in nm, n in m^-3, T in K, m in amu.
+        From: N. Konjevic & / Physics Reports 316 (1999) 339}401
+        """
+        mu = m1*m2/(m1+m2)
+
+        ### upper
+        EH = 13.59844
+        nj = np.sqrt(EH/(Eion-Eu))
+        Ru2 = 0.5*(nj**2) * (5 * (nj**2) + 1 - 3*lu * (lu + 1))
+
+        ### lower
+        nj = np.sqrt(EH/(Eion-El))
+        Rl2 = 0.5*(nj**2) * (5 * (nj**2) + 1 - 3*ll * (ll + 1))
+
+        R = np.sqrt(Ru2 - Rl2)
+        alpha = alpha*1e6 # to cm^3
+        n = n/1e6 # to cm^-3
+        xc = xc/1e7 # to cm
+        w = 8.18e-12 * (xc**2 ) * ((alpha * R**2)**(2/5)) * ((T/mu)**(3/10))*n
+        return w*1e7 # to nm
+
+
+    def hydrogen_profile(self,x,T,n):
+        """ Data from NIST: J. Phys. Chem. Ref. Data, Vol. 38, No. 3, 2009"""
+        middle_wl = x[int(len(x)/2)] - 0.5*abs((x[-1]-x[0])/(len(x)-1))
+        xc = self.transition.wl
+        m1 = self.transition.particle.m
+        m2 = self.pert.m
+        Eion = self.transition.particle.Ei
+        a = self.pert.dipole_polarizability*const.value('Bohr radius')**3
+
+        if round(self.transition.wl, 0) == 656:
+            H = self.transition.particle
+            #[Aik*gi, wl, Eu, El, lu, ll]
+            components = [
+            [2.2448e-01*4, 656.2724, 12.087507, 10.19881, 1, 0],
+            [2.2449e-01*2, 656.2771, 12.08749, 10.19881, 1, 0],
+
+            [4.2097e-02*2, 656.2909, 12.087495, 10.19885, 0, 1],
+            [2.1046e-02*2, 656.2752, 12.087495, 10.198806, 0, 1],
+
+            [6.4651e-01*6, 656.2852, 12.08751, 10.19885, 0, 1],
+            [5.3877e-01*4, 656.2701, 12.087507, 10.198806, 2, 1],
+            [1.0775e-01*4, 656.2868, 12.087507, 10.19885, 2, 1]]
+
+            y = np.zeros(len(x))
+            for comp in components:
+                Aik = comp[0]
+                wl = comp[1]     
+                w = self.get_width2(xc,m1,m2,T,n,Eion,*comp[2:],a)
+                y = y + Aik*lorentz_function(x,wl-656.280+middle_wl,w)
+
+
+        if round(self.transition.wl, 0) == 486:
+            H = self.transition.particle
+            #[Aik*gi, wl, Eu, El, lu, ll]
+            components = [
+            [1.7188e+07*4, 486.1278624, 12.74853800, 10.19880606, 2, 1],
+            [2.0625e+07*6, 486.1361516, 12.74853989, 10.19885143, 2, 1],
+            [3.4375e+06*4, 486.1365118, 12.74853800, 10.19885143, 2, 1],
+
+            [9.6680e+06*4, 486.1286949, 12.74853801, 10.19881044, 1, 0],
+            [9.6683e+06*2, 486.1297761, 12.74853234, 10.19881044, 1, 0],
+
+            [8.5941e+05*2, 486.1288370, 12.74853289, 10.19880606, 0, 1],
+            [1.7190e+06*2, 486.1374864, 12.74853289, 10.19885143, 0, 1]]
+
+            y = np.zeros(len(x))
+            for comp in components:
+                Aik = comp[0]
+                wl = comp[1]
+                w = self.get_width2(xc,m1,m2,T,n,Eion,*comp[2:],a)
+                y = y + Aik*lorentz_function(x,wl-486.133+middle_wl,w)
+
+
+        return y/max(y)
```

### Comparing `owlspec-0.2.1/owlspec.egg-info/PKG-INFO` & `owlspec-0.2.2/owlspec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owlspec
-Version: 0.2.1
+Version: 0.2.2
 Summary: Library for optical emission spectroscopy of low-temperature plasmas.
 Home-page: https://github.com/mimurrayy/owl
 Author: Julian Held
 Author-email: julian.held@umn.edu
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `owlspec-0.2.1/owlspec.egg-info/SOURCES.txt` & `owlspec-0.2.2/owlspec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owlspec-0.2.1/setup.py` & `owlspec-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="owlspec",
-    version="0.2.1",
+    version="0.2.2",
     author="Julian Held",
     author_email="julian.held@umn.edu",
     license='MIT',
     platforms=['any'],
     description="Library for optical emission spectroscopy of low-temperature plasmas.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

