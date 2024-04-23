# Comparing `tmp/pyKoalaRemote-1.0.2.tar.gz` & `tmp/pykoalaremote-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyKoalaRemote-1.0.2.tar", last modified: Mon Nov 13 15:54:49 2023, max compression
+gzip compressed data, was "pykoalaremote-1.0.3.tar", last modified: Tue Apr 23 14:17:52 2024, max compression
```

## Comparing `pyKoalaRemote-1.0.2.tar` & `pykoalaremote-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-11-13 15:54:49.132343 pyKoalaRemote-1.0.2/
--rw-rw-rw-   0        0        0     1070 2023-10-31 16:10:32.000000 pyKoalaRemote-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     3827 2023-11-13 15:54:49.131347 pyKoalaRemote-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3151 2023-11-10 16:33:51.000000 pyKoalaRemote-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-11-13 15:54:49.125362 pyKoalaRemote-1.0.2/pyKoalaRemote/
--rw-rw-rw-   0        0        0       20 2023-10-31 16:10:32.000000 pyKoalaRemote-1.0.2/pyKoalaRemote/__init__.py
--rw-rw-rw-   0        0        0    39621 2023-11-10 13:02:01.000000 pyKoalaRemote-1.0.2/pyKoalaRemote/client.py
--rw-rw-rw-   0        0        0     1539 2023-10-31 16:10:32.000000 pyKoalaRemote-1.0.2/pyKoalaRemote/remote_utils.py
-drwxrwxrwx   0        0        0        0 2023-11-13 15:54:49.129351 pyKoalaRemote-1.0.2/pyKoalaRemote.egg-info/
--rw-rw-rw-   0        0        0     3827 2023-11-13 15:54:49.000000 pyKoalaRemote-1.0.2/pyKoalaRemote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-11-13 15:54:49.000000 pyKoalaRemote-1.0.2/pyKoalaRemote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-13 15:54:49.000000 pyKoalaRemote-1.0.2/pyKoalaRemote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-11-13 15:54:49.000000 pyKoalaRemote-1.0.2/pyKoalaRemote.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-13 15:54:49.132343 pyKoalaRemote-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      805 2023-11-13 15:04:24.000000 pyKoalaRemote-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:17:52.258649 pykoalaremote-1.0.3/
+-rw-rw-rw-   0        0        0     1121 2024-04-23 14:15:15.000000 pykoalaremote-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3827 2024-04-23 14:17:52.257651 pykoalaremote-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3151 2023-11-14 08:27:16.000000 pykoalaremote-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 14:17:52.251667 pykoalaremote-1.0.3/pyKoalaRemote/
+-rw-rw-rw-   0        0        0       20 2023-10-31 16:10:32.000000 pykoalaremote-1.0.3/pyKoalaRemote/__init__.py
+-rw-rw-rw-   0        0        0    52981 2024-04-23 14:12:34.000000 pykoalaremote-1.0.3/pyKoalaRemote/client.py
+-rw-rw-rw-   0        0        0     1539 2023-10-31 16:10:32.000000 pykoalaremote-1.0.3/pyKoalaRemote/remote_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:17:52.256654 pykoalaremote-1.0.3/pyKoalaRemote.egg-info/
+-rw-rw-rw-   0        0        0     3827 2024-04-23 14:17:52.000000 pykoalaremote-1.0.3/pyKoalaRemote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-04-23 14:17:52.000000 pykoalaremote-1.0.3/pyKoalaRemote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 14:17:52.000000 pykoalaremote-1.0.3/pyKoalaRemote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-23 14:17:52.000000 pykoalaremote-1.0.3/pyKoalaRemote.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 14:17:52.258649 pykoalaremote-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      805 2024-04-23 14:12:34.000000 pykoalaremote-1.0.3/setup.py
```

### Comparing `pyKoalaRemote-1.0.2/LICENSE` & `pykoalaremote-1.0.3/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 Parent Jerome
+Copyright (c) 2024 Lyncée Tec SA (Parent Jerome, Colomb Tristan, Mendels Francois)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyKoalaRemote-1.0.2/PKG-INFO` & `pykoalaremote-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyKoalaRemote
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python wrapper for dotNet Koala Remote Client provided by LyncéeTec to control Digital Holographique Microscope using proprietary Koala software
 Home-page: https://github.com/lynceetec/pyKoalaRemote
 Author: Software Team: J. Parent - F. Mendels - T. Colomb
 Author-email: software@lynceetec.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pyKoalaRemote-1.0.2/README.md` & `pykoalaremote-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyKoalaRemote-1.0.2/pyKoalaRemote/client.py` & `pykoalaremote-1.0.3/pyKoalaRemote/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # -*- coding: utf-8 -*-
 """
 This class enables easy access to Koala TCP/IP remote interface
 Prompt dialog for connection and login
 Get functions return numpy Array
 2023-03-30 Modified by TCO (all functions using Remote Manual orders)
+2024.04.23 Add command to acquire a stack of data for different reconstruction distances
 """
 #from pythonnet import get_runtime_info
 #a = get_runtime_info()
 
 #import python package
 from pyKoalaRemote import remote_utils as ru
 import numpy as np
 import sys
 import clr
 import time
