# Comparing `tmp/Xodia24-0.0.9.tar.gz` & `tmp/Xodia24-0.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Xodia24-0.0.9.tar", last modified: Fri Apr 19 06:01:03 2024, max compression
+gzip compressed data, was "Xodia24-0.1.19.tar", last modified: Tue Apr 23 18:54:43 2024, max compression
```

## Comparing `Xodia24-0.0.9.tar` & `Xodia24-0.1.19.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 06:01:03.326712 Xodia24-0.0.9/
--rw-rw-rw-   0        0        0     1088 2024-04-01 14:18:58.000000 Xodia24-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     8044 2024-04-19 06:01:03.326712 Xodia24-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     7225 2024-04-19 05:57:27.000000 Xodia24-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 06:01:03.277905 Xodia24-0.0.9/Xodia24/
--rw-rw-rw-   0        0        0       21 2024-04-19 06:00:48.000000 Xodia24-0.0.9/Xodia24/__init__.py
--rw-rw-rw-   0        0        0     3844 2024-04-19 05:35:28.000000 Xodia24-0.0.9/Xodia24/env.py
--rw-rw-rw-   0        0        0      385 2024-04-01 13:45:24.000000 Xodia24-0.0.9/Xodia24/path.py
-drwxrwxrwx   0        0        0        0 2024-04-19 06:01:03.323140 Xodia24-0.0.9/Xodia24.egg-info/
--rw-rw-rw-   0        0        0     8044 2024-04-19 06:01:02.000000 Xodia24-0.0.9/Xodia24.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2024-04-19 06:01:02.000000 Xodia24-0.0.9/Xodia24.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 06:01:02.000000 Xodia24-0.0.9/Xodia24.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-19 06:01:02.000000 Xodia24-0.0.9/Xodia24.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-19 06:01:02.000000 Xodia24-0.0.9/Xodia24.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 06:01:03.326712 Xodia24-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1244 2024-04-19 06:00:58.000000 Xodia24-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:54:43.832418 Xodia24-0.1.19/
+-rw-rw-rw-   0        0        0     1088 2024-04-01 14:18:58.000000 Xodia24-0.1.19/LICENSE
+-rw-rw-rw-   0        0        0     7459 2024-04-23 18:54:43.832418 Xodia24-0.1.19/PKG-INFO
+-rw-rw-rw-   0        0        0     6632 2024-04-19 16:52:58.000000 Xodia24-0.1.19/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 18:54:43.786781 Xodia24-0.1.19/Xodia24/
+-rw-rw-rw-   0        0        0       21 2024-04-19 06:00:48.000000 Xodia24-0.1.19/Xodia24/__init__.py
+-rw-rw-rw-   0        0        0     7941 2024-04-23 18:51:00.000000 Xodia24-0.1.19/Xodia24/env.py
+-rw-rw-rw-   0        0        0      385 2024-04-01 13:45:24.000000 Xodia24-0.1.19/Xodia24/path.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:54:43.830359 Xodia24-0.1.19/Xodia24.egg-info/
+-rw-rw-rw-   0        0        0     7459 2024-04-23 18:54:43.000000 Xodia24-0.1.19/Xodia24.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2024-04-23 18:54:43.000000 Xodia24-0.1.19/Xodia24.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 18:54:43.000000 Xodia24-0.1.19/Xodia24.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-23 18:54:43.000000 Xodia24-0.1.19/Xodia24.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 18:54:43.000000 Xodia24-0.1.19/Xodia24.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 18:54:43.832418 Xodia24-0.1.19/setup.cfg
+-rw-rw-rw-   0        0        0     1245 2024-04-23 18:51:42.000000 Xodia24-0.1.19/setup.py
```

### Comparing `Xodia24-0.0.9/LICENSE` & `Xodia24-0.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `Xodia24-0.0.9/PKG-INFO` & `Xodia24-0.1.19/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xodia24
-Version: 0.0.9
+Version: 0.1.19
 Summary: Python package providing a custom environment for simulating tank battles
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,reinforcement-learning,tank-battle
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -47,19 +47,18 @@
 
 # Train RL model using the environment
 # ...
 ```
 
 3. **Using the Custom PocketTank Environment:**
    If you want to utilize a custom implementation of the PocketTank environment, you can create your subclass and override the necessary methods. Here's a sample implementation:
