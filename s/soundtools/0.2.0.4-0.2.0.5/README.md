# Comparing `tmp/soundtools-0.2.0.4.tar.gz` & `tmp/soundtools-0.2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundtools-0.2.0.4.tar", last modified: Fri Apr 19 12:40:15 2024, max compression
+gzip compressed data, was "soundtools-0.2.0.5.tar", last modified: Tue Apr 23 10:58:29 2024, max compression
```

## Comparing `soundtools-0.2.0.4.tar` & `soundtools-0.2.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 12:40:15.362657 soundtools-0.2.0.4/
--rw-rw-rw-   0        0        0      701 2024-04-19 12:40:15.362657 soundtools-0.2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.2.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 12:40:15.363657 soundtools-0.2.0.4/setup.cfg
--rw-rw-rw-   0        0        0      789 2024-04-19 12:39:58.000000 soundtools-0.2.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 12:40:15.359654 soundtools-0.2.0.4/soundtools/
--rw-rw-rw-   0        0        0      399 2024-04-19 12:39:36.000000 soundtools-0.2.0.4/soundtools/__init__.py
--rw-rw-rw-   0        0        0    36640 2024-04-19 12:39:45.000000 soundtools-0.2.0.4/soundtools/soundtools.py
-drwxrwxrwx   0        0        0        0 2024-04-19 12:40:15.362657 soundtools-0.2.0.4/soundtools.egg-info/
--rw-rw-rw-   0        0        0      701 2024-04-19 12:40:15.000000 soundtools-0.2.0.4/soundtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-19 12:40:15.000000 soundtools-0.2.0.4/soundtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 12:40:15.000000 soundtools-0.2.0.4/soundtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-19 12:40:15.000000 soundtools-0.2.0.4/soundtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 10:58:29.932450 soundtools-0.2.0.5/
+-rw-rw-rw-   0        0        0      701 2024-04-23 10:58:29.929930 soundtools-0.2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.2.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 10:58:29.933450 soundtools-0.2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      789 2024-04-23 10:58:18.000000 soundtools-0.2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:58:29.917046 soundtools-0.2.0.5/soundtools/
+-rw-rw-rw-   0        0        0      399 2024-04-23 10:58:06.000000 soundtools-0.2.0.5/soundtools/__init__.py
+-rw-rw-rw-   0        0        0    37291 2024-04-23 10:58:00.000000 soundtools-0.2.0.5/soundtools/soundtools.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:58:29.920046 soundtools-0.2.0.5/soundtools.egg-info/
+-rw-rw-rw-   0        0        0      701 2024-04-23 10:58:29.000000 soundtools-0.2.0.5/soundtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-23 10:58:29.000000 soundtools-0.2.0.5/soundtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 10:58:29.000000 soundtools-0.2.0.5/soundtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-23 10:58:29.000000 soundtools-0.2.0.5/soundtools.egg-info/top_level.txt
```

### Comparing `soundtools-0.2.0.4/PKG-INFO` & `soundtools-0.2.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: soundtools
-Version: 0.2.0.4
+Version: 0.2.0.5
 Summary: used to work with sounds waves
 Author: Mohammad Erfan Karami
 Author-email: erfan012amir016@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
 made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.0.4
