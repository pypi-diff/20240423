# Comparing `tmp/pyt2s-0.0.1.tar.gz` & `tmp/pyt2s-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyt2s-0.0.1.tar", last modified: Sun Mar 31 14:17:42 2024, max compression
+gzip compressed data, was "pyt2s-0.0.2.tar", last modified: Tue Apr 23 12:57:30 2024, max compression
```

## Comparing `pyt2s-0.0.1.tar` & `pyt2s-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:17:42.745331 pyt2s-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-31 14:17:26.000000 pyt2s-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-31 14:17:42.745331 pyt2s-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 14:17:26.000000 pyt2s-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-31 14:17:26.000000 pyt2s-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 14:17:42.745331 pyt2s-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:17:42.741331 pyt2s-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:17:42.741331 pyt2s-0.0.1/src/pyt2s/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 14:17:26.000000 pyt2s-0.0.1/src/pyt2s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-31 14:17:26.000000 pyt2s-0.0.1/src/pyt2s/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:17:42.745331 pyt2s-0.0.1/src/pyt2s/services/
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-03-31 14:17:26.000000 pyt2s-0.0.1/src/pyt2s/services/acapela.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-31 14:17:26.000000 pyt2s-0.0.1/src/pyt2s/services/cepstral.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-31 14:17:26.000000 pyt2s-0.0.1/src/pyt2s/services/ibm_watson.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-03-31 14:17:26.000000 pyt2s-0.0.1/src/pyt2s/services/oddcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-03-31 14:17:26.000000 pyt2s-0.0.1/src/pyt2s/services/stream_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-03-31 14:17:26.000000 pyt2s-0.0.1/src/pyt2s/services/streamlabs.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-31 14:17:26.000000 pyt2s-0.0.1/src/pyt2s/services/voice_forge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:17:42.745331 pyt2s-0.0.1/src/pyt2s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-31 14:17:42.000000 pyt2s-0.0.1/src/pyt2s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-31 14:17:42.000000 pyt2s-0.0.1/src/pyt2s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:17:42.000000 pyt2s-0.0.1/src/pyt2s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-31 14:17:42.000000 pyt2s-0.0.1/src/pyt2s.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:57:30.873890 pyt2s-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-23 12:57:22.000000 pyt2s-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-23 12:57:30.873890 pyt2s-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-23 12:57:22.000000 pyt2s-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-23 12:57:22.000000 pyt2s-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 12:57:30.873890 pyt2s-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:57:30.869890 pyt2s-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:57:30.869890 pyt2s-0.0.2/src/pyt2s/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:57:22.000000 pyt2s-0.0.2/src/pyt2s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-23 12:57:22.000000 pyt2s-0.0.2/src/pyt2s/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:57:30.873890 pyt2s-0.0.2/src/pyt2s/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-23 12:57:22.000000 pyt2s-0.0.2/src/pyt2s/services/acapela.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-23 12:57:22.000000 pyt2s-0.0.2/src/pyt2s/services/cepstral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-23 12:57:22.000000 pyt2s-0.0.2/src/pyt2s/services/ibm_watson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-23 12:57:22.000000 pyt2s-0.0.2/src/pyt2s/services/oddcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-23 12:57:22.000000 pyt2s-0.0.2/src/pyt2s/services/stream_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-23 12:57:22.000000 pyt2s-0.0.2/src/pyt2s/services/streamlabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-23 12:57:22.000000 pyt2s-0.0.2/src/pyt2s/services/voice_forge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:57:30.873890 pyt2s-0.0.2/src/pyt2s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-23 12:57:30.000000 pyt2s-0.0.2/src/pyt2s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-23 12:57:30.000000 pyt2s-0.0.2/src/pyt2s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:57:30.000000 pyt2s-0.0.2/src/pyt2s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 12:57:30.000000 pyt2s-0.0.2/src/pyt2s.egg-info/top_level.txt
```

### Comparing `pyt2s-0.0.1/LICENSE` & `pyt2s-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyt2s-0.0.1/src/pyt2s/services/acapela.py` & `pyt2s-0.0.2/src/pyt2s/services/acapela.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from ..service import Service
+from pyt2s.service import Service
 import requests
 
 class Acapela(Service):
 
     __validNames__ = [ 'graham22k', 'harry22k', 'lucy22k', 'lucy_nt22k', 'peter22k', 'peter_nt22k', 'queenelizabeth22k', 'queenelizabeth_nt22k', 'rachel22k', 'rachel_nt22k', 
         'rosie22k', 'sophiabtob22k', 'sophiabtob_nt22k', 'rhona22k', 'rhona_nt22k', 'liam22k', 'lisa22k', 'lisa_nt22k', 'olivia22k', 'tyler22k', 'tyler_nt22k', 
         'deepa22k', 'deepa_nt22k', 'nizareng22k', 'nizareng_nt22k', 'darius22k', 'darius_nt22k', 'ella22k', 'emilioenglish22k', 'josh22k', 'karen22k', 'karen_nt22k',
```

### Comparing `pyt2s-0.0.1/src/pyt2s/services/cepstral.py` & `pyt2s-0.0.2/src/pyt2s/services/cepstral.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 import time
-from ..service import Service
+from pyt2s.service import Service
 
 class Cepstral(Service):
 
     __validNames__ = [ 'Allison', 'Amy', 'Belle', 'Callie', 'Charlie', 'Dallas', 'Damien', 'David', 'Diane', 'Duchess', 'Emily', 'Linda', 'Robin', 'Shouty', 'Walter', 
         'William', 'Whispery', 'Lawrence', 'Millie', 'Duncan', 'Vittoria', 'Katrin', 'Matthias', 'Isabelle', 'Jean-Pierre', 'Alejandra', 'Miguel' ]
 
     __session__ = requests.session()
```

### Comparing `pyt2s-0.0.1/src/pyt2s/services/oddcast.py` & `pyt2s-0.0.2/src/pyt2s/services/oddcast.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-from ..service import Service
+from pyt2s.service import Service
 
 class Oddcast(Service):
 
     __validNames__ = [ '4-3-1', '6-2-1', '5-4-1', '4-2-1', '5-3-1', '2-7-1', '1-7-1', '7-4-1', '5-2-1', '12-4-1', '8-4-1', '9-2-1', '10-2-1', '4-7-1', '4-4-1', '10-4-1', 
         '3-7-1', '13-4-1', '5-7-1', '6-7-1', '9-4-1', '11-2-1', '7-2-1', '6-3-1', '8-3-1', '7-7-1', '3-1-1', '1-1-1', '2-2-1', '7-3-1', '2-4-1', '3-3-1', '1-3-1', 
         '2-1-1', '2-3-1', '4-1-1', '11-4-1', '8-2-1', '1-2-1', '3-4-1', '8-7-1', '1-7-27', '2-7-27', '2-2-27', '1-4-27', '1-2-27', '1-4-22', '3-2-5', '2-2-5', 
         '1-2-5', '1-4-5', '3-3-10', '5-3-10', '4-3-10', '1-2-10', '2-2-10', '4-4-10', '4-7-10', '6-3-10', '7-3-10', '1-4-10', '3-7-10', '2-7-10', '1-7-10', '2-4-10',
```

### Comparing `pyt2s-0.0.1/src/pyt2s/services/stream_elements.py` & `pyt2s-0.0.2/src/pyt2s/services/stream_elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-from ..service import Service
+from pyt2s.service import Service
 
 class StreamElements(Service):
 
     __validNames__ = [ 'Brian', 'Amy', 'Emma', 'Geraint', 'Russell', 'Nicole', 'Joey', 'Justin', 'Matthew', 'Ivy', 'Joanna', 'Kendra', 'Kimberly', 'Salli', 'Raveena', 'Zhiyu', 
         'Mads', 'Naja', 'Ruben', 'Lotte', 'Mathieu', 'Celine', 'Chantal', 'Hans', 'Marlene', 'Vicki', 'Aditi', 'Karl', 'Dora', 'Carla', 'Bianca', 'Giorgio', 
         'Takumi', 'Mizuki', 'Seoyeon', 'Liv', 'Ewa', 'Maja', 'Jacek', 'Jan', 'Ricardo', 'Vitoria', 'Cristiano', 'Ines', 'Carmen', 'Maxim', 'Tatyana', 'Enrique', 
         'Conchita', 'Mia', 'Miguel', 'Penelope', 'Astrid', 'Filiz', 'Gwyneth', 'en-US-Wavenet-A', 'en-US-Wavenet-B', 'en-US-Wavenet-C', 'en-US-Wavenet-D',
```

### Comparing `pyt2s-0.0.1/src/pyt2s/services/streamlabs.py` & `pyt2s-0.0.2/src/pyt2s/services/streamlabs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-from ..service import Service
+from pyt2s.service import Service
 
 class StreamLabs(Service):
     
     __validNames__ = [ 'Brian', 'Amy', 'Emma', 'Geraint', 'Russell', 'Nicole', 'Joey', 'Justin', 'Matthew', 'Ivy', 'Joanna', 'Kendra', 'Kimberly', 'Salli', 'Raveena', 'Zeina', 
         'Zhiyu', 'Mads', 'Naja', 'Ruben', 'Lotte', 'Mathieu', 'Celine', 'Lea', 'Chantal', 'Hans', 'Marlene', 'Vicki', 'Aditi', 'Karl', 'Dora', 'Carla', 'Bianca', 
         'Giorgio', 'Takumi', 'Mizuki', 'Seoyeon', 'Liv', 'Ewa', 'Maja', 'Jacek', 'Jan', 'Ricardo', 'Camila', 'Vitoria', 'Cristiano', 'Ines', 'Carmen', 'Maxim', 
         'Tatyana', 'Enrique', 'Conchita', 'Lucia', 'Mia', 'Miguel', 'Lupe', 'Penelope', 'Astrid', 'Filiz', 'Gwyneth' ]
```

### Comparing `pyt2s-0.0.1/src/pyt2s/services/voice_forge.py` & `pyt2s-0.0.2/src/pyt2s/services/voice_forge.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-from ..service import Service
+from pyt2s.service import Service
 
 class VoiceForge(Service):
     
     __validNames__ = [ 'Conrad', 'Designer', 'Diesel', 'Dog', 'Evilgenius', 'Frank', 'French-fry', 'Gregory', 'Jerkface', 'JerseyGirl', 'Kayla', 'Kevin', 
         'Kidaroo', 'Princess', 'RansomNote', 'Robot', 'Shygirl', 'Susan', 'Tamika', 'TopHat', 'Vixen', 'Vlad', 'Warren', 'Wiseguy', 'Zach', 'Obama' ]
     
     __url1__ = 'https://api.voiceforge.com/swift_engine?'
```