-
+   
+# Custom PocketTank
 ```python
-# custom_pocket_tank.py
-
-from Xodia24.pocket_tank import PocketTank
+from Xodia24.env import PocketTank
 from gymnasium import spaces
 import numpy as np
 
 class CustomPocketTank(PocketTank):
     def __init__(self):
         super().__init__()
         """
@@ -79,83 +78,91 @@
         Args:
             diff_distance (float): Difference in distance between the bullet and the target tank.
 
         Returns:
             float: Custom reward value based on the difference in distance.
         """
         # Implement your custom reward logic here
-        custom_reward = 1.0 / (1.0 + diff_distance)  # Example: Inverse distance as reward
+        custom_reward = 0 # Add your reward Function
         return custom_reward
 ```
 
 ## Dependencies
 
 - `gymnasium`: A toolkit for developing and comparing reinforcement learning algorithms.
 - `numpy`: Library for numerical computations and array operations.
 - `matplotlib`: Library for creating plots and visualizations.
 
 
-### Action Space
+## Action Space
 
 The action space in the Xodia24 PocketTank environment refers to the set of possible actions that the reinforcement learning (RL) agent can take at each time step. In the tank battle scenario, the agent controls one of the tanks and has several actions available to it, including adjusting the power and angle of the tank's cannon and moving the tank across the 2D grid.
 
-#### Available Actions:
+### Available Actions:
 - **Adjust Power**: The agent can adjust the power setting of the tank's cannon, determining the force with which the projectile is fired.
+Range: 0-100
 - **Adjust Angle**: The agent can adjust the angle of the tank's cannon, controlling the direction in which the projectile is launched.
+Range: 0 deg - 90 deg
 - **Move Tank**: The agent can move the tank across the 2D grid, changing its position on the battlefield.
+0 = Dont move only fire
+1 = move +25 and then fire
+2 = move -25 and then fire
 
-The action space is typically represented as a discrete or continuous space, depending on the specific implementation of the environment.
 
-### Observation Space
+## Observation Space
 
 The observation space refers to the information that the RL agent receives from the environment at each time step. This information helps the agent make decisions about which actions to take in order to achieve its objective. In the Xodia24 PocketTank environment, the observation space includes various features of the battlefield and the tanks' positions.
 
-#### Example Observations:
-- **Tank Positions**: The coordinates of both the agent-controlled tank and the opponent tank on the 2D grid.
-- **Terrain Information**: Information about the terrain features, such as obstacles or cover, that may affect the trajectory of the projectile.
-- **Projectile Position**: The current position of the projectile fired by the tanks.
-
-The observation space can be represented as a vector, matrix, or other data structure depending on the complexity of the environment and the information that needs to be conveyed to the agent.
+obs = [x1,x2,b]
 
+x1: Your Tank Location
+x2: Enemy Tank Location
+b : bullet type ID
 
-Here's the documentation for the reinforcement learning environment for the Pocket Tanks game, with updated information for the fourth bullet:
 
 
 ## Bullet Types
 
 The tank has seven different types of bullets available, each with unique properties and effects. The tank has access to each bullet type an unlimited number of times.
 
 1. *Standard Shell*:
     - *Description*: A classic projectile bullet that follows projectile motion.
     - *Damage*: Deals 20 damage upon hitting the target.
     - *Trajectory*: Parabolic trajectory determined by initial angle and velocity.
+    - *ID*: 0
 
 2. *Triple Threat*:
     - *Description*: A bullet that splits into three smaller bullets upon firing.
     - *Damage*: Each of the three bullets deals 20 damage, similar to the Standard Shell.
     - *Trajectory*: Parabolic trajectory similar to Standard Shell.
+     - *ID*: 1
 
 3. *Long Shot*:
     - *Description*: A bullet that deals more damage based on the distance it travels before hitting the ground.
     - *Damage*: Damage increases as the distance traveled increases.
     - *Trajectory*: Parabolic trajectory similar to the Standard Shell.
+    - *ID*: 2
 
 4. *Heavy Impact*:
     - *Description*: A high-damage bullet with limited range and velocity.
     - *Damage*: Deals 40 damage upon hitting the target.
     - *Trajectory*: Limited velocity and range compared to other bullets.
