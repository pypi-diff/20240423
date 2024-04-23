# Comparing `tmp/commonroad-reactive-planner-2023.1.tar.gz` & `tmp/commonroad_reactive_planner-2024.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/commonroad-reactive-planner-2023.1.tar", last modified: Wed Oct  4 08:57:30 2023, max compression
+gzip compressed data, was "commonroad_reactive_planner-2024.1.tar", max compression
```

## Comparing `commonroad-reactive-planner-2023.1.tar` & `commonroad_reactive_planner-2024.1.tar`

### file list

```diff
@@ -1,54 +1,18 @@
-drwxrwxr-x   0 gerald    (1000) gerald    (1000)        0 2023-10-04 08:57:30.000000 commonroad-reactive-planner-2023.1/
--rw-rw-r--   0 gerald    (1000) gerald    (1000)      168 2023-10-03 20:09:30.000000 commonroad-reactive-planner-2023.1/.gitignore
--rw-rw-r--   0 gerald    (1000) gerald    (1000)     1570 2023-10-03 20:09:30.000000 commonroad-reactive-planner-2023.1/LICENSE
--rw-rw-r--   0 gerald    (1000) gerald    (1000)     2879 2023-10-04 08:57:30.000000 commonroad-reactive-planner-2023.1/PKG-INFO
--rwxrwxr-x   0 gerald    (1000) gerald    (1000)     2193 2023-10-04 08:15:48.000000 commonroad-reactive-planner-2023.1/README.md
-drwxrwxr-x   0 gerald    (1000) gerald    (1000)        0 2023-10-04 08:57:30.000000 commonroad-reactive-planner-2023.1/commonroad_reactive_planner.egg-info/
--rw-rw-r--   0 gerald    (1000) gerald    (1000)     2879 2023-10-04 08:57:29.000000 commonroad-reactive-planner-2023.1/commonroad_reactive_planner.egg-info/PKG-INFO
--rw-rw-r--   0 gerald    (1000) gerald    (1000)     1296 2023-10-04 08:57:29.000000 commonroad-reactive-planner-2023.1/commonroad_reactive_planner.egg-info/SOURCES.txt
--rw-rw-r--   0 gerald    (1000) gerald    (1000)        1 2023-10-04 08:57:29.000000 commonroad-reactive-planner-2023.1/commonroad_reactive_planner.egg-info/dependency_links.txt
--rw-rw-r--   0 gerald    (1000) gerald    (1000)        1 2023-10-04 08:48:19.000000 commonroad-reactive-planner-2023.1/commonroad_reactive_planner.egg-info/not-zip-safe
--rw-rw-r--   0 gerald    (1000) gerald    (1000)      227 2023-10-04 08:57:29.000000 commonroad-reactive-planner-2023.1/commonroad_reactive_planner.egg-info/requires.txt
--rw-rw-r--   0 gerald    (1000) gerald    (1000)       14 2023-10-04 08:57:29.000000 commonroad-reactive-planner-2023.1/commonroad_reactive_planner.egg-info/top_level.txt
-drwxrwxr-x   0 gerald    (1000) gerald    (1000)        0 2023-10-04 08:57:30.000000 commonroad-reactive-planner-2023.1/commonroad_rp/
--rw-r--r--   0 gerald    (1000) gerald    (1000)        0 2020-12-21 10:16:39.000000 commonroad-reactive-planner-2023.1/commonroad_rp/__init__.py
--rw-rw-r--   0 gerald    (1000) gerald    (1000)     3209 2023-06-22 13:43:48.000000 commonroad-reactive-planner-2023.1/commonroad_rp/cost_function.py
--rwxrwxr-x   0 gerald    (1000) gerald    (1000)    13196 2023-10-03 20:09:30.000000 commonroad-reactive-planner-2023.1/commonroad_rp/polynomial_trajectory.py
--rwxrwxr-x   0 gerald    (1000) gerald    (1000)    57089 2023-07-19 11:52:18.000000 commonroad-reactive-planner-2023.1/commonroad_rp/reactive_planner.py
--rwxrwxr-x   0 gerald    (1000) gerald    (1000)    18633 2023-07-19 11:50:15.000000 commonroad-reactive-planner-2023.1/commonroad_rp/sampling.py
--rw-rw-r--   0 gerald    (1000) gerald    (1000)     3115 2023-05-10 13:02:01.000000 commonroad-reactive-planner-2023.1/commonroad_rp/state.py
--rwxrwxr-x   0 gerald    (1000) gerald    (1000)    17214 2023-10-03 20:09:30.000000 commonroad-reactive-planner-2023.1/commonroad_rp/trajectories.py
-drwxrwxr-x   0 gerald    (1000) gerald    (1000)        0 2023-10-04 08:57:30.000000 commonroad-reactive-planner-2023.1/commonroad_rp/utility/
--rw-rw-r--   0 gerald    (1000) gerald    (1000)        0 2022-05-10 21:12:04.000000 commonroad-reactive-planner-2023.1/commonroad_rp/utility/__init__.py
--rw-rw-r--   0 gerald    (1000) gerald    (1000)    11902 2023-08-02 15:53:54.000000 commonroad-reactive-planner-2023.1/commonroad_rp/utility/config.py
--rw-rw-r--   0 gerald    (1000) gerald    (1000)    14783 2023-07-19 11:50:15.000000 commonroad-reactive-planner-2023.1/commonroad_rp/utility/evaluation.py
--rw-rw-r--   0 gerald    (1000) gerald    (1000)     1984 2023-05-10 13:02:01.000000 commonroad-reactive-planner-2023.1/commonroad_rp/utility/general.py
--rw-rw-r--   0 gerald    (1000) gerald    (1000)     1626 2023-07-19 11:50:15.000000 commonroad-reactive-planner-2023.1/commonroad_rp/utility/logger.py
--rw-rw-r--   0 gerald    (1000) gerald    (1000)     8165 2023-10-03 20:09:30.000000 commonroad-reactive-planner-2023.1/commonroad_rp/utility/utils_coordinate_system.py
--rw-rw-r--   0 gerald    (1000) gerald    (1000)    10645 2023-07-19 11:50:15.000000 commonroad-reactive-planner-2023.1/commonroad_rp/utility/visualization.py
-drwxrwxr-x   0 gerald    (1000) gerald    (1000)        0 2023-10-04 08:57:30.000000 commonroad-reactive-planner-2023.1/configurations/
--rw-rw-r--   0 gerald    (1000) gerald    (1000)      372 2023-10-03 16:04:40.000000 commonroad-reactive-planner-2023.1/configurations/DEU_Test-1_1_T-1.yaml
--rw-rw-r--   0 gerald    (1000) gerald    (1000)      353 2023-10-03 19:51:47.000000 commonroad-reactive-planner-2023.1/configurations/ZAM_Over-1_1.yaml
--rw-rw-r--   0 gerald    (1000) gerald    (1000)      380 2023-10-03 20:09:30.000000 commonroad-reactive-planner-2023.1/configurations/ZAM_Tjunction-1_42_T-1.yaml
-drwxrwxr-x   0 gerald    (1000) gerald    (1000)        0 2023-10-04 08:57:30.000000 commonroad-reactive-planner-2023.1/doc/
--rw-rw-r--   0 gerald    (1000) gerald    (1000)      638 2022-02-02 10:39:49.000000 commonroad-reactive-planner-2023.1/doc/Makefile
-drwxrwxr-x   0 gerald    (1000) gerald    (1000)        0 2023-10-04 08:57:30.000000 commonroad-reactive-planner-2023.1/doc/images/
--rw-rw-r--   0 gerald    (1000) gerald    (1000)  2772511 2023-10-04 08:15:48.000000 commonroad-reactive-planner-2023.1/doc/images/ZAM_Tjunction-1_42_T-1.gif
--rw-rw-r--   0 gerald    (1000) gerald    (1000)      799 2022-02-02 10:39:49.000000 commonroad-reactive-planner-2023.1/doc/make.bat
-drwxrwxr-x   0 gerald    (1000) gerald    (1000)        0 2023-10-04 08:57:30.000000 commonroad-reactive-planner-2023.1/doc/source/
-drwxrwxr-x   0 gerald    (1000) gerald    (1000)        0 2023-10-04 08:57:30.000000 commonroad-reactive-planner-2023.1/doc/source/api/
--rw-rw-r--   0 gerald    (1000) gerald    (1000)     4279 2022-05-19 14:31:41.000000 commonroad-reactive-planner-2023.1/doc/source/api/commonroad_rp.rst
--rw-rw-r--   0 gerald    (1000) gerald    (1000)      181 2022-02-02 10:39:49.000000 commonroad-reactive-planner-2023.1/doc/source/api/index.rst
--rw-rw-r--   0 gerald    (1000) gerald    (1000)     2857 2022-02-02 10:39:49.000000 commonroad-reactive-planner-2023.1/doc/source/conf.py
--rw-rw-r--   0 gerald    (1000) gerald    (1000)     2157 2022-05-19 14:39:03.000000 commonroad-reactive-planner-2023.1/doc/source/index.rst
-drwxrwxr-x   0 gerald    (1000) gerald    (1000)        0 2023-10-04 08:57:30.000000 commonroad-reactive-planner-2023.1/doc/source/user/
--rw-rw-r--   0 gerald    (1000) gerald    (1000)      122 2022-02-02 10:39:49.000000 commonroad-reactive-planner-2023.1/doc/source/user/index.rst
-drwxrwxr-x   0 gerald    (1000) gerald    (1000)        0 2023-10-04 08:57:30.000000 commonroad-reactive-planner-2023.1/example_scenarios/
--rw-rw-r--   0 gerald    (1000) gerald    (1000)    69849 2023-08-02 15:52:59.000000 commonroad-reactive-planner-2023.1/example_scenarios/DEU_Test-1_1_T-1.xml
--rw-rw-r--   0 gerald    (1000) gerald    (1000)   183125 2021-07-19 14:31:54.000000 commonroad-reactive-planner-2023.1/example_scenarios/ZAM-Ramp-1_1-T-1.xml
--rw-rw-r--   0 gerald    (1000) gerald    (1000)    73875 2023-08-02 16:06:24.000000 commonroad-reactive-planner-2023.1/example_scenarios/ZAM_Over-1_1.xml
--rw-rw-r--   0 gerald    (1000) gerald    (1000)   316651 2023-10-03 20:09:30.000000 commonroad-reactive-planner-2023.1/example_scenarios/ZAM_Tjunction-1_42_T-1.xml
--rw-rw-r--   0 gerald    (1000) gerald    (1000)      273 2023-10-03 20:09:30.000000 commonroad-reactive-planner-2023.1/requirements.txt
--rw-rw-r--   0 gerald    (1000) gerald    (1000)     4649 2023-10-03 20:09:30.000000 commonroad-reactive-planner-2023.1/run_planner.py
--rw-rw-r--   0 gerald    (1000) gerald    (1000)       38 2023-10-04 08:57:30.000000 commonroad-reactive-planner-2023.1/setup.cfg
--rw-rw-r--   0 gerald    (1000) gerald    (1000)     1449 2023-10-04 08:56:53.000000 commonroad-reactive-planner-2023.1/setup.py
+-rw-r--r--   0        0        0     1570 2023-11-15 15:23:48.783401 commonroad_reactive_planner-2024.1/LICENSE
+-rwxr-xr-x   0        0        0     2224 2024-04-23 12:49:17.941227 commonroad_reactive_planner-2024.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 13:40:26.804782 commonroad_reactive_planner-2024.1/commonroad_rp/__init__.py
+-rw-r--r--   0        0        0     3212 2024-04-23 08:56:37.329745 commonroad_reactive_planner-2024.1/commonroad_rp/cost_function.py
+-rwxr-xr-x   0        0        0    12838 2024-04-23 13:31:58.542873 commonroad_reactive_planner-2024.1/commonroad_rp/polynomial_trajectory.py
+-rwxr-xr-x   0        0        0    58114 2024-04-23 12:43:42.167941 commonroad_reactive_planner-2024.1/commonroad_rp/reactive_planner.py
+-rwxr-xr-x   0        0        0    18636 2024-04-23 08:56:37.333745 commonroad_reactive_planner-2024.1/commonroad_rp/sampling.py
+-rw-r--r--   0        0        0     3115 2023-11-15 15:23:48.783401 commonroad_reactive_planner-2024.1/commonroad_rp/state.py
+-rwxr-xr-x   0        0        0    17217 2024-04-23 08:56:37.333745 commonroad_reactive_planner-2024.1/commonroad_rp/trajectories.py
+-rw-r--r--   0        0        0        0 2024-04-23 13:40:26.808782 commonroad_reactive_planner-2024.1/commonroad_rp/utility/__init__.py
+-rw-r--r--   0        0        0    11554 2024-04-22 16:39:23.490076 commonroad_reactive_planner-2024.1/commonroad_rp/utility/config.py
+-rw-r--r--   0        0        0    14802 2024-04-23 08:56:37.333745 commonroad_reactive_planner-2024.1/commonroad_rp/utility/evaluation.py
+-rw-r--r--   0        0        0     2405 2024-04-22 16:39:23.490076 commonroad_reactive_planner-2024.1/commonroad_rp/utility/general.py
+-rw-r--r--   0        0        0     1626 2023-11-15 15:23:48.783401 commonroad_reactive_planner-2024.1/commonroad_rp/utility/logger.py
+-rw-r--r--   0        0        0     8244 2024-04-23 08:56:37.333745 commonroad_reactive_planner-2024.1/commonroad_rp/utility/utils_coordinate_system.py
+-rw-r--r--   0        0        0    11573 2024-04-23 12:43:42.167941 commonroad_reactive_planner-2024.1/commonroad_rp/utility/visualization.py
+-rw-r--r--   0        0        0     1482 2024-04-23 13:31:19.494725 commonroad_reactive_planner-2024.1/pyproject.toml
+-rw-r--r--   0        0        0     3615 1970-01-01 00:00:00.000000 commonroad_reactive_planner-2024.1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `commonroad-reactive-planner-2023.1/LICENSE` & `commonroad_reactive_planner-2024.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commonroad-reactive-planner-2023.1/PKG-INFO` & `commonroad_reactive_planner-2024.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,53 @@
-Metadata-Version: 2.1
-Name: commonroad-reactive-planner
-Version: 2023.1
-Summary: CommonRoad Reactive Planner: Sampling-based Frenet Planner
-Home-page: https://commonroad.in.tum.de/
-Author: Cyber-Physical Systems Group, Technical University of Munich
-Author-email: commonroad@lists.lrz.de
-License: BSD
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Reactive Planner
 
 This project generates solutions to trajectory planning problems given in the [CommonRoad](https://commonroad.in.tum.de/) scenario format.
 The trajectories are generated using the sampling-based approach in [1][2]. This approach plans motions by sampling a 
 discrete set of trajectories, represented as quintic polynomials in a Frenet frame and selecting an optimal trajectory according
 to a given cost function.
 
-<img src="doc/images/ZAM_Tjunction-1_42_T-1.gif" alt="reactive-planner" width="400"/>
+<img src="doc/images/ZAM_Tjunction-1_42_T-1.gif" alt="reactive-planner" width="600"/>
 
 
 ## Getting Started
 These instructions should help you to install the trajectory planner and use it for development and testing purposes.
 
-To install the trajectory planner from PyPi, please run:
+To install the package from PyPi, please run:
 ```shell
 pip install commonroad-reactive-planner
 ```
 
 ### Requirements
-The software is  developed and tested on recent versions of Linux. The required python dependencies are listed in `requirements.txt`.
+The software is  written in Python 3.8 and tested on Ubuntu 18.04-22.04. The required python dependencies are listed in `pyproject.toml`.
 
 For the python installation, we suggest the usage of [Anaconda](http://www.anaconda.com/download/#download).
 
 For the development IDE we suggest [PyCharm](http://www.jetbrains.com/pycharm/)
 
 
 ### Installation from Source
-1. Clone this repository & create a new conda environment, e.g.,  `conda create -n commonroad-py37 python=3.7`
+1. Clone this repository & create a new conda environment, e.g.,  `conda create -n commonroad-py38 python=3.8`
 
 
-2. Install the package:
+2. Go to cloned root directory and install the package:
+    * Install the package via poetry: `poetry install`
     * Install the package via pip: `pip install .`
-    * **Or** install the dependencies with `pip install -r requirements.txt` and add the root folder to the python path of your interpreter
 
 
 
 ### How to run
 
-Main example script `run_planner.py`: The example script shows how to run the planner on an exemplary 
-CommonRoad scenario. Therein, the following steps are included:
+**Main example script** `run_planner.py`: 
+
+The example script shows how to run the planner on an exemplary CommonRoad scenario with the following steps:
 * creating a planner configuration
 * instantiating the reactive planner
-* running the planner in planning cycles with a fixed re-planning frequency
+* running the planner in a cyclic replanning loop with a fixed replanning fequency
+
+In addition we also provide an interactive Jupyter notebook tutorial in the `tutorial/` folder.
 
 
 ## Literature
 [1] Werling M., et al. *Optimal trajectory generation for dynamic street scenarios in a frenet frame*. In: IEEE International Conference on Robotics and Automation, Anchorage, Alaska, 987–993.
 
 [2] Werling M., et al. *Optimal trajectories for time-critical street scenarios using discretized terminal manifolds* In:
 The International Journal of Robotics Research, 2012
```

