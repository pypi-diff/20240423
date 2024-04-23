# Comparing `tmp/pylake-0.1.5.tar.gz` & `tmp/pylake-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pylake-0.1.5.tar", last modified: Thu Nov 17 10:08:50 2022, max compression
+gzip compressed data, was "pylake-0.1.6.tar", last modified: Tue Apr 23 13:13:07 2024, max compression
```

## Comparing `pylake-0.1.5.tar` & `pylake-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-11-17 10:08:50.082565 pylake-0.1.5/
--rw-rw-rw-   0        0        0     1390 2022-11-17 10:08:50.081564 pylake-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1079 2022-07-11 08:10:52.000000 pylake-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2022-11-17 10:08:50.063660 pylake-0.1.5/pylake/
--rw-rw-rw-   0        0        0       56 2022-07-06 09:30:47.000000 pylake-0.1.5/pylake/__init__.py
--rw-rw-rw-   0        0        0     6237 2022-07-12 09:07:41.000000 pylake-0.1.5/pylake/functions.py
--rw-rw-rw-   0        0        0     1555 2022-07-12 12:59:07.000000 pylake-0.1.5/pylake/functions_meta.py
--rw-rw-rw-   0        0        0    30696 2022-11-17 09:57:08.000000 pylake-0.1.5/pylake/pylake.py
--rw-rw-rw-   0        0        0    25005 2022-07-12 14:06:32.000000 pylake-0.1.5/pylake/pylake_metabolizer.py
-drwxrwxrwx   0        0        0        0 2022-11-17 10:08:50.075760 pylake-0.1.5/pylake.egg-info/
--rw-rw-rw-   0        0        0     1390 2022-11-17 10:08:49.000000 pylake-0.1.5/pylake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2022-11-17 10:08:49.000000 pylake-0.1.5/pylake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-17 10:08:49.000000 pylake-0.1.5/pylake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2022-11-17 10:08:49.000000 pylake-0.1.5/pylake.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-11-17 10:08:49.000000 pylake-0.1.5/pylake.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-17 10:08:50.082565 pylake-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      793 2022-11-17 10:08:04.000000 pylake-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-17 10:08:50.077875 pylake-0.1.5/test/
--rw-rw-rw-   0        0        0     1425 2022-07-06 14:57:39.000000 pylake-0.1.5/test/test.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:13:07.693514 pylake-0.1.6/
+-rw-rw-rw-   0        0        0     1410 2024-04-23 13:13:07.691520 pylake-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1079 2024-04-23 13:00:55.000000 pylake-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 13:13:07.674907 pylake-0.1.6/pylake/
+-rw-rw-rw-   0        0        0       56 2024-04-23 13:00:55.000000 pylake-0.1.6/pylake/__init__.py
+-rw-rw-rw-   0        0        0     6237 2024-04-23 13:00:55.000000 pylake-0.1.6/pylake/functions.py
+-rw-rw-rw-   0        0        0     1555 2024-04-23 13:00:55.000000 pylake-0.1.6/pylake/functions_meta.py
+-rw-rw-rw-   0        0        0    30692 2024-04-23 13:00:55.000000 pylake-0.1.6/pylake/pylake.py
+-rw-rw-rw-   0        0        0    25005 2024-04-23 13:00:55.000000 pylake-0.1.6/pylake/pylake_metabolizer.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:13:07.686539 pylake-0.1.6/pylake.egg-info/
+-rw-rw-rw-   0        0        0     1410 2024-04-23 13:13:07.000000 pylake-0.1.6/pylake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-04-23 13:13:07.000000 pylake-0.1.6/pylake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 13:13:07.000000 pylake-0.1.6/pylake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2024-04-23 13:13:07.000000 pylake-0.1.6/pylake.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-23 13:13:07.000000 pylake-0.1.6/pylake.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 13:13:07.693514 pylake-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-04-23 13:12:55.000000 pylake-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:13:07.689528 pylake-0.1.6/test/
+-rw-rw-rw-   0        0        0     1425 2024-04-23 13:00:55.000000 pylake-0.1.6/test/test.py
```

### Comparing `pylake-0.1.5/PKG-INFO` & `pylake-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pylake
-Version: 0.1.5
+Version: 0.1.6
 Summary: pylake
