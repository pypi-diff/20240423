# Comparing `tmp/rlsdk_python-0.1.1.tar.gz` & `tmp/rlsdk_python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlsdk_python-0.1.1.tar", max compression
+gzip compressed data, was "rlsdk_python-0.2.1.tar", max compression
```

## Comparing `rlsdk_python-0.1.1.tar` & `rlsdk_python-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      318 2024-04-21 20:56:37.388717 rlsdk_python-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1640 2024-04-21 20:56:20.206780 rlsdk_python-0.1.1/README.md
--rw-r--r--   0        0        0      107 2024-04-16 11:12:58.877877 rlsdk_python-0.1.1/rlsdk_python/__init__.py
--rw-r--r--   0        0        0     1812 2024-04-18 23:00:20.787805 rlsdk_python-0.1.1/rlsdk_python/event_handling.py
--rw-r--r--   0        0        0     1814 2024-04-18 21:23:06.061748 rlsdk_python-0.1.1/rlsdk_python/events.py
--rw-r--r--   0        0        0     4038 2024-04-17 01:30:35.234518 rlsdk_python-0.1.1/rlsdk_python/frida_script.py
--rw-r--r--   0        0        0    36018 2024-04-21 20:26:34.484877 rlsdk_python-0.1.1/rlsdk_python/game_objects.py
--rw-r--r--   0        0        0    15039 2024-04-21 17:06:11.842639 rlsdk_python-0.1.1/rlsdk_python/sdk.py
--rw-r--r--   0        0        0     1982 1970-01-01 00:00:00.000000 rlsdk_python-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      318 2024-04-23 15:29:27.105419 rlsdk_python-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1640 2024-04-21 20:56:20.206780 rlsdk_python-0.2.1/README.md
+-rw-r--r--   0        0        0      107 2024-04-16 11:12:58.877877 rlsdk_python-0.2.1/rlsdk_python/__init__.py
+-rw-r--r--   0        0        0     1812 2024-04-18 23:00:20.787805 rlsdk_python-0.2.1/rlsdk_python/event_handling.py
+-rw-r--r--   0        0        0     1814 2024-04-18 21:23:06.061748 rlsdk_python-0.2.1/rlsdk_python/events.py
+-rw-r--r--   0        0        0     4038 2024-04-17 01:30:35.234518 rlsdk_python-0.2.1/rlsdk_python/frida_script.py
+-rw-r--r--   0        0        0    42302 2024-04-23 15:28:57.392660 rlsdk_python-0.2.1/rlsdk_python/game_objects.py
+-rw-r--r--   0        0        0    17791 2024-04-23 15:00:21.419337 rlsdk_python-0.2.1/rlsdk_python/sdk.py
+-rw-r--r--   0        0        0     1982 1970-01-01 00:00:00.000000 rlsdk_python-0.2.1/PKG-INFO
```

### Comparing `rlsdk_python-0.1.1/README.md` & `rlsdk_python-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.1.1/rlsdk_python/event_handling.py` & `rlsdk_python-0.2.1/rlsdk_python/event_handling.py`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.1.1/rlsdk_python/events.py` & `rlsdk_python-0.2.1/rlsdk_python/events.py`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.1.1/rlsdk_python/frida_script.py` & `rlsdk_python-0.2.1/rlsdk_python/frida_script.py`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.1.1/rlsdk_python/game_objects.py` & `rlsdk_python-0.2.1/rlsdk_python/game_objects.py`

 * *Files 14% similar despite different names*