### Comparing `commonroad-reactive-planner-2023.1/commonroad_rp/cost_function.py` & `commonroad_reactive_planner-2024.1/commonroad_rp/cost_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Gerald Würsching, Christian Pek"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["BMW Group CAR@TUM, interACT"]
-__version__ = "1.0"
+__version__ = "2024.1"
 __maintainer__ = "Gerald Würsching"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Beta"
 
 from abc import ABC, abstractmethod
 from typing import Optional
```

### Comparing `commonroad-reactive-planner-2023.1/commonroad_rp/reactive_planner.py` & `commonroad_reactive_planner-2024.1/commonroad_rp/reactive_planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Gerald Würsching, Christian Pek"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["BMW Group CAR@TUM, interACT"]
-__version__ = "1.0"
+__version__ = "2024.1"
 __maintainer__ = "Gerald Würsching"
 __email__ = "gerald.wuersching@tum.de"
 __status__ = "Beta"
 
 # python packages
 import math
 import time
@@ -17,15 +17,15 @@
 
 # commonroad-io
 from commonroad.common.validity import is_real_number
 from commonroad.geometry.shape import Rectangle
 from commonroad.prediction.prediction import TrajectoryPrediction
 from commonroad.scenario.obstacle import DynamicObstacle, ObstacleType
 from commonroad.scenario.trajectory import Trajectory