-Home-page: https://github.com/hugocruzz/pylake
+Home-page: https://github.com/eawag-surface-waters-research/PyLake
 Author: Hugo Cruz
 Author-email: <huggcruzz@gmail.com>
 License: MIT
 Keywords: python,pylake,Lake analyzer,environmental data,Physical properties
 Description-Content-Type: text/markdown
 
 # PyLake
```

### Comparing `pylake-0.1.5/README.md` & `pylake-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pylake-0.1.5/pylake/functions.py` & `pylake-0.1.6/pylake/functions.py`

 * *Files identical despite different names*

### Comparing `pylake-0.1.5/pylake/functions_meta.py` & `pylake-0.1.6/pylake/functions_meta.py`

 * *Files identical despite different names*

### Comparing `pylake-0.1.5/pylake/pylake.py` & `pylake-0.1.6/pylake/pylake.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,15 +444,15 @@
         depth resolution for the integral calculus
     NaN_interp: bool, defaults : False
         If NaN_interp=True, it will perform a linear interpolation to replace NaN values
         The Schmidt stability calculation perform poorly if NaN are present.
     
     Returns
     ----------
-        - Schmidt stability (J.m-2)
+        - Schmidt stability (J/m**2)
 
     Example
     ----------
     >>>    bthA	=	np.array([1000,900,864,820,200,10])
     ...    bthD	=	np.array([0,2.3,2.5,4.2,5.8,7]) 
     ...    wtr	=	np.array([28,27,26.4,26,25.4,24,23.3])
     ...    depth=   np.array([0,1,2,3,4,5,6])  
@@ -561,15 +561,15 @@
         Average density of the hypolimnion
     g: scalar, default: 9.81
         gravity acceleration (m/s2)
 
     Returns
     ---------
     T1: array_like, scalar
-        Mode-1 vertical seiche period (h)
+        Mode-1 vertical seiche period (s)
 
     example
     ---------
     >>>    bthA =np.array([1000,900,864,820,200,10])
     ...    bthD=np.array([0,2.3,2.5,4.2,5.8,7])
     ...    depth	= np.array([0,1,2,3,4,5,6])
     ...    Zt = 4.5
@@ -580,15 +580,15 @@
     ...    1445418 
     '''
     g_reduced = g*delta_rho/AvHyp_rho
     Zd = depth[-1]
     h2 = Zd-Zt
     h1 = Zt
     T1 = 2*Lt*np.sqrt((h1+h2)/(g_reduced*h1*h2))
-    return T1*60*60
+    return T1 
 
 def Lake_number(bthA, bthD, ustar, St, metaT, metaB, averageHypoDense, g=9.81):
     '''
     Description: The Lake Number, defined by Imberger and Patterson (1990), has been used to
     describe processes relevant to the internal mixing of lakes induced by wind
     forcings. Lower values of Lake Number represent a higher potential for
     increased diapycnal mixing, which increases the vertical flux of mass and
```

### Comparing `pylake-0.1.5/pylake/pylake_metabolizer.py` & `pylake-0.1.6/pylake/pylake_metabolizer.py`

 * *Files identical despite different names*

### Comparing `pylake-0.1.5/pylake.egg-info/PKG-INFO` & `pylake-0.1.6/pylake.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pylake
-Version: 0.1.5
+Version: 0.1.6
 Summary: pylake
-Home-page: https://github.com/hugocruzz/pylake
+Home-page: https://github.com/eawag-surface-waters-research/PyLake
 Author: Hugo Cruz
 Author-email: <huggcruzz@gmail.com>
 License: MIT
 Keywords: python,pylake,Lake analyzer,environmental data,Physical properties
 Description-Content-Type: text/markdown
 
 # PyLake
```

### Comparing `pylake-0.1.5/setup.py` & `pylake-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     README = f.read()
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 DESCRIPTION = 'pylake'
 
 setup(
     name="pylake",
     version=VERSION,
     author="Hugo Cruz",
     author_email="<huggcruzz@gmail.com>",
     description=DESCRIPTION,
     long_description=README,
     long_description_content_type='text/markdown',
     packages=find_packages(),
-    url='https://github.com/hugocruzz/pylake',
+    url='https://github.com/eawag-surface-waters-research/PyLake',
     install_requires=[
         'numpy>=1.19.5',
         'pandas>=1.1.5',
         'PyYAML>=6.0',
         'scipy>=1.5.4',
         'dask>=2022.02.1',
         'xarray>=0.19.0',
```

### Comparing `pylake-0.1.5/test/test.py` & `pylake-0.1.6/test/test.py`

 * *Files identical despite different names*