+import os
 
 #Add required dotNet reference
 clr.AddReference("System")
 import System
 from System import Array
 
 #Class pyRemote to manage dotNet dll in Python
@@ -866,21 +868,244 @@
     
     def StartStroboscopeFixedFrequency(self, cycleMode, numberOfPeriods):
         return self.host.StartStroboscopeFixedFrequency(cycleMode, numberOfPeriods)
     
     def StopStroboscope(self):
         return self.host.StopStroboscope()
 
+#specific codes
+    def CreateDirectory(self, directoryPath):
+        if not os.path.exists(directoryPath):
+            os.makedirs(directoryPath)   
+    
+    def SaveStackRecDistCM(self, distCM_Min, distCM_Max, distCM_step, savePath, saveIntensity=True,
+                             savePhase=True, saveAsBin=True, saveAsTxt=False, saveAsTif=False, saveLambda1=True,
+                             saveLambda2=False, saveLambdaSynthLong=False,
+                             saveLambdaSynthShort=False):
+        '''
+        distCM_Min : minimal reconstruction distance in cm
+        distCM_max : maximal reconstruction distance in cm
+        distCm_step : step in cm for the stack
+        savePath : path to save the data
+        saveIntensity : save Amplitude
+        savePhase : save Phase
+        saveAsBin : save as .bin format
+        saveAsTxt : save as .txt format
+        saveAsTif : save as .tif format
+        saveLambda1 : save data for lambda 1 #configuration lambda 1, 12 or 13
+        saveLambda2 : save data for second lambda  #configuration lambda 12 or 13
+        saveLambdaSynthLong : save data for long synthetic #configuration lambda 12 or 13
+        saveLambdaSynthShort : save data for short synthetic #configuration lambda 12 or 13
+        '''
+        Nsteps = (int)((distCM_Max-distCM_Min)/distCM_step)+1
+        d_stack = []
+        if Nsteps >= 1:
+            for k in range(Nsteps):
+                d = distCM_Min+k*distCM_step
+                d_stack.append(d)
+                self.SetRecDistCM(d)
+                self.OnDistanceChange()
+                if saveLambda1:
+                    if saveIntensity:
+                        self.SelectDisplayWL(2048)
+                        directory_amp = os.path.join(savePath,"Lambda1","Intensity","Float")
+                        if saveAsBin:
+                            directory = os.path.join(directory_amp,"Bin")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"_intensity.bin")
+                            self.SaveImageFloatToFile(2, fname, True)
+                        if saveAsTxt:
+                            directory = os.path.join(directory_amp,"Txt")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"_intensity.txt")
+                            self.SaveImageFloatToFile(2, fname, False)
+                        if saveAsTif:
+                            directory = os.path.join(savePath,"Lambda1","Intensity","Image")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"_intensity.jpg")
+                            self.SaveImageToFile(2, fname)
+                    if savePhase:
+                        self.SelectDisplayWL(8192)
+                        directory_amp = os.path.join(savePath,"Lambda1","Phase","Float")
+                        if saveAsBin:
+                            directory = os.path.join(directory_amp,"Bin")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"_phase.bin")
+                            self.SaveImageFloatToFile(4, fname, True)
+                        if saveAsTxt:
+                            directory = os.path.join(directory_amp,"Txt")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"_phase.txt")
+                            self.SaveImageFloatToFile(4, fname, False)
+                        if saveAsTif:
+                            directory = os.path.join(savePath,"Lambda1","Phase","Image")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"_phase.jpg")
+                            self.SaveImageToFile(4, fname)
+                            
+                if saveLambda2:
+                    if saveIntensity:
+                        self.SelectDisplayWL(4096)
+                        directory_amp = os.path.join(savePath,"Lambda2","Intensity","Float")
+                        if saveAsBin:
+                            directory = os.path.join(directory_amp,"Bin")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"_intensity.bin")
+                            self.SaveImageFloatToFile(2, fname, True)
+                        if saveAsTxt:
+                            directory = os.path.join(directory_amp,"Txt")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"_intensity.txt")
+                            self.SaveImageFloatToFile(2, fname, False)
+                        if saveAsTif:
+                            directory = os.path.join(savePath,"Lambda2","Intensity","Image")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"_intensity.jpg")
+                            self.SaveImageToFile(2, fname)
+                    if savePhase:
+                        self.SelectDisplayWL(16384)
+                        directory_amp = os.path.join(savePath,"Lambda2","Phase","Float")
+                        if saveAsBin:
+                            directory = os.path.join(directory_amp,"Bin")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"_phase.bin")
+                            self.SaveImageFloatToFile(4, fname, True)
+                        if saveAsTxt:
+                            directory = os.path.join(directory_amp,"Txt")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"_phase.txt")
+                            self.SaveImageFloatToFile(4, fname, False)
+                        if saveAsTif:
+                            directory = os.path.join(savePath,"Lambda2","Phase","Image")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"_phase.jpg")
+                            self.SaveImageToFile(4, fname)
+                            
+                if saveLambdaSynthLong:
+                    if savePhase:
+                        self.SelectDisplayWL(32768)
+                        directory_amp = os.path.join(savePath,"LambdaSynthLong","Phase","Float")
+                        if saveAsBin:
+                            directory = os.path.join(directory_amp,"Bin")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"_phase.bin")
+                            self.SaveImageFloatToFile(4, fname, True)
+                        if saveAsTxt:
+                            directory = os.path.join(directory_amp,"Txt")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"_phase.txt")
+                            self.SaveImageFloatToFile(4, fname, False)
+                        if saveAsTif:
+                            directory = os.path.join(savePath,"LambdaSynthLong","Phase","Image")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"_phase.jpg")
+                            self.SaveImageToFile(4, fname)
+                        
+                if saveLambdaSynthShort:
+                    if savePhase:
+                        self.SelectDisplayWL(65536)
+                        directory_amp = os.path.join(savePath,"LambdaSynthSort","Phase","Float")
+                        if saveAsBin:
+                            directory = os.path.join(directory_amp,"Bin")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"phase.bin")
+                            self.SaveImageFloatToFile(4, fname, True)
+                        if saveAsTxt:
+                            directory = os.path.join(directory_amp,"Txt")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"phase.txt")
+                            self.SaveImageFloatToFile(4, fname, False)
+                        if saveAsTif:
+                            directory = os.path.join(savePath,"LambdaSynthShort","Phase","Image")
+                            self.CreateDirectory(directory)
+                            fname = os.path.join(directory,str(k).zfill(5)+"phase.jpg")
+                            self.SaveImageToFile(4, fname)
+        else:
+            print("Number of steps are smaller than one. Verify that minimal distance is smaller than maximal one and that the step is correct")
+        return np.array(d_stack)
+    def GetStackRecDistCM(self, distCM_Min, distCM_Max, distCM_step, GetIntensity=True,
+                             GetPhase=True, GetLambda1=True,
+                             GetLambda2=False, GetLambdaSynthLong=False,
+                             GetLambdaSynthShort=False):
+        
+        '''
+        distCM_Min : minimal reconstruction distance in cm
+        distCM_max : maximal reconstruction distance in cm
+        distCm_step : step in cm for the stack
+        saveIntensity : save Amplitude Stack
+        savePhase : save Phase Stack
+        saveLambda1 : save data for lambda 1 #configuration lambda 1, 12 or 13
+        saveLambda2 : save data for second lambda  #configuration lambda 12 or 13
+        saveLambdaSynthLong : save data for long synthetic #configuration lambda 12 or 13
+        saveLambdaSynthShort : save data for short synthetic #configuration lambda 12 or 13
+        '''
+        Nsteps = (int)((distCM_Max-distCM_Min)/distCM_step)+1
+        w = self.GetPhaseWidth()
+        h = self.GetPhaseHeight()
+        IntensityLambda1Stack = None
+        IntensityLambda2Stack = None
+        PhaseLambda1Stack = None
+        PhaseLambda2Stack = None
+        PhaseLambdaSynthLongStack = None
+        PhaseLambdaSynthShortStack = None
+        d_stack = []
+        if Nsteps >= 1:
+            for k in range(Nsteps):
+                d = distCM_Min+k*distCM_step
+                d_stack.append(d)
+                self.SetRecDistCM(d)
+                self.OnDistanceChange()
+                if GetLambda1:
+                    if GetIntensity:
+                        self.SelectDisplayWL(2048)
+                        if k == 0 :
+                            IntensityLambda1Stack = np.ones((h,w,Nsteps))*np.nan
+                        IntensityLambda1Stack[:,:,k]= self.GetIntensity32fImage()
+                    if GetPhase:
+                        self.SelectDisplayWL(8192)
+                        if k == 0 :
+                            PhaseLambda1Stack = np.ones((h,w,Nsteps))*np.nan
+                        PhaseLambda1Stack[:,:,k]= self.GetPhase32fImage()
+                            
+                if GetLambda2:
+                    if GetIntensity:
+                        self.SelectDisplayWL(4096)
+                        if k == 0 :
+                            IntensityLambda2Stack = np.ones((h,w,Nsteps))*np.nan
+                        IntensityLambda2Stack[:,:,k]= self.GetIntensity32fImage()
+                    if GetPhase:
+                        self.SelectDisplayWL(16384)
+                        if k == 0 :
+                            PhaseLambda2Stack = np.ones((h,w,Nsteps))*np.nan
+                        PhaseLambda2Stack[:,:,k]= self.GetPhase32fImage()
+                            
+                if GetLambdaSynthLong:
+                    if GetPhase:
+                        self.SelectDisplayWL(32768)
+                        if k == 0 :
+                            PhaseLambdaSynthLongStack = np.ones((h,w,Nsteps))*np.nan
+                        PhaseLambdaSynthLongStack[:,:,k]= self.GetPhase32fImage()
+                        
+                if GetLambdaSynthShort:
+                    if GetPhase:
+                        self.SelectDisplayWL(65536)
+                        if k == 0 :
+                            PhaseLambdaSynthShortStack = np.ones((h,w,Nsteps))*np.nan
+                        PhaseLambdaSynthShortStack[:,:,k]= self.GetPhase32fImage()
+        else:
+            print("Number of steps are smaller than one. Verify that minimal distance is smaller than maximal one and that the step is correct")
+
+        return IntensityLambda1Stack,PhaseLambda1Stack, IntensityLambda2Stack,PhaseLambda2Stack,PhaseLambdaSynthLongStack,PhaseLambdaSynthShortStack, np.array(d_stack)
 
 #test the class when running this file directly
 if __name__ == '__main__' :
     remote = pyKoalaRemoteClient()
     remote.ConnectAndLoginDialog()
     remote.OpenConfigDialog()