```diff
@@ -329,14 +329,54 @@
         # Lire chaque caractère de la chaîne
         for i in range(array_count - 1):  # -1 car il y a souvent un caractère null de terminaison
             char = self.sdk.pm.read_ushort(array_data_address + (i * 2))  # lire 2 octets à la fois
             result += chr(char)
 
         return result
     
+    
+    
+    
+# // Class Engine.PlayerReplicationInfo
+# // 0x01A8 (0x0268 - 0x0410)
+# class APlayerReplicationInfo : public AReplicationInfo
+# {
+# public:
+# 	class UObjectProvider*                             ObjectProvider;                                // 0x0268 (0x0008) [0x0000000004080008] (CPF_ExportObject | CPF_Component | CPF_EditInline)
+# 	class UGroupComponent_ORS*                         RegistryGroup;                                 // 0x0270 (0x0008) [0x0000000004080008] (CPF_ExportObject | CPF_Component | CPF_EditInline)
+# 	int32_t                                            Score;                                         // 0x0278 (0x0004) [0x0000000100000020] (CPF_Net)     
+# 	int32_t                                            Deaths;                                        // 0x027C (0x0004) [0x0000000000000020] (CPF_Net)     
+# 	uint8_t                                            Ping;                                          // 0x0280 (0x0001) [0x0000000000000020] (CPF_Net)     
+# 	ETTSSpeaker                                        TTSSpeaker;                                    // 0x0281 (0x0001) [0x0000000000002000] (CPF_Transient)
+# 	uint8_t                                           UnknownData00[0x2];                            // 0x0282 (0x0002) MISSED OFFSET
+# 	int32_t                                            NumLives;                                      // 0x0284 (0x0004) [0x0000000000000000]               
+# 	class FString                                      PlayerName;                                    // 0x0288 (0x0010) [0x0000000100400020] (CPF_Net | CPF_NeedCtorLink)
+# 	class FString                                      OldName;                                       // 0x0298 (0x0010) [0x0000000000400000] (CPF_NeedCtorLink)
+# 	int32_t                                            PlayerID;                                      // 0x02A8 (0x0004) [0x0000000000000020] (CPF_Net)     
+# 	uint8_t                                           UnknownData01[0x4];                            // 0x02AC (0x0004) MISSED OFFSET
+# 	class ATeamInfo*                                   Team;                                          // 0x02B0 (0x0008) [0x0000000104000020] (CPF_Net | CPF_EditInline)
+# 	uint32_t                                           bAdmin : 1;                                    // 0x02B8 (0x0004) [0x0000000000000020] [0x00000001] (CPF_Net)
+# 	uint32_t                                           bIsSpectator : 1;                              // 0x02B8 (0x0004) [0x0000000100000020] [0x00000002] (CPF_Net)
+# 	uint32_t                                           bOnlySpectator : 1;                            // 0x02B8 (0x0004) [0x0000000000000020] [0x00000004] (CPF_Net)
+# 	uint32_t                                           bWaitingPlayer : 1;                            // 0x02B8 (0x0004) [0x0000000000000020] [0x00000008] (CPF_Net)
+# 	uint32_t                                           bReadyToPlay : 1;                              // 0x02B8 (0x0004) [0x0000000000000020] [0x00000010] (CPF_Net)
+# 	uint32_t                                           bOutOfLives : 1;                               // 0x02B8 (0x0004) [0x0000000000000020] [0x00000020] (CPF_Net)
+# 	uint32_t                                           bBot : 1;                                      // 0x02B8 (0x0004) [0x0000000000000020] [0x00000040] (CPF_Net)
+# 	uint32_t                                           bIsInactive : 1;                               // 0x02B8 (0x0004) [0x0000000100000020] [0x00000080] (CPF_Net)
+# 	uint32_t                                           bFromPreviousLevel : 1;                        // 0x02B8 (0x0004) [0x0000000000000020] [0x00000100] (CPF_Net)
+# 	uint32_t                                           bTimedOut : 1;                                 // 0x02B8 (0x0004) [0x0000000000000020] [0x00000200] (CPF_Net)
+# 	uint32_t                                           bUnregistered : 1;                             // 0x02B8 (0x0004) [0x0000000000002000] [0x00000400] (CPF_Transient)
+# 	int32_t                                            StartTime;                                     // 0x02BC (0x0004) [0x0000000000000000]               
+# 	class FString                                      StringSpectating;                              // 0x02C0 (0x0010) [0x0000000000408002] (CPF_Const | CPF_Localized | CPF_NeedCtorLink)
+# 	class FString                                      StringUnknown;                                 // 0x02D0 (0x0010) [0x0000000000408002] (CPF_Const | CPF_Localized | CPF_NeedCtorLink)
+# 	int32_t                                            Kills;                                         // 0x02E0 (0x0004) [0x0000000000000000]               
+# 	float                                              ExactPing;                                     // 0x02E4 (0x0004) [0x0000000000000000]               
+# 	class FString                                      SavedNetworkAddress;                           // 0x02E8 (0x0010) [0x0000000000400000] (CPF_NeedCtorLink)
+
+
 class PlayerReplicationInfo(Pointer):
     size = 0x0410
 
     def get_player_name(self):
         player_name_address = self.address + 0x0288
         return FString(player_name_address, sdk=self.sdk).get_string()
     
@@ -352,14 +392,47 @@
 
     def get_ping(self):
         bytes = self.sdk.pm.read_bytes(self.address +  0x0280, 1)
         return int.from_bytes(bytes, byteorder='little')
     
     def get_player_id(self):
         return self.sdk.pm.read_int(self.address + 0x02A8)
+    
+    def is_admin(self):
+        return (self.sdk.pm.read_int(self.address + 0x02B8) >> 0) & 1
+    
+    def is_specator(self):
+        return (self.sdk.pm.read_int(self.address + 0x02B8) >> 1) & 1
+    
+    def is_only_spectator(self):
+        return (self.sdk.pm.read_int(self.address + 0x02B8) >> 2) & 1
+    
+    def is_waiting_player(self):
+        return (self.sdk.pm.read_int(self.address + 0x02B8) >> 3) & 1
+    
+    def is_ready_to_play(self):
+        return (self.sdk.pm.read_int(self.address + 0x02B8) >> 4) & 1
+    
+    def is_out_of_lives(self):
+        return (self.sdk.pm.read_int(self.address + 0x02B8) >> 5) & 1
+    
+    def is_bot(self):
+        return (self.sdk.pm.read_int(self.address + 0x02B8) >> 6) & 1
+    
+    def is_inactive(self):
+        return (self.sdk.pm.read_int(self.address + 0x02B8) >> 7) & 1
+    
+    def is_from_previous_level(self):
+        return (self.sdk.pm.read_int(self.address + 0x02B8) >> 8) & 1
+    
+    def is_timed_out(self):
+        return (self.sdk.pm.read_int(self.address + 0x02B8) >> 9) & 1
+    
+    def is_unregistered(self):
+        return (self.sdk.pm.read_int(self.address + 0x02B8) >> 10) & 1
 
 class PRI(PlayerReplicationInfo):
     size = 0x0BD0
 
     def get_car(self):
         car_address = self.sdk.pm.read_ulonglong(self.address + 0x0490)
         return Car(car_address, sdk=self.sdk)
```