+    - *ID*: 3
 
 5. *Blast Radius*:
     - *Description*: A bullet that causes area damage within a radius of 100.
     - *Damage*: Deals 10 damage in a radius of 100 around the impact point.
     - *Trajectory*: Parabolic trajectory similar to the Standard Shell.
+    - *ID*: 4
 
 6. *Healing Halo*:
     - *Description*: A bullet that heals the tank upon impact.
     - *Healing*: Heals the tank by 10 points upon hitting the ground or a target.
     - *Trajectory*: Parabolic trajectory similar to the Standard Shell.
+    - *ID*: 5
 
 7. *Boomerang Blast*:
     - *Description*: A bullet that follows a unique trajectory resembling a boomerang.
     - *Damage*: Deals 20 damage upon hitting the target.
     - *Trajectory*: Follows a curved trajectory that slightly reverses direction, like a boomerang.
+    - *ID*: 6
```

### Comparing `Xodia24-0.0.9/README.md` & `Xodia24-0.1.19/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,19 +28,18 @@
 
 # Train RL model using the environment
 # ...
 ```
 
 3. **Using the Custom PocketTank Environment:**
    If you want to utilize a custom implementation of the PocketTank environment, you can create your subclass and override the necessary methods. Here's a sample implementation:
-
+   
+# Custom PocketTank
 ```python
-# custom_pocket_tank.py
-
-from Xodia24.pocket_tank import PocketTank
+from Xodia24.env import PocketTank
 from gymnasium import spaces
 import numpy as np
 
 class CustomPocketTank(PocketTank):
     def __init__(self):
         super().__init__()
         """
@@ -60,83 +59,91 @@
         Args:
             diff_distance (float): Difference in distance between the bullet and the target tank.
 
         Returns:
             float: Custom reward value based on the difference in distance.
         """
         # Implement your custom reward logic here
-        custom_reward = 1.0 / (1.0 + diff_distance)  # Example: Inverse distance as reward
+        custom_reward = 0 # Add your reward Function
         return custom_reward
 ```
 
 ## Dependencies
 
 - `gymnasium`: A toolkit for developing and comparing reinforcement learning algorithms.
 - `numpy`: Library for numerical computations and array operations.
 - `matplotlib`: Library for creating plots and visualizations.
 
 
-### Action Space
+## Action Space
 
 The action space in the Xodia24 PocketTank environment refers to the set of possible actions that the reinforcement learning (RL) agent can take at each time step. In the tank battle scenario, the agent controls one of the tanks and has several actions available to it, including adjusting the power and angle of the tank's cannon and moving the tank across the 2D grid.
 
-#### Available Actions:
+### Available Actions:
 - **Adjust Power**: The agent can adjust the power setting of the tank's cannon, determining the force with which the projectile is fired.
+Range: 0-100
 - **Adjust Angle**: The agent can adjust the angle of the tank's cannon, controlling the direction in which the projectile is launched.
+Range: 0 deg - 90 deg
 - **Move Tank**: The agent can move the tank across the 2D grid, changing its position on the battlefield.
+0 = Dont move only fire
+1 = move +25 and then fire
+2 = move -25 and then fire
 
-The action space is typically represented as a discrete or continuous space, depending on the specific implementation of the environment.
 
-### Observation Space
+## Observation Space
 
 The observation space refers to the information that the RL agent receives from the environment at each time step. This information helps the agent make decisions about which actions to take in order to achieve its objective. In the Xodia24 PocketTank environment, the observation space includes various features of the battlefield and the tanks' positions.
 
-#### Example Observations:
-- **Tank Positions**: The coordinates of both the agent-controlled tank and the opponent tank on the 2D grid.
-- **Terrain Information**: Information about the terrain features, such as obstacles or cover, that may affect the trajectory of the projectile.
-- **Projectile Position**: The current position of the projectile fired by the tanks.
-
-The observation space can be represented as a vector, matrix, or other data structure depending on the complexity of the environment and the information that needs to be conveyed to the agent.
+obs = [x1,x2,b]
 
+x1: Your Tank Location
+x2: Enemy Tank Location
+b : bullet type ID
 
-Here's the documentation for the reinforcement learning environment for the Pocket Tanks game, with updated information for the fourth bullet:
 
 
 ## Bullet Types
 
 The tank has seven different types of bullets available, each with unique properties and effects. The tank has access to each bullet type an unlimited number of times.
 
 1. *Standard Shell*:
     - *Description*: A classic projectile bullet that follows projectile motion.
     - *Damage*: Deals 20 damage upon hitting the target.
     - *Trajectory*: Parabolic trajectory determined by initial angle and velocity.
+    - *ID*: 0
 
 2. *Triple Threat*:
     - *Description*: A bullet that splits into three smaller bullets upon firing.
     - *Damage*: Each of the three bullets deals 20 damage, similar to the Standard Shell.
     - *Trajectory*: Parabolic trajectory similar to Standard Shell.
+     - *ID*: 1
 
 3. *Long Shot*:
     - *Description*: A bullet that deals more damage based on the distance it travels before hitting the ground.
     - *Damage*: Damage increases as the distance traveled increases.
     - *Trajectory*: Parabolic trajectory similar to the Standard Shell.
+    - *ID*: 2
 
 4. *Heavy Impact*:
     - *Description*: A high-damage bullet with limited range and velocity.
     - *Damage*: Deals 40 damage upon hitting the target.
     - *Trajectory*: Limited velocity and range compared to other bullets.
+    - *ID*: 3
 
 5. *Blast Radius*:
     - *Description*: A bullet that causes area damage within a radius of 100.
     - *Damage*: Deals 10 damage in a radius of 100 around the impact point.
     - *Trajectory*: Parabolic trajectory similar to the Standard Shell.
+    - *ID*: 4
 
 6. *Healing Halo*:
     - *Description*: A bullet that heals the tank upon impact.
     - *Healing*: Heals the tank by 10 points upon hitting the ground or a target.
     - *Trajectory*: Parabolic trajectory similar to the Standard Shell.
+    - *ID*: 5
 
 7. *Boomerang Blast*:
     - *Description*: A bullet that follows a unique trajectory resembling a boomerang.
     - *Damage*: Deals 20 damage upon hitting the target.
     - *Trajectory*: Follows a curved trajectory that slightly reverses direction, like a boomerang.
+    - *ID*: 6
```