-from commonroad.scenario.state import CustomState, InputState
+from commonroad.scenario.state import CustomState, InputState, InitialState
 from commonroad.scenario.scenario import Scenario
 
 # commonroad_dc
 import commonroad_dc.pycrcc as pycrcc
 from commonroad_dc.boundary.boundary import create_road_boundary_obstacle
 from commonroad_dc.collision.collision_detection.pycrcc_collision_dispatch import create_collision_object
 from commonroad_dc.collision.trajectory_queries.trajectory_queries import trajectory_preprocess_obb_sum
@@ -90,15 +90,15 @@
         # desired speed
         self._desired_speed: Optional[float] = None
         self._desired_lon_position: Optional[float] = None
         # threshold for low velocity mode
         self._low_vel_mode = False
 
         # Debug setting: visualize trajectory set
-        self._draw_traj_set = config.debug.draw_traj_set and (config.debug.save_plots or config.debug.save_plots)
+        self._draw_traj_set = config.debug.draw_traj_set and (config.debug.show_plots or config.debug.save_plots)
 
         # set/reset configuration
         self.config: Optional[ReactivePlannerConfiguration] = None
         self.reset(config)
 
         # set sampling space
         self.sampling_space: Optional[Type[SamplingSpace]] = None
@@ -191,43 +191,45 @@
             # create new collision checker from updated scenario
             self.set_collision_checker(scenario=self.config.scenario)
         else:
             # use passed collision checker object
             self.set_collision_checker(collision_checker=collision_checker)
 
         # reset ref path and CoSys