-    remote.LoadHolo(r'C:\tmp\holo.tif',1)
+    remote.LoadHolo(r'C:\tmp_remote_test\Hologram12.tif',2)
     remote.OpenHoloWin()
     remote.OpenIntensityWin()
     remote.OpenPhaseWin()
     remote.OpenReconstructionSettingsWin()
     time.sleep(0.1) #wait window is open
     remote.AddCorrSegment(50,10,800,0)
 
@@ -891,8 +1116,15 @@
     remote.SetUnwrap2DState(True)
     remote.AddCorrZone(100,100,900,900)
     remote.ComputePhaseCorrection(4,2)
     remote.ResetCorrZone()
     remote.SetUnwrap2DState(False)
     remote.ResetPhaseOffsetAdjustmentZone()
     remote.AddPhaseOffsetAdjustmentZone(50,50, 200,200)
+    distCM_Min = 0
+    distCM_Max = 9.81
+    distCM_step = 0.5
+    savePath = r'C:\tmp_remote_test'
+    d_stack = remote.SaveStackRecDistCM(distCM_Min, distCM_Max, distCM_step, savePath)
+    print(d_stack)
+#    IntensityLambda1Stack,PhaseLambda1Stack, IntensityLambda2Stack,PhaseLambda2Stack,PhaseLambdaSynthLongStack,PhaseLambdaSynthShortStack = remote.GetStackRecDistCM(distCM_Min, distCM_Max, distCM_step)
     remote.Logout()
```

### Comparing `pyKoalaRemote-1.0.2/pyKoalaRemote/remote_utils.py` & `pykoalaremote-1.0.3/pyKoalaRemote/remote_utils.py`

 * *Files identical despite different names*

### Comparing `pyKoalaRemote-1.0.2/pyKoalaRemote.egg-info/PKG-INFO` & `pykoalaremote-1.0.3/pyKoalaRemote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyKoalaRemote
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python wrapper for dotNet Koala Remote Client provided by LyncéeTec to control Digital Holographique Microscope using proprietary Koala software
 Home-page: https://github.com/lynceetec/pyKoalaRemote
 Author: Software Team: J. Parent - F. Mendels - T. Colomb
 Author-email: software@lynceetec.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pyKoalaRemote-1.0.2/setup.py` & `pykoalaremote-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyKoalaRemote",
-    version="1.0.2",
+    version="1.0.3",
     author="Software Team: J. Parent - F. Mendels - T. Colomb",
     author_email="software@lynceetec.com",
     description="Python wrapper for dotNet Koala Remote Client provided by LyncéeTec to control Digital Holographique Microscope using proprietary Koala software",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lynceetec/pyKoalaRemote",
     packages=setuptools.find_packages(),
```