+version: 0.2.0.5
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves
```

### Comparing `soundtools-0.2.0.4/setup.py` & `soundtools-0.2.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 setup(
 name='soundtools',
-version='0.2.0.4',
+version='0.2.0.5',
 description="used to work with sounds waves",
 long_description="""made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.0.4
+version: 0.2.0.5
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves""",
 author='Mohammad Erfan Karami',
```

### Comparing `soundtools-0.2.0.4/soundtools/soundtools.py` & `soundtools-0.2.0.5/soundtools/soundtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """### made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-### version: 0.2.0.4
+### version: 0.2.0.5
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves"""
 
@@ -235,15 +235,16 @@
         buf += vol*0.9 * np.sin(pi_2_samples_num * freq*2 / self.default_sample_rate)
         buf += vol * np.sin(pi_2_samples_num * freq*4 / self.default_sample_rate)
         buf += vol*0.6 * np.sin(pi_2_samples_num * freq*6 / self.default_sample_rate)
         buf += vol*0.7 * np.sin(pi_2_samples_num * freq*16 / self.default_sample_rate)
         buf += vol*0.5 * np.sin(pi_2_samples_num * freq*20 / self.default_sample_rate)
         buf += vol*0.3 * np.sin(pi_2_samples_num * freq*24 / self.default_sample_rate)
 
-        wave = (buf/7*0.4247).astype(self.dtype)
+        wave = (buf/7*1.424).astype(self.dtype)
+        # wave = (buf/7*1.4247).astype(self.dtype) # for better percision (might cause quality issues on high volumes)
         return wave
     
     @cache_wave("marimb")
     def marimba(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         """creates a "not even close to marimba" sound based on the given frequency, duration and amplitude or volume\n
         warning!: very annoying sound"""
         
@@ -394,15 +395,15 @@
             sampwidth = int.from_bytes(data[4:6], "little")
             channels = int.from_bytes(data[6:8], "little")
             
             self.stream = self.AUDIO_OBJECT.open(format=self.AUDIO_OBJECT.get_format_from_width(sampwidth),
                                                  channels=channels,
                                                  rate=sample_rate,
                                                  output=True)
-            return data[8:]
+            return np.frombuffer(data[8:], self.get_sampwidth_from_int(sampwidth))
     
     
     def erfan_to_wav(self, file_name: str, dir: str="", dtype=np.float32) -> None:
         """converts a \".erfan\" file to a \".wav\" file"""
         file_short_name = file_name.removesuffix(".erfan")
         with open(file_name, "rb") as f:
             data = f.read()
@@ -662,20 +663,23 @@
             
         
         #-- other files such as mp3, ogg, wav, aiff, flac --#
         else:
             return sfRead(file_path)
     
     
-    def pitch_shift(self, wave: SoundBuffer, semitones: float, sample_rate: int|None=None, semitones_per_octave: int=12) -> SoundBuffer:
+    def pitch_shift(self, wave: SoundBuffer, n_semitones: float, sample_rate: int|None=None, semitones_per_octave: int=12) -> SoundBuffer:
         """shifts the pitch by the given number of semitones"""
         if not sample_rate:
             sample_rate = self.default_sample_rate
         
-        return effect.pitch_shift(wave, sample_rate, semitones, semitones_per_octave)
+        return effect.pitch_shift(wave,
+                                  sr=sample_rate,
+                                  n_steps=n_semitones,
+                                  bins_per_octave=semitones_per_octave)
     
     
     # creates a note buffer but doesn't turn it into bytes
     def generate_note_buffer(self, note:str|float|int, wave_type: Wave, duration:str|float=0, volume:float=0) -> SoundBuffer:
         """creates a sound wave based on the given note, wave type, duration and volume\n
         ### parameter note:
         can be a float as a frequency, or a string representing the note name forexample: \"A4\" or \"c#3\" or 220
@@ -749,20 +753,28 @@
         """generates then plays a note with the given arguments"""
         buf: bytes = self.generate_note_buffer(note, wave_type, duration, volume).tobytes()
     
         self.play_buffer(buf)
     
     
     # plays a buffer
-    def play_buffer(self, wave: np.ndarray|bytes) -> None:
+    def play_buffer(self, wave: SoundBuffer|bytes, chunk:int=3200, dtype:Dtype|None=None) -> None:
         """plays the given wave"""
-        if type(wave) != bytes:
-            wave = wave.tobytes()
         
-        self.stream.write(wave)
+        if type(wave) == bytes:
+            dtype = self.dtype if not dtype else dtype
+            wave = np.frombuffer(wave, self.dtype)
+        
+        n_chunks = int(wave.size / chunk)
+        for i in range(n_chunks):
+            b = wave[i*chunk : (i+1)*chunk].data.tobytes()
+            self.stream.write(b)
+        
+        b = wave[(i+1)*chunk : ].data.tobytes()
+        self.stream.write(b)
     
     
     # created a chord sound buffer and plays it
     def play_chord(self, notes: Iterable, wave_type: Wave, duration:str|float=0, volume:float=0) -> None:
         """generates then plays a chord with the given arguments"""
         buf = self.generate_chord_buffer(notes, wave_type, duration, volume).tobytes()
         
@@ -821,15 +833,15 @@
         plt.xlim(0, duration)
         plt.colorbar()
         plt.show()
     
     
     def done(self) -> None:
         """will stop and close the stream and terminate the audio_object (basicly closes everything)"""
-        if not self.stream.is_stopped():
+        if self.stream.is_active():
             self.stream.stop_stream()
-        if not self.input_stream.is_stopped():
+        if self.input_stream.is_active():
             self.input_stream.stop_stream()
         
         self.stream.close()
         self.input_stream.close()
         self.AUDIO_OBJECT.terminate()
```

### Comparing `soundtools-0.2.0.4/soundtools.egg-info/PKG-INFO` & `soundtools-0.2.0.5/soundtools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: soundtools
-Version: 0.2.0.4
+Version: 0.2.0.5
 Summary: used to work with sounds waves
 Author: Mohammad Erfan Karami
 Author-email: erfan012amir016@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
 made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.0.4
+version: 0.2.0.5
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves
```