-        if coordinate_system is None:
-            # create new CoSys from reference path
-            self.set_reference_path(reference_path=self.config.planning.reference_path)
-        else:
+        if coordinate_system is not None:
             # use passed CoSys object
             self.set_reference_path(coordinate_system=coordinate_system)
 
-        # if planner init state is empty: Convert cartesian initial state from planning problem
+        # if planner init state is empty
         if self.x_0 is None and initial_state_cart is None:
-            self.x_0 = ReactivePlannerState.create_from_initial_state(self.config.planning_problem.initial_state,
-                                                                      self.vehicle_params.wheelbase,
-                                                                      self.vehicle_params.wb_rear_axle)
+            if self.config.planning_problem:
+                # Get cartesian initial state from planning problem (if available)
+                self.x_0 = ReactivePlannerState.create_from_initial_state(self.config.planning_problem.initial_state,
+                                                                          self.vehicle_params.wheelbase,
+                                                                          self.vehicle_params.wb_rear_axle)
+            else:
+                # otherwise set to None and provide later
+                self.x_0 = None
         else:
             self.x_0 = initial_state_cart if initial_state_cart is not None else self.x_0
 
-        # set low velocity mode given initial velocity in self.x_0
-        self._low_vel_mode = True if self.x_0.velocity < self.config.planning.low_vel_mode_threshold else False
-
         # convert Cartesian initial state or pass given curvilinear initial state
         self.x_0_cl = initial_state_curv if initial_state_curv is not None else self._compute_initial_states(self.x_0)
 
-    def set_collision_checker(self, scenario: Scenario = None, collision_checker: pycrcc.CollisionChecker = None):
+    def set_collision_checker(self, scenario: Scenario = None, collision_checker: pycrcc.CollisionChecker = None,
+                              road_boundary_obstacle=None):
         """
         Sets the collision checker used by the planner using either of the two options:
         If a collision_checker object is passed, then it is used directly by the planner.
         If no collision checker object is passed, then a CommonRoad scenario must be provided from which the collision
         checker is created and set.
         :param scenario: CommonRoad Scenario object
         :param collision_checker: pycrcc.CollisionChecker object
+        :param road_boundary_obstacle: obstacle of type pycrcc.CollisionObject. Can be passed directly to avoid
+        recomputing the road boundary obstacle every time
         """
         if collision_checker is None:
             assert scenario is not None, '<ReactivePlanner.set collision checker>: Please provide a CommonRoad ' \
                                          'scenario OR a ' \
                                          'CollisionChecker object to the planner.'
             cc_scenario = pycrcc.CollisionChecker()
             for co in scenario.static_obstacles:
@@ -237,16 +239,19 @@
                 tvo = create_collision_object(co)
                 if self.config.planning.continuous_collision_check:
                     tvo, err = trajectory_preprocess_obb_sum(tvo)
                     if err == -1:
                         raise Exception("Invalid input for trajectory_preprocess_obb_sum: dynamic "
                                         "obstacle elements overlap")
                 cc_scenario.add_collision_object(tvo)
-            _, road_boundary_sg_obb = create_road_boundary_obstacle(scenario)
-            cc_scenario.add_collision_object(road_boundary_sg_obb)
+            if road_boundary_obstacle is None:
+                _, road_boundary_sg_obb = create_road_boundary_obstacle(scenario)
+                cc_scenario.add_collision_object(road_boundary_sg_obb)
+            else:
+                cc_scenario.add_collision_object(road_boundary_obstacle)
             self._cc: pycrcc.CollisionChecker = cc_scenario
         else:
             assert scenario is None, '<ReactivePlanner.set collision checker>: Please provide a CommonRoad scenario ' \
                                      'OR a ' \
                                      'CollisionChecker object to the planner.'
             self._cc: pycrcc.CollisionChecker = collision_checker
 