### Comparing `Xodia24-0.0.9/Xodia24.egg-info/PKG-INFO` & `Xodia24-0.1.19/Xodia24.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xodia24
-Version: 0.0.9
+Version: 0.1.19
 Summary: Python package providing a custom environment for simulating tank battles
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,reinforcement-learning,tank-battle
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -47,19 +47,18 @@
 
 # Train RL model using the environment
 # ...
 ```
 
 3. **Using the Custom PocketTank Environment:**
    If you want to utilize a custom implementation of the PocketTank environment, you can create your subclass and override the necessary methods. Here's a sample implementation:
-
+   
+# Custom PocketTank
 ```python
-# custom_pocket_tank.py
-
-from Xodia24.pocket_tank import PocketTank
+from Xodia24.env import PocketTank
 from gymnasium import spaces
 import numpy as np
 
 class CustomPocketTank(PocketTank):
     def __init__(self):
         super().__init__()
         """
@@ -79,83 +78,91 @@
         Args:
             diff_distance (float): Difference in distance between the bullet and the target tank.
 
         Returns:
             float: Custom reward value based on the difference in distance.
         """
         # Implement your custom reward logic here
-        custom_reward = 1.0 / (1.0 + diff_distance)  # Example: Inverse distance as reward
+        custom_reward = 0 # Add your reward Function
         return custom_reward
 ```
 
 ## Dependencies
 
 - `gymnasium`: A toolkit for developing and comparing reinforcement learning algorithms.
 - `numpy`: Library for numerical computations and array operations.
 - `matplotlib`: Library for creating plots and visualizations.
 
 
-### Action Space
+## Action Space
 
 The action space in the Xodia24 PocketTank environment refers to the set of possible actions that the reinforcement learning (RL) agent can take at each time step. In the tank battle scenario, the agent controls one of the tanks and has several actions available to it, including adjusting the power and angle of the tank's cannon and moving the tank across the 2D grid.
 
-#### Available Actions:
+### Available Actions:
 - **Adjust Power**: The agent can adjust the power setting of the tank's cannon, determining the force with which the projectile is fired.
+Range: 0-100
 - **Adjust Angle**: The agent can adjust the angle of the tank's cannon, controlling the direction in which the projectile is launched.
+Range: 0 deg - 90 deg
 - **Move Tank**: The agent can move the tank across the 2D grid, changing its position on the battlefield.
+0 = Dont move only fire
+1 = move +25 and then fire
+2 = move -25 and then fire
 
-The action space is typically represented as a discrete or continuous space, depending on the specific implementation of the environment.
 
-### Observation Space
+## Observation Space
 
 The observation space refers to the information that the RL agent receives from the environment at each time step. This information helps the agent make decisions about which actions to take in order to achieve its objective. In the Xodia24 PocketTank environment, the observation space includes various features of the battlefield and the tanks' positions.
 
-#### Example Observations:
-- **Tank Positions**: The coordinates of both the agent-controlled tank and the opponent tank on the 2D grid.
-- **Terrain Information**: Information about the terrain features, such as obstacles or cover, that may affect the trajectory of the projectile.
-- **Projectile Position**: The current position of the projectile fired by the tanks.
-
-The observation space can be represented as a vector, matrix, or other data structure depending on the complexity of the environment and the information that needs to be conveyed to the agent.
+obs = [x1,x2,b]
 
+x1: Your Tank Location
+x2: Enemy Tank Location
+b : bullet type ID
 
-Here's the documentation for the reinforcement learning environment for the Pocket Tanks game, with updated information for the fourth bullet:
 
 
 ## Bullet Types
 
 The tank has seven different types of bullets available, each with unique properties and effects. The tank has access to each bullet type an unlimited number of times.
 
 1. *Standard Shell*:
     - *Description*: A classic projectile bullet that follows projectile motion.
     - *Damage*: Deals 20 damage upon hitting the target.
     - *Trajectory*: Parabolic trajectory determined by initial angle and velocity.
+    - *ID*: 0
 
 2. *Triple Threat*:
     - *Description*: A bullet that splits into three smaller bullets upon firing.
     - *Damage*: Each of the three bullets deals 20 damage, similar to the Standard Shell.
     - *Trajectory*: Parabolic trajectory similar to Standard Shell.
+     - *ID*: 1
 
 3. *Long Shot*:
     - *Description*: A bullet that deals more damage based on the distance it travels before hitting the ground.
     - *Damage*: Damage increases as the distance traveled increases.
     - *Trajectory*: Parabolic trajectory similar to the Standard Shell.
+    - *ID*: 2
 
 4. *Heavy Impact*:
     - *Description*: A high-damage bullet with limited range and velocity.
     - *Damage*: Deals 40 damage upon hitting the target.
     - *Trajectory*: Limited velocity and range compared to other bullets.
+    - *ID*: 3
 
 5. *Blast Radius*:
     - *Description*: A bullet that causes area damage within a radius of 100.
     - *Damage*: Deals 10 damage in a radius of 100 around the impact point.
     - *Trajectory*: Parabolic trajectory similar to the Standard Shell.
+    - *ID*: 4
 
 6. *Healing Halo*:
     - *Description*: A bullet that heals the tank upon impact.
     - *Healing*: Heals the tank by 10 points upon hitting the ground or a target.
     - *Trajectory*: Parabolic trajectory similar to the Standard Shell.
+    - *ID*: 5
 
 7. *Boomerang Blast*:
     - *Description*: A bullet that follows a unique trajectory resembling a boomerang.
     - *Damage*: Deals 20 damage upon hitting the target.
     - *Trajectory*: Follows a curved trajectory that slightly reverses direction, like a boomerang.
+    - *ID*: 6
```

### Comparing `Xodia24-0.0.9/setup.py` & `Xodia24-0.1.19/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 
-VERSION = '0.0.9' 
+VERSION = '0.1.19' 
 DESCRIPTION = 'Python package providing a custom environment for simulating tank battles'
 LONG_DESCRIPTION = 'Xodia24 is a Python package providing a custom environment for simulating a tank battle scenario where two tanks are positioned on a 2D grid.'
 
 # Setting up
 setup(
     name="Xodia24",
     version=VERSION,
```