### Comparing `rlsdk_python-0.1.1/rlsdk_python/sdk.py` & `rlsdk_python-0.2.1/rlsdk_python/sdk.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pymem
-
+import pymem.pattern
 import ctypes
 import frida
 import time
 import threading
 from typing import Callable, Any, Protocol
 from .event_handling import Event
 from .events import EventFunctionHooked, EventBoostPadChanged, EventTypes, EventPlayerTick, EventRoundActiveStateChanged, EventResetPickups, EventGameEventStarted, EventKeyPressed, EventGameEventDestroyed
@@ -45,26 +45,42 @@
 
 
 
 
 class RLSDK:
 
     def __init__(self, hook_player_tick=False):
-
+      
         try:
             self.pm = pymem.Pymem(PROCESS_NAME)
             self.frida = frida.attach(PROCESS_NAME)
         except:
             raise Exception("Process not found")
+        
+        
+        print("Finding GNames offset...")
+        try:
+            self.g_names_offset = self.resolve_gnames_offset()
+        except:
+            raise Exception("GNames offset not found")
 
-        self.event = Event()
+
+        print("GNames offset: " + hex(self.g_names_offset))
+        
+        print("Finding GObjects offset...")
+        
+        try:
+            self.g_object_offset = self.resolve_gobjects_offset()
+        except:
+            raise Exception("GObjects offset not found")
         
