# Comparing `tmp/opencast-camera-control-0.1.0.tar.gz` & `tmp/opencast-camera-control-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencast-camera-control-0.1.0.tar", last modified: Tue Mar 26 07:45:34 2024, max compression
+gzip compressed data, was "opencast-camera-control-0.3.0.tar", last modified: Tue Apr 23 17:06:15 2024, max compression
```

## Comparing `opencast-camera-control-0.1.0.tar` & `opencast-camera-control-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2024-03-26 07:45:34.322811 opencast-camera-control-0.1.0/
--rw-r--r--   0 lars      (1000) lars      (1000)    35149 2024-01-22 11:54:36.000000 opencast-camera-control-0.1.0/LICENSE
--rw-r--r--   0 lars      (1000) lars      (1000)    44014 2024-03-26 07:45:34.322811 opencast-camera-control-0.1.0/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)     3028 2024-03-26 07:44:21.000000 opencast-camera-control-0.1.0/README.md
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2024-03-26 07:45:34.321811 opencast-camera-control-0.1.0/occameracontrol/
--rw-r--r--   0 lars      (1000) lars      (1000)     3500 2024-02-11 13:50:53.000000 opencast-camera-control-0.1.0/occameracontrol/__main__.py
--rw-r--r--   0 lars      (1000) lars      (1000)     4163 2024-02-28 22:23:58.000000 opencast-camera-control-0.1.0/occameracontrol/agent.py
--rw-r--r--   0 lars      (1000) lars      (1000)     4688 2024-02-11 13:48:49.000000 opencast-camera-control-0.1.0/occameracontrol/camera.py
--rw-r--r--   0 lars      (1000) lars      (1000)     3939 2024-02-11 15:29:59.000000 opencast-camera-control-0.1.0/occameracontrol/metrics.py
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2024-03-26 07:45:34.321811 opencast-camera-control-0.1.0/opencast_camera_control.egg-info/
--rw-r--r--   0 lars      (1000) lars      (1000)    44014 2024-03-26 07:45:34.000000 opencast-camera-control-0.1.0/opencast_camera_control.egg-info/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)      431 2024-03-26 07:45:34.000000 opencast-camera-control-0.1.0/opencast_camera_control.egg-info/SOURCES.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        1 2024-03-26 07:45:34.000000 opencast-camera-control-0.1.0/opencast_camera_control.egg-info/dependency_links.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       74 2024-03-26 07:45:34.000000 opencast-camera-control-0.1.0/opencast_camera_control.egg-info/entry_points.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       60 2024-03-26 07:45:34.000000 opencast-camera-control-0.1.0/opencast_camera_control.egg-info/requires.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       16 2024-03-26 07:45:34.000000 opencast-camera-control-0.1.0/opencast_camera_control.egg-info/top_level.txt
--rw-r--r--   0 lars      (1000) lars      (1000)      784 2024-02-28 22:23:58.000000 opencast-camera-control-0.1.0/pyproject.toml
--rw-r--r--   0 lars      (1000) lars      (1000)       38 2024-03-26 07:45:34.322811 opencast-camera-control-0.1.0/setup.cfg
--rw-r--r--   0 lars      (1000) lars      (1000)       38 2024-02-28 22:23:58.000000 opencast-camera-control-0.1.0/setup.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2024-04-23 17:06:15.652330 opencast-camera-control-0.3.0/
+-rw-r--r--   0 lars      (1000) lars      (1000)    35149 2024-03-26 17:05:42.000000 opencast-camera-control-0.3.0/LICENSE
+-rw-r--r--   0 lars      (1000) lars      (1000)    45509 2024-04-23 17:06:15.652330 opencast-camera-control-0.3.0/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)     4523 2024-04-23 16:57:55.000000 opencast-camera-control-0.3.0/README.md
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2024-04-23 17:06:15.650330 opencast-camera-control-0.3.0/occameracontrol/
+-rw-r--r--   0 lars      (1000) lars      (1000)     3657 2024-04-23 16:28:47.000000 opencast-camera-control-0.3.0/occameracontrol/__main__.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     4991 2024-04-23 16:28:47.000000 opencast-camera-control-0.3.0/occameracontrol/agent.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     5696 2024-04-23 16:28:47.000000 opencast-camera-control-0.3.0/occameracontrol/camera.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     4734 2024-04-23 16:28:42.000000 opencast-camera-control-0.3.0/occameracontrol/metrics.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2024-04-23 17:06:15.651330 opencast-camera-control-0.3.0/opencast_camera_control.egg-info/
+-rw-r--r--   0 lars      (1000) lars      (1000)    45509 2024-04-23 17:06:15.000000 opencast-camera-control-0.3.0/opencast_camera_control.egg-info/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)      431 2024-04-23 17:06:15.000000 opencast-camera-control-0.3.0/opencast_camera_control.egg-info/SOURCES.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        1 2024-04-23 17:06:15.000000 opencast-camera-control-0.3.0/opencast_camera_control.egg-info/dependency_links.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       74 2024-04-23 17:06:15.000000 opencast-camera-control-0.3.0/opencast_camera_control.egg-info/entry_points.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       60 2024-04-23 17:06:15.000000 opencast-camera-control-0.3.0/opencast_camera_control.egg-info/requires.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       16 2024-04-23 17:06:15.000000 opencast-camera-control-0.3.0/opencast_camera_control.egg-info/top_level.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)      834 2024-04-23 17:06:11.000000 opencast-camera-control-0.3.0/pyproject.toml
+-rw-r--r--   0 lars      (1000) lars      (1000)       38 2024-04-23 17:06:15.652330 opencast-camera-control-0.3.0/setup.cfg
+-rw-r--r--   0 lars      (1000) lars      (1000)       38 2024-03-26 17:05:42.000000 opencast-camera-control-0.3.0/setup.py
```

### Comparing `opencast-camera-control-0.1.0/LICENSE` & `opencast-camera-control-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opencast-camera-control-0.1.0/PKG-INFO` & `opencast-camera-control-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencast-camera-control
-Version: 0.1.0
+Version: 0.3.0
 Summary: Automated Camera Control for Opencast
 Author-email: Lars Kiesow <lkiesow@uos.de>, Jan-Matthis Niermann <janiermann@uos.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -684,46 +684,114 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Opencast Camera Control
 
 Control PTZ camera to move to certain presets when starting a scheduled recording.
 