@@ -440,14 +445,18 @@
 
     def _compute_initial_states(self, x_0: ReactivePlannerState) -> (np.ndarray, np.ndarray):
         """
         Computes the curvilinear initial states for the polynomial planner based on the Cartesian initial state
         :param x_0: The Cartesion state object representing the initial state of the vehicle
         :return: A tuple containing the initial longitudinal and lateral states (lon,lat)
         """
+        # if no coordinate system is given return None
+        if not self._co:
+            return None
+
         # compute curvilinear position
         try:
             s, d = self._co.convert_to_curvilinear_coords(x_0.position[0], x_0.position[1])
         except ValueError:
             logger.critical("Initial state could not be transformed.")
             raise ValueError("Initial state could not be transformed.")
 
@@ -563,21 +572,31 @@
         Plans an optimal trajectory
         :param current_sampling_level: A specific sampling level to evaluate (no iteration)
         :return: Optimal trajectory as tuple
         """
         # start timer
         planning_start_time = time.time()
 
-        # check if initial states are provided
+        # check if cartesian initial state is provided
         assert self.x_0 is not None, "<ReactivePlanner.plan(): Planner Cartesian initial state is empty!>"
+
+        # check if coordinate system is provided
+        assert self._co is not None, "<ReactivePlanner.plan(): No coordinate system given. Call set_reference_path()>"
+
+        # check if curvilinear initial state is provided and compute if necessary
+        if not self.x_0_cl:
+            self.x_0_cl = self._compute_initial_states(self.x_0)
         assert self.x_0_cl is not None, "<ReactivePlanner.plan(): Planner curvilinear initial state is empty!>"
 
         # get curvilinear initial states
         x_0_lon, x_0_lat = self.x_0_cl
 
+        # set low velocity mode given initial velocity in self.x_0
+        self._low_vel_mode = True if self.x_0.velocity < self.config.planning.low_vel_mode_threshold else False
+
         logger.info("===============================================================")
         logger.info("=================== Starting Planning Cycle ===================")
         logger.info(f"==== Initial state Cartesian ====")
         logger.info(f"time_step={self.x_0.time_step}")
         logger.info(
             f"position={self.x_0.position}, steering_angle={self.x_0.steering_angle}, velocity={self.x_0.velocity}")
         logger.info(
@@ -592,15 +611,15 @@
 
         # initialize optimal trajectory dummy
         optimal_trajectory = None
 
         # initial index of sampling set to use
         i = 1 if current_sampling_level is None else current_sampling_level
 
-        while optimal_trajectory is None and i <= self.sampling_level:
+        while optimal_trajectory is None and i < self.sampling_level:
             # sample trajectory bundle
             bundle = self._create_trajectory_bundle(x_0_lon, x_0_lat, samp_level=i)
 
             # find optimal trajectory (kinematic check/sorting/collision check)
             t0 = time.time()
             optimal_trajectory = self._get_optimal_trajectory(bundle)
 
@@ -1129,8 +1148,12 @@
             new_state_list.append(state.shift_positions_to_center(self.vehicle_params.wb_rear_axle))
 
         trajectory = Trajectory(initial_time_step=new_state_list[0].time_step, state_list=new_state_list)
         # get shape of vehicle
         shape = Rectangle(self.vehicle_params.length, self.vehicle_params.width)
         # get trajectory prediction
         prediction = TrajectoryPrediction(trajectory, shape)
-        return DynamicObstacle(obstacle_id, ObstacleType.CAR, shape, trajectory.state_list[0], prediction)
+        # get initial state
+        init_state = InitialState()
+        init_state = trajectory.state_list[0].convert_state_to_state(init_state)
+
+        return DynamicObstacle(obstacle_id, ObstacleType.CAR, shape, init_state, prediction)
```

### Comparing `commonroad-reactive-planner-2023.1/commonroad_rp/sampling.py` & `commonroad_reactive_planner-2024.1/commonroad_rp/sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Gerald Würsching, Christian Pek"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["BMW Group CAR@TUM, interACT"]
-__version__ = "1.0"
+__version__ = "2024.1"
 __maintainer__ = "Gerald Würsching"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Beta"
 
 import numpy as np
 from abc import ABC, abstractmethod
 from typing import Dict, Optional, List
```

### Comparing `commonroad-reactive-planner-2023.1/commonroad_rp/state.py` & `commonroad_reactive_planner-2024.1/commonroad_rp/state.py`

 * *Files identical despite different names*

### Comparing `commonroad-reactive-planner-2023.1/commonroad_rp/trajectories.py` & `commonroad_reactive_planner-2024.1/commonroad_rp/trajectories.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Christian Pek, Gerald Würsching"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["BMW Group CAR@TUM, interACT"]
-__version__ = "1.0"
+__version__ = "2024.1"
 __maintainer__ = "Gerald Würsching"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Beta"
 
 from typing import Union, List, Optional
 from enum import Enum
 import numpy as np
```

### Comparing `commonroad-reactive-planner-2023.1/commonroad_rp/utility/config.py` & `commonroad_reactive_planner-2024.1/commonroad_rp/utility/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import dataclasses
 import inspect
 import os.path
 from dataclasses import dataclass, field
 from typing import Union, Any, Optional, Dict, List
 import pathlib
 from omegaconf import OmegaConf
+import warnings
 
 from commonroad.scenario.state import InitialState
 from commonroad_dc.feasibility.vehicle_dynamics import VehicleParameterMapping
 from commonroad.common.solution import VehicleType
 from commonroad.scenario.scenario import Scenario
 from commonroad.planning.planning_problem import PlanningProblem, PlanningProblemSet
 from commonroad_route_planner.route import Route
@@ -77,31 +78,33 @@
         """
         try:
             self.__setattr__(key, value)
         except AttributeError as e:
             raise KeyError(f"{key} is not a parameter of {self.__class__.__name__}") from e
 
     @classmethod