-        self.g_names_offset = 0x242B630
-        self.g_object_offset = 0x242B678
+        print("GObjects offset: " + hex(self.g_object_offset))
 
+        self.event = Event()
+ 
         self.address_indexed_gnames = {}
         self.name_indexed_gnames = {}
         self.index_indexed_gnames = {}
 
         self.static_classes = {}
         self.static_functions = {}
 
@@ -111,16 +127,61 @@
         
         print("RLSDK initialized")
 
         self.event.subscribe(EventTypes.ON_HOOKED_FUNCTION, self.on_function_hooked)
 
         self.field = Field(self)
       
- 
+    
+    
+    def resolve_gobjects_offset(self):
+        # Pattern recherché
+        pattern = rb'\xE8....\x8B\x5D\xAF'
+        
+        # Trouver l'adresse de base du pattern
+        base_address = self.pm.pattern_scan_all(pattern, return_multiple=False)
+        if base_address is None:
+            return None
+
+        # Calcul des différents offsets pour atteindre l'adresse finale
+        # Lire l'offset relatif à partir de l'adresse de base + 1 et ajouter à base_address
+        relative_offset = self.pm.read_int(base_address + 1)
+        intermediate_address = base_address + 1 + relative_offset + 4  # +4 pour la taille de l'int lu
+
+        # Lire l'offset relatif à partir du nouvel emplacement + 0x65 et ajouter à l'adresse intermédiaire
+        final_relative_offset = self.pm.read_int(intermediate_address + 0x65 + 3)
+        final_address = intermediate_address + 0x65 + 3 + final_relative_offset + 4  # +4 pour la taille de l'int lu
+        
+        if not final_address:
+            raise Exception("GObjects offset not found")
+
+        return final_address - self.pm.base_address
+
+    def resolve_gnames_offset(self):
+        # Pattern recherché
+        pattern = rb'\x75.\xE8....\x48\xC7\xC7'
+        
+        # Trouver l'adresse de base du pattern
+        base_address = self.pm.pattern_scan_all(pattern, return_multiple=False)
+        if base_address is None:
+            return None
+
+        # Calcul des différents offsets pour atteindre l'adresse finale
+        # Lire l'offset relatif à partir de l'adresse de base + 3 et ajouter à base_address
+        relative_offset = self.pm.read_int(base_address + 3)
+        intermediate_address = base_address + 3 + relative_offset + 4  # +4 pour la taille de l'int lu
+
+        # Lire l'offset relatif à partir du nouvel emplacement + 0x2F et ajouter à l'adresse intermédiaire
+        final_relative_offset = self.pm.read_int(intermediate_address + 0x2F + 3)
+        final_address = intermediate_address + 0x2F + 3 + final_relative_offset + 4  # +4 pour la taille de l'int lu
+        
+        if not final_address:
+            raise Exception("GNames offset not found")
 
+        return final_address - self.pm.base_address
 
     def scan_functions(self, duration=10):
         print("Scanning functions...")
         
         self.scan_response_received_event.clear()
         self.frida_script.post({"type": "scan_functions", "duration": duration})
         received = self.scan_response_received_event.wait(duration + 10)
```

### Comparing `rlsdk_python-0.1.1/PKG-INFO` & `rlsdk_python-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlsdk_python
-Version: 0.1.1
+Version: 0.2.1
 Summary: 
 Author: MarlburroW
 Author-email: nik0o@hotmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