-This tool communicated with [Opencast](https://opencast.org) to get scheduled
-evens for a list of configured capture agents. When an event starts, cameras
+This tool communicates with [Opencast](https://opencast.org) to get scheduled
+events for a list of configured capture agents. When an event starts, cameras
 configured to be part of the agent's setup are then automatically turned to an
 active position specified by a configurable camera preset. When the event ends,
 the camera is turned back to a neutral position.
 
 This allows you, for example, to automatically turn cameras to the wall when no
 recordings are active.
 
 https://github.com/virtUOS/opencast-camera-control/assets/1008395/a8e37229-f760-4a54-82b2-1a555c960736
 
 <small><i>(Camera moves when a one minute scheduled recording starts and returns to point at the wall at the end)</i></small>
 
-## Getting started
+## Installation
 
+### PIP
+
+We release Opencast Camera Control via [the Python Package Index](https://pypi.org/).
+This means you can easily install the tool via pip:
+
+```
+❯ pip install opencast-camera-control
+❯ opencast-camera-control
+```
+
+
+### RPM Repository
+
+On RHEL 9 like distributions (CentOS Stream, Rocky, Alma, …) you can use the RPM repository to install Opencast Camera Control.
+Install the repository by adding a file `/etc/yum.repos.d/opencast-camera-control.repo`:
+
+```ini
+[opencast-camera-control]
+name = Opencast camera control el$releasever repository
+baseurl  = https://raw.githubusercontent.com/virtUOS/opencast-camera-control/rpm-el$releasever/
+enabled  = 1
+gpgcheck = 1
+gpgkey = https://raw.githubusercontent.com/virtUOS/opencast-camera-control/rpm-el$releasever/opencast-camera-control.key
+```
+
+Then activate the EPEL repository and install `opencast-camera-control`:
+
+```
+❯ dnf install -y epel-release
+❯ dnf install -y opencast-camera-control
 ```
-❯ pip install -r requirements.txt
-❯ python -m occameracontrol
+
+The RPM packages provide a Systemd unit to run the tool as service:
+
+```
+❯ systemctl start opencast-camera-control.service
+❯ systemctl enable opencast-camera-control.service
+```
+
+
+## Container
+
+We also provide a container image.
+A simple docker compose example would look like this
+
+```yaml
+---
+services:
+  camera-control:
+    image: ghcr.io/virtuos/opencast-camera-control:0.3.0
+    container_name: opencast-camera-control
+    ports:
+      - '8000:8000'
+    volumes:
+      - './your_config.yml:/etc/camera-control.yml'
 ```
 
 
 ## Configuration
 
 Take a look at the [camera-control.yml](camera-control.yml) configuration file.
 All available options are documented in there.
 
+The tool uses the first configuration it can find. It looks for files in the following order:
+
+- `./camera-control.yml`
+- `~/camera-control.yml`
+- `/etc/camera-control.yml`
+
 You can provide custom configuration files using the `--config` option:
 
 ```
-❯ python -m occameracontrol --config custom-config.yml
+❯ opencast-camera-control --config custom-config.yml
 ```
 
+## Supported Cameras
+
+The tool supports PTZ cameras from Panasonic and Sony.
+The following cameras have been confirmed to be working:
+
+- Panasonic AW-UE50
+- Panasonic AW-UE70
+- Sony SRG-300SE
+- Sony SRG-X120
+
 ## Opencast User
 
 To improve security, you can limit the access rights for the Opencast user by
 creating a user which has only the role `ROLE_CAPTURE_AGENT` assigned.
 
 ## Metrics
 
@@ -747,24 +815,7 @@
 # HELP agent_calendar_update_time Time of the last calendar update
 # TYPE agent_calendar_update_time gauge
 agent_calendar_update_time{agent="test_agent"} 1.707571943100096e+09
 # HELP camera_position Last position (preset number) a camera moved to
 # TYPE camera_position gauge
 camera_position{camera="http://camera-2-panasonic.example.com"} 10.0
 ```
-
-## Docker
-
-We also provide a container image.
-A simple docker compose example would look like this
-
-```yaml
----
-version: '3'
-services:
-  app:
-    image: ghcr.io/virtuos/opencast-camera-control:main
-    ports:
-      - '8000:8000'
-    volumes:
-      - './your_config.yml:/etc/camera-control.yml'
-```
```

### Comparing `opencast-camera-control-0.1.0/occameracontrol/__main__.py` & `opencast-camera-control-0.3.0/occameracontrol/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import argparse
 import logging
+import sys
 import time
 
 from confygure import setup, config_t, config_rt
 from threading import Thread
 
 from occameracontrol.agent import Agent
 from occameracontrol.camera import Camera
@@ -73,36 +74,40 @@
             './camera-control.yml',
             '~/camera-control.yml',
             '/etc/camera-control.yml']
     if args.config:
         config_files = [args.config]
 
     setup(files=config_files, logger=['loglevel'])
+    if not config_t(dict):
+        print('Could not find a configuration file in', config_files)
+        sys.exit(1)
 
     cameras = []
     agents = []
     for agent_id, agent_cameras in config_rt(dict, 'camera').items():
         agent = Agent(agent_id)
+        agent.verify_agent()
         agents.append(agent)
         logger.debug('Configuring agent %s', agent_id)
         for camera in agent_cameras:
             cam = Camera(agent, **camera)
             logger.debug('Configuring camera: %s', cam)
             cameras.append(cam)
 
     threads = []
     agent_update = Thread(target=update_agents, args=(agents,))
     threads.append(agent_update)
     agent_update.start()
 
     for camera in cameras:
         logger.info('Starting camera control for %s', camera)
-        control_truead = Thread(target=control_camera, args=(camera,))
-        threads.append(control_truead)
-        control_truead.start()
+        control_thread = Thread(target=control_camera, args=(camera,))
+        threads.append(control_thread)
+        control_thread.start()
 
     # Start delivering metrics
     start_metrics_exporter()
 
     try:
         for thread in threads:
             thread.join()
```

### Comparing `opencast-camera-control-0.1.0/occameracontrol/agent.py` & `opencast-camera-control-0.3.0/occameracontrol/agent.py`

 * *Files 20% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
 
 class Agent:
     '''A capture agent with it's name and calendar
     '''
     agent_id: str
     events: list[Event] = []
+    calendar_initialized: bool = False
 
     def __init__(self, agent_id: str):
         self.agent_id = agent_id
 
     def cutoff(self) -> int:
         '''Returns the calendar cutoff time in milliseconds.
         '''
@@ -104,14 +105,15 @@
         response.raise_for_status()
 
         calendar = response.json()
         logger.debug('Calendar data: %s', calendar)
 
         self.events = self.parse_calendar(calendar)
         register_calendar_update(self.agent_id)
+        self.calendar_initialized = True
 
     def active_events(self):
         '''Return a list of active events
         '''
         # Remove old events from cached events
         now = time.time()
         return [e for e in self.events if e.end >= now]
@@ -121,7 +123,26 @@
         If no future events are scheduled for this agent, and empty event with
         start and end set to 0 will be returned.
         '''
         events = self.active_events()
         if not events:
             return Event('', 0, 0)
         return events[0]
+
+    def verify_agent(self):
+        '''Verify that an agent exists when it is created
+        '''
+        server = config_rt(str, 'opencast', 'server').rstrip('/')
+        username = config_rt(str, 'opencast', 'username')
+        password = config_rt(str, 'opencast', 'password')
+        auth = (username, password)
+        url = f'{server}/capture-admin/agents/{self.agent_id}.json'
+        logger.info('Verification of agent `%s`', self.agent_id)
+
+        response = requests.get(url, auth=auth, timeout=5)
+        try:
+            response.raise_for_status()
+        except Exception:
+            raise LookupError(
+                f'Agent {self.agent_id} does not exist in Opencast.')
+
+        logger.debug(f'Agent {self.agent_id} verified.')
```

### Comparing `opencast-camera-control-0.1.0/occameracontrol/camera.py` & `opencast-camera-control-0.3.0/occameracontrol/camera.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+import datetime
 import logging
 import requests
 import time
 
+from confygure import config_t
 from enum import Enum
 from requests.auth import HTTPDigestAuth
 from typing import Optional
 
 from occameracontrol.agent import Agent
 from occameracontrol.metrics import register_camera_move
 
@@ -43,14 +45,16 @@
     password: Optional[str] = None
     position: int = -1
     type: CameraType
     url: str
     user: Optional[str] = None
     preset_active: int = 1
     preset_inactive: int = 10
+    last_updated: float = 0.0
+    update_frequency: int = 300
 
     def __init__(self,
                  agent: Agent,
                  url: str,
                  type: str,
                  user: Optional[str] = None,
                  password: Optional[str] = None,
@@ -59,14 +63,15 @@
         self.agent = agent
         self.url = url.rstrip('/')
         self.type = CameraType[type]
         self.user = user
         self.password = password
         self.preset_active = preset_active
         self.preset_inactive = preset_inactive
+        self.update_frequency = config_t(int, 'camera_update_frequency') or 300
 
     def __str__(self) -> str:
         '''Returns a string representation of this camera
         '''
         return f"'{self.agent.agent_id}' @ '{self.url}'"
 
     def move_to_preset(self, preset: int):
@@ -79,51 +84,69 @@
                 if self.user and self.password else None
             logger.debug('GET %s with params: %s', url, params)
             response = requests.get(url, auth=auth, params=params, timeout=5)
             response.raise_for_status()
 
         elif self.type == CameraType.sony:
             url = f'{self.url}/command/presetposition.cgi'
-            params = {'PresetCall': preset}
+            params = {'PresetCall': f'{preset},24'}
             headers = {'referer': f'{self.url}/'}
             auth = HTTPDigestAuth(self.user, self.password) \
                 if self.user and self.password else None
             logger.debug('GET %s with params: %s', url, params)
             response = requests.get(url,
                                     auth=auth,
                                     headers=headers,
                                     params=params,
                                     timeout=5)
             response.raise_for_status()
 
         self.position = preset
         register_camera_move(self.url, preset)
+        self.last_updated = time.time()
+
+    def from_now(self, ts: float) -> str:
+        '''Get a string representation of the time until the provided time
+        stamp is reached.
+        '''
+        seconds = int(ts - time.time())  # seconds are enough accuracy
+        return str(datetime.timedelta(seconds=seconds))
 
     def update_position(self):
         '''Check for currently active events with the camera's capture agent
         and move the camera to the appropriate (active, inactive) position if
         necessary.
         '''
         agent_id = self.agent.agent_id
+        level = logging.DEBUG if int(time.time()) % 60 else logging.INFO
+
+        while not self.agent.calendar_initialized:
+            logger.log(level, '[%s] Calendar not yet initialized…', agent_id)
+            time.sleep(1)
+
         event = self.agent.next_event()
 
         if event.future():
-            logger.info('[%s] Next event `%s` starts in %i seconds',
-                        agent_id, event.title, event.start - time.time())
+            logger.log(level, '[%s] Next event `%s` starts in %s',
+                       agent_id, event.title[:40], self.from_now(event.start))
         elif event.active():
-            logger.info('[%s] Active event `%s` ends in %i seconds',
-                        agent_id, event.title, event.end - time.time())
+            logger.log(level, '[%s] Active event `%s` ends in %s',
+                       agent_id, event.title[:40], self.from_now(event.end))
         else:
-            logger.info('[%s] No planned events', agent_id)
+            logger.log(level, '[%s] No planned events', agent_id)
 
-        if event.active():
+        if event.active():  # active event
             if self.position != self.preset_active:
                 logger.info('[%s] Event `%s` started', agent_id, event.title)
                 logger.info('[%s] Moving to preset %i', agent_id,
                             self.preset_active)
                 self.move_to_preset(self.preset_active)
-
         else:  # No active event
             if self.position != self.preset_inactive:
                 logger.info('[%s] Returning to preset %i', agent_id,
                             self.preset_inactive)
                 self.move_to_preset(self.preset_inactive)
+
+        if time.time() - self.last_updated >= self.update_frequency:
+            logger.info('[%s] Re-sending preset %i to camera', agent_id,
+                        self.position)
+            self.move_to_preset(self.position)
```

### Comparing `opencast-camera-control-0.1.0/opencast_camera_control.egg-info/PKG-INFO` & `opencast-camera-control-0.3.0/opencast_camera_control.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencast-camera-control
-Version: 0.1.0
+Version: 0.3.0
 Summary: Automated Camera Control for Opencast
 Author-email: Lars Kiesow <lkiesow@uos.de>, Jan-Matthis Niermann <janiermann@uos.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -684,46 +684,114 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Opencast Camera Control
 
 Control PTZ camera to move to certain presets when starting a scheduled recording.
 
-This tool communicated with [Opencast](https://opencast.org) to get scheduled
-evens for a list of configured capture agents. When an event starts, cameras
+This tool communicates with [Opencast](https://opencast.org) to get scheduled
+events for a list of configured capture agents. When an event starts, cameras
 configured to be part of the agent's setup are then automatically turned to an
 active position specified by a configurable camera preset. When the event ends,
 the camera is turned back to a neutral position.
 
 This allows you, for example, to automatically turn cameras to the wall when no
 recordings are active.
 
 https://github.com/virtUOS/opencast-camera-control/assets/1008395/a8e37229-f760-4a54-82b2-1a555c960736
 
 <small><i>(Camera moves when a one minute scheduled recording starts and returns to point at the wall at the end)</i></small>
 
-## Getting started
+## Installation
 
+### PIP
+
+We release Opencast Camera Control via [the Python Package Index](https://pypi.org/).
+This means you can easily install the tool via pip:
+
+```
+❯ pip install opencast-camera-control
+❯ opencast-camera-control
+```
+
+
+### RPM Repository
+
+On RHEL 9 like distributions (CentOS Stream, Rocky, Alma, …) you can use the RPM repository to install Opencast Camera Control.
+Install the repository by adding a file `/etc/yum.repos.d/opencast-camera-control.repo`:
+
+```ini
+[opencast-camera-control]
+name = Opencast camera control el$releasever repository
+baseurl  = https://raw.githubusercontent.com/virtUOS/opencast-camera-control/rpm-el$releasever/
+enabled  = 1
+gpgcheck = 1
+gpgkey = https://raw.githubusercontent.com/virtUOS/opencast-camera-control/rpm-el$releasever/opencast-camera-control.key
+```
+
+Then activate the EPEL repository and install `opencast-camera-control`:
+
+```
+❯ dnf install -y epel-release
+❯ dnf install -y opencast-camera-control
 ```
-❯ pip install -r requirements.txt
-❯ python -m occameracontrol
+
+The RPM packages provide a Systemd unit to run the tool as service:
+
+```
+❯ systemctl start opencast-camera-control.service
+❯ systemctl enable opencast-camera-control.service
+```
+
+
+## Container
+
+We also provide a container image.
+A simple docker compose example would look like this
+
+```yaml
+---
+services:
+  camera-control:
+    image: ghcr.io/virtuos/opencast-camera-control:0.3.0
+    container_name: opencast-camera-control
+    ports:
+      - '8000:8000'
+    volumes:
+      - './your_config.yml:/etc/camera-control.yml'
 ```
 
 
 ## Configuration
 
 Take a look at the [camera-control.yml](camera-control.yml) configuration file.
 All available options are documented in there.
 
+The tool uses the first configuration it can find. It looks for files in the following order:
+
+- `./camera-control.yml`
+- `~/camera-control.yml`
+- `/etc/camera-control.yml`
+
 You can provide custom configuration files using the `--config` option:
 
 ```
-❯ python -m occameracontrol --config custom-config.yml
+❯ opencast-camera-control --config custom-config.yml
 ```
 
+## Supported Cameras
+
+The tool supports PTZ cameras from Panasonic and Sony.
+The following cameras have been confirmed to be working:
+
+- Panasonic AW-UE50
+- Panasonic AW-UE70
+- Sony SRG-300SE
+- Sony SRG-X120
+
 ## Opencast User
 
 To improve security, you can limit the access rights for the Opencast user by
 creating a user which has only the role `ROLE_CAPTURE_AGENT` assigned.
 
 ## Metrics
 
@@ -747,24 +815,7 @@
 # HELP agent_calendar_update_time Time of the last calendar update
 # TYPE agent_calendar_update_time gauge
 agent_calendar_update_time{agent="test_agent"} 1.707571943100096e+09
 # HELP camera_position Last position (preset number) a camera moved to
 # TYPE camera_position gauge
 camera_position{camera="http://camera-2-panasonic.example.com"} 10.0
 ```
-
-## Docker
-
-We also provide a container image.
-A simple docker compose example would look like this
-
-```yaml
----
-version: '3'
-services:
-  app:
-    image: ghcr.io/virtuos/opencast-camera-control:main
-    ports:
-      - '8000:8000'
-    volumes:
-      - './your_config.yml:/etc/camera-control.yml'
-```
```

### Comparing `opencast-camera-control-0.1.0/pyproject.toml` & `opencast-camera-control-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools >= 61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'opencast-camera-control'
-version = '0.1.0'
+version = '0.3.0'
 authors = [
     {name = 'Lars Kiesow', email = 'lkiesow@uos.de'},
     {name = 'Jan-Matthis Niermann', email = 'janiermann@uos.de'}
 ]
 description = 'Automated Camera Control for Opencast'
 readme = {file = 'README.md', content-type = 'text/markdown'}
 requires-python = ">=3.9"
@@ -22,7 +22,10 @@
 
 [project.urls]
 Homepage = 'https://github.com/virtUOS/opencast-camera-control'
 Repository = 'https://github.com/virtUOS/opencast-camera-control'
 
 [project.scripts]
 opencast-camera-control = 'occameracontrol.__main__:main'
+
+[tool.setuptools]
+packages = ['occameracontrol']
```