-    def load(cls, file_path: Union[pathlib.Path, str], scenario_name: str, validate_types: bool = True) \
+    def load(cls, file_path: Union[pathlib.Path, str], scenario_name: Optional[str] = None, validate_types: bool = True) \
             -> 'ReactivePlannerConfiguration':
         """
-        Loads config file and creates parameter class.
+        Loads parameters from a config yaml file and returns the Configuration class.
 
         :param file_path: Path to yaml file containing config parameters.
-        :param scenario_name: Name of scenario which should be used.
+        :param scenario_name: Name of scenario which should be used. If provided, scenario and planning problem are
+                              loaded from a CR scenario XML file.
         :param validate_types:  Boolean indicating whether loaded config should be validated against CARLA parameters.
         :return: Base parameter class.
         """
         file_path = pathlib.Path(file_path)
         assert file_path.suffix == ".yaml", f"File type {file_path.suffix} is unsupported! Please use .yaml!"
         loaded_yaml = OmegaConf.load(file_path)
         if validate_types:
             OmegaConf.merge(OmegaConf.structured(ReactivePlannerConfiguration), loaded_yaml)
         params = _dict_to_params(OmegaConf.to_object(loaded_yaml), cls)
-        params.general.set_path_scenario(scenario_name)
+        if scenario_name:
+            params.general.set_path_scenario(scenario_name)
         return params
 
 
 @dataclass
 class PlanningConfiguration(BaseConfiguration):
     """Planning parameters for reactive planner."""
 
@@ -122,19 +125,14 @@
     # The list can contain these constraints: velocity, acceleration, kappa, kappa_dot,
     # yaw_rate (Exact naming important!!)
     constraints_to_check: List[str] = \
         field(default_factory=lambda: ["velocity", "acceleration", "kappa", "kappa_dot", "yaw_rate"])
     # lookahead in dt*standstill_lookahead seconds if current velocity <= 0.1 and after specified time too
     standstill_lookahead: int = 10
 
-    def __post_init__(self):
-        # global route and reference path is stored in planning config
-        self.route: Optional[Route] = None
-        self.reference_path: Optional[np.ndarray] = None
-
 
 @dataclass
 class SamplingConfiguration(BaseConfiguration):
     """Sampling parameters for reactive planner."""
 
     # choose sampling method
     # 1: sampling in fixed intervals (see above)
@@ -216,25 +214,27 @@
     delta_max: float = vehicle_parameters.steering.max
     v_delta_min: float = vehicle_parameters.steering.v_min
     v_delta_max: float = vehicle_parameters.steering.v_max
 
     # wheelbase
     wheelbase: float = vehicle_parameters.a + vehicle_parameters.b
 
+    def __post_init__(self):
+        self.kappa_max = np.tan(self.delta_max) / self.wheelbase
+
 
 @dataclass
 class GeneralConfiguration(BaseConfiguration):
     """General parameters for evaluations."""
 
     # paths are relative to the root directory
     path_scenarios: str = "example_scenarios/"
     path_output: str = "output/"
     path_logs: str = "output/logs/"
     path_pickles: str = "output/pickles/"
-    path_offline_data: str = "output/offline_data/"
     path_scenario: Optional[str] = None
     name_scenario: Optional[str] = None
 
     def set_path_scenario(self, scenario_name: str):
         """
         Setter for scenario path.
 
@@ -259,41 +259,32 @@
         self.planning_problem_set: Optional[PlanningProblemSet] = None
 
     @property
     def name_scenario(self) -> str:
         return self.general.name_scenario
 
     def update(self, scenario: Scenario = None, planning_problem: PlanningProblem = None,
-               state_initial: InitialState = None):
+               idx_planning_problem: Optional[int] = None):
         """
         Updates configuration based on the given attributes.
         Function used to construct initial configuration before planner initialization and update configuration during
         re-planning.
 
         :param scenario: (initial or updated) Scenario object
         :param planning_problem: (initial or updated) planning problem
         :param state_initial: initial state (can be different from planning problem initial state during re-planning)
         """
         # update scenario and planning problem with explicitly given ones
-        if scenario:
-            self.scenario = scenario
-        if planning_problem:
-            self.planning_problem = planning_problem
+        self.scenario = scenario
+        self.planning_problem = planning_problem
 
-        # if scenario and planning problem not explicitly given
+        # if both scenario and planning problem are not explicitly provided
         if scenario is None and planning_problem is None:
-            if self.scenario is None or self.planning_problem is None:
-                # read original scenario and pp from scenario file
+            try:
                 self.scenario, self.planning_problem, self.planning_problem_set = \
-                    load_scenario_and_planning_problem(self.general.path_scenario)
-            else:
-                # keep previously stored scenario and planning problem
-                pass
-        else:
-            raise RuntimeError("ReactiveParams::update: Scenario or Planning not None")
+                    load_scenario_and_planning_problem(self.general.path_scenario, idx_planning_problem)
+            except FileNotFoundError:
+                warnings.warn(f"<ReactivePlannerConfiguration.update()>: No scenario .xml file found at "
+                              f"path_scenario = {self.general.path_scenario}")
 
-        # Check that scenario and planning problem are set
+        # Check that a scenario is set (planning problem can be set afterwards)
         assert self.scenario is not None, "<Configuration.update()>: no scenario has been specified"
-        assert self.planning_problem is not None, "<Configuration.update()>: no planning problem has been specified"
-
-        # update initial state for planning if explicitly given
-        self.planning.state_initial = state_initial if state_initial else self.planning_problem.initial_state
```

### Comparing `commonroad-reactive-planner-2023.1/commonroad_rp/utility/evaluation.py` & `commonroad_reactive_planner-2024.1/commonroad_rp/utility/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 __author__ = "Gerald Würsching"
 __copyright__ = "TUM Cyber-Physical Systems Group"
-__version__ = "1.0"
+__version__ = "2024.1"
 __maintainer__ = "Gerald Würsching"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Beta"
 
 
 from typing import List, Union
 from matplotlib import pyplot as plt
 import numpy as np
+import warnings
 
 from commonroad.scenario.trajectory import Trajectory
 from commonroad.scenario.state import InputState, TraceState
 from commonroad.planning.planning_problem import PlanningProblem
 from commonroad.scenario.scenario import Scenario
 from commonroad.common.solution import Solution, PlanningProblemSolution, VehicleModel, \
     VehicleType, CostFunction
@@ -30,16 +31,16 @@
     """
     Creates a CommonRoad solution Trajectory from the planning results, evaluates state and input feasibility, plots
     solution Trajectory
     :return cr_solution: Planner solution as CR solution object
     :return feasibility_list: List[Bool] indicating feasibility of each state transition
     """
     ego_solution_trajectory = create_full_solution_trajectory(config, state_list)
-    cr_solution, feasibility_list = evaluate_results(config, ego_solution_trajectory, input_list)
     plot_final_trajectory(config.scenario, config.planning_problem, ego_solution_trajectory.state_list, config)
+    cr_solution, feasibility_list = evaluate_results(config, ego_solution_trajectory, input_list)
 
     return cr_solution, feasibility_list
 
 
 def evaluate_results(config: ReactivePlannerConfiguration, ego_solution_trajectory, record_input_list):
     """
     Solution is evaluated via input reconstruction from commonroad_dc.feasibility.feasibility_checker
```

### Comparing `commonroad-reactive-planner-2023.1/commonroad_rp/utility/general.py` & `commonroad_reactive_planner-2024.1/commonroad_rp/utility/general.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,34 @@
-from typing import Tuple
+from typing import Tuple, Optional
 
 import numpy as np
 
 from commonroad.common.file_reader import CommonRoadFileReader
 from commonroad.planning.planning_problem import PlanningProblem, PlanningProblemSet
 from commonroad.scenario.scenario import Scenario
 from commonroad.scenario.trajectory import Trajectory
 
 
-def load_scenario_and_planning_problem(path_scenario, idx_planning_problem: int = 0)\
+def load_scenario_and_planning_problem(path_scenario, idx_planning_problem: Optional[int] = None)\
         -> Tuple[Scenario, PlanningProblem, PlanningProblemSet]:
     """
     Loads a scenario and planning problem from the configuration.
     :param path_scenario: full path to scenario XML file
-    :param idx_planning_problem: index of the planning problem
+    :param idx_planning_problem: index of the planning problem (if none provided, first planning problem is returned)
     :return: scenario and planning problem and planning problem set
     """
     scenario, planning_problem_set = CommonRoadFileReader(path_scenario).open()
-    planning_problem = list(planning_problem_set.planning_problem_dict.values())[idx_planning_problem]
+    if idx_planning_problem is not None:
+        try:
+            planning_problem = planning_problem_set.find_planning_problem_by_id(idx_planning_problem)
+        except KeyError:
+            raise KeyError(f"<ReactivePlannerConfiguration.update()>:"
+                           f"Planning Problem with ID: {idx_planning_problem} does not exist!")
+    else:
+        planning_problem = list(planning_problem_set.planning_problem_dict.values())[0]
 
     return scenario, planning_problem, planning_problem_set
 
 
 def retrieve_desired_velocity_from_pp(planning_problem: PlanningProblem):
     """Simple approach which retrieves average velocity from goal configuration"""
     goal = planning_problem.goal
```

### Comparing `commonroad-reactive-planner-2023.1/commonroad_rp/utility/logger.py` & `commonroad_reactive_planner-2024.1/commonroad_rp/utility/logger.py`

 * *Files identical despite different names*

### Comparing `commonroad-reactive-planner-2023.1/commonroad_rp/utility/utils_coordinate_system.py` & `commonroad_reactive_planner-2024.1/commonroad_rp/utility/utils_coordinate_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Gerald Würsching, Christian Pek"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["BMW Group CAR@TUM, interACT"]
-__version__ = "1.0"
+__version__ = "2024.1"
 __maintainer__ = "Gerald Würsching"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Alpha"
 
 from copy import deepcopy
 import numpy as np
 from scipy.interpolate import splprep, splev
@@ -81,30 +81,31 @@
     ref_path = np.array([x_new, y_new]).transpose()
     reference = resample_polyline(ref_path, resample_step)
     return reference
 
 
 class CoordinateSystem:
 
-    def __init__(self, reference: np.ndarray = None, ccosy: CurvilinearCoordinateSystem = None):
+    def __init__(self, reference: np.ndarray = None, ccosy: CurvilinearCoordinateSystem = None, smooth_reference=True):
         if ccosy is None:
             assert reference is not None, '<CoordinateSystem>: Please provide a reference path OR a ' \
                                           'CurvilinearCoordinateSystem object.'
             # set reference and create ccosy from given reference
 
             # remove duplicated vertices in reference path
             _, idx = np.unique(reference, axis=0, return_index=True)
             reference = reference[np.sort(idx)]
 
-            # smooth reference path
-            reference = smooth_ref_path(reference)
-
-            # remove duplicated vertices in reference path after smoothing
-            _, idx = np.unique(reference, axis=0, return_index=True)
-            reference = reference[np.sort(idx)]
+            if smooth_reference:
+                # smooth reference path
+                reference = smooth_ref_path(reference)
+
+                # remove duplicated vertices in reference path after smoothing
+                _, idx = np.unique(reference, axis=0, return_index=True)
+                reference = reference[np.sort(idx)]
 
             self.reference = reference
         else:
             assert ccosy is not None, '<CoordinateSystem>: Please provide a reference path OR a ' \
                                           'CurvilinearCoordinateSystem object.'
             # set ccosy and use reference from given ccosy
             self.ccosy = ccosy
```

### Comparing `commonroad-reactive-planner-2023.1/commonroad_rp/utility/visualization.py` & `commonroad_reactive_planner-2024.1/commonroad_rp/utility/visualization.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 __author__ = "Gerald Würsching"
 __copyright__ = "TUM Cyber-Physical Systems Group"
-__version__ = "1.0"
+__version__ = "2024.1"
 __maintainer__ = "Gerald Würsching"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Beta"
 
 
 # standard imports
-from typing import List, Union
+from typing import List, Union, Optional
 import os
 import logging
 
 # third party
 import matplotlib.pyplot as plt
 import numpy as np
 import imageio
@@ -46,30 +46,31 @@
 
 def visualize_scenario_and_pp(scenario: Scenario, planning_problem: PlanningProblem, cosy=None):
     """Visualizes scenario, planning problem and (optionally) the reference path"""
     plot_limits = None
     ref_path = None
     if cosy is not None:
         ref_path = cosy.reference
-        x_min = np.min(ref_path[:, 0]) - 50
-        x_max = np.max(ref_path[:, 0]) + 50
-        y_min = np.min(ref_path[:, 1]) - 50
-        y_max = np.max(ref_path[:, 1]) + 50
+        x_min = np.min(ref_path[:, 0]) - 20
+        x_max = np.max(ref_path[:, 0]) + 20
+        y_min = np.min(ref_path[:, 1]) - 20
+        y_max = np.max(ref_path[:, 1]) + 20
         plot_limits = [x_min, x_max, y_min, y_max]
 
     rnd = MPRenderer(figsize=(20, 10), plot_limits=plot_limits)
     rnd.draw_params.time_begin = 0
+    rnd.draw_params.dynamic_obstacle.draw_icon = True
     scenario.draw(rnd)
     planning_problem.draw(rnd)
     rnd.render()
     if ref_path is not None:
-        rnd.ax.plot(ref_path[:, 0], ref_path[:, 1], color='g', marker='.', markersize=1, zorder=19,
+        rnd.ax.plot(ref_path[:, 0], ref_path[:, 1], color='g', marker='.', markersize=1, zorder=100,
                     linewidth=0.8, label='reference path')
         proj_domain_border = np.array(cosy.ccosy.projection_domain())
-        rnd.ax.plot(proj_domain_border[:, 0], proj_domain_border[:, 1], color="orange", linewidth=0.8)
+        rnd.ax.plot(proj_domain_border[:, 0], proj_domain_border[:, 1], color="orange", linewidth=0.8, zorder=100)
     plt.show(block=True)
 
 
 def visualize_collision_checker(scenario: Scenario, cc: pycrcc.CollisionChecker):
     """
     Visualizes the collision checker, i.e., all collision objects and, if applicable, the road boundary.
     :param scenario CommonRoad scenario object
@@ -94,27 +95,36 @@
     :param config: Configuration object for plot/save settings
     :param traj_set: List of sampled trajectories (optional)
     :param ref_path: Reference path for planner as polyline [(nx2) np.ndarray] (optional)
     :param rnd: MPRenderer object (optional: if none is passed, the function creates a new renderer object; otherwise it
     will visualize on the existing object)
     :param plot_limits: x, y axis limits for plotting
     """
+    # get plot limits from ref path
+    if plot_limits is None and ref_path is not None:
+        x_min = np.min(ref_path[:, 0]) - 20
+        x_max = np.max(ref_path[:, 0]) + 20
+        y_min = np.min(ref_path[:, 1]) - 20
+        y_max = np.max(ref_path[:, 1]) + 20
+        plot_limits = [x_min, x_max, y_min, y_max]
+
     # create renderer object (if no existing renderer is passed)
     if rnd is None:
         rnd = MPRenderer(figsize=(20, 10), plot_limits=plot_limits)
 
     # set renderer draw params
     rnd.draw_params.time_begin = timestep
     rnd.draw_params.dynamic_obstacle.draw_icon = config.debug.draw_icons
     rnd.draw_params.planning_problem.initial_state.state.draw_arrow = False
     rnd.draw_params.planning_problem.initial_state.state.radius = 0.5
 
     # set ego vehicle draw params
     ego_params = DynamicObstacleParams()
     ego_params.time_begin = timestep
+    ego_params.time_end = 1000
     ego_params.draw_icon = config.debug.draw_icons
     ego_params.vehicle_shape.occupancy.shape.facecolor = "#E37222"
     ego_params.vehicle_shape.occupancy.shape.edgecolor = "#9C4100"
     ego_params.vehicle_shape.occupancy.shape.zorder = 50
     ego_params.vehicle_shape.occupancy.shape.opacity = 1
 
     # visualize scenario, planning problem, ego vehicle
@@ -152,26 +162,36 @@
 
     # show plot
     if config.debug.show_plots:
         plt.show(block=True)
 
 
 def plot_final_trajectory(scenario: Scenario, planning_problem: PlanningProblem, state_list: List[CustomState],
-                          config: ReactivePlannerConfiguration, ref_path: np.ndarray = None):
+                          config: ReactivePlannerConfiguration, ref_path: np.ndarray = None,
+                          plot_limits: Optional[List[Union[int, float]]] = None):
     """
     Function plots occupancies for a given CommonRoad trajectory (of the ego vehicle)
     :param scenario: CommonRoad scenario object
     :param planning_problem CommonRoad Planning problem object
     :param state_list: List of trajectory States
     :param config: Configuration object for plot/save settings
     :param ref_path: Reference path as [(nx2) np.ndarray] (optional)
     :param save_path: Path to save plot as .png (optional)
     """
+    # get plot limits from trajectory
+    if plot_limits is None:
+        position_array = np.array([state.position for state in state_list])
+        x_min = np.min(position_array[:, 0]) - 20
+        x_max = np.max(position_array[:, 0]) + 20
+        y_min = np.min(position_array[:, 1]) - 20
+        y_max = np.max(position_array[:, 1]) + 20
+        plot_limits = [x_min, x_max, y_min, y_max]
+
     # create renderer object (if no existing renderer is passed)
-    rnd = MPRenderer(figsize=(20, 10))
+    rnd = MPRenderer(figsize=(20, 10), plot_limits=plot_limits)
 
     # set renderer draw params
     rnd.draw_params.time_begin = 0
     rnd.draw_params.planning_problem.initial_state.state.draw_arrow = False
     rnd.draw_params.planning_problem.initial_state.state.radius = 0.5
 
     # set occupancy shape params
```

